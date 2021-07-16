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
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="09903-103">Exemples de requêtes pour le rapport des Insights de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="09903-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="09903-104">cet article fournit des exemples de requêtes pour les rapports de Informations de partenaire.</span><span class="sxs-lookup"><span data-stu-id="09903-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="09903-105">Vous pouvez utiliser ces requêtes en appelant le point de terminaison de l’API Créer une requête de rapport.</span><span class="sxs-lookup"><span data-stu-id="09903-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="09903-106">Si nécessaire, l’appel de l' [API de création de requête de rapport](insights-programmatic-access-paradigm.md#create-report-query-api) peut être modifié pour ajouter d’autres colonnes, ajuster la période de calcul et ajouter des conditions de filtre.</span><span class="sxs-lookup"><span data-stu-id="09903-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="09903-107">Pour plus d’informations sur les noms de colonnes, les attributs et les descriptions, reportez-vous aux [définitions de données](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="09903-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="09903-108">Détails du client</span><span class="sxs-lookup"><span data-stu-id="09903-108">Customer details</span></span>

<span data-ttu-id="09903-109">Ces exemples de requêtes s’appliquent au rapport Détails des clients :</span><span class="sxs-lookup"><span data-stu-id="09903-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="09903-110">Par zone géographique</span><span class="sxs-lookup"><span data-stu-id="09903-110">By geography</span></span>

<span data-ttu-id="09903-111">Liste des clients d’une zone géographique spécifique au cours du mois dernier.</span><span class="sxs-lookup"><span data-stu-id="09903-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="09903-112">Par référence (SKU) et revenu facturé</span><span class="sxs-lookup"><span data-stu-id="09903-112">By SKU and billed revenue</span></span>

<span data-ttu-id="09903-113">La liste des clients utilisant une référence SKU spécifique et le chiffre d’affaires facturé est supérieure à 20 000 au cours des 6 derniers mois</span><span class="sxs-lookup"><span data-stu-id="09903-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="09903-114">Par sièges disponibles</span><span class="sxs-lookup"><span data-stu-id="09903-114">By available seats</span></span>

<span data-ttu-id="09903-115">10 principaux clients basés sur les sièges disponibles au cours du mois dernier</span><span class="sxs-lookup"><span data-stu-id="09903-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="09903-116">Profil de partenaire</span><span class="sxs-lookup"><span data-stu-id="09903-116">Partner Profile</span></span>

<span data-ttu-id="09903-117">Ces exemples de requêtes s’appliquent au rapport profil de partenaire :</span><span class="sxs-lookup"><span data-stu-id="09903-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="09903-118">Par zone géographique</span><span class="sxs-lookup"><span data-stu-id="09903-118">By geography</span></span>

<span data-ttu-id="09903-119">Liste des partenaires d’une zone géographique spécifique.</span><span class="sxs-lookup"><span data-stu-id="09903-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="09903-120">Par partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="09903-120">By MPN partner</span></span>

<span data-ttu-id="09903-121">Liste des partenaires sous le même partenaire MPN PGA</span><span class="sxs-lookup"><span data-stu-id="09903-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="09903-122">Performances du revendeur</span><span class="sxs-lookup"><span data-stu-id="09903-122">Reseller Performance</span></span>

<span data-ttu-id="09903-123">Ces exemples de requêtes s’appliquent au rapport des performances du revendeur :</span><span class="sxs-lookup"><span data-stu-id="09903-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="09903-124">Par zone géographique</span><span class="sxs-lookup"><span data-stu-id="09903-124">By geography</span></span>

<span data-ttu-id="09903-125">Liste des revendeurs d’une zone géographique spécifique au cours du mois dernier.</span><span class="sxs-lookup"><span data-stu-id="09903-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="09903-126">Par revendeur</span><span class="sxs-lookup"><span data-stu-id="09903-126">By reseller</span></span>

<span data-ttu-id="09903-127">Nombre de clients, nombre d’abonnements, total des sièges disponibles, nombre total de sièges affectés, chiffre d’affaires total pour un revendeur spécifique.</span><span class="sxs-lookup"><span data-stu-id="09903-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="09903-128">10 premiers par chiffre d’affaires</span><span class="sxs-lookup"><span data-stu-id="09903-128">Top 10 by revenue</span></span>

<span data-ttu-id="09903-129">Les 10 principaux revendeurs en fonction du chiffre d’affaires total au cours du mois dernier.</span><span class="sxs-lookup"><span data-stu-id="09903-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="09903-130">Détails de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="09903-130">Subscription Details</span></span>

<span data-ttu-id="09903-131">Ces exemples de requêtes s’appliquent au rapport Détails de l’abonnement :</span><span class="sxs-lookup"><span data-stu-id="09903-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="09903-132">Par éligibilité du renouvellement</span><span class="sxs-lookup"><span data-stu-id="09903-132">By renewal eligibility</span></span>

<span data-ttu-id="09903-133">Liste des abonnements qui ne peuvent pas être renouvelés automatiquement au cours du mois dernier.</span><span class="sxs-lookup"><span data-stu-id="09903-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="09903-134">Par État d’abonnement</span><span class="sxs-lookup"><span data-stu-id="09903-134">By subscription state</span></span>

<span data-ttu-id="09903-135">Liste des abonnements qui sont en état de désactivation au cours du mois dernier.</span><span class="sxs-lookup"><span data-stu-id="09903-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="09903-136">Nombre de six mois</span><span class="sxs-lookup"><span data-stu-id="09903-136">Counts for six months</span></span>

<span data-ttu-id="09903-137">Nombre d’abonnements, total des sièges vendus et nombre de clients pour un partenaire spécifique au cours des six derniers mois.</span><span class="sxs-lookup"><span data-stu-id="09903-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="09903-138">Utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="09903-138">Azure Usage</span></span>

<span data-ttu-id="09903-139">Ces exemples de requêtes s’appliquent au rapport d’utilisation Azure :</span><span class="sxs-lookup"><span data-stu-id="09903-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="09903-140">Par catégorie de compteur</span><span class="sxs-lookup"><span data-stu-id="09903-140">By meter category</span></span>

<span data-ttu-id="09903-141">Liste des abonnements d’utilisation Azure avec unités d’utilisation et ACR pour une catégorie de compteur spécifique au cours des six derniers mois.</span><span class="sxs-lookup"><span data-stu-id="09903-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="09903-142">Par ACR total</span><span class="sxs-lookup"><span data-stu-id="09903-142">By total ACR</span></span>

<span data-ttu-id="09903-143">Liste des abonnements d’utilisation Azure où le ACR total est supérieur à 20 000 au cours des six derniers mois</span><span class="sxs-lookup"><span data-stu-id="09903-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="09903-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="09903-144">Next steps</span></span>

- [<span data-ttu-id="09903-145">API permettant d’accéder aux données analytiques de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="09903-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)