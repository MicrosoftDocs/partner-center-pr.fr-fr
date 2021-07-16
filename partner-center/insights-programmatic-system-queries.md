---
title: Liste des requêtes système pour l’accès par programme à un partenaire Insights
description: En savoir plus sur les requêtes système que vous pouvez utiliser pour accéder aux données de l’analytique Partner Insights.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375045"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a><span data-ttu-id="2e3c4-103">Liste des requêtes système pour l’accès par programme à un partenaire Insights</span><span class="sxs-lookup"><span data-stu-id="2e3c4-103">List of system queries for partner insights programmatic access</span></span>

<span data-ttu-id="2e3c4-104">Les requêtes système suivantes peuvent être utilisées dans l' [API de création de rapport](insights-programmatic-access-paradigm.md#create-report-api) directement avec un QueryId.</span><span class="sxs-lookup"><span data-stu-id="2e3c4-104">The following system queries can be used in the [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directly with a QueryId.</span></span> <span data-ttu-id="2e3c4-105">Les requêtes système sont similaires aux rapports d’exportation dans l’espace partenaires pour une période de calcul de six mois (6 M).</span><span class="sxs-lookup"><span data-stu-id="2e3c4-105">The system queries are like the export reports in Partner Center for a six-month (6M) computation period.</span></span>

<span data-ttu-id="2e3c4-106">Pour plus d’informations sur les noms de colonnes, les attributs et la description, reportez-vous aux [définitions de données](insights-data-definitions.md) .</span><span class="sxs-lookup"><span data-stu-id="2e3c4-106">For more details on the column names, attributes, and description, please refer to the [Data Definitions](insights-data-definitions.md)</span></span>

<span data-ttu-id="2e3c4-107">Les sections suivantes fournissent des requêtes de rapport pour différents rapports.</span><span class="sxs-lookup"><span data-stu-id="2e3c4-107">The following sections provide report queries for various reports.</span></span>

## <a name="customers"></a><span data-ttu-id="2e3c4-108">Clients</span><span class="sxs-lookup"><span data-stu-id="2e3c4-108">Customers</span></span>

<span data-ttu-id="2e3c4-109">Rapport des clients pour les six derniers mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-109">The Customers report for the last six months</span></span>

<span data-ttu-id="2e3c4-110">ID de requête : `6664daf3-c161-423a-92a1-0ea6db2c0384`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-110">Query ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-111">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-111">Report query</span></span>
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a><span data-ttu-id="2e3c4-112">Abonnements aux sièges et chiffre d’affaires</span><span class="sxs-lookup"><span data-stu-id="2e3c4-112">Seats Subscriptions and Revenue</span></span>

<span data-ttu-id="2e3c4-113">Rapport sur les sièges, les abonnements et les revenus au cours des six derniers mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-113">Seats, subscriptions, and revenue report for the last six months</span></span>

<span data-ttu-id="2e3c4-114">ID de requête : `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-114">Query ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-115">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-115">Report query</span></span>

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a><span data-ttu-id="2e3c4-116">Profil de partenaire</span><span class="sxs-lookup"><span data-stu-id="2e3c4-116">Partner Profile</span></span>

<span data-ttu-id="2e3c4-117">Données de profil</span><span class="sxs-lookup"><span data-stu-id="2e3c4-117">Profile data</span></span>

<span data-ttu-id="2e3c4-118">ID de requête : `e65f3a4f-fb99-4319-97ff-59e57566a871`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-118">Query ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-119">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-119">Report query</span></span>

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a><span data-ttu-id="2e3c4-120">Utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="2e3c4-120">Azure Usage</span></span>

<span data-ttu-id="2e3c4-121">Rapport AzureUsage pour les six derniers mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-121">AzureUsage report for the last six months</span></span>

<span data-ttu-id="2e3c4-122">ID de requête : `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-122">Query ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-123">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-123">Report query</span></span>

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a><span data-ttu-id="2e3c4-124">Office Syntaxe</span><span class="sxs-lookup"><span data-stu-id="2e3c4-124">Office Usage</span></span>

