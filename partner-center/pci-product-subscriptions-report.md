---
title: Rapport sur les abonnements de l’espace partenaires
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez ce que vous êtes en train de faire et où vous pouvez améliorer en ce qui concerne les abonnements Cloud que vous vendez ou gérez pour vos clients.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf2663122ca95e8d610c8be792a26682ae1718bf
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276312"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Rapport sur les abonnements au produit disponible dans le tableau de bord Insights de l’espace partenaires

**Rôles appropriés**: administrateur général | Agent d’administration | Visionneuse de rapports | Visionneuse de rapports Executive

Le rapport abonnements aux produits présente des analyses sur les abonnements Cloud que vous avez vendus ou que vous gérez pour vos clients. Il s’agit d’un rapport spécifique à un produit qui comprend les performances des abonnements associés à des produits Cloud tels qu’Office 365, Azure, Dynamics et d’autres.

Vous pouvez consulter les sections suivantes dans le rapport abonnements aux produits.

- Résumé
- Répartition géographique des abonnements
- Tendance d’ajout/d’évolution des abonnements
- Distribution des abonnements par emplacement de partenaire, canal de vente, SKU, type d’attachement de partenaire, segment
- Tendance par État d’abonnement
- Tendance des produits

 > [!NOTE]
 > Ce rapport est disponible dans le tableau de bord Insights. Pour afficher ce rapport, vous devez être affecté à un rôle spécifique dans l’espace partenaires, par exemple administrateur général, administrateur de compte, visionneuse de rapports ou visionneuse de rapports Executive. Pour plus d’informations, consultez l’administrateur général de votre société. les types spécifiques de données de ce rapport peuvent également être disponibles uniquement pour les utilisateurs disposant de privilèges de visionneuse de rapports exécutifs.

## <a name="summary"></a>Résumé

La section Résumé présente une vue instantanée des indicateurs de performance clés (KPI) relatifs aux abonnements vendus ou gérés par vos clients.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Résumé du rapport d’abonnements.":::

Pour plus d’informations sur chaque section du résumé, voir ci-dessous :

- Abonnements :
  - Nombre actuel d’abonnements au produit Cloud vendus ou gérés par vous.
  - Pourcentage de croissance ou de refus d’abonnements au cours de la plage de dates sélectionnée.
  - Le micro-graphique présente une tendance mensuelle du nombre d’abonnements pendant la plage de dates sélectionnée.

- Abonnements actifs :
  - Nombre actuel d’abonnements à un produit Cloud avec utilisation active mesurée en fonction de la télémétrie du produit. Cela exclut tous les abonnements d’essai dans le cas d’abonnements Azure.
  - Croissance en pourcentage ou baisse des abonnements actifs sur la période sélectionnée.
  - Le micro-graphique présente une tendance de mois sur mois des abonnements actifs pendant la plage de dates sélectionnée.

- Abonnements ajoutés :
  - Nombre total d’abonnements client ajoutés (vendus ou gérés) par vous pendant la plage de dates sélectionnée. Les nouveaux abonnements avec état **actif** ou **renouvelé** sont comptabilisés comme des abonnements ajoutés.
  - Croissance en pourcentage ou baisse des abonnements ajoutés au dernier mois complet par rapport au premier mois complet.
  - Le micro-graphique présente une tendance mensuelle des abonnements ajoutés au cours de la plage de dates sélectionnée.

- Abonnements en passe :
  - Le nombre total d’abonnements client a été mis à jour pendant la plage de dates sélectionnée. Les abonnements dont **l’État est** annulé ou **suspendu** dans le mois sont comptabilisés en tant qu’abonnement en cours d’exécution.  
  - Pourcentage d’abonnements ayant été mis à jour au cours de la plage de dates sélectionnée.
  - Le micro-graphique présente une tendance mensuelle des abonnements ayant été réactivés au cours de la plage de dates sélectionnée.

- Abonnements par produit : répartition du nombre d’abonnements actuel par produits Cloud.

