---
title: Crédit Partenaires pour les services managés
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les crédits Partenaires Microsoft pour les services managés sont calculés et payés, et comment vérifier que vous êtes éligible.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622165"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Calcul et paiement du crédit Partenaires

**Rôles appropriés**

- Administrateur général
- Administrateur des utilisateurs
- Agent d’administration
- Administrateur de la facturation
- Agent commercial

Le crédit Partenaires (PEC, partner earned credit) pour les services managés reconnaît et récompense les partenaires qui gère et contrôle les opérations informatiques 24h/24 et 7j/7 de tout ou partie de l’environnent Azure de leurs clients. Par défaut, les partenaires engagés dans le programme Fournisseur de solutions Cloud bénéficient de droits d’accès à l’abonnement du client, ce qui leur permet de gérer et de contrôler les opérations 24 h/24 et 7 j/7 des ressources de l’abonnement. Les autres moyens dont dispose le client pour accorder un accès au partenaire de transactions sont décrits dans la section suivante. Le montant de facturation mensuelle s’entend hors crédit Partenaires. Le partenaire peut consulter le détail du crédit PEC dans le fichier de rapprochement mensuel. Pour connaître les autres moyens dont dispose les clients pour provisionner un accès au partenaire de transactions, consultez [Gérer les abonnements et les ressources dans le plan Azure](azure-plan-manage.md).

Lire également [Rétablir les privilèges d’administrateur pour les abonnements Azure CSP](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Éligibilité

Pour recevoir le crédit partenaire gagné (PEC), les conditions suivantes s’appliquent : 

- Vous devez avoir un contrat MPN actif et un rôle de contrôle d’accès en fonction du rôle (RBAC) valide pour bénéficier d’un crédit Partenaires pour les ressources Azure que vous gérez.

- Vous devez disposer d’un contrôle et d’une gestion opérationnels 24h/24 et 7j/7 sur les ressources Azure du client dans le cadre du programme Fournisseur de solutions Cloud. Cela signifie que vous devez disposer de privilèges d’administrateur sur l’abonnement Azure, le groupe de ressources Azure et la ressource Azure du client. Dans le cas des fournisseurs indirects et de leurs revendeurs indirects, le fournisseur indirect est éligible au crédit PEC si le fournisseur indirect, le revendeur indirect ou les deux disposent de ce contrôle opérationnel. Pour en découvrir plus à ce sujet, consultez [Rétablir les privilèges d’administrateur pour les abonnements Azure CSP](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).

- En plus des exigences ci-dessus, le crédit PEC n’est applicable qu’aux services figurant dans les tarifs de la consommation de plan Azure, que vous pouvez exporter à partir de la page des [tarifs du plan Azure](https://partner.microsoft.com/commerce/sales).

- Le crédit PEC n’est **pas** applicable aux services suivants :
    - Réservations de plan Azure
    - Produits tiers identifiés comme étant tiers dans la colonne Étiquettes du tarif de consommation de plan Azure
    - Produits figurant dans la liste des prix de la Place de marché
    - [Machines virtuelles Azure Spot](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- Il est possible d’obtenir un crédit PEC jusqu’au niveau des ressources Azure. Si vous avez un accès valide au niveau de l’abonnement ou du groupe de ressources, chaque ressource qui atteint l’entité supérieure obtient un crédit PEC.

- Les détails du crédit PEC sont également disponibles dans la page [Azure Cost Management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners).

### <a name="calculation"></a>Calcul

Le crédit PEC est calculé tous les jours et peut être consulté dans le fichier d’utilisation quotidienne et dans le fichier de rapprochement de facturation mensuelle. Pour obtenir un crédit PEC, le partenaire (fournisseur indirect ou revendeur indirect) doit bénéficier d’un accès tout au long de la journée (24h/24, 7j/7). Le crédit PEC est calculé tous les jours sur la base des ressources Azure managées. Le crédit PEC maximal pour une période de facturation donnée (mois) est de 15 %. Les partenaires qui gardent un accès privilégié persistant pendant tout le mois (plage d’accès) et pour toutes les ressources éligibles (étendue d’accès) obtiennent un crédit PEC total de 15 %. La réduction de l’étendue et de la plage entraîne un taux de PEC plus bas pour le mois. Le fichier d’utilisation évaluée quotidiennement s’affiche tous les jours sur la base d’une ressource Azure, que le crédit PEC soit appliqué ou non. Les partenaires peuvent aussi s’inscrire à des alertes pour superviser les changements apportés à l’accès privilégié persistant.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) avec Cost Analysis vous permet, en tant que partenaire, de voir les coûts qui ont bénéficié du crédit PEC.  

1. Dans le [portail Azure](https://portal.azure.com), connectez-vous à votre locataire partenaire, puis sélectionnez **Cost Management + Facturation**.

2. Sélectionnez **Cost Management**

3. Sélectionnez **Cost Analysis**

   La vue Cost Analysis montre les coûts de votre compte de facturation, pour tous les services achetés et consommés aux prix que vous payez Microsoft.

4. Sélectionnez **PartnerEarnedCreditApplied** dans la liste déroulante d’un graphique croisé dynamique pour voir les coûts auxquels un crédit PEC est appliqué. Quand la propriété **PartnerEarnedCreditApplied** a la valeur True, le coût associé bénéficie du crédit Partenaires. 

   Quand la propriété PartnerEarnedCreditApplied a la valeur False, le coût associé n’a pas répondu aux critères d’éligibilité requise pour le crédit ou le service acheté n’est pas éligible au crédit Partenaires.

   >[!NOTE] 
   >En règle générale, l’utilisation des services prend de 8 à 24 heures pour s’afficher dans **Cost Management**, et les crédits PEC apparaîtront dans les 48 heures à partir de l’heure d’accès dans Azure Cost Management.

5. Vous pouvez également regrouper et filtrer selon la propriété **PartnerEarnedCreditApplied** à l’aide des fonctionnalités de filtre **Group by and Add** (Regrouper par et ajouter) pour analyser les coûts avec un crédit PEC et les coûts auxquels aucun PEC n’est appliqué.

## <a name="next-steps"></a>Étapes suivantes

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)

- Vous trouverez des exemples détaillés de calculs de crédit PEC dans la liste des tarifs à laquelle vous pouvez accéder via le tableau de bord de l’Espace partenaires (connexion nécessaire).

- [Passer au plan Azure – Démarrer](azure-plan-get-started.md)

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)

- [Révoquer ou rétablir les privilèges d’administrateur pour les abonnements Azure CSP](revoke-reinstate-csp.md)
