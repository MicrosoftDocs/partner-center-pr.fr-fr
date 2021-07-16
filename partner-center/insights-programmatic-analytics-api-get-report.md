---
title: obtient l’API de rapport-données de Informations
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour récupérer tous les ID de rapport disponibles dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375603"
---
# <a name="get-report-api"></a><span data-ttu-id="8ba76-103">API Obtenir le rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-103">Get report API</span></span>

<span data-ttu-id="8ba76-104">Cette API permet d’obtenir tous les rapports planifiés.</span><span class="sxs-lookup"><span data-stu-id="8ba76-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="8ba76-105">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="8ba76-105">**Request syntax**</span></span>

|    <span data-ttu-id="8ba76-106">Méthode</span><span class="sxs-lookup"><span data-stu-id="8ba76-106">Method</span></span>    |    <span data-ttu-id="8ba76-107">URI de demande</span><span class="sxs-lookup"><span data-stu-id="8ba76-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8ba76-108">GET</span><span class="sxs-lookup"><span data-stu-id="8ba76-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="8ba76-109">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="8ba76-109">**Request header**</span></span>

|    <span data-ttu-id="8ba76-110">En-tête</span><span class="sxs-lookup"><span data-stu-id="8ba76-110">Header</span></span>    |    <span data-ttu-id="8ba76-111">Type</span><span class="sxs-lookup"><span data-stu-id="8ba76-111">Type</span></span>    |    <span data-ttu-id="8ba76-112">Description</span><span class="sxs-lookup"><span data-stu-id="8ba76-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="8ba76-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="8ba76-113">Authorization</span></span>    |    <span data-ttu-id="8ba76-114">string</span><span class="sxs-lookup"><span data-stu-id="8ba76-114">string</span></span>    |    <span data-ttu-id="8ba76-115">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="8ba76-115">Required.</span></span> <span data-ttu-id="8ba76-116">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="8ba76-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="8ba76-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ba76-117">Content-Type</span></span>    |    <span data-ttu-id="8ba76-118">string</span><span class="sxs-lookup"><span data-stu-id="8ba76-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="8ba76-119">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="8ba76-119">**Path parameter**</span></span>

<span data-ttu-id="8ba76-120">Aucun</span><span class="sxs-lookup"><span data-stu-id="8ba76-120">None</span></span>

<span data-ttu-id="8ba76-121">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="8ba76-121">**Query parameter**</span></span>

|    <span data-ttu-id="8ba76-122">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="8ba76-122">Parameter Name</span></span>    |    <span data-ttu-id="8ba76-123">Type</span><span class="sxs-lookup"><span data-stu-id="8ba76-123">Type</span></span>    |    <span data-ttu-id="8ba76-124">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="8ba76-124">Required</span></span>    |    <span data-ttu-id="8ba76-125">Description</span><span class="sxs-lookup"><span data-stu-id="8ba76-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="8ba76-126">reportId</span><span class="sxs-lookup"><span data-stu-id="8ba76-126">reportId</span></span>     |    <span data-ttu-id="8ba76-127">string</span><span class="sxs-lookup"><span data-stu-id="8ba76-127">string</span></span>    |    <span data-ttu-id="8ba76-128">Non</span><span class="sxs-lookup"><span data-stu-id="8ba76-128">No</span></span>    |    <span data-ttu-id="8ba76-129">Filtre pour afficher uniquement les détails des rapports avec le reportId donné dans cet argument</span><span class="sxs-lookup"><span data-stu-id="8ba76-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="8ba76-130">reportName</span><span class="sxs-lookup"><span data-stu-id="8ba76-130">reportName</span></span>     |    <span data-ttu-id="8ba76-131">string</span><span class="sxs-lookup"><span data-stu-id="8ba76-131">string</span></span>    |    <span data-ttu-id="8ba76-132">Non</span><span class="sxs-lookup"><span data-stu-id="8ba76-132">No</span></span>    |    <span data-ttu-id="8ba76-133">Filtre pour afficher uniquement les détails des rapports avec le rapport reportName fourni dans cet argument</span><span class="sxs-lookup"><span data-stu-id="8ba76-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="8ba76-134">queryId</span><span class="sxs-lookup"><span data-stu-id="8ba76-134">queryId</span></span>     |    <span data-ttu-id="8ba76-135">string</span><span class="sxs-lookup"><span data-stu-id="8ba76-135">string</span></span>    |    <span data-ttu-id="8ba76-136">Non</span><span class="sxs-lookup"><span data-stu-id="8ba76-136">No</span></span>    |    <span data-ttu-id="8ba76-137">Filtre pour extraire uniquement les détails des rapports avec l’queryId donné dans cet argument</span><span class="sxs-lookup"><span data-stu-id="8ba76-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="8ba76-138">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="8ba76-138">**Request payload**</span></span>

<span data-ttu-id="8ba76-139">Aucun</span><span class="sxs-lookup"><span data-stu-id="8ba76-139">None</span></span>

