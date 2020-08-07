---
title: Tarifs du plan Azure pour les partenaires fournisseurs de solutions Cloud
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires du programme Fournisseur de solutions Microsoft Cloud peuvent utiliser l’Espace partenaires pour voir le tarif des abonnements relevant du plan Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 980f6429d146757edbab4c97cebfd3616cb48760
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527555"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Tarifs de la nouvelle expérience de commerce du programme Fournisseur de solutions cloud pour Azure

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général
- Agent du support technique
- Agent commercial
- Administrateur de la gestion des utilisateurs

Les tarifs de la nouvelle expérience de commerce Azure du programme Fournisseur de solutions cloud sont publiés dans l’Espace partenaires. Les tarifs sont délivrés de façon dynamique dans un fichier précis en temps réel et les prix sont affichés en USD uniquement. Toutefois, la facturation s’effectue dans la devise prise en charge correspondant à la zone monétaire du client. Pour plus d’informations sur la facturation dans la zone monétaire du client, consultez [Plan Azure – facturation ](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Consulter les tarifs des abonnements dans le cadre des tarifs du plan Azure

1. Dans le menu de l’Espace partenaires sur la gauche, sélectionnez **Vendre** puis **Place de marché**.

2. Dans la page de tarification du plan Azure, sélectionnez le pays pour lequel vous souhaitez obtenir la tarification.

3. En regard de **Type d’exportation**, sélectionnez **Tarification de la consommation de plan Azure**, **Tarification des réservations de plan Azure** ou **Taux FX**. 

>[!NOTE] 
>Les **Taux de change** ne sont pas spécifiques à un pays.

4. En regard de **Tarification pour la date**, sélectionnez la date de votre choix, par exemple, **Actuelle**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="spécifique au pays":::

>[!NOTE] 
>Vous pouvez exporter deux tarifs différents : les tarifs de plan Azure et les tarifs tiers de la Place de marché.

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
|Devise|Devise de la tarification|
|UnitPrice|Prix unitaire|
|PricingTierRangeMin|Pour une tarification à plusieurs niveaux, le prix minimal s’applique|
|PricingTierRangeMax|Pour une tarification à plusieurs niveaux, le prix maximal s’applique|
|EffectiveStartDate|Date de début de la tarification|
|EffectiveEndDate|Date de fin de la tarification|
|MeterIds|ID de compteur de la référence produit|
|MeterType|Type de compteur|
|Balises|Propriétés de l’élément ; pour le tarif du plan Azure, il s’agit d’Azure ou d’Azure et réservations (spécifiquement pour les réservations)|

Vous pouvez exporter les listes de prix du plan Azure à partir de la [page Tarification et offres](https://partner.microsoft.com/dashboard/sell/pricingandoffers) de l’Espace partenaires.

## <a name="tiered-pricing"></a>Tarification à plusieurs niveaux

Certains services de consommation de plan Azure prennent en charge la tarification à plusieurs niveaux. Les partenaires peuvent trouver ces produits et ces références SKU dans la liste des prix du plan Azure. Les éléments qui ont des valeurs dans les colonnes de la plage de niveau tarifaire permettent aux partenaires de comprendre le prix en fonction de l’utilisation. Dans l’exemple ci-dessous qui contient des exemples de données, nous utilisons une référence SKU de produit avec trois niveaux tarifaires.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Dans cet exemple, si 101 unités sont utilisées, le montant facturé serait de 100,80. Les 100 premières unités comptent chacune pour 1 et l’unité suivante est facturée à 0,80.

## <a name="pricing-api-for-azure-plan"></a>API de prix pour le plan Azure

Vous pouvez utiliser l’[API de prix](https://docs.microsoft.com/partner/develop/pricing) pour récupérer par programmation les prix du plan Azure pour la consommation et les réservations. Vous pouvez également récupérer les taux de change.

L’API de prix ne se trouve pas sur le même point de terminaison que les autres API de l’Espace partenaires. Les informations fournies incluent les prix compteur en USD pour les ressources du plan Azure et les prix des réservations appliqués aux abonnements au plan Azure.

Cette API permet également aux partenaires de récupérer les taux de change mensuels dans la mesure où les plans Azure sont uniquement en USD. Vous pouvez utiliser les API pour récupérer les prix et les taux de change pour le mois en cours ou les mois précédents.

>[!NOTE]
> L’API de prix est spécifique aux prix du plan Azure. Il est toujours conseillé d’utiliser l’API RateCard existante et les listes de prix publiées dans la page « Prix et offres » de l’Espace partenaires pour les ressources ou réservations Azure déployées sur des abonnements à des plans non-Azure. L’API de tarification du plan Azure ne prend pas en charge la tarification basée sur le logiciel, sur la Place de marché ou sur les licences, comme Microsoft 365 ou Dynamics 365.

Pour plus d’informations sur les API de prix et de taux de change du plan Azure, consultez la [documentation complète sur l’API de prix](https://docs.microsoft.com/partner/develop/pricing).
