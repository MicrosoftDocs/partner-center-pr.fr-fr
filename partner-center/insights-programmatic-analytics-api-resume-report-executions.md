---
title: reprendre l’API d’exécution de rapport-données de Informations
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour reprendre l’exécution de tous les rapports suspendus dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375594"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="1af85-103">API Reprendre les exécutions de rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-103">Resume report executions API</span></span>

<span data-ttu-id="1af85-104">À l’exécution, cette API reprend l’exécution planifiée d’un rapport suspendu.</span><span class="sxs-lookup"><span data-stu-id="1af85-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="1af85-105">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="1af85-105">**Request syntax**</span></span>

|    <span data-ttu-id="1af85-106">Méthode</span><span class="sxs-lookup"><span data-stu-id="1af85-106">Method</span></span>    |    <span data-ttu-id="1af85-107">URI de requête</span><span class="sxs-lookup"><span data-stu-id="1af85-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1af85-108">PUT</span><span class="sxs-lookup"><span data-stu-id="1af85-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="1af85-109">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="1af85-109">**Request header**</span></span>

|    <span data-ttu-id="1af85-110">En-tête</span><span class="sxs-lookup"><span data-stu-id="1af85-110">Header</span></span>    |    <span data-ttu-id="1af85-111">Type</span><span class="sxs-lookup"><span data-stu-id="1af85-111">Type</span></span>    |    <span data-ttu-id="1af85-112">Description</span><span class="sxs-lookup"><span data-stu-id="1af85-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1af85-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="1af85-113">Authorization</span></span>    |    <span data-ttu-id="1af85-114">string</span><span class="sxs-lookup"><span data-stu-id="1af85-114">string</span></span>    |    <span data-ttu-id="1af85-115">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="1af85-115">Required.</span></span> <span data-ttu-id="1af85-116">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="1af85-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="1af85-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1af85-117">Content-Type</span></span>    |    <span data-ttu-id="1af85-118">string</span><span class="sxs-lookup"><span data-stu-id="1af85-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="1af85-119">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="1af85-119">**Path parameter**</span></span>

|    <span data-ttu-id="1af85-120">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="1af85-120">Parameter Name</span></span>    |    <span data-ttu-id="1af85-121">Type</span><span class="sxs-lookup"><span data-stu-id="1af85-121">Type</span></span>    |    <span data-ttu-id="1af85-122">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="1af85-122">Required</span></span>    |    <span data-ttu-id="1af85-123">Description</span><span class="sxs-lookup"><span data-stu-id="1af85-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1af85-124">reportId</span><span class="sxs-lookup"><span data-stu-id="1af85-124">reportId</span></span>     |    <span data-ttu-id="1af85-125">string</span><span class="sxs-lookup"><span data-stu-id="1af85-125">string</span></span>    |    <span data-ttu-id="1af85-126">Non</span><span class="sxs-lookup"><span data-stu-id="1af85-126">No</span></span>    |    <span data-ttu-id="1af85-127">ID du rapport en cours de modification</span><span class="sxs-lookup"><span data-stu-id="1af85-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="1af85-128">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="1af85-128">**Query parameter**</span></span>

<span data-ttu-id="1af85-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="1af85-129">None</span></span>

<span data-ttu-id="1af85-130">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="1af85-130">**Request payload**</span></span>

<span data-ttu-id="1af85-131">Aucun</span><span class="sxs-lookup"><span data-stu-id="1af85-131">None</span></span>

<span data-ttu-id="1af85-132">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="1af85-132">**Glossary**</span></span>

<span data-ttu-id="1af85-133">Aucune</span><span class="sxs-lookup"><span data-stu-id="1af85-133">None</span></span>

<span data-ttu-id="1af85-134">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="1af85-134">**Response**</span></span>

<span data-ttu-id="1af85-135">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="1af85-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="1af85-136">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="1af85-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="1af85-137">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="1af85-137">Response payload example:</span></span>

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

<span data-ttu-id="1af85-138">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="1af85-138">**Glossary**</span></span>

