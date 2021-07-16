---
title: suspendre l’exécution du rapport API-données de Informations
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour suspendre l’exécution d’un rapport dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375600"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="06f90-103">API Mettre en pause les exécutions de rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-103">Pause report executions API</span></span>

<span data-ttu-id="06f90-104">À l’exécution, cette API interrompt l’exécution planifiée des rapports.</span><span class="sxs-lookup"><span data-stu-id="06f90-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="06f90-105">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="06f90-105">**Request syntax**</span></span>

|    <span data-ttu-id="06f90-106">Méthode</span><span class="sxs-lookup"><span data-stu-id="06f90-106">Method</span></span>    |    <span data-ttu-id="06f90-107">URI de requête</span><span class="sxs-lookup"><span data-stu-id="06f90-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="06f90-108">PUT</span><span class="sxs-lookup"><span data-stu-id="06f90-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="06f90-109">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="06f90-109">**Request header**</span></span>

|    <span data-ttu-id="06f90-110">En-tête</span><span class="sxs-lookup"><span data-stu-id="06f90-110">Header</span></span>    |    <span data-ttu-id="06f90-111">Type</span><span class="sxs-lookup"><span data-stu-id="06f90-111">Type</span></span>    |    <span data-ttu-id="06f90-112">Description</span><span class="sxs-lookup"><span data-stu-id="06f90-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="06f90-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="06f90-113">Authorization</span></span>    |    <span data-ttu-id="06f90-114">string</span><span class="sxs-lookup"><span data-stu-id="06f90-114">string</span></span>    |    <span data-ttu-id="06f90-115">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="06f90-115">Required.</span></span> <span data-ttu-id="06f90-116">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="06f90-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="06f90-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06f90-117">Content-Type</span></span>    |    <span data-ttu-id="06f90-118">string</span><span class="sxs-lookup"><span data-stu-id="06f90-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="06f90-119">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="06f90-119">**Path parameter**</span></span>

|    <span data-ttu-id="06f90-120">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="06f90-120">Parameter Name</span></span>    |    <span data-ttu-id="06f90-121">Type</span><span class="sxs-lookup"><span data-stu-id="06f90-121">Type</span></span>    |    <span data-ttu-id="06f90-122">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="06f90-122">Required</span></span>    |    <span data-ttu-id="06f90-123">Description</span><span class="sxs-lookup"><span data-stu-id="06f90-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="06f90-124">reportId</span><span class="sxs-lookup"><span data-stu-id="06f90-124">reportId</span></span>     |    <span data-ttu-id="06f90-125">string</span><span class="sxs-lookup"><span data-stu-id="06f90-125">string</span></span>    |    <span data-ttu-id="06f90-126">Non</span><span class="sxs-lookup"><span data-stu-id="06f90-126">No</span></span>    |    <span data-ttu-id="06f90-127">ID du rapport en cours de modification</span><span class="sxs-lookup"><span data-stu-id="06f90-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="06f90-128">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="06f90-128">**Query parameter**</span></span>

<span data-ttu-id="06f90-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="06f90-129">None</span></span>

<span data-ttu-id="06f90-130">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="06f90-130">**Request payload**</span></span>

<span data-ttu-id="06f90-131">Aucun</span><span class="sxs-lookup"><span data-stu-id="06f90-131">None</span></span>

<span data-ttu-id="06f90-132">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="06f90-132">**Glossary**</span></span>

<span data-ttu-id="06f90-133">Aucune</span><span class="sxs-lookup"><span data-stu-id="06f90-133">None</span></span>

<span data-ttu-id="06f90-134">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="06f90-134">**Response**</span></span>

<span data-ttu-id="06f90-135">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="06f90-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="06f90-136">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="06f90-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="06f90-137">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="06f90-137">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="06f90-138">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="06f90-138">**Glossary**</span></span>

