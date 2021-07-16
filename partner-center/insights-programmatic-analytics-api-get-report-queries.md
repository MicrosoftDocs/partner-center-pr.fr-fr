---
title: API d’extraction de requêtes de rapport-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour obtenir toutes les requêtes disponibles à utiliser dans l’API de rapport.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375606"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="ead09-103">API Obtenir des requêtes de rapport</span><span class="sxs-lookup"><span data-stu-id="ead09-103">Get report queries API</span></span>

<span data-ttu-id="ead09-104">L’API obtenir des requêtes de rapport obtient toutes les requêtes qui peuvent être utilisées dans les rapports.</span><span class="sxs-lookup"><span data-stu-id="ead09-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="ead09-105">Elle obtient toutes les requêtes système et définies par l’utilisateur par défaut.</span><span class="sxs-lookup"><span data-stu-id="ead09-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="ead09-106">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="ead09-106">**Request syntax**</span></span>

|    <span data-ttu-id="ead09-107">Méthode</span><span class="sxs-lookup"><span data-stu-id="ead09-107">Method</span></span>    |    <span data-ttu-id="ead09-108">URI de demande</span><span class="sxs-lookup"><span data-stu-id="ead09-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ead09-109">GET</span><span class="sxs-lookup"><span data-stu-id="ead09-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="ead09-110">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="ead09-110">**Request header**</span></span>

|    <span data-ttu-id="ead09-111">En-tête</span><span class="sxs-lookup"><span data-stu-id="ead09-111">Header</span></span>    |    <span data-ttu-id="ead09-112">Type</span><span class="sxs-lookup"><span data-stu-id="ead09-112">Type</span></span>    |    <span data-ttu-id="ead09-113">Description</span><span class="sxs-lookup"><span data-stu-id="ead09-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ead09-114">Autorisation</span><span class="sxs-lookup"><span data-stu-id="ead09-114">Authorization</span></span>    |    <span data-ttu-id="ead09-115">string</span><span class="sxs-lookup"><span data-stu-id="ead09-115">string</span></span>    |    <span data-ttu-id="ead09-116">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="ead09-116">Required.</span></span> <span data-ttu-id="ead09-117">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ead09-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ead09-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ead09-118">Content-Type</span></span>    |    <span data-ttu-id="ead09-119">string</span><span class="sxs-lookup"><span data-stu-id="ead09-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ead09-120">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="ead09-120">**Path parameter**</span></span>

<span data-ttu-id="ead09-121">Aucun</span><span class="sxs-lookup"><span data-stu-id="ead09-121">None</span></span>

<span data-ttu-id="ead09-122">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="ead09-122">**Query parameter**</span></span>

|    <span data-ttu-id="ead09-123">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="ead09-123">Parameter Name</span></span>    |    <span data-ttu-id="ead09-124">Type</span><span class="sxs-lookup"><span data-stu-id="ead09-124">Type</span></span>    |    <span data-ttu-id="ead09-125">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="ead09-125">Required</span></span>    |    <span data-ttu-id="ead09-126">Description</span><span class="sxs-lookup"><span data-stu-id="ead09-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ead09-127">queryId</span><span class="sxs-lookup"><span data-stu-id="ead09-127">queryId</span></span>     |    <span data-ttu-id="ead09-128">string</span><span class="sxs-lookup"><span data-stu-id="ead09-128">string</span></span>     |    <span data-ttu-id="ead09-129">Non</span><span class="sxs-lookup"><span data-stu-id="ead09-129">No</span></span>    |    <span data-ttu-id="ead09-130">Filtre permettant d’obtenir les détails des seules requêtes avec l’ID fourni dans l’argument</span><span class="sxs-lookup"><span data-stu-id="ead09-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="ead09-131">NomRequête</span><span class="sxs-lookup"><span data-stu-id="ead09-131">queryName</span></span>     |    <span data-ttu-id="ead09-132">string</span><span class="sxs-lookup"><span data-stu-id="ead09-132">string</span></span>     |    <span data-ttu-id="ead09-133">Non</span><span class="sxs-lookup"><span data-stu-id="ead09-133">No</span></span>    |    <span data-ttu-id="ead09-134">Filtre permettant d’obtenir les détails des seules requête avec le nom founi dans l’argument</span><span class="sxs-lookup"><span data-stu-id="ead09-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="ead09-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="ead09-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="ead09-136">boolean</span><span class="sxs-lookup"><span data-stu-id="ead09-136">boolean</span></span>     |    <span data-ttu-id="ead09-137">Non</span><span class="sxs-lookup"><span data-stu-id="ead09-137">No</span></span>    |    <span data-ttu-id="ead09-138">Inclure les requêtes système prédéfinies dans la réponse</span><span class="sxs-lookup"><span data-stu-id="ead09-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="ead09-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="ead09-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="ead09-140">boolean</span><span class="sxs-lookup"><span data-stu-id="ead09-140">boolean</span></span>     |    <span data-ttu-id="ead09-141">Non</span><span class="sxs-lookup"><span data-stu-id="ead09-141">No</span></span>    |    <span data-ttu-id="ead09-142">Inclure uniquement les requêtes système dans la réponse</span><span class="sxs-lookup"><span data-stu-id="ead09-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="ead09-143">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="ead09-143">**Request payload**</span></span>