<span data-ttu-id="2e3c4-125">Rapport OfficeUsage pour les six derniers mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-125">OfficeUsage report for the last six months</span></span>

<span data-ttu-id="2e3c4-126">ID de requête : `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-126">Query ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-127">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-127">Report query</span></span>

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a><span data-ttu-id="2e3c4-128">Utilisation de Dynamics</span><span class="sxs-lookup"><span data-stu-id="2e3c4-128">Dynamics Usage</span></span>

<span data-ttu-id="2e3c4-129">Rapport DynamicsUsage pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-129">DynamicsUsage report for six months</span></span>

<span data-ttu-id="2e3c4-130">ID de requête : `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-130">Query ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-131">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-131">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a><span data-ttu-id="2e3c4-132">Utilisation de Power BI</span><span class="sxs-lookup"><span data-stu-id="2e3c4-132">Power BI usage</span></span>

<span data-ttu-id="2e3c4-133">Rapport PowerBIUsage pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-133">PowerBIUsage report for six months</span></span>

<span data-ttu-id="2e3c4-134">ID de requête : `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-134">Query ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-135">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-135">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a><span data-ttu-id="2e3c4-136">Utilisation d’EMS</span><span class="sxs-lookup"><span data-stu-id="2e3c4-136">EMS Usage</span></span>

<span data-ttu-id="2e3c4-137">Rapport EMSUsage pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-137">EMSUsage report for six months</span></span>

<span data-ttu-id="2e3c4-138">ID de requête : `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-138">Query ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-139">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-139">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a><span data-ttu-id="2e3c4-140">Rapport des exigences de performances des compétences</span><span class="sxs-lookup"><span data-stu-id="2e3c4-140">Competency Performance requirement report</span></span>

<span data-ttu-id="2e3c4-141">Rapport CompetencyPeformanceRequirement pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-141">CompetencyPeformanceRequirement report for six months</span></span>

<span data-ttu-id="2e3c4-142">ID de requête : `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-142">Query ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-143">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-143">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a><span data-ttu-id="2e3c4-144">Performances des revendeurs de produits Cloud</span><span class="sxs-lookup"><span data-stu-id="2e3c4-144">Cloud products reseller performance</span></span>

### <a name="report-description"></a><span data-ttu-id="2e3c4-145">Description du rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-145">Report description</span></span>

<span data-ttu-id="2e3c4-146">Rapport CloudProductsResellerPerformance pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-146">CloudProductsResellerPerformance report for six months</span></span>

<span data-ttu-id="2e3c4-147">ID de requête : `c09c2eda-861b-4664-8ee8-48a14745a26a`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-147">Query ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-148">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-148">Report query</span></span>

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a><span data-ttu-id="2e3c4-149">Propension de renouvellement de l’accord de la Convention</span><span class="sxs-lookup"><span data-stu-id="2e3c4-149">CLAS Agreement Renewal propensity</span></span>

<span data-ttu-id="2e3c4-150">Rapport CLASAgreementRenewalsPropensity pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-150">CLASAgreementRenewalsPropensity report for six months</span></span>

<span data-ttu-id="2e3c4-151">ID de requête : `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-151">Query ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-152">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-152">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a><span data-ttu-id="2e3c4-153">Propension Azure de la CLASSaire</span><span class="sxs-lookup"><span data-stu-id="2e3c4-153">CLAS Azure propensity</span></span>

<span data-ttu-id="2e3c4-154">Rapport CLASAzurePropensity pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-154">CLASAzurePropensity report for six months</span></span>

<span data-ttu-id="2e3c4-155">ID de requête : `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-155">Query ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-156">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-156">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a><span data-ttu-id="2e3c4-157">D365 de la distribution de la</span><span class="sxs-lookup"><span data-stu-id="2e3c4-157">CLAS D365 propensity</span></span>

<span data-ttu-id="2e3c4-158">Rapport CLASD365Propensity pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-158">CLASD365Propensity report for six months</span></span>

<span data-ttu-id="2e3c4-159">ID de requête : `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-159">Query ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-160">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-160">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a><span data-ttu-id="2e3c4-161">M365 de la distribution de la</span><span class="sxs-lookup"><span data-stu-id="2e3c4-161">CLAS M365 propensity</span></span>

