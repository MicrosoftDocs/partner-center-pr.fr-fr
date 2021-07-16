---
title: API d’extraction de tous les jeux de données-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour récupérer les détails de tous les jeux de données disponibles dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375358"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="08a68-103">API Obtenir tous les jeux de données</span><span class="sxs-lookup"><span data-stu-id="08a68-103">Get all datasets API</span></span>

<span data-ttu-id="08a68-104">L’API Obtenir tous les jeux de données obtient tous les jeux de données disponibles.</span><span class="sxs-lookup"><span data-stu-id="08a68-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="08a68-105">Les jeux de données listent les tables, les colonnes, les métriques et les intervalles de temps.</span><span class="sxs-lookup"><span data-stu-id="08a68-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="08a68-106">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="08a68-106">**Request syntax**</span></span>

|    <span data-ttu-id="08a68-107">Méthode</span><span class="sxs-lookup"><span data-stu-id="08a68-107">Method</span></span>    |    <span data-ttu-id="08a68-108">URI de demande</span><span class="sxs-lookup"><span data-stu-id="08a68-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="08a68-109">GET</span><span class="sxs-lookup"><span data-stu-id="08a68-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="08a68-110">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="08a68-110">**Request header**</span></span>

|    <span data-ttu-id="08a68-111">En-tête</span><span class="sxs-lookup"><span data-stu-id="08a68-111">Header</span></span>    |    <span data-ttu-id="08a68-112">Type</span><span class="sxs-lookup"><span data-stu-id="08a68-112">Type</span></span>    |    <span data-ttu-id="08a68-113">Description</span><span class="sxs-lookup"><span data-stu-id="08a68-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="08a68-114">Autorisation</span><span class="sxs-lookup"><span data-stu-id="08a68-114">Authorization</span></span>    |    <span data-ttu-id="08a68-115">string</span><span class="sxs-lookup"><span data-stu-id="08a68-115">string</span></span>    |    <span data-ttu-id="08a68-116">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="08a68-116">Required.</span></span> <span data-ttu-id="08a68-117">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="08a68-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="08a68-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08a68-118">Content-Type</span></span>    |    <span data-ttu-id="08a68-119">string</span><span class="sxs-lookup"><span data-stu-id="08a68-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="08a68-120">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="08a68-120">**Path parameter**</span></span>

<span data-ttu-id="08a68-121">Aucun</span><span class="sxs-lookup"><span data-stu-id="08a68-121">None</span></span>

<span data-ttu-id="08a68-122">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="08a68-122">**Query parameter**</span></span>

|    <span data-ttu-id="08a68-123">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="08a68-123">Parameter Name</span></span>    |    <span data-ttu-id="08a68-124">Type</span><span class="sxs-lookup"><span data-stu-id="08a68-124">Type</span></span>    |    <span data-ttu-id="08a68-125">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="08a68-125">Required</span></span>    |    <span data-ttu-id="08a68-126">Description</span><span class="sxs-lookup"><span data-stu-id="08a68-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="08a68-127">NomGroupeDonnées</span><span class="sxs-lookup"><span data-stu-id="08a68-127">datasetName</span></span>    |    <span data-ttu-id="08a68-128">string</span><span class="sxs-lookup"><span data-stu-id="08a68-128">string</span></span>    |    <span data-ttu-id="08a68-129">Non</span><span class="sxs-lookup"><span data-stu-id="08a68-129">No</span></span>    |    <span data-ttu-id="08a68-130">Filtrer pour afficher les détails d’un seul jeu de données</span><span class="sxs-lookup"><span data-stu-id="08a68-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="08a68-131">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="08a68-131">**Request payload**</span></span>

<span data-ttu-id="08a68-132">Aucun</span><span class="sxs-lookup"><span data-stu-id="08a68-132">None</span></span>

<span data-ttu-id="08a68-133">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="08a68-133">**Glossary**</span></span>

<span data-ttu-id="08a68-134">Aucune</span><span class="sxs-lookup"><span data-stu-id="08a68-134">None</span></span>

<span data-ttu-id="08a68-135">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="08a68-135">**Response**</span></span>

<span data-ttu-id="08a68-136">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="08a68-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="08a68-137">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="08a68-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="08a68-138">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="08a68-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="08a68-139">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="08a68-139">**Glossary**</span></span>

<span data-ttu-id="08a68-140">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="08a68-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="08a68-141">Paramètre</span><span class="sxs-lookup"><span data-stu-id="08a68-141">Parameter</span></span>    |    <span data-ttu-id="08a68-142">Description</span><span class="sxs-lookup"><span data-stu-id="08a68-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="08a68-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="08a68-143">DatasetName</span></span>     |    <span data-ttu-id="08a68-144">Nom du jeu de données défini par cet objet de tableau</span><span class="sxs-lookup"><span data-stu-id="08a68-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="08a68-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="08a68-145">SelectableColumns</span></span>     |    <span data-ttu-id="08a68-146">Colonnes brutes qui peuvent être spécifiées dans les colonnes sélectionnées</span><span class="sxs-lookup"><span data-stu-id="08a68-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="08a68-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="08a68-147">AvailableMetrics</span></span>     |    <span data-ttu-id="08a68-148">Noms des colonnes d’agrégation/métriques qui peuvent être spécifiées dans les colonnes sélectionnées</span><span class="sxs-lookup"><span data-stu-id="08a68-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="08a68-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="08a68-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="08a68-150">Plage de dates qui peut être utilisée dans les requêtes de rapport pour le jeu de données</span><span class="sxs-lookup"><span data-stu-id="08a68-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="08a68-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="08a68-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="08a68-152">Valeur minimale de l’intervalle de récurrence</span><span class="sxs-lookup"><span data-stu-id="08a68-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="08a68-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="08a68-153">TotalCount</span></span>     |    <span data-ttu-id="08a68-154">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="08a68-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="08a68-155">Message</span><span class="sxs-lookup"><span data-stu-id="08a68-155">Message</span></span>     |    <span data-ttu-id="08a68-156">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="08a68-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="08a68-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="08a68-157">StatusCode</span></span>     |    <span data-ttu-id="08a68-158">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="08a68-158">Result Code.</span></span> <span data-ttu-id="08a68-159">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="08a68-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