<span data-ttu-id="1af85-139">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="1af85-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="1af85-140">Paramètre</span><span class="sxs-lookup"><span data-stu-id="1af85-140">Parameter</span></span>    |    <span data-ttu-id="1af85-141">Description</span><span class="sxs-lookup"><span data-stu-id="1af85-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1af85-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="1af85-142">ReportId</span></span>     |    <span data-ttu-id="1af85-143">Identificateur unique universel (UUID) du rapport dont la reprise a été effectuée</span><span class="sxs-lookup"><span data-stu-id="1af85-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="1af85-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="1af85-144">ReportName</span></span>     |    <span data-ttu-id="1af85-145">Nom donné au rapport lors de la création</span><span class="sxs-lookup"><span data-stu-id="1af85-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="1af85-146">Description</span><span class="sxs-lookup"><span data-stu-id="1af85-146">Description</span></span>     |    <span data-ttu-id="1af85-147">Description donnée lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="1af85-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="1af85-148">QueryId</span></span>     |    <span data-ttu-id="1af85-149">ID de requête passé au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="1af85-150">Requête</span><span class="sxs-lookup"><span data-stu-id="1af85-150">Query</span></span>     |    <span data-ttu-id="1af85-151">Texte de requête qui sera exécuté pour ce rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="1af85-152">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="1af85-152">User</span></span>     |    <span data-ttu-id="1af85-153">ID d’utilisateur utilisé pour créer le rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="1af85-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="1af85-154">CreatedTime</span></span>     |    <span data-ttu-id="1af85-155">Heure de création du rapport.</span><span class="sxs-lookup"><span data-stu-id="1af85-155">Time the report was created.</span></span> <span data-ttu-id="1af85-156">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1af85-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1af85-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1af85-157">ModifiedTime</span></span>     |    <span data-ttu-id="1af85-158">Heure de dernière modification du rapport.</span><span class="sxs-lookup"><span data-stu-id="1af85-158">Time the report was last modified.</span></span> <span data-ttu-id="1af85-159">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1af85-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1af85-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="1af85-160">ExecuteNow</span></span>     |    <span data-ttu-id="1af85-161">Indicateur ExecuteNow défini au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="1af85-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="1af85-162">StartTime</span></span>     |    <span data-ttu-id="1af85-163">Heure de début de l’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="1af85-163">Time the report execution will begin.</span></span> <span data-ttu-id="1af85-164">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1af85-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1af85-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="1af85-165">ReportStatus</span></span>     |    <span data-ttu-id="1af85-166">État d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="1af85-166">Status of the report execution.</span></span> <span data-ttu-id="1af85-167">Les valeurs possibles sont Paused, Active et Inactive.</span><span class="sxs-lookup"><span data-stu-id="1af85-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="1af85-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="1af85-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="1af85-169">Intervalle de périodicité fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="1af85-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="1af85-170">RecurrenceCount</span></span>     |    <span data-ttu-id="1af85-171">Nombre de récurrences fourni lors de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="1af85-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="1af85-172">CallbackUrl</span></span>     |    <span data-ttu-id="1af85-173">URL de rappel fournie dans la requête</span><span class="sxs-lookup"><span data-stu-id="1af85-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="1af85-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="1af85-174">CallbackMethod</span></span>    |    <span data-ttu-id="1af85-175">Méthode de rappel fournie dans la demande</span><span class="sxs-lookup"><span data-stu-id="1af85-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="1af85-176">Format</span><span class="sxs-lookup"><span data-stu-id="1af85-176">Format</span></span>     |    <span data-ttu-id="1af85-177">Format des fichiers de rapport</span><span class="sxs-lookup"><span data-stu-id="1af85-177">Format of the report files</span></span>     |
|    <span data-ttu-id="1af85-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1af85-178">TotalCount</span></span>     |    <span data-ttu-id="1af85-179">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="1af85-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="1af85-180">Message</span><span class="sxs-lookup"><span data-stu-id="1af85-180">Message</span></span>     |    <span data-ttu-id="1af85-181">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="1af85-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="1af85-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="1af85-182">StatusCode</span></span>     |    <span data-ttu-id="1af85-183">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="1af85-183">Result Code.</span></span> <span data-ttu-id="1af85-184">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="1af85-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