<span data-ttu-id="8ba76-140">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="8ba76-140">**Glossary**</span></span>

<span data-ttu-id="8ba76-141">Aucune</span><span class="sxs-lookup"><span data-stu-id="8ba76-141">None</span></span>

<span data-ttu-id="8ba76-142">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="8ba76-142">**Response**</span></span>

<span data-ttu-id="8ba76-143">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="8ba76-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="8ba76-144">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="8ba76-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="8ba76-145">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="8ba76-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="8ba76-146">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="8ba76-146">**Glossary**</span></span>

<span data-ttu-id="8ba76-147">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="8ba76-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="8ba76-148">Paramètre</span><span class="sxs-lookup"><span data-stu-id="8ba76-148">Parameter</span></span>    |    <span data-ttu-id="8ba76-149">Description</span><span class="sxs-lookup"><span data-stu-id="8ba76-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="8ba76-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="8ba76-150">ReportId</span></span>     |    <span data-ttu-id="8ba76-151">UUID unique du rapport créé</span><span class="sxs-lookup"><span data-stu-id="8ba76-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="8ba76-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="8ba76-152">ReportName</span></span>     |    <span data-ttu-id="8ba76-153">Nom donné au rapport dans la charge utile de la requête</span><span class="sxs-lookup"><span data-stu-id="8ba76-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="8ba76-154">Description</span><span class="sxs-lookup"><span data-stu-id="8ba76-154">Description</span></span>     |    <span data-ttu-id="8ba76-155">Description fournie lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="8ba76-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="8ba76-156">QueryId</span></span>     |    <span data-ttu-id="8ba76-157">ID de requête passé au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="8ba76-158">Requête</span><span class="sxs-lookup"><span data-stu-id="8ba76-158">Query</span></span>     |    <span data-ttu-id="8ba76-159">Texte de requête qui sera exécuté pour ce rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="8ba76-160">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="8ba76-160">User</span></span>     |    <span data-ttu-id="8ba76-161">ID d’utilisateur utilisé pour créer le rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="8ba76-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="8ba76-162">CreatedTime</span></span>     |    <span data-ttu-id="8ba76-163">Heure de création du rapport.</span><span class="sxs-lookup"><span data-stu-id="8ba76-163">Time the report was created.</span></span> <span data-ttu-id="8ba76-164">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8ba76-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8ba76-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="8ba76-165">ModifiedTime</span></span>     |    <span data-ttu-id="8ba76-166">Heure de dernière modification du rapport.</span><span class="sxs-lookup"><span data-stu-id="8ba76-166">Time the report was last modified.</span></span> <span data-ttu-id="8ba76-167">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8ba76-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8ba76-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="8ba76-168">executeNow</span></span>     |    <span data-ttu-id="8ba76-169">Indicateur ExecuteNow défini au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="8ba76-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="8ba76-170">StartTime</span></span>     |    <span data-ttu-id="8ba76-171">Heure de début de l’exécution.</span><span class="sxs-lookup"><span data-stu-id="8ba76-171">Time execution will begin.</span></span> <span data-ttu-id="8ba76-172">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="8ba76-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="8ba76-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="8ba76-173">ReportStatus</span></span>     |    <span data-ttu-id="8ba76-174">État d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="8ba76-174">Status of the report execution.</span></span> <span data-ttu-id="8ba76-175">Les valeurs possibles sont Paused, Active et Inactive.</span><span class="sxs-lookup"><span data-stu-id="8ba76-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="8ba76-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="8ba76-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="8ba76-177">Intervalle de périodicité fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="8ba76-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="8ba76-178">RecurrenceCount</span></span>     |    <span data-ttu-id="8ba76-179">Nombre de récurrences fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="8ba76-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="8ba76-180">CallbackUrl</span></span>     |    <span data-ttu-id="8ba76-181">URL de rappel fournie dans la requête</span><span class="sxs-lookup"><span data-stu-id="8ba76-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="8ba76-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="8ba76-182">CallbackMethod</span></span>    |    <span data-ttu-id="8ba76-183">Méthode de rappel fournie dans la demande</span><span class="sxs-lookup"><span data-stu-id="8ba76-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="8ba76-184">Format</span><span class="sxs-lookup"><span data-stu-id="8ba76-184">Format</span></span>     |    <span data-ttu-id="8ba76-185">Format des fichiers de rapport</span><span class="sxs-lookup"><span data-stu-id="8ba76-185">Format of the report files</span></span>     |
|    <span data-ttu-id="8ba76-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="8ba76-186">TotalCount</span></span>     |    <span data-ttu-id="8ba76-187">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="8ba76-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="8ba76-188">Message</span><span class="sxs-lookup"><span data-stu-id="8ba76-188">Message</span></span>     |    <span data-ttu-id="8ba76-189">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="8ba76-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="8ba76-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="8ba76-190">StatusCode</span></span>     |    <span data-ttu-id="8ba76-191">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="8ba76-191">Result Code.</span></span> <span data-ttu-id="8ba76-192">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="8ba76-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |