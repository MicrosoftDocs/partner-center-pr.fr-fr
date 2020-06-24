---
title: Plan Azure – Gérer les abonnements et les ressources
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires peuvent utiliser différentes options de contrôle d’accès basé sur les rôles (RBAC) pour bénéficier d’une gestion et d’un contrôle opérationnels sur les ressources Azure d’un client.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: b0b66a5fc2c51c8e1e4ef282ffebae68758df428
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84908987"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Gérer les abonnements et les ressources dans le cadre du plan Azure

Quand vous opérez la transition d’un client vers le plan Azure, des droits d’administrateur privilégié vous sont attribués par défaut dans Azure (droits de propriétaire d’abonnement via les privilèges Administrateur au nom de).

 > [!NOTE]
 > Le client peut supprimer les droits d’administrateur sur l’abonnement Azure au niveau d’un abonnement, d’un groupe de ressources ou d’une charge de travail. 

 Les partenaires peuvent bénéficier d’une gestion et d’un contrôle opérationnels 24 h/24 et 7 j/7 sur les ressources Azure d’un client dans le cadre du programme Fournisseur de solutions Cloud en utilisant les différentes options fournies via la fonctionnalité RBAC (contrôle d’accès en fonction du rôle). 

- **Administrateur pour le compte de (AOBO)**  : avec les privilèges [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), tout utilisateur ayant le rôle d’agent d’administration dans le locataire de partenaire dispose d’un accès propriétaire RBAC aux abonnements Azure que vous créez dans le programme Fournisseur de solutions Cloud.

- **Azure Lighthouse** : les privilèges AOBO ne permettent pas de créer des groupes distincts qui fonctionnent avec différents clients, ni d’activer des rôles distincts pour les groupes ou les utilisateurs. En utilisant Azure Lighthouse, vous pouvez affecter différents groupes à différents clients ou rôles. Sachant que les utilisateurs disposent du niveau d’accès approprié via la gestion de ressources déléguée Azure, vous pouvez réduire le nombre d’utilisateurs ayant le rôle d’agent d’administration (et donc disposer d’un accès AOBO complet). Cela contribue à améliorer la sécurité en limitant les accès inutiles aux ressources de vos clients. Cela permet aussi de gérer plusieurs clients selon les besoins avec une plus grande souplesse. Pour plus d’informations, consultez [Azure Lighthouse et le programme Fournisseur de solutions cloud](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).

-  **Annuaire ou utilisateurs invités ou [principaux de services](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)**  : vous pouvez déléguer un accès précis aux abonnements CSP en ajoutant des utilisateurs dans l’annuaire du client ou en ajoutant des utilisateurs invités et en attribuant des rôles RBAC spécifiques. 

À des fins de sécurité, Microsoft recommande d’attribuer aux utilisateurs des autorisations minimales pour effectuer leur travail. Consultez [Ressources Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure). 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Lier votre ID partenaire (ID MPN) à vos informations d’identification pour gérer les ressources Azure du client

Le tableau suivant présente les différentes méthodes permettant d’associer votre ID partenaire à différentes options d’accès RBAC.

|**Catégorie**   |**Scénario**   |**Association de l’ID MPN**|
|-----------------|:------------------------|:------------------|
|AOBO   |Le fournisseur indirect ou le partenaire direct CSP crée l’abonnement pour le client, ce qui fait du fournisseur indirect ou du partenaire direct CSP le propriétaire par défaut de l’abonnement en utilisant les privilèges AOBO ; le fournisseur indirect ou le partenaire direct CSP accorde au revendeur indirect un accès à l’abonnement en utilisant les privilèges AOBO.|Automatique (aucun travail nécessaire de la part du partenaire)|
|Azure Lighthouse|Le partenaire crée une [offre Services managés sur la Place de marché ](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers). Cette offre est acceptée au niveau de l’abonnement CSP et le partenaire obtient un accès à l’abonnement CSP.|Automatique (aucun travail nécessaire de la part du partenaire)|
|Azure Lighthouse|Le partenaire déploie un [modèle ARM](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) dans un abonnement Azure.|Le partenaire doit associer l’ID MPN à l’utilisateur ou au principal du service du locataire du partenaire. Pour plus d’informations, consultez [Lier un ID partenaire](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|
|Annuaire ou utilisateur invité|Le partenaire crée un utilisateur ou un principal du service dans l’annuaire du client et accorde à l’utilisateur un accès à l’abonnement CSP. Le partenaire crée un utilisateur ou un principal du service dans l’annuaire du client. Le partenaire ajoute l’utilisateur à un groupe et accorde au groupe un accès à l’abonnement CSP.|Le partenaire doit associer l’ID MPN à l’utilisateur ou au principal du service du locataire du client. Pour plus d’informations, consultez [Lier un ID partenaire](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Vérifier que vous disposez d’un accès administrateur

Vous avez besoin d’un accès administrateur pour gérer les services de votre client et obtenir des crédits. Consultez [Crédits Partenaires](partner-earned-credit.md) pour plus d’informations sur les crédits obtenus. Vous pouvez savoir si vous disposez d’un accès administrateur de deux façons différentes.

- Examinez le fichier d’utilisation quotidienne – Le prix unitaire et le prix unitaire effectif qui y figurent vous permettent de déterminer si une remise est appliquée. Si vous bénéficiez d’une remise, cela signifie que vous êtes l’administrateur.

- Créez une alerte Azure Monitor – Vous pouvez créer une [alerte](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) dans le journal d’activité Azure Monitor pour être informé de la suppression de votre accès RBAC de l’abonnement CSP.

### <a name="create-an-azure-monitor-alert"></a>Créer une alerte Azure Monitor

1. Créez une alerte.

:::image type="content" source="images/azure/azurealert1.png" alt-text="alerte Azure":::

2. Sélectionnez le type d’action que vous souhaitez appliquer à l’alerte. Par exemple, si vous indiquez vouloir recevoir un e-mail, vous recevrez un message électronique pour vous informer de la suppression d’une attribution de rôle.

:::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="configurer l’alerte":::

### <a name="aobo-removal"></a>Suppression des privilèges AOBO

Les clients peuvent gérer l’accès à leur abonnement en accédant à **Contrôle d’accès** sur le portail Azure. Sous l’onglet **Attributions de rôles**, ils sélectionnent **Supprimer l’accès**. Dans ce cas, vous pouvez :

- Demander à votre client si l’accès administrateur peut être rétabli.
- Utiliser l’accès accordé via le [contrôle d’accès basé sur les rôles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview).
- Utiliser l’accès accordé via [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

L’accès basé sur les rôles se distingue de l’accès administrateur. Les rôles délimitent précisément ce que vous pouvez faire et ne pas faire. L’accès administrateur est plus étendu.

Pour connaître les rôles éligibles au crédit Partenaires, consultez [Rôles et autorisations nécessaires pour le crédit Partenaires](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).




**Pour plus d’informations**

- [Révocation et rétablissement des privilèges d’administrateur pour les abonnements Azure CSP](revoke-reinstate-csp.md)

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)

- [Crédit Partenaires pour les services managés](partner-earned-credit-explanation.md)