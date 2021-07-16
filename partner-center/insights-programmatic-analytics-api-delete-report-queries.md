---
title: API de suppression des requêtes de rapport-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour supprimer une requête définie par l’utilisateur dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375379"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="f4bee-103">API Supprimer des requêtes de rapport</span><span class="sxs-lookup"><span data-stu-id="f4bee-103">Delete report queries API</span></span>

<span data-ttu-id="f4bee-104">Cette API supprime les requêtes définies par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f4bee-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="f4bee-105">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="f4bee-105">**Request syntax**</span></span>

|    <span data-ttu-id="f4bee-106">Méthode</span><span class="sxs-lookup"><span data-stu-id="f4bee-106">Method</span></span>    |    <span data-ttu-id="f4bee-107">URI de demande</span><span class="sxs-lookup"><span data-stu-id="f4bee-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f4bee-108">Suppression</span><span class="sxs-lookup"><span data-stu-id="f4bee-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="f4bee-109">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="f4bee-109">**Request header**</span></span>

|    <span data-ttu-id="f4bee-110">En-tête</span><span class="sxs-lookup"><span data-stu-id="f4bee-110">Header</span></span>    |    <span data-ttu-id="f4bee-111">Type</span><span class="sxs-lookup"><span data-stu-id="f4bee-111">Type</span></span>    |    <span data-ttu-id="f4bee-112">Description</span><span class="sxs-lookup"><span data-stu-id="f4bee-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="f4bee-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="f4bee-113">Authorization</span></span>    |    <span data-ttu-id="f4bee-114">string</span><span class="sxs-lookup"><span data-stu-id="f4bee-114">string</span></span>    |    <span data-ttu-id="f4bee-115">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="f4bee-115">Required.</span></span> <span data-ttu-id="f4bee-116">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="f4bee-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="f4bee-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4bee-117">Content-Type</span></span>    |    <span data-ttu-id="f4bee-118">string</span><span class="sxs-lookup"><span data-stu-id="f4bee-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="f4bee-119">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="f4bee-119">**Path parameter**</span></span>

|    <span data-ttu-id="f4bee-120">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="f4bee-120">Parameter Name</span></span>    |    <span data-ttu-id="f4bee-121">Type</span><span class="sxs-lookup"><span data-stu-id="f4bee-121">Type</span></span>    |    <span data-ttu-id="f4bee-122">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="f4bee-122">Required</span></span>    |    <span data-ttu-id="f4bee-123">Description</span><span class="sxs-lookup"><span data-stu-id="f4bee-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="f4bee-124">queryId</span><span class="sxs-lookup"><span data-stu-id="f4bee-124">queryId</span></span>     |    <span data-ttu-id="f4bee-125">string</span><span class="sxs-lookup"><span data-stu-id="f4bee-125">string</span></span>     |    <span data-ttu-id="f4bee-126">Non</span><span class="sxs-lookup"><span data-stu-id="f4bee-126">No</span></span>    |    <span data-ttu-id="f4bee-127">Filtre permettant d’obtenir les détails des seules requêtes avec l’ID fourni dans l’argument</span><span class="sxs-lookup"><span data-stu-id="f4bee-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="f4bee-128">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="f4bee-128">**Query parameter**</span></span>

<span data-ttu-id="f4bee-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="f4bee-129">None</span></span>

<span data-ttu-id="f4bee-130">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="f4bee-130">**Request payload**</span></span>

<span data-ttu-id="f4bee-131">Aucun</span><span class="sxs-lookup"><span data-stu-id="f4bee-131">None</span></span>

<span data-ttu-id="f4bee-132">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="f4bee-132">**Glossary**</span></span>

<span data-ttu-id="f4bee-133">Aucune</span><span class="sxs-lookup"><span data-stu-id="f4bee-133">None</span></span>

<span data-ttu-id="f4bee-134">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="f4bee-134">**Response**</span></span>

<span data-ttu-id="f4bee-135">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="f4bee-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="f4bee-136">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="f4bee-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="f4bee-137">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="f4bee-137">Response payload example:</span></span>

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

<span data-ttu-id="f4bee-138">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="f4bee-138">**Glossary**</span></span>

<span data-ttu-id="f4bee-139">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="f4bee-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="f4bee-140">Paramètre</span><span class="sxs-lookup"><span data-stu-id="f4bee-140">Parameter</span></span>    |    <span data-ttu-id="f4bee-141">Description</span><span class="sxs-lookup"><span data-stu-id="f4bee-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f4bee-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="f4bee-142">QueryId</span></span>     |    <span data-ttu-id="f4bee-143">UUID unique de la requête qui a été supprimée</span><span class="sxs-lookup"><span data-stu-id="f4bee-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="f4bee-144">Nom</span><span class="sxs-lookup"><span data-stu-id="f4bee-144">Name</span></span>     |    <span data-ttu-id="f4bee-145">Nom de la requête supprimée</span><span class="sxs-lookup"><span data-stu-id="f4bee-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="f4bee-146">Description</span><span class="sxs-lookup"><span data-stu-id="f4bee-146">Description</span></span>     |    <span data-ttu-id="f4bee-147">Description de la requête supprimée</span><span class="sxs-lookup"><span data-stu-id="f4bee-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="f4bee-148">Requête</span><span class="sxs-lookup"><span data-stu-id="f4bee-148">Query</span></span>     |    <span data-ttu-id="f4bee-149">Chaîne de requête de rapport de la requête supprimée</span><span class="sxs-lookup"><span data-stu-id="f4bee-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="f4bee-150">Type</span><span class="sxs-lookup"><span data-stu-id="f4bee-150">Type</span></span>     |    <span data-ttu-id="f4bee-151">Défini sur userDefined pour les requêtes créées par l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="f4bee-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="f4bee-152">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="f4bee-152">User</span></span>     |    <span data-ttu-id="f4bee-153">ID de l’utilisateur qui a créé la requête</span><span class="sxs-lookup"><span data-stu-id="f4bee-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="f4bee-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="f4bee-154">CreatedTime</span></span>     |    <span data-ttu-id="f4bee-155">Heure de création de la requête</span><span class="sxs-lookup"><span data-stu-id="f4bee-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="f4bee-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="f4bee-156">TotalCount</span></span>     |    <span data-ttu-id="f4bee-157">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="f4bee-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="f4bee-158">Message</span><span class="sxs-lookup"><span data-stu-id="f4bee-158">Message</span></span>     |    <span data-ttu-id="f4bee-159">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="f4bee-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="f4bee-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="f4bee-160">StatusCode</span></span>     |    <span data-ttu-id="f4bee-161">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="f4bee-161">Result Code.</span></span> <span data-ttu-id="f4bee-162">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="f4bee-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