<span data-ttu-id="2e3c4-162">Rapport CLASM365Propensity pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-162">CLASM365Propensity report for six months</span></span>

<span data-ttu-id="2e3c4-163">ID de requête : `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-163">Query ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-164">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-164">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a><span data-ttu-id="2e3c4-165">Teams Applications 3P d’utilisation</span><span class="sxs-lookup"><span data-stu-id="2e3c4-165">Teams Usage 3P Apps</span></span>

<span data-ttu-id="2e3c4-166">Rapport TeamsUsage3PApps pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-166">TeamsUsage3PApps report for six months</span></span>

<span data-ttu-id="2e3c4-167">ID de requête : `42d287be-cc76-4109-a066-f3140ad97fe2`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-167">Query ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-168">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-168">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a><span data-ttu-id="2e3c4-169">charge de travail d’utilisation Teams</span><span class="sxs-lookup"><span data-stu-id="2e3c4-169">Teams usage workload</span></span>

<span data-ttu-id="2e3c4-170">Rapport TeamsUsageWorkload pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-170">TeamsUsageWorkload report for six months</span></span>

<span data-ttu-id="2e3c4-171">ID de requête : `817fe875-acb0-4c45-9201-b7a35a60235a`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-171">Query ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-172">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-172">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a><span data-ttu-id="2e3c4-173">réunions et appels de l’utilisation de Teams</span><span class="sxs-lookup"><span data-stu-id="2e3c4-173">Teams usage meetings and calls</span></span>

<span data-ttu-id="2e3c4-174">Rapport TeamsUsageMeetingsAndCalls pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-174">TeamsUsageMeetingsAndCalls report for six months</span></span>

<span data-ttu-id="2e3c4-175">ID de requête : `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-175">Query ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-176">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-176">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a><span data-ttu-id="2e3c4-177">Historique récapitulatif des compétences</span><span class="sxs-lookup"><span data-stu-id="2e3c4-177">Competency summary history</span></span>

<span data-ttu-id="2e3c4-178">Rapport CompetencySummaryHistory pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-178">CompetencySummaryHistory report for six months</span></span>

<span data-ttu-id="2e3c4-179">ID de requête : `fddab2aa-523d-47f6-90fe-588557306db4`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-179">Query ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-180">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-180">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a><span data-ttu-id="2e3c4-181">Fin de l’apprentissage</span><span class="sxs-lookup"><span data-stu-id="2e3c4-181">Training completion</span></span>

<span data-ttu-id="2e3c4-182">Rapport d’achèvement des formations pendant six mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-182">Training Completions report for six months</span></span>

<span data-ttu-id="2e3c4-183">ID de requête : `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-183">Query ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-184">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-184">Report query</span></span>

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a><span data-ttu-id="2e3c4-185">Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="2e3c4-185">Microsoft Learn</span></span>

<span data-ttu-id="2e3c4-186">Microsoft Learn rapport au cours des six derniers mois</span><span class="sxs-lookup"><span data-stu-id="2e3c4-186">Microsoft Learn report for the last six months</span></span>

<span data-ttu-id="2e3c4-187">ID de requête : `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span><span class="sxs-lookup"><span data-stu-id="2e3c4-187">Query ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span></span>

### <a name="report-query"></a><span data-ttu-id="2e3c4-188">Requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2e3c4-188">Report query</span></span>

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="2e3c4-189">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="2e3c4-189">Next steps</span></span>

- [<span data-ttu-id="2e3c4-190">API permettant d’accéder aux données analytiques de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="2e3c4-190">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
- [<span data-ttu-id="2e3c4-191">Exemple d’application pour l’accès aux données analytiques de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="2e3c4-191">Sample application for accessing partner insights analytics data</span></span>](insights-programmatic-sample-application.md)