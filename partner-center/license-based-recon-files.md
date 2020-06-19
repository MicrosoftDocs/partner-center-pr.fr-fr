---
title: Fichiers de rapprochement basés sur les licences
ms.topic: article
ms.date: 05/18/2020
description: Découvrez comment lire les fichiers de réconciliation basés sur des licences dans l’espace partenaires. Cet article explique la signification de chaque champ dans votre fichier de rapprochement basé sur une licence.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ce9400c3672ff09997321b2e55f46daf102ebbd
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909047"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Comprendre les champs des fichiers de rapprochement basés sur les licences de l’espace partenaires

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**
- Administrateur général
- Administrateur des utilisateurs
- Administrateur de la facturation
- Agent d’administration

Pour rapprocher vos modifications des commandes d’un client, comparez le **Syndication_Partner_Subscription_Number** du fichier de rapprochement à l' **ID d’abonnement** de l’espace partenaires.

## <a name="fields-in-license-based-reconciliation-files"></a>Champs dans les fichiers de réconciliation basés sur une licence

| Colonne | Description | Exemple de valeur |
| ------ | ----------- | ------------ |
| PartnerId | Identificateur unique au format GUID pour une entité de facturation spécifique. Non requis pour le rapprochement. Identique dans toutes les lignes. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Identificateur Microsoft unique du client au format GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’espace Partenaires. *Champ très important pour rapprocher la facture de vos informations système.* | *Client test A* |
| MpnId | Identificateur MPN du partenaire CSP. Consultez [Comment dénombrer par partenaire](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement.  |
| OrderId | Identificateur unique d’une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la commande lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *566890604832738111* |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme de facturation Microsoft. Peut être utile pour identifier l’abonnement lorsque vous contactez le support technique. Non utilisé pour le rapprochement. *Cette valeur n’est pas la même que l' **ID d’abonnement** dans la console d’administration partenaire. Veuillez consulter **SyndicationPartnerSubscriptionNumber** à la place.* | *usCBMgAAAAAAAAIA* |
| Syndication_Partner_Subscription_Number | Identificateur unique des abonnements. Un client peut avoir plusieurs abonnements pour le même plan. Cette colonne est importante pour l’analyse des fichiers de réconciliation. Ce champ correspond à l' **ID d’abonnement** dans la console d’administration du partenaire. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Identificateur d’offre unique. Identificateur d’offre standard, tel que défini dans la liste de prix. *Cette valeur ne correspond pas à l’ID de l' **offre** de la liste de prix. Consultez plutôt **DurableOfferID** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Identificateur unique de l’offre durable, tel que défini dans la liste des prix. *Cette valeur correspond à l’ID de l' **offre** de la liste de prix.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. | *Microsoft Office 365 (Plan&amp;nbsp;E3)* |
| SubscriptionStartDate | Date de début de l’abonnement. L’heure est toujours définie sur le début de la journée, 0:00. Ce champ est défini sur le jour après l’envoi de la commande. Utilisé conjointement avec le **SubscriptionEndDate** pour déterminer : si le client est encore au cours de la première année de l’abonnement, ou si l’abonnement a été renouvelé pour l’année suivante. | *2/1/2019 0:00* |
| SubscriptionEndDate | Date de fin de l’abonnement. L’heure est toujours définie sur le début de la journée, 0:00. *12 mois plus **x** jours après la date de début* , à aligner sur la date de facturation du partenaire ou sur *12 mois à compter de la date de renouvellement*. Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur. La communication avec les clients peut être nécessaire avant le renouvellement automatique. | *2/1/2019 0:00* |
| ChargeStartDate | Date de début des frais. L’heure est toujours définie sur le début de la journée, 0:00. Utilisé pour calculer les frais quotidiens (*proratas* ) lorsqu’un client change le numéro du siège. | *2/1/2019 0:00* |
| ChargeEndDate | Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59. Utilisé pour calculer les frais quotidiens (*proratas* ) lorsqu’un client change le numéro du siège. | *2/28/2019 23:59* |
| ChargeType | [Type de frais ou d'](recon-file-charge-types.md) ajustement. | Consultez [types de frais](recon-file-charge-types.md). |
| UnitPrice | Tarif par siège, tel qu’il a été publié dans le pricelist au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *6,82* |
| Quantité | Nombre de sièges. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *2* |
| Montant | Prix total pour la quantité. Permet de vérifier si le calcul de la quantité correspond à la façon dont vous calculez cette valeur pour vos clients. | *13.32* |
| TotalOtherDiscount | Montant de la remise appliquée à ces frais. Les licences de produits incluses dans une compétence ou des cartes, ou les nouveaux abonnements éligibles à un Incentive, comportent également un montant de remise dans cette colonne. | *2,32* |
| Sous-total | Total avant impôt. Vérifie si votre sous-total correspond au total attendu, en cas de remise. | *11* |
| Taxe | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *0* |
| TotalForCustomer | Total après impôts. Vérifie si les impôts sont retenus sur la facture. | *11* |
| Devise | Type de devise. Chaque entité de facturation n’a qu’une seule devise. Vérifiez si elle correspond à votre première facture. Vérifiez à nouveau après toute mise à jour de la plateforme de facturation majeure. | *EUR* |
| DomainName | Nom de domaine du client. Ce champ peut apparaître vide jusqu’au deuxième cycle de facturation. *N’utilisez pas ce champ comme identificateur unique pour le client. Le client/partenaire peut mettre à jour le personnel ou le domaine par défaut par le biais du portail Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Surnom de l’abonnement. Si aucun surnom n’est spécifié, l’espace partenaires utilise le **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s’agit d’un champ identique à **OfferName**.) | *PROJECT ONLINE PREMIUM SANS PROJECT CLIENT* |
| BillingCycleType | Fréquence de facturation unique.| *Tous les mois* |