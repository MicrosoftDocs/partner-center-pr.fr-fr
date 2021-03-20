---
title: Fichiers de rapprochement basés sur l’utilisation
ms.topic: article
ms.date: 06/08/2020
description: En savoir plus sur tous les éléments de votre fichier de réconciliation basé sur l’utilisation dans l’espace partenaires. Contient quelques exemples.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 403b2704c600f21fc06576e679ff538a74ae5046
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712968"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Comprendre les fichiers de rapprochement basés sur l’utilisation et leurs champs spécifiques dans l’espace partenaires

**Rôles appropriés**

- Administrateur des comptes
- Administrateur de la facturation

Pour concilier vos frais par rapport à l’utilisation d’un client, comparez les **ResellerID**, **nom du revendeur** et **ResellerBillableAccount** du fichier de réconciliation avec le **nom du client** et l’ID d' **abonnement** de l’espace partenaires.

## <a name="fields-in-usage-based-reconciliation-files"></a>Champs dans les fichiers de réconciliation basés sur l’utilisation

Les champs suivants décrivent les services utilisés et leurs taux.

| Colonne | Description | Exemple de valeur (s) |
| ------ | ----------- | ------------ |
| PartnerId | Identificateur du partenaire, au format GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nom du partenaire. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificateur du compte du partenaire. | *1010578050* |
| CustomerCompanyName | Nom de l’organisation du client comme indiqué dans l’espace Partenaires. *Très important pour rapprocher la facture de vos informations système.* | *Tester le client* |
| MpnId | Identificateur MPN du partenaire CSP. | *4390934* |
| ResellerMpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement.  |
| InvoiceNumber | Numéro de facture sur lequel figure la transaction spécifiée. | *D020001IVK* |
| ChargeStartDate | Date de début du cycle de facturation, sauf en cas de dates de données d’utilisation latente non facturées précédemment (du cycle de facturation précédent). L’heure est toujours définie sur le début de la journée, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Date de fin du cycle de facturation, sauf en cas de dates de données d’utilisation latente non facturées précédemment (du cycle de facturation précédent). L’heure indique toujours la fin de la journée, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. *Ce n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Surnom de l’offre de service. | *Microsoft Azure* |
| SubscriptionDescription | Secteur d’activité de l’offre de service. | *Microsoft Azure* |
| OrderID | Identificateur unique d’une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *566890604832738111* |
| NomService | Nom du service Azure en question. | *MACHINES VIRTUELLES* |
| ServiceType | Type spécifique du service Azure. | *Service bus – individuel ou Pack*, *SQL Azure base de données – édition Business ou Web* |
| ResourceGuid | Identificateur unique spécifique pour toute la structure de données et de tarification de service. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Nom_ressource | Nom de la ressource Azure. | *Transfert de données dans (Go)*, *transfert de données sortant (Go)* |
| Région | Région à laquelle l’utilisation s’applique. Principalement utilisé pour affecter des tarifs aux transferts de données, car les tarifs varient selon la région. | *Asie-Pacifique*, *Europe*, *Amérique latine* *Amérique du Nord* |
| Sku | Identificateur Microsoft unique pour une offre. | *7UD-00001* |
| DetailLineItemId | Identificateur et quantité pour dénombrer les différents taux d’un service ou d’une ressource dans une période de facturation donnée. Pour la tarification hiérarchisée Azure, il peut y avoir un tarif pour une certaine quantité d’unités facturables, puis un taux différent après cette quantité. | *1* |
| ConsumedQuantity | Quantité de service utilisée (par exemple, heures ou Go) pendant la période de rapport. Inclut également toute utilisation non facturée pour des périodes de rapport précédentes. | *11* |
| IncludedQuantity | Unités incluses dans le cadre de l’offre. En général absents du CSP. | *0* |
| OverageQuantity | Unités non incluses dans le cadre de l’offre. Celles-ci doivent être payées par le partenaire. Égal à **ConsumedQuantity** moins **IncludedQuantity**. | *11* |
| ListPrice | Prix de l’offre en vigueur à la date de début de l’abonnement. | *$0.0808* |
| PretaxCharges | Égal à **ListPrist** multiplié par **divisé par overagequantity**, arrondi au cent le plus proche. | *$0.085* |
| TaxAmount | Montant des taxes facturées. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *$0,08* |
| PostTaxTotal | Total après les taxes, lorsque des taxes s’appliquent. | *$0,93* |
| Devise | Type de devise. Chaque entité de facturation n’a qu’une seule devise. Vérifiez qu’il correspond à votre première facture, puis après toute mise à jour de la plateforme de facturation majeure. | *EUR* |
| PretaxEffectiveRate | Tarif unitaire avant impôts. Égal à **PretaxCharges** divisé par **divisé par overagequantity**, arrondi au cent le plus proche. | *$0,08* |
| PostTaxEffectiveRate | Tarif unitaire après impôts. Égal à **PostTaxTotal** divisé par **divisé par overagequantity**, arrondi au cent le plus proche. Ou, égal à **PretaxEffectiveRate** plus le taux d’imposition par montant unitaire, arrondi au cent le plus proche. | *$0,08* |
| ChargeType | [Type de frais ou d'](recon-file-charge-types.md) ajustement. | Consultez [types de frais](recon-file-charge-types.md). |
| CustomerId | Identificateur Microsoft unique du client, au format GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nom de domaine du client. Ce champ peut apparaître vide jusqu’au deuxième cycle de facturation. | *example.onmicrosoft.com* |
| BillingCycleType | Fréquence de facturation.| **Tous les mois**  |
| Unité | Unité du **nom** de la ressource. | *Go* ou *heures* |
| CustomerBillableAccount | Identificateur de compte unique dans la plateforme de facturation Microsoft. | *1280018095* |
| UsageDate | Date de déploiement du service. | *2/1/2019 0:00* |
| MeteredRegion | Identifie l’emplacement d’un centre de données dans la région (pour les services où cette valeur est applicable et remplie). | *Asie est*, *Sud Asie est*, *Europe du Nord*, Europe de l' *Ouest*, *nord du Centre des États*-Unis, *sud du Centre des États-Unis* |
| MeteredService | Identifie l’utilisation d’un service Azure individuel lorsqu’il n’est pas spécifiquement identifié dans la colonne **ServiceName** . Par exemple, les transferts de données sont signalés comme *Microsoft Azure tous les services* dans la colonne **ServiceName** . | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Sous-titre du champ **MeteredService** qui fournit des éclaircissements supplémentaires sur l’utilisation des services Azure. | *EXTERNAL* |
| Project | Nom défini par le client pour son instance de service. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Nombre de connexions Azure Service Bus qui ont été approvisionnées et utilisées pour un jour donné. | *1,000000 connexions/30 jours* (si vous aviez une connexion configurée individuellement au cours d’un mois de 30 jours), *25 connexions/30 jours – utilisée : 1,000000* (si vous aviez un pack de 25 connexions de service bus approvisionnées et que vous avez utilisé 1 pendant cette journée) |

## <a name="next-steps"></a>Étapes suivantes

- [Comprendre les champs des fichiers de rapprochement basés sur les licences de l’espace partenaires](license-based-recon-files.md)