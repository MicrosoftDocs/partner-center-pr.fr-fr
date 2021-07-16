---
title: Liste des exemples de requêtes
description: Utilisez les exemples de requêtes pour accéder par programmation aux données analytiques de Partner Insights.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375060"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Exemples de requêtes pour le rapport des Insights de l’espace partenaires

cet article fournit des exemples de requêtes pour les rapports de Informations de partenaire. Vous pouvez utiliser ces requêtes en appelant le point de terminaison de l’API Créer une requête de rapport. Si nécessaire, l’appel de l' [API de création de requête de rapport](insights-programmatic-access-paradigm.md#create-report-query-api) peut être modifié pour ajouter d’autres colonnes, ajuster la période de calcul et ajouter des conditions de filtre.

Pour plus d’informations sur les noms de colonnes, les attributs et les descriptions, reportez-vous aux [définitions de données](insights-data-definitions.md).

## <a name="customer-details"></a>Détails du client

Ces exemples de requêtes s’appliquent au rapport Détails des clients :

### <a name="by-geography"></a>Par zone géographique

Liste des clients d’une zone géographique spécifique au cours du mois dernier.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Par référence (SKU) et revenu facturé

La liste des clients utilisant une référence SKU spécifique et le chiffre d’affaires facturé est supérieure à 20 000 au cours des 6 derniers mois

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Par sièges disponibles

10 principaux clients basés sur les sièges disponibles au cours du mois dernier

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Profil de partenaire

Ces exemples de requêtes s’appliquent au rapport profil de partenaire :

### <a name="by-geography"></a>Par zone géographique

Liste des partenaires d’une zone géographique spécifique.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Par partenaire MPN

Liste des partenaires sous le même partenaire MPN PGA

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Performances du revendeur

Ces exemples de requêtes s’appliquent au rapport des performances du revendeur :

### <a name="by-geography"></a>Par zone géographique

Liste des revendeurs d’une zone géographique spécifique au cours du mois dernier.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Par revendeur

Nombre de clients, nombre d’abonnements, total des sièges disponibles, nombre total de sièges affectés, chiffre d’affaires total pour un revendeur spécifique.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>10 premiers par chiffre d’affaires

Les 10 principaux revendeurs en fonction du chiffre d’affaires total au cours du mois dernier.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Détails de l’abonnement

Ces exemples de requêtes s’appliquent au rapport Détails de l’abonnement :

### <a name="by-renewal-eligibility"></a>Par éligibilité du renouvellement

Liste des abonnements qui ne peuvent pas être renouvelés automatiquement au cours du mois dernier.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Par État d’abonnement

Liste des abonnements qui sont en état de désactivation au cours du mois dernier.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Nombre de six mois

Nombre d’abonnements, total des sièges vendus et nombre de clients pour un partenaire spécifique au cours des six derniers mois.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Utilisation d’Azure

Ces exemples de requêtes s’appliquent au rapport d’utilisation Azure :

### <a name="by-meter-category"></a>Par catégorie de compteur

Liste des abonnements d’utilisation Azure avec unités d’utilisation et ACR pour une catégorie de compteur spécifique au cours des six derniers mois.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Par ACR total

Liste des abonnements d’utilisation Azure où le ACR total est supérieur à 20 000 au cours des six derniers mois

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Étapes suivantes

- [API permettant d’accéder aux données analytiques de Partner Insights](insights-programmatic-analytics-available-api.md)