<span data-ttu-id="ead09-144">Aucun</span><span class="sxs-lookup"><span data-stu-id="ead09-144">None</span></span>

<span data-ttu-id="ead09-145">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="ead09-145">**Glossary**</span></span>

<span data-ttu-id="ead09-146">Aucune</span><span class="sxs-lookup"><span data-stu-id="ead09-146">None</span></span>

<span data-ttu-id="ead09-147">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="ead09-147">**Response**</span></span>

<span data-ttu-id="ead09-148">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="ead09-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="ead09-149">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ead09-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ead09-150">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="ead09-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="ead09-151">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="ead09-151">**Glossary**</span></span>

<span data-ttu-id="ead09-152">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="ead09-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ead09-153">Paramètre</span><span class="sxs-lookup"><span data-stu-id="ead09-153">Parameter</span></span>    |    <span data-ttu-id="ead09-154">Description</span><span class="sxs-lookup"><span data-stu-id="ead09-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ead09-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="ead09-155">QueryId</span></span>     |    <span data-ttu-id="ead09-156">UUID unique de la requête</span><span class="sxs-lookup"><span data-stu-id="ead09-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="ead09-157">Nom</span><span class="sxs-lookup"><span data-stu-id="ead09-157">Name</span></span>     |    <span data-ttu-id="ead09-158">Nom donné à la requête au moment de sa création</span><span class="sxs-lookup"><span data-stu-id="ead09-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="ead09-159">Description</span><span class="sxs-lookup"><span data-stu-id="ead09-159">Description</span></span>     |    <span data-ttu-id="ead09-160">Description donnée lors de la création de la requête</span><span class="sxs-lookup"><span data-stu-id="ead09-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="ead09-161">Requête</span><span class="sxs-lookup"><span data-stu-id="ead09-161">Query</span></span>     |    <span data-ttu-id="ead09-162">Chaîne de requête de rapport</span><span class="sxs-lookup"><span data-stu-id="ead09-162">Report query string</span></span>     |
|    <span data-ttu-id="ead09-163">Type</span><span class="sxs-lookup"><span data-stu-id="ead09-163">Type</span></span>     |    <span data-ttu-id="ead09-164">Défini sur userDefined pour les requêtes créées par l’utilisateur et système pour les requêtes système prédéfinies</span><span class="sxs-lookup"><span data-stu-id="ead09-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="ead09-165">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="ead09-165">User</span></span>     |    <span data-ttu-id="ead09-166">ID de l’utilisateur qui a créé la requête</span><span class="sxs-lookup"><span data-stu-id="ead09-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="ead09-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ead09-167">CreatedTime</span></span>     |    <span data-ttu-id="ead09-168">Heure de création de la requête</span><span class="sxs-lookup"><span data-stu-id="ead09-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="ead09-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ead09-169">TotalCount</span></span>     |    <span data-ttu-id="ead09-170">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="ead09-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ead09-171">Message</span><span class="sxs-lookup"><span data-stu-id="ead09-171">Message</span></span>     |    <span data-ttu-id="ead09-172">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="ead09-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ead09-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="ead09-173">StatusCode</span></span>     |    <span data-ttu-id="ead09-174">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="ead09-174">Result Code.</span></span> <span data-ttu-id="ead09-175">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ead09-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
