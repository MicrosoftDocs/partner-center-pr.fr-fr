---
title: Fichiers de réconciliation basés sur l’utilisation | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Tous les éléments de votre fichier de réconciliation basé sur l’utilisation sont expliqués, avec des exemples.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b73962b1e9d2925b0e61632a18522a1c22e4d346
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943382"
---
# <a name="usage-based-file-fields"></a>Champs des fichiers basés sur l’utilisation

S'applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Pour concilier vos frais par rapport à l’utilisation d’un client, comparez les **ResellerID**, **nom du revendeur**et **ResellerBillableAccount** du fichier de réconciliation avec le **nom du client** et l’ID d' **abonnement** de l’espace partenaires.

## <a name="fields-in-usage-based-reconciliation-files"></a>Champs dans les fichiers de réconciliation basés sur l’utilisation

Les champs suivants décrivent les services utilisés et leurs taux.

| Colonne | Description | Exemple de valeur (s) |
| ------ | ----------- | ------------ |
| PartnerID | Identificateur du partenaire, au format GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nom du partenaire. | *Contoso, Ltd.* |
| PartnerBillableAccountID | Identificateur du compte du partenaire. | *1010578050* |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’espace Partenaires. *Très important pour rapprocher la facture de vos informations système.* | *Tester le client* |
| MPNID | Identificateur MPN du partenaire CSP. | *4390934* |
| ResellerMPNID | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. Pour plus d’informations, consultez [Comment dénombrer par partenaire](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| InvoiceNumber | Le numéro de la facture dans laquelle la transaction spécifiée apparaît. | *D020001IVK* |
| ChargeStartDate | Date de début du cycle de facturation, sauf en cas de dates de données d’utilisation latente non facturées précédemment (du cycle de facturation précédent). L’heure indique toujours le début de la journée, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Date de fin du cycle de facturation, sauf en cas de dates de données d’utilisation latente non facturées précédemment (du cycle de facturation précédent). L’heure indique toujours la fin de la journée, 23:59. | *2/28/2019 23:59* |
| SubscriptionID | Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. *Ce n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Surnom de l’offre de service. | *Microsoft Azure* |
| SubscriptionDescription | Secteur d’activité de l’offre de service. | *Microsoft Azure* |
| OrderId | Identificateur unique pour une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *566890604832738111* |
| ServiceName | Nom du service Azure en question. | *MACHINES VIRTUELLES* |
| ServiceType | Type spécifique du service Azure. | *Service bus – individuel ou Pack*, *SQL Azure base de données – édition Business ou Web* |
| ResourceGUID | Identificateur unique spécifique pour toutes les données de service et la structure de tarification. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Nom_ressource | Nom de la ressource Azure. | *Transfert de données dans (Go)* , *transfert de données sortant (Go)* |
| Région | Région à laquelle l’utilisation s’applique. Principalement utilisé pour affecter des tarifs aux transferts de données, car les tarifs varient selon la région. | *Asie-Pacifique*, *Europe*, *Amérique latine* *Amérique du Nord* |
| SKU | Identificateur Microsoft unique pour une offre. | *7UD-00001* |
| DetailLineItemId | Identificateur et quantité pour dénombrer les différents taux d’un service ou d’une ressource dans une période de facturation donnée. Pour la tarification hiérarchisée Azure, il peut y avoir un tarif pour une certaine quantité d’unités facturables, puis un taux différent après cette quantité. | *1* |
| ConsumedQuantity | Quantité de service utilisée (par exemple, heures ou Go) pendant la période de rapport. Inclut également toute utilisation non facturée pour les périodes précédentes. | *11* |
| IncludedQuantity | Unités incluses dans le cadre de l’offre. En général absents du CSP. | *0* |
| OverageQuantity | Unités non incluses dans le cadre de l’offre. Celles-ci doivent être payées par le partenaire. Égal à **ConsumedQuantity** moins **IncludedQuantity**. | *11* |
| ListPrice | Prix de l’offre en vigueur à la date de début de l’abonnement. | *$0,0808* |
| PretaxCharges | Égal à **ListPrist** multiplié par **divisé par overagequantity**, arrondi au cent le plus proche. | *$0,085* |
| TaxAmount | Montant des taxes facturées. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *$0,08* |
| PostTaxTotal | Total après impôts, le cas échéant. | *$0,93* |
| Symbole monétaire | Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez qu’il correspond à votre première facture, puis après toute mise à jour de la plateforme de facturation majeure. | *0,35* |
| PretaxEffectiveRate | Prix avant impôts par unité. Égal à **PretaxCharges** divisé par **divisé par overagequantity**, arrondi au cent le plus proche. | *$0,08* |
| PostTaxEffectiveRate | Prix après impôts par unité. Égal à **PostTaxTotal** divisé par **divisé par overagequantity**, arrondi au cent le plus proche. Ou, égal à **PretaxEffectiveRate** plus taux d’imposition l’par unité Amoun, arrondi au cent le plus proche. | *$0,08* |
| ChargeType | [Type de frais ou d'](recon-file-charge-types.md) ajustement. | Consultez [types de frais](recon-file-charge-types.md). |
| CustomerBillableAccount | Identificateur de compte unique dans la plateforme de facturation Microsoft. | *1280018095* |
| UsageDate | Date du déploiement du service. | *2/1/2019 0:00* |
| MeteredRegion | Identifie l’emplacement d’un centre de données dans la région (pour les services où cette valeur est applicable et remplie). | *Asie est*, *Sud Asie est*, *Europe du Nord*, Europe de l' *Ouest*, *nord du Centre des États*-Unis, *sud du Centre des États-Unis* |
| MeteredService | Identifie l’utilisation d’un service Azure individuel lorsqu’il n’est pas spécifiquement identifié dans la colonne **ServiceName** . Par exemple, les transferts de données sont signalés comme *Microsoft Azure tous les services* dans la colonne **ServiceName** . | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Sous-titre du champ **MeteredService** qui fournit des éclaircissements supplémentaires sur l’utilisation des services Azure. | *EXTERNAL* |
| Project | Nom défini par le client pour son instance de service. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Nombre de connexions Azure Service Bus qui ont été approvisionnées et utilisées pour un jour donné. | *1,000000 connexions/30 jours* (si vous aviez une connexion configurée individuellement au cours d’un mois de 30 jours), *25 connexions/30 jours – utilisée : 1,000000* (si vous aviez un pack de 25 connexions de service bus approvisionnées et que vous avez utilisé 1 pendant cette journée) |
| CustomerID | Identificateur Microsoft unique du client, au format GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nom de domaine du client. Ce champ peut rester vide jusqu'au deuxième cycle de facturation. | *example.onmicrosoft.com* |
| Unit | Unité du **nom**de la ressource. | *Go* ou *heures* |
