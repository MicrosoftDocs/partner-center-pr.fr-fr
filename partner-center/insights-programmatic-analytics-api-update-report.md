---
title: API Mettre à jour le rapport
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour mettre à jour les paramètres de rapport dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375579"
---
# <a name="update-report-api"></a><span data-ttu-id="0c904-103">API Mettre à jour le rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-103">Update report API</span></span>

<span data-ttu-id="0c904-104">Cette API vous permet de modifier un paramètre de rapport.</span><span class="sxs-lookup"><span data-stu-id="0c904-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="0c904-105">**Syntaxe de la requête**</span><span class="sxs-lookup"><span data-stu-id="0c904-105">**Request syntax**</span></span>

|    <span data-ttu-id="0c904-106">Méthode</span><span class="sxs-lookup"><span data-stu-id="0c904-106">Method</span></span>    |    <span data-ttu-id="0c904-107">URI de requête</span><span class="sxs-lookup"><span data-stu-id="0c904-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0c904-108">PUT</span><span class="sxs-lookup"><span data-stu-id="0c904-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="0c904-109">**En-tête de requête**</span><span class="sxs-lookup"><span data-stu-id="0c904-109">**Request header**</span></span>

|    <span data-ttu-id="0c904-110">En-tête</span><span class="sxs-lookup"><span data-stu-id="0c904-110">Header</span></span>    |    <span data-ttu-id="0c904-111">Type</span><span class="sxs-lookup"><span data-stu-id="0c904-111">Type</span></span>    |    <span data-ttu-id="0c904-112">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="0c904-113">Autorisation</span><span class="sxs-lookup"><span data-stu-id="0c904-113">Authorization</span></span>    |    <span data-ttu-id="0c904-114">string</span><span class="sxs-lookup"><span data-stu-id="0c904-114">string</span></span>    |    <span data-ttu-id="0c904-115">Obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0c904-115">Required.</span></span> <span data-ttu-id="0c904-116">le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="0c904-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="0c904-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c904-117">Content-Type</span></span>    |    <span data-ttu-id="0c904-118">string</span><span class="sxs-lookup"><span data-stu-id="0c904-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="0c904-119">**Paramètre de chemin**</span><span class="sxs-lookup"><span data-stu-id="0c904-119">**Path parameter**</span></span>

|    <span data-ttu-id="0c904-120">Nom du paramètre</span><span class="sxs-lookup"><span data-stu-id="0c904-120">Parameter Name</span></span>    |    <span data-ttu-id="0c904-121">Type</span><span class="sxs-lookup"><span data-stu-id="0c904-121">Type</span></span>    |    <span data-ttu-id="0c904-122">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0c904-122">Required</span></span>    |    <span data-ttu-id="0c904-123">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0c904-124">reportId</span><span class="sxs-lookup"><span data-stu-id="0c904-124">reportId</span></span>     |    <span data-ttu-id="0c904-125">string</span><span class="sxs-lookup"><span data-stu-id="0c904-125">string</span></span>    |    <span data-ttu-id="0c904-126">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-126">No</span></span>    |    <span data-ttu-id="0c904-127">ID du rapport en cours de modification</span><span class="sxs-lookup"><span data-stu-id="0c904-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="0c904-128">**Paramètre de requête.**</span><span class="sxs-lookup"><span data-stu-id="0c904-128">**Query parameter**</span></span>

<span data-ttu-id="0c904-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="0c904-129">None</span></span>

<span data-ttu-id="0c904-130">**Charge utile de demande**</span><span class="sxs-lookup"><span data-stu-id="0c904-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="0c904-131">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="0c904-131">**Glossary**</span></span>

<span data-ttu-id="0c904-132">Ce tableau liste les définitions clés des éléments dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0c904-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="0c904-133">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0c904-133">Parameter</span></span>    |    <span data-ttu-id="0c904-134">Obligatoire</span><span class="sxs-lookup"><span data-stu-id="0c904-134">Required</span></span>    |    <span data-ttu-id="0c904-135">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-135">Description</span></span>    |    <span data-ttu-id="0c904-136">Valeurs autorisées</span><span class="sxs-lookup"><span data-stu-id="0c904-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0c904-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="0c904-137">ReportName</span></span>     |    <span data-ttu-id="0c904-138">Oui</span><span class="sxs-lookup"><span data-stu-id="0c904-138">Yes</span></span>     |    <span data-ttu-id="0c904-139">Nom à assigner au rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="0c904-140">String</span><span class="sxs-lookup"><span data-stu-id="0c904-140">String</span></span>     |
|    <span data-ttu-id="0c904-141">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-141">Description</span></span>     |    <span data-ttu-id="0c904-142">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-142">No</span></span>     |    <span data-ttu-id="0c904-143">Description du rapport créé</span><span class="sxs-lookup"><span data-stu-id="0c904-143">Description of the created report</span></span>     |    <span data-ttu-id="0c904-144">String</span><span class="sxs-lookup"><span data-stu-id="0c904-144">String</span></span>     |
|    <span data-ttu-id="0c904-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="0c904-145">StartTime</span></span>     |    <span data-ttu-id="0c904-146">Oui</span><span class="sxs-lookup"><span data-stu-id="0c904-146">Yes</span></span>    |    <span data-ttu-id="0c904-147">Horodatage à partir duquel la génération du rapport commence</span><span class="sxs-lookup"><span data-stu-id="0c904-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="0c904-148">String</span><span class="sxs-lookup"><span data-stu-id="0c904-148">String</span></span>     |
|    <span data-ttu-id="0c904-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0c904-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="0c904-150">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-150">No</span></span>     |    <span data-ttu-id="0c904-151">Fréquence à laquelle le rapport doit être généré, en heures.</span><span class="sxs-lookup"><span data-stu-id="0c904-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="0c904-152">La valeur minimale est 4</span><span class="sxs-lookup"><span data-stu-id="0c904-152">Minimum value is 4</span></span>     |    <span data-ttu-id="0c904-153">Integer</span><span class="sxs-lookup"><span data-stu-id="0c904-153">Integer</span></span>     |
|    <span data-ttu-id="0c904-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0c904-154">RecurrenceCount</span></span>     |    <span data-ttu-id="0c904-155">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-155">No</span></span>     |    <span data-ttu-id="0c904-156">Nombre de rapports à générer.</span><span class="sxs-lookup"><span data-stu-id="0c904-156">Numbers of report to be generated.</span></span> <span data-ttu-id="0c904-157">La valeur par défaut est indéfinie.</span><span class="sxs-lookup"><span data-stu-id="0c904-157">Default is indefinite.</span></span>     |    <span data-ttu-id="0c904-158">Integer</span><span class="sxs-lookup"><span data-stu-id="0c904-158">Integer</span></span>     |
|    <span data-ttu-id="0c904-159">Format</span><span class="sxs-lookup"><span data-stu-id="0c904-159">Format</span></span>     |    <span data-ttu-id="0c904-160">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-160">No</span></span>    |    <span data-ttu-id="0c904-161">Format du fichier exporté.</span><span class="sxs-lookup"><span data-stu-id="0c904-161">File format of the exported file.</span></span> <span data-ttu-id="0c904-162">La valeur par défaut est CSV</span><span class="sxs-lookup"><span data-stu-id="0c904-162">Default is CSV</span></span>     |    <span data-ttu-id="0c904-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="0c904-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="0c904-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="0c904-164">CallbackURL</span></span>     |    <span data-ttu-id="0c904-165">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-165">No</span></span>     |    <span data-ttu-id="0c904-166">URL de rappel HTTPS à appeler lors de la génération du rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="0c904-167">String</span><span class="sxs-lookup"><span data-stu-id="0c904-167">String</span></span>     |
|    <span data-ttu-id="0c904-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0c904-168">CallbackMethod</span></span>    |    <span data-ttu-id="0c904-169">Non</span><span class="sxs-lookup"><span data-stu-id="0c904-169">No</span></span>    |    <span data-ttu-id="0c904-170">Méthode http à utiliser pour le rappel</span><span class="sxs-lookup"><span data-stu-id="0c904-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="0c904-171">RECEVOIR/POSTER</span><span class="sxs-lookup"><span data-stu-id="0c904-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="0c904-172">**Réponse**</span><span class="sxs-lookup"><span data-stu-id="0c904-172">**Response**</span></span>

<span data-ttu-id="0c904-173">La charge utile de la réponse est structurée comme suit :</span><span class="sxs-lookup"><span data-stu-id="0c904-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="0c904-174">Code de réponse : 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0c904-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0c904-175">Exemple de charge utile de réponse :</span><span class="sxs-lookup"><span data-stu-id="0c904-175">Response payload example:</span></span>

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

<span data-ttu-id="0c904-176">**Glossaire**</span><span class="sxs-lookup"><span data-stu-id="0c904-176">**Glossary**</span></span>

<span data-ttu-id="0c904-177">Ce tableau définit les éléments clés de la réponse :</span><span class="sxs-lookup"><span data-stu-id="0c904-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="0c904-178">Paramètre</span><span class="sxs-lookup"><span data-stu-id="0c904-178">Parameter</span></span>    |    <span data-ttu-id="0c904-179">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0c904-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="0c904-180">ReportId</span></span>     |    <span data-ttu-id="0c904-181">Identificateur unique universel (UUID) du rapport en cours de mise à jour</span><span class="sxs-lookup"><span data-stu-id="0c904-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="0c904-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="0c904-182">ReportName</span></span>     |    <span data-ttu-id="0c904-183">Nom donné au rapport dans la charge utile de la requête</span><span class="sxs-lookup"><span data-stu-id="0c904-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0c904-184">Description</span><span class="sxs-lookup"><span data-stu-id="0c904-184">Description</span></span>     |    <span data-ttu-id="0c904-185">Description donnée au rapport dans la charge utile de la demande</span><span class="sxs-lookup"><span data-stu-id="0c904-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0c904-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="0c904-186">QueryId</span></span>     |    <span data-ttu-id="0c904-187">ID de requête passé au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="0c904-188">Requête</span><span class="sxs-lookup"><span data-stu-id="0c904-188">Query</span></span>     |    <span data-ttu-id="0c904-189">Texte de requête qui sera exécuté pour ce rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="0c904-190">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="0c904-190">User</span></span>     |    <span data-ttu-id="0c904-191">ID d’utilisateur utilisé pour créer le rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="0c904-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0c904-192">CreatedTime</span></span>     |    <span data-ttu-id="0c904-193">Heure de création du rapport.</span><span class="sxs-lookup"><span data-stu-id="0c904-193">Time the report was created.</span></span> <span data-ttu-id="0c904-194">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0c904-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0c904-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0c904-195">ModifiedTime</span></span>     |    <span data-ttu-id="0c904-196">Heure de dernière modification du rapport.</span><span class="sxs-lookup"><span data-stu-id="0c904-196">Time the report was last modified.</span></span> <span data-ttu-id="0c904-197">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0c904-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0c904-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0c904-198">ExecuteNow</span></span>     |    <span data-ttu-id="0c904-199">Indicateur ExecuteNow défini au moment de la création du rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="0c904-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="0c904-200">StartTime</span></span>     |    <span data-ttu-id="0c904-201">Heure de début de l’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="0c904-201">Time the report execution will begin.</span></span> <span data-ttu-id="0c904-202">Le format d’heure est aaaa-MM-jjThh:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0c904-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0c904-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="0c904-203">ReportStatus</span></span>     |    <span data-ttu-id="0c904-204">État d’exécution du rapport.</span><span class="sxs-lookup"><span data-stu-id="0c904-204">Status of the report execution.</span></span> <span data-ttu-id="0c904-205">Les valeurs possibles sont Paused, Active et Inactive.</span><span class="sxs-lookup"><span data-stu-id="0c904-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="0c904-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0c904-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="0c904-207">Intervalle de récurrence fourni dans la charge utile de la demande</span><span class="sxs-lookup"><span data-stu-id="0c904-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="0c904-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0c904-208">RecurrenceCount</span></span>     |    <span data-ttu-id="0c904-209">Nombre de récurrences fourni dans la charge utile de la demande</span><span class="sxs-lookup"><span data-stu-id="0c904-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="0c904-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0c904-210">CallbackUrl</span></span>     |    <span data-ttu-id="0c904-211">URL de rappel fournie dans la requête</span><span class="sxs-lookup"><span data-stu-id="0c904-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="0c904-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0c904-212">CallbackMethod</span></span>    |    <span data-ttu-id="0c904-213">Méthode de rappel fournie dans la demande</span><span class="sxs-lookup"><span data-stu-id="0c904-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="0c904-214">Format</span><span class="sxs-lookup"><span data-stu-id="0c904-214">Format</span></span>     |    <span data-ttu-id="0c904-215">Format des fichiers de rapport</span><span class="sxs-lookup"><span data-stu-id="0c904-215">Format of the report files</span></span>     |
|    <span data-ttu-id="0c904-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="0c904-216">TotalCount</span></span>     |    <span data-ttu-id="0c904-217">Nombre de jeux de données dans le tableau de valeurs</span><span class="sxs-lookup"><span data-stu-id="0c904-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="0c904-218">Message</span><span class="sxs-lookup"><span data-stu-id="0c904-218">Message</span></span>     |    <span data-ttu-id="0c904-219">Message d’état d’’exécution de l’API</span><span class="sxs-lookup"><span data-stu-id="0c904-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="0c904-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0c904-220">StatusCode</span></span>     |    <span data-ttu-id="0c904-221">Code de résultat.</span><span class="sxs-lookup"><span data-stu-id="0c904-221">Result Code.</span></span> <span data-ttu-id="0c904-222">Les valeurs possibles sont 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0c904-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |