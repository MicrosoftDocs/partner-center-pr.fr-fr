---
title: Faire passer les clients des offres Azure actuelles au plan Azure
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires fournisseurs de solutions Cloud peuvent utiliser l’Espace partenaires pour faire passer les clients des offres Azure CSP existantes aux services Azure relevant du plan Azure.
author: mowrim
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: a6f2c3cfe2c19c2764b8149a00c065eb1c429a98
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948390"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Assurer la transition des clients vers le plan Azure à partir des offres Azure CSP existantes

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général
- Agent du support technique
- Agent commercial
- Administrateur de la gestion des utilisateurs

Les fournisseurs indirects et les partenaires de facturation directe peuvent passer à la nouvelle expérience de commerce disponible dans le programme CSP pour Azure. (Les revendeurs indirects devront utiliser leurs fournisseurs indirects.) Les clients pourront acheter des services cloud de façon simplifiée, que ce soit auprès de partenaires, de vendeurs Microsoft ou directement sur le Web.

La possibilité de transition s’adresse uniquement aux clients qui passent à la nouvelle expérience de commerce pour Azure et qui ont signé le Contrat client Microsoft, et non à d’autres offres du programme CSP, comme Office 365 ou Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Passer d’offres CSP existantes à un plan Azure

Vous pouvez faire basculer les offres CSP Azure existantes d’un client vers les services Azure relevant du plan Azure de la nouvelle expérience de commerce du programme CSP, et ce à partir de l’Espace partenaires. Pour cela, le partenaire et le client doivent avoir établi une relation de revendeur via l’Espace partenaires, et le client doit avoir signé le Contrat client Microsoft.

### <a name="select-transition-to-azure-plan"></a>Sélectionner la transition vers le plan Azure

1. Sélectionnez le plan Azure pour votre client.

2. Sélectionnez **Transition de la facturation vers un plan Azure**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Capture d’écran montrant les informations de rapport des abonnements basés sur l’utilisation avec une option sélectionnable appelée : Transition de la facturation de l’abonnement Azure vers un plan Azure.":::

3. Sélectionnez **Continuer**.

   :::image type="content" source="images/azure/transition2.png" alt-text="Boîte de dialogue intitulée Transition vers un plan Azure avec des implications à lire sur la transition, et deux options à sélectionner : Continuer ou Annuler.":::

   Votre client sera transféré vers le plan Azure.

   **Le workflow de transition automatise les étapes prérequises** :

   - Achat d’un ou plusieurs plans Azure
   - Un plan par client dans les scénarios CSP Direct  
   - Un plan par revendeur  

   Par exemple, un partenaire a acheté deux offres Microsoft Azure et a inclus deux partenaires de référence distincts dans l’achat. Dans ce cas, le workflow de transition achète deux plans Azure (un par revendeur) et mappe automatiquement les abonnements Azure respectifs dans le cadre des plans Azure.  

   **Mappage d’un abonnement Azure à un plan Azure**

   Après l’achat d’un ou plusieurs plans Azure, notre système mappe les abonnements Azure existants aux plans Azure. La progression peut être examinée sur le portail Azure et dans l’Espace partenaires.

4. Revenez à la page de **Abonnements** de l’Espace partenaires de votre client pour mettre à jour sa limite budgétaire dans sa devise locale.

   :::image type="content" source="images/azure/transition3.png" alt-text="Vue partielle de la page Abonnements de l’Espace partenaires, avec les limites budgétaires définies en devise locale pour une période de facturation.":::

   >[!NOTE]
   >Le budget que vous définissez dans l’Espace partenaires n’est pas reporté sur le portail Azure. Vous devez aussi définir le budget et l’alerte sur le portail Azure.

   Quand vous passez au plan Azure, vous ne pouvez plus acheter d’abonnements Azure pour ce client. Vous devez créer les abonnements relevant du plan Azure sur le portail Azure.

   >[!NOTE]
   > Tous les abonnements Azure achetés via RBAC dans le plan Azure sont tarifés et facturés en monnaie locale. Les taux de change ne seront pas utilisés.

### <a name="track-your-transition-details"></a>Suivre les détails de votre transition

Vous pouvez suivre la progression de la transition sur le portail Azure et dans l’Espace partenaires.

:::image type="content" source="images/azure/details1.png" alt-text="Capture d’écran montrant le tableau avec la liste des détails de la transition par abonnement : comprend l’ID d’abonnement, la date de la transition et l’état de la transition.":::

### <a name="billing-impact-to-partners"></a>Impact sur la facturation des partenaires

Si vous opérez la transition d’un client à partir d’une offre Azure CSP existante, les impacts sur la facturation seront les suivants :

- Votre facture CSP existante portera sur l’ensemble de votre consommation jusqu’à la date de fin de l’abonnement Azure CSP d’origine.

- Si vous disposiez de droits d’accès d’administrateur à l’abonnement CSP existant, vous continuerez d’y avoir accès une fois la migration de l’abonnement effectuée.

Pour opérer la transition de contrats Entreprise directs vers des inscriptions CSP et Serveur et des inscriptions Cloud vers des services Azure, consultez [Obtenir la propriété de facturation d’abonnements Azure pour un Contrat Partenaire Microsoft](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Journal d’audit

Pour rapprocher la facturation, consultez votre historique des abonnements « Microsoft Azure » (0145P) dans la page **Subscriptions** (Abonnements).

L’abonnement « Microsoft Azure » (0145P) se compose de deux parties :

1. Abonnement Commerce
2. Abonnement Azure (droit d’utilisation)

Une fois la transition terminée, l’abonnement Azure est rattaché à un nouveau plan Azure et l’abonnement Commerce est suspendu de façon à éviter toute communication de consommation supplémentaire.  

>[!NOTE]
>Quand l’abonnement Microsoft Azure (0145P) est acheté dans le cadre du programme CSP, l’abonnement Commerce et l’abonnement Azure (droit d’utilisation) ont la même valeur. Ce n’est qu’en cas de changements ou de transferts de propriété de facturation que les valeurs diffèrent.

### <a name="transition-issues"></a>Problèmes de transition

Pendant les transitions, aucun problème n’est censé se produire selon nous. Si cela devait se produire, nous vous en informerons dans le workflow de transition proprement dit. Il n’y aura aucune perturbation dans l’utilisation d’Azure.  

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)
