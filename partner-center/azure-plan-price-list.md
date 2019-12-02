---
title: Tarifs du plan Azure | Espace partenaires
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment utiliser l’Espace partenaires pour voir la liste de prix des abonnements dans le cadre du plan Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: f06b4b625f84ab6115f0c16de6814a991513435c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252680"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Tarifs de la nouvelle expérience de commerce du programme Fournisseur de solutions cloud pour Azure 

Les tarifs de la nouvelle expérience de commerce Azure du programme Fournisseur de solutions cloud sont publiés dans l’Espace partenaires. Les tarifs sont délivrés de façon dynamique dans un fichier précis en temps réel et les prix sont affichés en USD uniquement. Toutefois, la facturation s’effectue dans la devise prise en charge correspondant à la zone monétaire du client. Pour plus d’informations sur la facturation dans la zone monétaire du client, consultez [Plan Azure – facturation ](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Consulter les tarifs des abonnements dans le cadre des tarifs du plan Azure

1. Dans le menu de l’Espace partenaires sur la gauche, sélectionnez **Vendre** puis **Place de marché**.

2. Dans la page de tarification du plan Azure, sélectionnez le pays pour lequel vous souhaitez obtenir la tarification.

3. En regard de **Type d’exportation**, sélectionnez **Tarification de la consommation de plan Azure**, **Tarification des réservations de plan Azure** ou **Taux FX**. Remarque: Les **Taux de change** ne sont pas spécifiques à un pays.

3. En regard de **Tarification pour la date**, sélectionnez la date de votre choix, par exemple, **Actuelle**. 


![spécifique au pays](images/azure/pricingnew.png)

Remarque: Vous pouvez exporter deux tarifs différents : les tarifs de plan Azure et les tarifs tiers de la Place de marché. 

## <a name="azure-price-list-specifics"></a>Détail des tarifs Azure

- Les tarifs du plan Azure sont disponibles dans la page Place de marché de l’Espace partenaires, sous **Vendre**.

- Des exportations sont disponibles pour les services de consommation du plan Azure, les réservations Azure et les taux de change.

- Les options d’exportation incluent les suivantes :

    - **Tarification du jour** : Elle comprend tous les compteurs et la tarification du 1er du mois jusqu’à la date actuelle du mois en cours. Elle comprend les nouveaux prix, les prix modifiés et les prix supprimés. Tous les prix ont des dates de début et de fin effectives qui indiquent s’ils sont nouveaux ou supprimés.

    - **Tarification du mois précédent** : Les téléchargements de chaque type de ressource sont effectués par mois. Pour les fichiers des prix, cela inclut tous les compteurs qui étaient disponibles au cours de ce mois. Si un nouveau compteur est apparu au milieu du mois, il apparaît sous forme de compteur avec une date de prise d’effet reflétant sa disponibilité. Il en va de même pour les prix qui sont abandonnés, affichés avec une date de fin effective indiquant le moment où ils ne sont plus disponibles.

    - **Taux Fx** : Les taux de change sont disponibles au téléchargement le jour avant le 1er du mois, à 18h00 PST. Par exemple, si vous voulez les taux de novembre, téléchargez-les le 31 octobre. Les taux de change du mois précédent sont également disponibles.

- Les prix figurant dans les tarifs sont les prix directs. Certains partenaires peuvent être éligibles aux crédits Partenaires. Pour obtenir des informations sur la façon de calculer le crédit Partenaires, lisez [Calcul et paiement du crédit Partenaires](partner-earned-credit-explanation.md).

- **Services éligibles** : Le crédit Partenaires s’applique aux services figurant dans les **tarifs de la consommation de plan Azure** que les partenaires peuvent exporter à partir de la page des [tarifs du plan Azure](https://partner.microsoft.com/commerce/sales). Notez qu’il existe des exceptions incluant, sans toutefois s’y limiter, les produits tiers identifiés en tant que « Tiers » dans la colonne Étiquettes des tarifs de consommation de plan Azure et les réservations de plan Azure.

## <a name="price-list-data"></a>Données des tarifs

|**Champ**   |**Description**   |
|--------------------------|:---------------------------|
|ProductTitle  |Titre ou nom du produit|
|ProductID   |ID du produit|
|SKuId|ID de référence SKU|
|SkuTitle|Titre ou nom de la référence SKU|
|Éditeur|La première partie est toujours Microsoft|
|SkuDescription|Description de la référence SKU|
|UnitOfMeasure|Unités qui seront imputées ou facturées|
|TermDuration|Pour les produits basés sur un délai, longueur du délai qui s’applique aux réservations|
|Marché|Marché de la tarification|
|Symbole monétaire|Devise de la tarification|
|UnitPrice|Prix unitaire|
|PricingTierRangeMin|Pour une tarification à plusieurs niveaux, le prix minimal s’applique|
|PricingTierRangeMax|Pour une tarification à plusieurs niveaux, le prix maximal s’applique|
|EffectiveStartDate|Date de début de la tarification|
|EffectiveEndDate|Date de fin de la tarification|
|MeterIds|ID de compteur de la référence produit|
|MeterType|Type de compteur|
|Balises|Propriétés de l’élément ; pour le tarif du plan Azure, il s’agit d’Azure ou d’Azure et réservations (spécifiquement pour les réservations)|

Pour le détail des [informations tarifaires](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