## <a name="geographical-spread-of-subscriptions"></a>Répartition géographique des abonnements

La vue **abonnements par géographie** affiche la répartition géographique du nombre total d’abonnements par marché client. Le montant total de l’abonnement comprend les abonnements vendus et les abonnements actifs.

Le tableau **nombre de pays/région** présente le nombre total de pays/régions dans lesquels vous avez des abonnements et le montant par pays des abonnements totaux et actifs.

Vous pouvez rechercher et sélectionner un pays de la grille pour zoomer sur un emplacement de la carte. Appuyez sur l’option de **démarrage** sur la carte pour revenir à la vue d’origine. Pointez sur la carte pour afficher tous les abonnements et les abonnements actifs par pays. Les deux champs de la grille peuvent être triés.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="les abonnements par zone géographique.":::

## <a name="subscription-addschurns"></a>Ajouts/évolutions d’abonnement

Cet affichage présente une tendance des abonnements. Celles-ci sont divisées en différentes catégories (nouvelles, existantes, mises à jour) pour la plage de dates sélectionnée. L’axe des X représente les mois de la plage de dates sélectionnée. L’axe des Y représente le nombre d’abonnements. Les abonnements mis à niveau sont représentés sur l’échelle négative de l’axe des Y. 

L’histogramme empilé présente une répartition des abonnements nouveaux, existants et à l’évolution du mois. Vous pouvez régénérer l’histogramme, décomposées avec des éléments de pile spécifiques. Pour ce faire, sélectionnez ces éléments spécifiques dans la légende. Vous pouvez également utiliser le curseur en haut du graphique pour effectuer un zoom avant sur une période spécifique.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="les ajouts et les évolutions de l’abonnement.":::

## <a name="subscription-distribution"></a>Distribution des abonnements

Cet affichage présente la répartition de vos abonnements actuels par vos emplacements MPN, les segments de clientèle, le modèle de tarification des ventes/Azure et le type d’attribution (par exemple, DPOR, DAP, etc.). Sélectionnez les onglets respectifs pour afficher la répartition selon ces catégories. Pour créer le graphique à secteurs avec une répartition de catégories d’éléments spécifiques, sélectionnez ces catégories d’éléments dans la légende.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribution des abonnements.":::

## <a name="subscription-state-distribution"></a>Distribution de l’état de l’abonnement

Cet affichage montre la répartition de vos abonnements clients actuels par État ou état d’abonnement. Cela comprend les États **d'** abonnement suivants : **actif**, **désactivé**, en **service**, **ouvert**, **InGracePeriod**, **fermé**, etc.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribution de l’état de l’abonnement.":::

## <a name="products-trend"></a>Tendance des produits

Cet affichage montre un graphique à barres et deux graphiques à secteurs. Le graphique à barres présente une tendance mensuelle des abonnements répartis par produits commerciaux, tels qu’Azure, Office, Dynamics, etc.

Les deux graphiques en secteurs affichent une répartition de vos abonnements client actuels. Le premier graphique à secteurs décompose les abonnements par produits. Le second graphique divise les abonnements par références SKU ou plans. Lorsque vous sélectionnez un produit dans le graphique à secteurs décomposition **par produits** , le graphique à secteurs adjacents affiche une répartition des abonnements de ce produit par SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendances des produits.":::

> [!NOTE]
 > Le nombre d’abonnements divisé par SKU peut ne pas toujours correspondre au nombre total d’abonnements pour ce produit. Cela peut se produire si un client a acheté plusieurs références SKU sous le même abonnement au produit.

## <a name="next-steps"></a>Étapes suivantes

- Pour obtenir d’autres rapports, consultez la section Insights de l' [espace partenaires](partner-center-insights.md).

>[!NOTE] 
> Vous pouvez télécharger les données brutes qui alimentent ce rapport à partir de la section Télécharger des rapports dans le tableau de bord Insights. [En savoir plus](pci-download-reports.md) 
