---
title: Tarifs du plan Azure | Espace partenaires
ms.topic: article
ms.date: 10/15/2019
description: Comment afficher les tarifs des abonnements dans le cadre du plan Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 64f7b6930f31afc63397ae3ed0e0dba2357b0f1e
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171278"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Tarifs de la nouvelle expérience de commerce du programme Fournisseur de solutions cloud pour Azure 

Les tarifs de la nouvelle expérience de commerce Azure du programme Fournisseur de solutions cloud sont publiés dans l’Espace partenaires. Les tarifs sont délivrés de façon dynamique dans un fichier précis en temps réel et les prix sont affichés en USD uniquement. La facturation, toutefois, s’effectue dans la devise prise en charge correspondant à la zone monétaire du client. Pour plus d’informations sur la facturation dans la zone monétaire du client, consultez [Plan Azure – facturation ](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Consulter les tarifs des abonnements dans le cadre des tarifs du plan Azure

1. Dans le menu de l’Espace partenaires sur la gauche, sélectionnez **Vendre** puis **Place de marché**.

2. En regard de **Type d’exportation**, sélectionnez **Tarification de la consommation de plan Azure**.

3. En regard de **Tarification pour la date**, sélectionnez la date de votre choix, par exemple, **Actuelle**. Remarque : Vous pouvez également sélectionner **Taux Fx** pour exporter les taux de change actuels.

![tarification azure 2](images/azure/pricelist2.jpg)

4. Sous **Place de marché**, sélectionnez le **type** et la **catégorie** de produit, ou recherchez un produit. Les produits disponibles correspondant à votre recherche sont affichés.

![pricing](images/azure/Azurepricelist1.jpg)

5. Ensuite, sélectionnez **Exporter les tarifs du plan Azure** pour télécharger les prix du ou des produits que vous sélectionnez dans le cadre du plan Azure.


![exporter les tarifs](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Détail des tarifs Azure

- Les tarifs du plan Azure sont disponibles dans la page Place de marché de l’Espace partenaires, sous **Vendre**.

- Des exportations sont disponibles pour les services de consommation du plan Azure, les réservations Azure et les taux de change.

- Les options d’exportation incluent les suivantes :

    - **Tarification du jour** : Elle comprend tous les compteurs et la tarification du 1er du mois jusqu’à la date actuelle du mois en cours. Elle comprend les nouveaux prix, les prix modifiés et les prix supprimés. Tous les prix ont des dates de début et de fin effectives qui indiquent s’ils sont nouveaux ou supprimés.

    - **Tarification du mois précédent** : Les téléchargements de chaque type de ressource sont effectués par mois. Pour les fichiers des prix, cela inclut tous les compteurs qui étaient disponibles au cours de ce mois. Si un nouveau compteur est apparu au milieu du mois, il apparaît comme un compteur avec une date de prise d’effet reflétant sa disponibilité. Il en va de même pour les prix qui sont abandonnés, affichés avec une date de fin effective indiquant le moment où ils ne sont plus disponibles.

    - **Taux Fx** : Les taux de change sont disponibles au téléchargement le jour avant le 1er du mois, à 18h00 PST. Par exemple, si vous voulez les taux de novembre, téléchargez-les le 31 octobre. Les taux de change du mois précédent sont également disponibles.

    - **Services éligibles** : Le crédit Partenaires s’applique aux services figurant dans les **tarifs de la consommation de plan Azure** que les partenaires peuvent exporter à partir de la page des tarifs du plan Azure. Notez cependant qu’il existe des exceptions, telles que notamment les réservations tierces et Azure.

- Les prix figurant dans les tarifs sont les prix directs. Certains partenaires peuvent être éligibles aux crédits Partenaires. Pour obtenir des informations sur la façon de calculer le crédit Partenaires, lisez [Calcul et paiement du crédit Partenaires](partner-earned-credit-explanation.md).


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