<span data-ttu-id="06f90-139">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="06f90-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="06f90-140">Paramètre</span><span class="sxs-lookup"><span data-stu-id="06f90-140">Parameter</span></span>    |    <span data-ttu-id="06f90-141">Description</span><span class="sxs-lookup"><span data-stu-id="06f90-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="06f90-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="06f90-142">ReportId</span></span>     |    <span data-ttu-id="06f90-143">Identificateur unique universel (UUID) du rapport suspendu</span><span class="sxs-lookup"><span data-stu-id="06f90-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="06f90-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="06f90-144">ReportName</span></span>     |    <span data-ttu-id="06f90-145">Nom donné au rapport lors de la création</span><span class="sxs-lookup"><span data-stu-id="06f90-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="06f90-146">Description</span><span class="sxs-lookup"><span data-stu-id="06f90-146">Description</span></span>     |    <span data-ttu-id="06f90-147">Description donnée lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="06f90-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="06f90-148">QueryId</span></span>     |    <span data-ttu-id="06f90-149">ID de requête passé au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="06f90-150">Requête</span><span class="sxs-lookup"><span data-stu-id="06f90-150">Query</span></span>     |    <span data-ttu-id="06f90-151">Texte de requête qui sera exécuté pour ce rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="06f90-152">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="06f90-152">User</span></span>     |    <span data-ttu-id="06f90-153">ID d’utilisateur utilisé pour créer le rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="06f90-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="06f90-154">CreatedTime</span></span>     |    <span data-ttu-id="06f90-155">Heure de création du rapport.</span><span class="sxs-lookup"><span data-stu-id="06f90-155">Time the report was created.</span></span> <span data-ttu-id="06f90-156">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="06f90-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="06f90-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="06f90-157">ModifiedTime</span></span>     |    <span data-ttu-id="06f90-158">Heure de dernière modification du rapport.</span><span class="sxs-lookup"><span data-stu-id="06f90-158">Time the report was last modified.</span></span> <span data-ttu-id="06f90-159">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="06f90-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="06f90-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="06f90-160">ExecuteNow</span></span>     |    <span data-ttu-id="06f90-161">Indicateur ExecuteNow défini au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="06f90-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="06f90-162">StartTime</span></span>     |    <span data-ttu-id="06f90-163">Heure de début de l’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="06f90-163">Time the report execution will begin.</span></span> <span data-ttu-id="06f90-164">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="06f90-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="06f90-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="06f90-165">ReportStatus</span></span>     |    <span data-ttu-id="06f90-166">État d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="06f90-166">Status of the report execution.</span></span> <span data-ttu-id="06f90-167">Les valeurs possibles sont Paused, Active et Inactive.</span><span class="sxs-lookup"><span data-stu-id="06f90-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="06f90-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="06f90-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="06f90-169">Intervalle de périodicité fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="06f90-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="06f90-170">RecurrenceCount</span></span>     |    <span data-ttu-id="06f90-171">Nombre de récurrences fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="06f90-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="06f90-172">CallbackUrl</span></span>     |    <span data-ttu-id="06f90-173">URL de rappel fournie dans la requête</span><span class="sxs-lookup"><span data-stu-id="06f90-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="06f90-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="06f90-174">CallbackMethod</span></span>    |    <span data-ttu-id="06f90-175">Méthode de rappel fournie dans la demande</span><span class="sxs-lookup"><span data-stu-id="06f90-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="06f90-176">Format</span><span class="sxs-lookup"><span data-stu-id="06f90-176">Format</span></span>     |    <span data-ttu-id="06f90-177">Format des fichiers de rapport</span><span class="sxs-lookup"><span data-stu-id="06f90-177">Format of the report files</span></span>     |
|    <span data-ttu-id="06f90-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="06f90-178">TotalCount</span></span>     |    <span data-ttu-id="06f90-179">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="06f90-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="06f90-180">Message</span><span class="sxs-lookup"><span data-stu-id="06f90-180">Message</span></span>     |    <span data-ttu-id="06f90-181">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="06f90-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="06f90-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="06f90-182">StatusCode</span></span>     |    <span data-ttu-id="06f90-183">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="06f90-183">Result Code.</span></span> <span data-ttu-id="06f90-184">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="06f90-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
