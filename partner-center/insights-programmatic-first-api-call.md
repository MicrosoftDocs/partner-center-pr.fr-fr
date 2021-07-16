---
title: Effectuer votre premier appel d’API pour accéder aux données analytiques de Partner Insights
description: Exemples d’apprentissage de l’utilisation de l’API pour l’accès aux données analytiques de Partner Insights.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375069"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Effectuer votre premier appel d’API pour accéder aux données analytiques de Partner Insights

Pour obtenir la liste des API permettant d’accéder aux données analytiques de Partner Insights, consultez la page [API permettant d’accéder aux données analytiques de Partner Insights](insights-programmatic-analytics-available-api.md). avant d’effectuer votre premier appel d’API, assurez-vous que vous avez respecté les [conditions](insights-programmatic-prerequisites.md) préalables à l’accès par programmation aux données du partenaire Informations analytics.

## <a name="token-generation"></a>Génération de jetons

avant d’appeler l’une des méthodes, vous devez d’abord obtenir un jeton d’accès Azure Active Directory (AAD). Vous devez transmettre le jeton d’accès Azure AD à l’en-tête d’autorisation de chaque méthode de l’API. Après avoir obtenu un jeton d’accès, vous disposez de 60 minutes pour l’utiliser avant qu’il n’expire. Une fois le jeton expiré, vous pouvez actualiser le jeton et continuer à l’utiliser pour d’autres appels à l’API.

Reportez-vous à l’exemple de requête ci-dessous pour générer un jeton. Les trois valeurs requises pour générer le jeton sont `clientId`, `clientSecret` et `tenantId`. Le paramètre de ressource doit avoir la valeur `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Exemple de requête

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Pour plus d’informations sur la façon d’obtenir un jeton de Azure AD pour votre application, consultez [accéder aux données d’analyse à l’aide des services de magasin.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Appel d’API programmatique

Après avoir obtenu le jeton AAD comme décrit dans la section précédente, procédez comme suit pour créer votre premier rapport d’accès par programme.

Les données peuvent être téléchargées à partir des jeux de données suivants (datasetName) :

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profil
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

Dans la section suivante, nous verrons des exemples de la façon d’accéder par programmation `SubscriptionId` à partir du jeu de données DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Étape 1 : effectuer un appel REST à l’aide de l’API obtenir des jeux de données

La réponse de l’API fournit le nom du jeu de données à partir duquel vous pouvez télécharger le rapport. Pour le jeu de données spécifique, la réponse de l’API fournit également la liste des colonnes sélectionnables pouvant être utilisées pour votre modèle de rapport personnalisé. Vous pouvez également faire référence aux [définitions de données](insights-data-definitions.md) pour récupérer les noms des colonnes.

#### <a name="request-example"></a>Exemple de requête

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Étape 2 : créer la requête personnalisée

Dans cette étape, nous allons utiliser SubscriptionId à partir du jeu de données DynamicsUsage pour créer une requête personnalisée pour le rapport de votre choix. La valeur TimeSpan par défaut s’il n’est pas spécifié dans la requête est de 6 mois.

#### <a name="request-example"></a>Exemple de requête

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Si l’exécution de la requête aboutit, un `queryId` est généré et doit être utilisé pour générer le rapport.

### <a name="step-3-execute-test-query-api"></a>Étape 3 : Exécuter l’API de requête de test

Dans cette étape, nous allons utiliser l’API test Query pour obtenir les 100 premières lignes pour la requête qui a été créée.

#### <a name="request-example"></a>Exemple de requête

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Étape 4 : Créer le rapport

Dans cette étape, nous allons utiliser l’QueryId généré précédemment pour créer le rapport.

#### <a name="request-example"></a>Exemple de requête

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Si l’exécution aboutit, un `reportId` est généré et doit être utilisé pour planifier un téléchargement du rapport.

### <a name="step-5-execute-report-executions-api"></a>Étape 5 : Exécuter l’API des exécutions de rapport

Dans cette étape, nous allons utiliser l’API d’exécution de rapport pour obtenir l’emplacement sécurisé (URL) du rapport.

#### <a name="request-example"></a>Exemple de requête

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Exemple de réponse

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Étapes suivantes

- Tester les API par le biais de l’URL de l' [API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)