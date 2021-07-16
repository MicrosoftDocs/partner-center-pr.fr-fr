---
title: API Essayer des requêtes de rapport
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour tester votre requête et valider les résultats dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375582"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="027c4-103">API Essayer des requêtes de rapport</span><span class="sxs-lookup"><span data-stu-id="027c4-103">Try report queries API</span></span>

<span data-ttu-id="027c4-104">Cette API exécute une instruction de requête de rapport.</span><span class="sxs-lookup"><span data-stu-id="027c4-104">This API executes a Report query statement.</span></span> <span data-ttu-id="027c4-105">L’API retourne uniquement 100 enregistrements que vous pouvez utiliser comme partenaire pour vérifier si les données sont les mêmes que prévu.</span><span class="sxs-lookup"><span data-stu-id="027c4-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="027c4-106">Cette API a un délai d’expiration d’exécution de requête de 100 secondes.</span><span class="sxs-lookup"><span data-stu-id="027c4-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="027c4-107">Si vous remarquez que l’API prend plus de 100 secondes, il est très probable que la requête soit syntaxiquement correcte, sinon vous auriez reçu un code d’erreur autre que 200.</span><span class="sxs-lookup"><span data-stu-id="027c4-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="027c4-108">La génération du rapport réussit si la syntaxe de la requête est correcte.</span><span class="sxs-lookup"><span data-stu-id="027c4-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="027c4-109">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="027c4-109">**Request syntax**</span></span>

|    <span data-ttu-id="027c4-110">Méthode</span><span class="sxs-lookup"><span data-stu-id="027c4-110">Method</span></span>    |    <span data-ttu-id="027c4-111">URI de demande</span><span class="sxs-lookup"><span data-stu-id="027c4-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="027c4-112">GET</span><span class="sxs-lookup"><span data-stu-id="027c4-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="027c4-113">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="027c4-113">**Request header**</span></span>

|    <span data-ttu-id="027c4-114">En-tête</span><span class="sxs-lookup"><span data-stu-id="027c4-114">Header</span></span>    |    <span data-ttu-id="027c4-115">Type</span><span class="sxs-lookup"><span data-stu-id="027c4-115">Type</span></span>    |    <span data-ttu-id="027c4-116">Description</span><span class="sxs-lookup"><span data-stu-id="027c4-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="027c4-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="027c4-117">Authorization</span></span>    |    <span data-ttu-id="027c4-118">string</span><span class="sxs-lookup"><span data-stu-id="027c4-118">string</span></span>    |    <span data-ttu-id="027c4-119">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="027c4-119">Required.</span></span> <span data-ttu-id="027c4-120">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="027c4-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="027c4-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="027c4-121">Content-Type</span></span>    |    <span data-ttu-id="027c4-122">string</span><span class="sxs-lookup"><span data-stu-id="027c4-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="027c4-123">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="027c4-123">**Path parameter**</span></span>

<span data-ttu-id="027c4-124">Aucun</span><span class="sxs-lookup"><span data-stu-id="027c4-124">None</span></span>

<span data-ttu-id="027c4-125">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="027c4-125">**Query parameter**</span></span>

