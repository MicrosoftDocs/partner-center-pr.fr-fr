---
title: paradigme d’accès par programme pour Informations données
description: Comprendre le flux général du modèle d’appel d’API pour l’analytique programmatique. Les API permettant d’accéder aux rapports analytiques de Partner Insights sont également couvertes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375382"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="0b229-104">Paradigme de l’accès programmatique</span><span class="sxs-lookup"><span data-stu-id="0b229-104">Programmatic access paradigm</span></span>

<span data-ttu-id="0b229-105">Ce diagramme montre le modèle d’appel d’API utilisé pour créer un modèle de rapport, planifier le rapport personnalisé et récupérer les données d’échec.</span><span class="sxs-lookup"><span data-stu-id="0b229-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Circuit de haut niveau":::
<span data-ttu-id="0b229-107">***Figure 1 : déroulement de haut niveau du modèle d’appel d’API***</span><span class="sxs-lookup"><span data-stu-id="0b229-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="0b229-108">Cette liste fournit plus de détails sur la Figure 1.</span><span class="sxs-lookup"><span data-stu-id="0b229-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="0b229-109">L’application cliente peut définir le schéma/modèle de rapport personnalisé en appelant l'[API Créer une requête de rapport](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="0b229-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="0b229-110">Vous pouvez également choisir un modèle de rapport (QueryId) dans les exemples de la bibliothèque de modèles de rapport répertoriés [ici.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="0b229-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="0b229-111">En cas de réussite, l’API de création de requête de rapport retourne l’QueryId.</span><span class="sxs-lookup"><span data-stu-id="0b229-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="0b229-112">L’application cliente doit ensuite appeler l' [API de création de rapport](#create-report-api) à l’aide du QueryId avec la date de début du rapport, l’intervalle de répétition, la récurrence et un URI de rappel facultatif.</span><span class="sxs-lookup"><span data-stu-id="0b229-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="0b229-113">En cas de réussite, l' [API de création de rapport](#create-report-api) retourne ReportID.</span><span class="sxs-lookup"><span data-stu-id="0b229-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="0b229-114">L’application cliente est notifiée à l’URL de rappel dès que les données du rapport sont prêtes à être téléchargées.</span><span class="sxs-lookup"><span data-stu-id="0b229-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="0b229-115">L’application cliente utilise ensuite l' [API obtenir des exécutions de rapport](#get-report-execution-api) pour interroger l’état du rapport avec l’ID de rapport et la plage de dates.</span><span class="sxs-lookup"><span data-stu-id="0b229-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="0b229-116">En cas de réussite, le lien de téléchargement du rapport est renvoyé et l’application peut lancer le téléchargement des données.</span><span class="sxs-lookup"><span data-stu-id="0b229-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="0b229-117">Spécification du langage de requête de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-117">Report query language specification</span></span>

<span data-ttu-id="0b229-118">Alors que nous fournissons des [requêtes système](insights-programmatic-system-queries.md) que vous pouvez utiliser pour créer des rapports, vous pouvez également créer vos propres requêtes en fonction des besoins de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="0b229-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="0b229-119">Pour en savoir plus sur les requêtes personnalisées, consultez [spécification de requête personnalisée](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="0b229-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="0b229-120">API Créer une requête de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-120">Create report query API</span></span>

<span data-ttu-id="0b229-121">L’API permet de créer des requêtes personnalisées qui définissent le jeu de données à partir duquel les colonnes et les mesures doivent être exportées.</span><span class="sxs-lookup"><span data-stu-id="0b229-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="0b229-122">L’API offre la flexibilité nécessaire pour créer un nouveau modèle de rapport basé sur les besoins de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="0b229-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="0b229-123">Vous pouvez également utiliser les [requêtes système](insights-programmatic-system-queries.md) que nous fournissons.</span><span class="sxs-lookup"><span data-stu-id="0b229-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="0b229-124">Lorsque des modèles de rapport personnalisés ne sont pas nécessaires, vous pouvez appeler l' [API de création de rapports](#create-report-api) directement à l’aide de la QueryIds des requêtes système fournies.</span><span class="sxs-lookup"><span data-stu-id="0b229-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="0b229-125">L’exemple suivant montre comment créer une requête personnalisée pour obtenir les 10 premiers clients par revenu pour le mois dernier.</span><span class="sxs-lookup"><span data-stu-id="0b229-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0b229-126">Syntaxe de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-126">Request syntax</span></span>

|    <span data-ttu-id="0b229-127">Méthode</span><span class="sxs-lookup"><span data-stu-id="0b229-127">Method</span></span>     |    <span data-ttu-id="0b229-128">URI de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0b229-129">POST</span><span class="sxs-lookup"><span data-stu-id="0b229-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="0b229-130">En-tête de requête</span><span class="sxs-lookup"><span data-stu-id="0b229-130">Request header</span></span>

|    <span data-ttu-id="0b229-131">En-tête</span><span class="sxs-lookup"><span data-stu-id="0b229-131">Header</span></span>     |    <span data-ttu-id="0b229-132">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-132">Type</span></span>     |    <span data-ttu-id="0b229-133">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0b229-134">Autorisation</span><span class="sxs-lookup"><span data-stu-id="0b229-134">Authorization</span></span>     |    <span data-ttu-id="0b229-135">string</span><span class="sxs-lookup"><span data-stu-id="0b229-135">string</span></span> |<span data-ttu-id="0b229-136">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0b229-136">Required.</span></span> <span data-ttu-id="0b229-137">Jeton d’accès Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0b229-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0b229-138">Le format est  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="0b229-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0b229-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b229-139">Content-Type</span></span>     |<span data-ttu-id="0b229-140">string</span><span class="sxs-lookup"><span data-stu-id="0b229-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="0b229-141">Paramètre de chemin</span><span class="sxs-lookup"><span data-stu-id="0b229-141">Path parameter</span></span>

<span data-ttu-id="0b229-142">Aucune</span><span class="sxs-lookup"><span data-stu-id="0b229-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="0b229-143">Paramètre de requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-143">Query parameter</span></span>

<span data-ttu-id="0b229-144">Aucune</span><span class="sxs-lookup"><span data-stu-id="0b229-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="0b229-145">Exemple de charge utile de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="0b229-146">Glossaire</span><span class="sxs-lookup"><span data-stu-id="0b229-146">Glossary</span></span>

<span data-ttu-id="0b229-147">Ce tableau fournit les définitions clés des éléments dans la charge utile de requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="0b229-148">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-148">Parameter</span></span>|    <span data-ttu-id="0b229-149">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0b229-149">Required</span></span>     |    <span data-ttu-id="0b229-150">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-150">Description</span></span>     |    <span data-ttu-id="0b229-151">Valeurs autorisées</span><span class="sxs-lookup"><span data-stu-id="0b229-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="0b229-152">Nom</span><span class="sxs-lookup"><span data-stu-id="0b229-152">Name</span></span> |    <span data-ttu-id="0b229-153">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-153">Yes</span></span>     |    <span data-ttu-id="0b229-154">Nom convivial de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-154">Friendly name of the query</span></span>     |    <span data-ttu-id="0b229-155">string</span><span class="sxs-lookup"><span data-stu-id="0b229-155">string</span></span>     |
|    <span data-ttu-id="0b229-156">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-156">Description</span></span>     |    <span data-ttu-id="0b229-157">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-157">No</span></span>     |    <span data-ttu-id="0b229-158">Description de ce que la requête renvoie</span><span class="sxs-lookup"><span data-stu-id="0b229-158">Description of what the query returns</span></span>     |    <span data-ttu-id="0b229-159">string</span><span class="sxs-lookup"><span data-stu-id="0b229-159">string</span></span>     |
|    <span data-ttu-id="0b229-160">Requête</span><span class="sxs-lookup"><span data-stu-id="0b229-160">Query</span></span>     |    <span data-ttu-id="0b229-161">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-161">Yes</span></span>     |    <span data-ttu-id="0b229-162">Chaîne de requête de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-162">Report query string</span></span>     |    <span data-ttu-id="0b229-163">Type de données : chaîne</span><span class="sxs-lookup"><span data-stu-id="0b229-163">Data type: string</span></span> <br> <span data-ttu-id="0b229-164">[Requête personnalisée](insights-programmatic-custom-query.md) basée sur les besoins de l’entreprise</span><span class="sxs-lookup"><span data-stu-id="0b229-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="0b229-165">Pour obtenir des exemples de requêtes personnalisées, consultez [exemples d’exemples de requêtes.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="0b229-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="0b229-166">Exemple de réponse</span><span class="sxs-lookup"><span data-stu-id="0b229-166">Sample response</span></span>

<span data-ttu-id="0b229-167">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="0b229-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="0b229-168">Codes de réponse : 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0b229-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="0b229-169">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="0b229-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="0b229-170">Glossaire</span><span class="sxs-lookup"><span data-stu-id="0b229-170">Glossary</span></span>

<span data-ttu-id="0b229-171">Ce tableau fournit les définitions clés des éléments dans la charge utile de requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="0b229-172">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-172">Parameter</span></span>     |    <span data-ttu-id="0b229-173">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="0b229-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="0b229-174">QueryId</span></span>     |    <span data-ttu-id="0b229-175">Identificateur unique universel (UUID) de la requête créée</span><span class="sxs-lookup"><span data-stu-id="0b229-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="0b229-176">Nom</span><span class="sxs-lookup"><span data-stu-id="0b229-176">Name</span></span>     |    <span data-ttu-id="0b229-177">Nom convivial donné à la requête dans la charge utile de requête</span><span class="sxs-lookup"><span data-stu-id="0b229-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="0b229-178">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-178">Description</span></span>     |    <span data-ttu-id="0b229-179">Description donnée lors de la création de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="0b229-180">Requête</span><span class="sxs-lookup"><span data-stu-id="0b229-180">Query</span></span>     |    <span data-ttu-id="0b229-181">Requête de rapport transmise en tant qu’entrée lors de la création de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="0b229-182">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-182">Type</span></span>     |    <span data-ttu-id="0b229-183">Paramètre à définir sur `userDefined`</span><span class="sxs-lookup"><span data-stu-id="0b229-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="0b229-184">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="0b229-184">User</span></span>     |    <span data-ttu-id="0b229-185">ID d’utilisateur utilisé pour créer la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="0b229-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0b229-186">CreatedTime</span></span>     |    <span data-ttu-id="0b229-187">Heure UTC de création de la requête au format suivant : aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0b229-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0b229-188">TotalCount</span></span>     |    <span data-ttu-id="0b229-189">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="0b229-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="0b229-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0b229-190">StatusCode</span></span>     |    <span data-ttu-id="0b229-191">Code de résultat</span><span class="sxs-lookup"><span data-stu-id="0b229-191">Result Code</span></span> <br> <span data-ttu-id="0b229-192">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0b229-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="0b229-193">message</span><span class="sxs-lookup"><span data-stu-id="0b229-193">message</span></span>     |    <span data-ttu-id="0b229-194">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="0b229-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="0b229-195">API Créer un rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-195">Create report API</span></span>

<span data-ttu-id="0b229-196">Lors de la création d’un modèle de rapport personnalisé avec succès et la réception de l’élément QueryID dans le cadre de la réponse à la [requête de création de rapport](#create-report-query-api) , cette API peut être appelée pour planifier l’exécution d’une requête à intervalles réguliers.</span><span class="sxs-lookup"><span data-stu-id="0b229-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="0b229-197">Vous pouvez définir une fréquence et une planification pour le rapport à remettre.</span><span class="sxs-lookup"><span data-stu-id="0b229-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="0b229-198">Pour les requêtes système que nous fournissons, l’API Créer un rapport peut également être appelée avec [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="0b229-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="0b229-199">Callback URL (URL de rappel)</span><span class="sxs-lookup"><span data-stu-id="0b229-199">Callback URL</span></span>

<span data-ttu-id="0b229-200">L’API de création de rapport accepte une URL de rappel.</span><span class="sxs-lookup"><span data-stu-id="0b229-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="0b229-201">Cette URL sera appelée une fois la génération du rapport réussie.</span><span class="sxs-lookup"><span data-stu-id="0b229-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="0b229-202">L’URL de rappel doit être publiquement accessible.</span><span class="sxs-lookup"><span data-stu-id="0b229-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="0b229-203">En plus de l’URL, une méthode de rappel peut également être donnée.</span><span class="sxs-lookup"><span data-stu-id="0b229-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="0b229-204">La méthode de rappel peut uniquement être « obtient » ou « poster ».</span><span class="sxs-lookup"><span data-stu-id="0b229-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="0b229-205">La méthode par défaut si aucune valeur n’est passée est « poster ».</span><span class="sxs-lookup"><span data-stu-id="0b229-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="0b229-206">Le reportId dont la génération est terminée sera toujours renvoyé pendant le rappel.</span><span class="sxs-lookup"><span data-stu-id="0b229-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="0b229-207">Rappel de publication : si l’URL transmise était `https://www.contosso.com/callback` , l’URL d’arrière-plan sera `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="0b229-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="0b229-208">Obtient le rappel : si l’URL passée était `https://www.contosso.com/callback` , l’URL d’arrière-plan appelée sera `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="0b229-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="0b229-209">Rapports ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0b229-209">ExecuteNow reports</span></span>

<span data-ttu-id="0b229-210">Il existe une provision pour générer un rapport sans planification.</span><span class="sxs-lookup"><span data-stu-id="0b229-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="0b229-211">La charge utile de l’API de création de rapport peut accepter un paramètre `ExecuteNow` , qui met en file d’attente le rapport à générer dès que l’API est appelée.</span><span class="sxs-lookup"><span data-stu-id="0b229-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="0b229-212">Lorsque `ExecuteNow` a la valeur true, les champs : `StartTime` , `RecurrenceCount` , `RecurrenceInterval` sont ignorés, car ces rapports ne sont pas planifiés.</span><span class="sxs-lookup"><span data-stu-id="0b229-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="0b229-213">Deux champs supplémentaires peuvent être passés lorsque `ExecuteNow` a la valeur true, `QueryStartTime` et `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="0b229-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="0b229-214">Ces deux champs remplacent le `TIMESPAN` champ dans la requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="0b229-215">Ces champs ne s’appliquent pas aux rapports planifiés, car les données sont générées en continu pendant une période fixe qui ne change pas.</span><span class="sxs-lookup"><span data-stu-id="0b229-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0b229-216">Syntaxe de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-216">Request syntax</span></span>

|    <span data-ttu-id="0b229-217">Méthode</span><span class="sxs-lookup"><span data-stu-id="0b229-217">Method</span></span>     |    <span data-ttu-id="0b229-218">URI de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0b229-219">POST</span><span class="sxs-lookup"><span data-stu-id="0b229-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="0b229-220">En-tête de requête</span><span class="sxs-lookup"><span data-stu-id="0b229-220">Request header</span></span>

|    <span data-ttu-id="0b229-221">En-tête</span><span class="sxs-lookup"><span data-stu-id="0b229-221">Header</span></span>     |    <span data-ttu-id="0b229-222">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-222">Type</span></span>     |    <span data-ttu-id="0b229-223">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0b229-224">Autorisation</span><span class="sxs-lookup"><span data-stu-id="0b229-224">Authorization</span></span>     |    <span data-ttu-id="0b229-225">string</span><span class="sxs-lookup"><span data-stu-id="0b229-225">string</span></span> |<span data-ttu-id="0b229-226">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0b229-226">Required.</span></span> <span data-ttu-id="0b229-227">Jeton d’accès Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0b229-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0b229-228">Le format est  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="0b229-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0b229-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b229-229">Content-Type</span></span>     |<span data-ttu-id="0b229-230">string</span><span class="sxs-lookup"><span data-stu-id="0b229-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="0b229-231">Paramètre Path</span><span class="sxs-lookup"><span data-stu-id="0b229-231">Path Parameter</span></span>

<span data-ttu-id="0b229-232">Aucune</span><span class="sxs-lookup"><span data-stu-id="0b229-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="0b229-233">Paramètre de requête</span><span class="sxs-lookup"><span data-stu-id="0b229-233">Query Parameter</span></span>

<span data-ttu-id="0b229-234">Aucune</span><span class="sxs-lookup"><span data-stu-id="0b229-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="0b229-235">Exemple de charge utile de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="0b229-236">Glossaire</span><span class="sxs-lookup"><span data-stu-id="0b229-236">Glossary</span></span>

<span data-ttu-id="0b229-237">Les définitions de clé des éléments dans la charge utile de la demande sont articulées ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="0b229-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="0b229-238">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-238">Parameter</span></span>     |    <span data-ttu-id="0b229-239">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0b229-239">Required</span></span>     |    <span data-ttu-id="0b229-240">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-240">Description</span></span>     |    <span data-ttu-id="0b229-241">Valeurs autorisées</span><span class="sxs-lookup"><span data-stu-id="0b229-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0b229-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="0b229-242">ReportName</span></span>     |    <span data-ttu-id="0b229-243">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-243">Yes</span></span>     |    <span data-ttu-id="0b229-244">Nom à assigner au rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="0b229-245">string</span><span class="sxs-lookup"><span data-stu-id="0b229-245">string</span></span>     |
|    <span data-ttu-id="0b229-246">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-246">Description</span></span>     |    <span data-ttu-id="0b229-247">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-247">No</span></span>     |    <span data-ttu-id="0b229-248">Description du rapport créé</span><span class="sxs-lookup"><span data-stu-id="0b229-248">Description of the created report</span></span>     |    <span data-ttu-id="0b229-249">string</span><span class="sxs-lookup"><span data-stu-id="0b229-249">string</span></span>     |
|    <span data-ttu-id="0b229-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="0b229-250">QueryId</span></span>     |    <span data-ttu-id="0b229-251">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-251">Yes</span></span>     |    <span data-ttu-id="0b229-252">ID de equête de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-252">Report query ID</span></span>     |    <span data-ttu-id="0b229-253">string</span><span class="sxs-lookup"><span data-stu-id="0b229-253">string</span></span>     |
|    <span data-ttu-id="0b229-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="0b229-254">StartTime</span></span>     |    <span data-ttu-id="0b229-255">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-255">Yes</span></span>     |    <span data-ttu-id="0b229-256">Horodatage UTC à partir duquel la génération du rapport commence.</span><span class="sxs-lookup"><span data-stu-id="0b229-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="0b229-257">Le format doit être : aaaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="0b229-258">string</span><span class="sxs-lookup"><span data-stu-id="0b229-258">string</span></span>     |
|    <span data-ttu-id="0b229-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0b229-259">ExecuteNow</span></span>     |    <span data-ttu-id="0b229-260">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-260">No</span></span>     |    <span data-ttu-id="0b229-261">Ce paramètre doit être utilisé pour créer un rapport à exécution unique.</span><span class="sxs-lookup"><span data-stu-id="0b229-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="0b229-262">`StartTime`, `RecurrenceInterval` et `RecurrenceCount` sont ignorés si cette propriété a la valeur true.</span><span class="sxs-lookup"><span data-stu-id="0b229-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="0b229-263">Le rapport est exécuté immédiatement de manière asynchrone</span><span class="sxs-lookup"><span data-stu-id="0b229-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="0b229-264">true/false</span><span class="sxs-lookup"><span data-stu-id="0b229-264">true/false</span></span>     |
|    <span data-ttu-id="0b229-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="0b229-265">QueryStartTime</span></span>     |    <span data-ttu-id="0b229-266">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-266">No</span></span>     |    <span data-ttu-id="0b229-267">(Facultatif) Spécifie l’heure de début de la requête qui extrait les données.</span><span class="sxs-lookup"><span data-stu-id="0b229-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="0b229-268">Ce paramètre s’applique uniquement à un rapport d’exécution unique dont la propriété a la valeur `ExecuteNow` true.</span><span class="sxs-lookup"><span data-stu-id="0b229-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="0b229-269">La définition de ce paramètre se substitue `TIMESPAN` à la valeur fournie dans la requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="0b229-270">Le format doit être aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="0b229-271">Timestamp sous forme de chaîne</span><span class="sxs-lookup"><span data-stu-id="0b229-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="0b229-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="0b229-272">QueryEndTime</span></span>     |    <span data-ttu-id="0b229-273">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-273">No</span></span>     |    <span data-ttu-id="0b229-274">(Facultatif) Spécifie l’heure de fin de la requête qui extrait les données.</span><span class="sxs-lookup"><span data-stu-id="0b229-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="0b229-275">Ce paramètre s’applique uniquement à un rapport d’exécution unique dont la propriété a la valeur `ExecuteNow` true.</span><span class="sxs-lookup"><span data-stu-id="0b229-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="0b229-276">La définition de ce paramètre se substitue `TIMESPAN` à la valeur fournie dans la requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="0b229-277">Le format doit être aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="0b229-278">Timestamp sous forme de chaîne</span><span class="sxs-lookup"><span data-stu-id="0b229-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="0b229-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0b229-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="0b229-280">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-280">Yes</span></span>     |    <span data-ttu-id="0b229-281">Fréquence en heures à laquelle le rapport doit être généré.</span><span class="sxs-lookup"><span data-stu-id="0b229-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="0b229-282">La valeur minimale est 4 et la valeur maximale est 2160.</span><span class="sxs-lookup"><span data-stu-id="0b229-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="0b229-283">entier</span><span class="sxs-lookup"><span data-stu-id="0b229-283">integer</span></span>     |
|    <span data-ttu-id="0b229-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0b229-284">RecurrenceCount</span></span>     |    <span data-ttu-id="0b229-285">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-285">No</span></span>     |    <span data-ttu-id="0b229-286">Nombre de rapports à générer.</span><span class="sxs-lookup"><span data-stu-id="0b229-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="0b229-287">entier</span><span class="sxs-lookup"><span data-stu-id="0b229-287">integer</span></span>     |
|    <span data-ttu-id="0b229-288">Format</span><span class="sxs-lookup"><span data-stu-id="0b229-288">Format</span></span>     |    <span data-ttu-id="0b229-289">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-289">No</span></span>     |    <span data-ttu-id="0b229-290">Format du fichier exporté.</span><span class="sxs-lookup"><span data-stu-id="0b229-290">File format of the exported file.</span></span> <br> <span data-ttu-id="0b229-291">La valeur par défaut est CSV.</span><span class="sxs-lookup"><span data-stu-id="0b229-291">Default is CSV.</span></span>    |    <span data-ttu-id="0b229-292">« CSV »/« TSV »</span><span class="sxs-lookup"><span data-stu-id="0b229-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="0b229-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0b229-293">CallbackUrl</span></span>     |    <span data-ttu-id="0b229-294">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-294">No</span></span>     |    <span data-ttu-id="0b229-295">URL publiquement accessible qui peut éventuellement être configurée en tant que destination de rappel</span><span class="sxs-lookup"><span data-stu-id="0b229-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="0b229-296">Chaîne (URL http)</span><span class="sxs-lookup"><span data-stu-id="0b229-296">String (http URL)</span></span>     |
|    <span data-ttu-id="0b229-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0b229-297">CallbackMethod</span></span>     |    <span data-ttu-id="0b229-298">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-298">No</span></span>     |    <span data-ttu-id="0b229-299">Méthode à utiliser pour le rappel</span><span class="sxs-lookup"><span data-stu-id="0b229-299">The method to be used for callback</span></span>     |    <span data-ttu-id="0b229-300">RECEVOIR/POSTER</span><span class="sxs-lookup"><span data-stu-id="0b229-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="0b229-301">Exemple de réponse</span><span class="sxs-lookup"><span data-stu-id="0b229-301">Sample response</span></span>

<span data-ttu-id="0b229-302">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="0b229-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="0b229-303">Codes de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0b229-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0b229-304">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="0b229-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="0b229-305">Glossaire</span><span class="sxs-lookup"><span data-stu-id="0b229-305">Glossary</span></span>

<span data-ttu-id="0b229-306">Les définitions de clé des éléments de la réponse sont articulées ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="0b229-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="0b229-307">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-307">Parameter</span></span>     |    <span data-ttu-id="0b229-308">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="0b229-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="0b229-309">ReportId</span></span>     |    <span data-ttu-id="0b229-310">Identificateur unique universel (UUID) du rapport créé</span><span class="sxs-lookup"><span data-stu-id="0b229-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="0b229-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="0b229-311">ReportName</span></span>     |    <span data-ttu-id="0b229-312">Nom donné au rapport dans la charge utile de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0b229-313">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-313">Description</span></span>     |    <span data-ttu-id="0b229-314">Description donnée lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="0b229-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="0b229-315">QueryId</span></span>     |    <span data-ttu-id="0b229-316">ID de requête transmis au moment où vous avez créé le rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="0b229-317">Requête</span><span class="sxs-lookup"><span data-stu-id="0b229-317">Query</span></span>     |    <span data-ttu-id="0b229-318">Texte de requête qui sera exécuté pour ce rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="0b229-319">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="0b229-319">User</span></span>     |    <span data-ttu-id="0b229-320">ID d’utilisateur utilisé pour créer le rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="0b229-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0b229-321">CreatedTime</span></span>     |    <span data-ttu-id="0b229-322">Heure UTC de création du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0b229-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0b229-323">ModifiedTime</span></span>     |    <span data-ttu-id="0b229-324">Heure UTC de dernière modification du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0b229-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0b229-325">ExecuteNow</span></span>     |    <span data-ttu-id="0b229-326">`ExecuteNow` indicateur défini au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="0b229-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="0b229-327">StartTime</span></span>     |    <span data-ttu-id="0b229-328">Heure UTC de début d’exécution du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0b229-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="0b229-329">ReportStatus</span></span>     |    <span data-ttu-id="0b229-330">État d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="0b229-330">Status of the report execution.</span></span> <span data-ttu-id="0b229-331">Les valeurs possibles sont `Paused` , `Active` et `Inactive`</span><span class="sxs-lookup"><span data-stu-id="0b229-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="0b229-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0b229-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="0b229-333">Intervalle de périodicité fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="0b229-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0b229-334">RecurrenceCount</span></span>     |    <span data-ttu-id="0b229-335">Nombre de récurrences fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="0b229-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0b229-336">CallbackUrl</span></span>     |    <span data-ttu-id="0b229-337">URL de rappel fournie dans la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="0b229-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0b229-338">CallbackMethod</span></span>     |    <span data-ttu-id="0b229-339">Méthode de rappel fournie dans la demande</span><span class="sxs-lookup"><span data-stu-id="0b229-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="0b229-340">Format</span><span class="sxs-lookup"><span data-stu-id="0b229-340">Format</span></span>     |    <span data-ttu-id="0b229-341">Format des fichiers de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-341">Format of the report files.</span></span> <span data-ttu-id="0b229-342">Les valeurs possibles sont `CSV` ou `TSV` .</span><span class="sxs-lookup"><span data-stu-id="0b229-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="0b229-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0b229-343">TotalCount</span></span>     |    <span data-ttu-id="0b229-344">Nombre d’enregistrements dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="0b229-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="0b229-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0b229-345">StatusCode</span></span>     |    <span data-ttu-id="0b229-346">Code de résultat</span><span class="sxs-lookup"><span data-stu-id="0b229-346">Result Code</span></span>     |
|    <span data-ttu-id="0b229-347">message</span><span class="sxs-lookup"><span data-stu-id="0b229-347">message</span></span>     |    <span data-ttu-id="0b229-348">Les valeurs possibles sont 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="0b229-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="0b229-349">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="0b229-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="0b229-350">Obtient l’API d’exécution de rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-350">Get report execution API</span></span>

<span data-ttu-id="0b229-351">Vous pouvez utiliser cette méthode pour interroger l’état d’une exécution de rapport à l’aide du ReportId reçu à partir de l' [API de création de rapport](#create-report-api).</span><span class="sxs-lookup"><span data-stu-id="0b229-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="0b229-352">La méthode renvoie le lien de téléchargement du rapport si le rapport est prêt à être téléchargé.</span><span class="sxs-lookup"><span data-stu-id="0b229-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="0b229-353">Sinon, la méthode renvoie l’état.</span><span class="sxs-lookup"><span data-stu-id="0b229-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="0b229-354">Vous pouvez également utiliser cette API pour obtenir toutes les exécutions intervenues pour un rapport donné.</span><span class="sxs-lookup"><span data-stu-id="0b229-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="0b229-355">Les paramètres de requête par défaut de cette API sont définis pour `executionStatus=Completed` et `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="0b229-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="0b229-356">Par conséquent, l’appel de l’API avant la première exécution réussie du rapport renvoie 404.</span><span class="sxs-lookup"><span data-stu-id="0b229-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="0b229-357">Les exécutions en attente peuvent être obtenues en définissant `executionStatus=Pending`.</span><span class="sxs-lookup"><span data-stu-id="0b229-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="0b229-358">Syntaxe de la requête</span><span class="sxs-lookup"><span data-stu-id="0b229-358">Request syntax</span></span>

|    <span data-ttu-id="0b229-359">Méthode</span><span class="sxs-lookup"><span data-stu-id="0b229-359">Method</span></span>     |    <span data-ttu-id="0b229-360">URI de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="0b229-361">GET</span><span class="sxs-lookup"><span data-stu-id="0b229-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="0b229-362">En-tête de requête</span><span class="sxs-lookup"><span data-stu-id="0b229-362">Request header</span></span>

|    <span data-ttu-id="0b229-363">En-tête</span><span class="sxs-lookup"><span data-stu-id="0b229-363">Header</span></span>     |    <span data-ttu-id="0b229-364">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-364">Type</span></span>     |    <span data-ttu-id="0b229-365">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="0b229-366">Autorisation</span><span class="sxs-lookup"><span data-stu-id="0b229-366">Authorization</span></span>     |    <span data-ttu-id="0b229-367">string</span><span class="sxs-lookup"><span data-stu-id="0b229-367">string</span></span> |<span data-ttu-id="0b229-368">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0b229-368">Required.</span></span> <span data-ttu-id="0b229-369">Jeton d’accès Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0b229-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="0b229-370">Le format est  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="0b229-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="0b229-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b229-371">Content-Type</span></span>     |<span data-ttu-id="0b229-372">string</span><span class="sxs-lookup"><span data-stu-id="0b229-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="0b229-373">Paramètre de chemin</span><span class="sxs-lookup"><span data-stu-id="0b229-373">Path parameter</span></span>

|    <span data-ttu-id="0b229-374">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-374">Parameter Name</span></span>    |    <span data-ttu-id="0b229-375">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0b229-375">Required</span></span>    |    <span data-ttu-id="0b229-376">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-376">Type</span></span>    |    <span data-ttu-id="0b229-377">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0b229-378">reportId</span><span class="sxs-lookup"><span data-stu-id="0b229-378">reportId</span></span>    |    <span data-ttu-id="0b229-379">Oui</span><span class="sxs-lookup"><span data-stu-id="0b229-379">Yes</span></span>    |    <span data-ttu-id="0b229-380">string</span><span class="sxs-lookup"><span data-stu-id="0b229-380">string</span></span>    |    <span data-ttu-id="0b229-381">Filtre pour récupérer les détails de l’exécution des rapports uniquement avec le reportId donné dans cet argument.</span><span class="sxs-lookup"><span data-stu-id="0b229-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="0b229-382">Plusieurs reportIds peuvent être spécifiés en les séparant par un point-virgule « ; ».</span><span class="sxs-lookup"><span data-stu-id="0b229-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="0b229-383">Paramètre de requête.</span><span class="sxs-lookup"><span data-stu-id="0b229-383">Query parameter</span></span>

|    <span data-ttu-id="0b229-384">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-384">Parameter Name</span></span>    |    <span data-ttu-id="0b229-385">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0b229-385">Required</span></span>    |    <span data-ttu-id="0b229-386">Type</span><span class="sxs-lookup"><span data-stu-id="0b229-386">Type</span></span>    |    <span data-ttu-id="0b229-387">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0b229-388">executionId</span><span class="sxs-lookup"><span data-stu-id="0b229-388">executionId</span></span>    |    <span data-ttu-id="0b229-389">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-389">No</span></span>    |    <span data-ttu-id="0b229-390">string</span><span class="sxs-lookup"><span data-stu-id="0b229-390">string</span></span>    |    <span data-ttu-id="0b229-391">Filtre pour extraire uniquement les détails des rapports avec le executionId donné dans cet argument.</span><span class="sxs-lookup"><span data-stu-id="0b229-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="0b229-392">Plusieurs executionIds peuvent être spécifiés en les séparant par un point-virgule « ; ».</span><span class="sxs-lookup"><span data-stu-id="0b229-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="0b229-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="0b229-393">executionStatus</span></span>    |    <span data-ttu-id="0b229-394">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-394">No</span></span>    |    <span data-ttu-id="0b229-395">Chaîne/enum</span><span class="sxs-lookup"><span data-stu-id="0b229-395">String/enum</span></span>    |    <span data-ttu-id="0b229-396">Filtre pour extraire uniquement les détails des rapports avec le executionStatus donné dans cet argument.</span><span class="sxs-lookup"><span data-stu-id="0b229-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="0b229-397">Les valeurs valides sont les suivantes : `Pending` , `Running` `Paused` et `Completed` .</span><span class="sxs-lookup"><span data-stu-id="0b229-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="0b229-398">La valeur par défaut est `Completed`.</span><span class="sxs-lookup"><span data-stu-id="0b229-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="0b229-399">Plusieurs États peuvent être spécifiés en les séparant par un point-virgule « ; ».</span><span class="sxs-lookup"><span data-stu-id="0b229-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="0b229-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="0b229-400">getLatestExecution</span></span>    |    <span data-ttu-id="0b229-401">Non</span><span class="sxs-lookup"><span data-stu-id="0b229-401">No</span></span>    |    <span data-ttu-id="0b229-402">boolean</span><span class="sxs-lookup"><span data-stu-id="0b229-402">boolean</span></span>    |    <span data-ttu-id="0b229-403">L’API retourne les détails de l’exécution la plus récente.</span><span class="sxs-lookup"><span data-stu-id="0b229-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="0b229-404">Par défaut, ce paramètre a la valeur true.</span><span class="sxs-lookup"><span data-stu-id="0b229-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="0b229-405">Si vous choisissez de passer la valeur de ce paramètre comme false, l’API retourne les dernières instances d’exécution de 90 jours.</span><span class="sxs-lookup"><span data-stu-id="0b229-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="0b229-406">Exemple de charge utile de demande</span><span class="sxs-lookup"><span data-stu-id="0b229-406">Sample Request Payload</span></span>

<span data-ttu-id="0b229-407">Aucune</span><span class="sxs-lookup"><span data-stu-id="0b229-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="0b229-408">Exemple de réponse</span><span class="sxs-lookup"><span data-stu-id="0b229-408">Sample Response</span></span>

<span data-ttu-id="0b229-409">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="0b229-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="0b229-410">Codes de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0b229-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0b229-411">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="0b229-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="0b229-412">Une fois l’exécution du rapport terminée, l’état d’exécution `Completed` est affiché.</span><span class="sxs-lookup"><span data-stu-id="0b229-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="0b229-413">Vous pouvez télécharger le rapport en sélectionnant l’URL dans le `reportAccessSecureLink`.</span><span class="sxs-lookup"><span data-stu-id="0b229-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="0b229-414">Glossaire</span><span class="sxs-lookup"><span data-stu-id="0b229-414">Glossary</span></span>

<span data-ttu-id="0b229-415">Définitions clés des éléments dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0b229-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="0b229-416">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0b229-416">Parameter</span></span>    |    <span data-ttu-id="0b229-417">Description</span><span class="sxs-lookup"><span data-stu-id="0b229-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0b229-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="0b229-418">ExecutionId</span></span>    |    <span data-ttu-id="0b229-419">Identificateur unique universel (UUID) de l’instance d’exécution</span><span class="sxs-lookup"><span data-stu-id="0b229-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="0b229-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="0b229-420">ReportId</span></span>    |    <span data-ttu-id="0b229-421">ID de rapport associé à l’instance d’exécution</span><span class="sxs-lookup"><span data-stu-id="0b229-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="0b229-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0b229-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="0b229-423">Intervalle de périodicité fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="0b229-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0b229-424">RecurrenceCount</span></span>    |    <span data-ttu-id="0b229-425">Nombre de récurrences fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="0b229-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0b229-426">CallbackUrl</span></span>    |    <span data-ttu-id="0b229-427">URL de rappel associée à l’instance d’exécution</span><span class="sxs-lookup"><span data-stu-id="0b229-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="0b229-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0b229-428">CallbackMethod</span></span>    |    <span data-ttu-id="0b229-429">Méthode de rappel associée à l’instance d’exécution</span><span class="sxs-lookup"><span data-stu-id="0b229-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="0b229-430">Format</span><span class="sxs-lookup"><span data-stu-id="0b229-430">Format</span></span>    |    <span data-ttu-id="0b229-431">Format du fichier généré à la fin de l’exécution</span><span class="sxs-lookup"><span data-stu-id="0b229-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="0b229-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="0b229-432">ExecutionStatus</span></span>    |    <span data-ttu-id="0b229-433">État de l’instance d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="0b229-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="0b229-434">Les valeurs valides sont `Pending`, `Running`, `Paused` et `Completed`.</span><span class="sxs-lookup"><span data-stu-id="0b229-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="0b229-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="0b229-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="0b229-436">Lien permettant d’accéder en toute sécurité au rapport</span><span class="sxs-lookup"><span data-stu-id="0b229-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="0b229-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="0b229-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="0b229-438">Heure UTC après laquelle le lien du rapport expire au format suivant : aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="0b229-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="0b229-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="0b229-440">Heure UTC à laquelle le rapport a été généré au format suivant : aaaa-MM-jjTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0b229-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="0b229-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0b229-441">TotalCount</span></span>    |    <span data-ttu-id="0b229-442">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="0b229-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="0b229-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0b229-443">StatusCode</span></span>    |    <span data-ttu-id="0b229-444">Code de résultat</span><span class="sxs-lookup"><span data-stu-id="0b229-444">Result Code</span></span> <br> <span data-ttu-id="0b229-445">Les valeurs possibles sont 200, 400, 401, 403, 404 et 500.</span><span class="sxs-lookup"><span data-stu-id="0b229-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="0b229-446">message</span><span class="sxs-lookup"><span data-stu-id="0b229-446">message</span></span>    |    <span data-ttu-id="0b229-447">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="0b229-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="0b229-448">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0b229-448">Next steps</span></span>

- <span data-ttu-id="0b229-449">Tester les API par le biais de l’URL de l' [API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="0b229-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="0b229-450">Effectuer votre premier appel d’API</span><span class="sxs-lookup"><span data-stu-id="0b229-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)