---
title: Fichiers de réconciliation basés sur une licence | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Comprendre les fichiers de réconciliation basés sur les licences dans l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 617b49556851a4d9999e6294d61d79c4fe1befa1
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389817"
---
# <a name="license-based-reconciliation-files"></a>Fichiers de rapprochement basés sur les licences

S’applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Pour rapprocher vos modifications des commandes d’un client, comparez le **Syndication_Partner_Subscription_Number** du fichier de rapprochement à l' **ID d’abonnement** de l’espace partenaires.

## <a name="fields-in-license-based-reconciliation-files"></a>Champs dans les fichiers de réconciliation basés sur une licence

| colonne | Description | Valeur échantillon |
| ------ | ----------- | ------------ |
| PartnerId | Identificateur unique au format GUID pour une entité de facturation spécifique. Non requis pour le rapprochement. Identique dans toutes les lignes. | *8ddd03642-test-Test-test-46b58d356b4e* |
| CustomerID | Identificateur Microsoft unique du client au format GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Identificateur unique pour une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la commande lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *566890604832738111* |
| SubscriptionID | Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. *Cette valeur n’est pas la même que l' **ID d’abonnement** dans la console d’administration partenaire. Veuillez consulter **SyndicationPartnerSubscriptionNumber** à la place.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificateur unique des abonnements. Un client peut avoir plusieurs abonnements pour le même plan. Cette colonne est importante pour l’analyse des fichiers de réconciliation. Ce champ correspond à l' **ID d’abonnement** dans la console d’administration du partenaire. | *fb977ab5-test-Test-test-24c8d9591708* |
| OfferID | Identificateur d’offre unique. Identificateur d’offre standard, tel que défini dans la liste de prix. *Cette valeur ne correspond pas à l’ID de l' **offre** de la liste de prix. Consultez plutôt **DurableOfferID** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Identificateur unique de l’offre durable, tel que défini dans la liste des prix. *Cette valeur correspond à l’ID de l' **offre** de la liste de prix.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Date de début de l’abonnement. L’heure indique toujours le début de la journée, 0:00. Ce champ est défini sur le jour après l’envoi de la commande. Utilisé conjointement avec le **SubscriptionEndDate** pour déterminer : si le client est encore au cours de la première année de l’abonnement, ou si l’abonnement a été renouvelé pour l’année suivante. | *2/1/2019 0:00* |
| SubscriptionEndDate | Date de fin de l’abonnement. L’heure indique toujours le début de la journée, 0:00. *12 mois plus **x** jours après la date de début* , à aligner sur la date de facturation du partenaire ou sur *12 mois à compter de la date de renouvellement*. Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur. La communication avec les clients peut être nécessaire avant le renouvellement automatique. | *2/1/2019 0:00* |
| ChargeStartDate | Date de début des frais. L’heure indique toujours le début de la journée, 0:00. Utilisé pour calculer les frais quotidiens (*proratas* ) lorsqu’un client change le numéro du siège. | *2/1/2019 0:00* |
| ChargeEndDate | Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59. Utilisé pour calculer les frais quotidiens (*proratas* ) lorsqu’un client change le numéro du siège. | *2/28/2019 23:59* |
| ChargeType | [Type de frais ou d'](recon-file-charge-types.md) ajustement. | Consultez [types de frais](recon-file-charge-types.md). |
| UnitPrice | Prix par siège, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *6,82* |
| Quantité | Nombre de sièges. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *2* |
| Montant | Prix total pour la quantité. Permet de vérifier si le calcul de la quantité correspond à la façon dont vous calculez cette valeur pour vos clients. | *13,32* |
| TotalOtherDiscount | Montant de la remise appliquée à ces frais. Les licences de produits incluses dans une compétence ou des cartes, ou les nouveaux abonnements éligibles à un Incentive, comportent également un montant de remise dans cette colonne. | *2,32* |
| Sous-total | Total avant impôt. Vérifie si votre sous-total correspond au total attendu, en cas de remise. | *11* |
| Taxe | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *0* |
| TotalForCustomer | Total après impôts. Vérifie si les impôts sont retenus sur la facture. | *11* |
| Currency | Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez si elle correspond à votre première facture. Vérifiez à nouveau après toute mise à jour de la plateforme de facturation majeure. | *0,35* |
| CustomerName | Nom de l’organisation du client, tel qu’indiqué dans l’espace partenaires. *Champ très important pour rapprocher la facture de vos informations système.* | *Tester un client A* |
| MPNID | Identificateur MPN du partenaire CSP. Consultez [Comment dénombrer par partenaire](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. Consultez [Comment dénombrer par partenaire](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Nom de domaine du client. Ce champ peut rester vide jusqu'au deuxième cycle de facturation. *N’utilisez pas ce champ comme identificateur unique pour le client. Le client/partenaire peut mettre à jour le personnel ou le domaine par défaut par le biais du portail Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Pseudo d'abonnement. Si aucun surnom n’est spécifié, l’espace partenaires utilise le **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s’agit d’un champ identique à **OfferName**.) | *PROJECT ONLINE PREMIUM SANS CLIENT DE PROJET* |