|    <span data-ttu-id="027c4-126">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="027c4-126">Parameter Name</span></span>    |    <span data-ttu-id="027c4-127">Type</span><span class="sxs-lookup"><span data-stu-id="027c4-127">Type</span></span>    |    <span data-ttu-id="027c4-128">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="027c4-128">Required</span></span>    |    <span data-ttu-id="027c4-129">Description</span><span class="sxs-lookup"><span data-stu-id="027c4-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="027c4-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="027c4-130">exportQuery</span></span>     |    <span data-ttu-id="027c4-131">string</span><span class="sxs-lookup"><span data-stu-id="027c4-131">string</span></span>    |    <span data-ttu-id="027c4-132">Non</span><span class="sxs-lookup"><span data-stu-id="027c4-132">No</span></span>    |    <span data-ttu-id="027c4-133">Chaîne de requête de rapport qui doit être exécutée</span><span class="sxs-lookup"><span data-stu-id="027c4-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="027c4-134">queryId</span><span class="sxs-lookup"><span data-stu-id="027c4-134">queryId</span></span>     |    <span data-ttu-id="027c4-135">string</span><span class="sxs-lookup"><span data-stu-id="027c4-135">string</span></span>    |    <span data-ttu-id="027c4-136">Non</span><span class="sxs-lookup"><span data-stu-id="027c4-136">No</span></span>    |    <span data-ttu-id="027c4-137">ID de requête existant valide.</span><span class="sxs-lookup"><span data-stu-id="027c4-137">A valid existing query ID.</span></span> <span data-ttu-id="027c4-138">S’exclut mutuellement avec la chaîne de requête spécifiée dans le paramètre exportQuery</span><span class="sxs-lookup"><span data-stu-id="027c4-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="027c4-139">startTime</span><span class="sxs-lookup"><span data-stu-id="027c4-139">startTime</span></span>     |    <span data-ttu-id="027c4-140">string</span><span class="sxs-lookup"><span data-stu-id="027c4-140">string</span></span>    |    <span data-ttu-id="027c4-141">Non</span><span class="sxs-lookup"><span data-stu-id="027c4-141">No</span></span>    |    <span data-ttu-id="027c4-142">Heure de début à partir de laquelle les données doivent être recherchées.</span><span class="sxs-lookup"><span data-stu-id="027c4-142">Start time from which we want the data.</span></span> <span data-ttu-id="027c4-143">Elle remplace la période spécifiée dans la requête</span><span class="sxs-lookup"><span data-stu-id="027c4-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="027c4-144">endTime</span><span class="sxs-lookup"><span data-stu-id="027c4-144">endTime</span></span>     |    <span data-ttu-id="027c4-145">string</span><span class="sxs-lookup"><span data-stu-id="027c4-145">string</span></span>    |    <span data-ttu-id="027c4-146">Non</span><span class="sxs-lookup"><span data-stu-id="027c4-146">No</span></span>    |    <span data-ttu-id="027c4-147">Heure de fin jusqu’à laquelle les données doivent être recherchées.</span><span class="sxs-lookup"><span data-stu-id="027c4-147">End time till which we want the data.</span></span> <span data-ttu-id="027c4-148">Elle remplace la période spécifiée dans la requête</span><span class="sxs-lookup"><span data-stu-id="027c4-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="027c4-149">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="027c4-149">**Request payload**</span></span>

<span data-ttu-id="027c4-150">Aucun</span><span class="sxs-lookup"><span data-stu-id="027c4-150">None</span></span>

<span data-ttu-id="027c4-151">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="027c4-151">**Glossary**</span></span>

<span data-ttu-id="027c4-152">Aucune</span><span class="sxs-lookup"><span data-stu-id="027c4-152">None</span></span>

<span data-ttu-id="027c4-153">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="027c4-153">**Response**</span></span>

<span data-ttu-id="027c4-154">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="027c4-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="027c4-155">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="027c4-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="027c4-156">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="027c4-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="027c4-157">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="027c4-157">**Glossary**</span></span>

<span data-ttu-id="027c4-158">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="027c4-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="027c4-159">Paramètre</span><span class="sxs-lookup"><span data-stu-id="027c4-159">Parameter</span></span>    |    <span data-ttu-id="027c4-160">Description</span><span class="sxs-lookup"><span data-stu-id="027c4-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="027c4-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="027c4-161">TotalCount</span></span>     |    <span data-ttu-id="027c4-162">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="027c4-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="027c4-163">Message</span><span class="sxs-lookup"><span data-stu-id="027c4-163">Message</span></span>     |    <span data-ttu-id="027c4-164">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="027c4-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="027c4-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="027c4-165">StatusCode</span></span>     |    <span data-ttu-id="027c4-166">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="027c4-166">Result Code.</span></span> <span data-ttu-id="027c4-167">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="027c4-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
