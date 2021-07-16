---
title: Liste des API permettant d’accéder aux données de Partner Insights
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Liste des API permettant d’accéder aux données de Partner Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375570"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="2f3ce-103">API disponibles pour l’analyse partenaire Insights</span><span class="sxs-lookup"><span data-stu-id="2f3ce-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="2f3ce-104">Voici la liste des API pour l’analytique Partner Insights et leurs fonctionnalités associées.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="2f3ce-105">API d’extraction de jeux de données</span><span class="sxs-lookup"><span data-stu-id="2f3ce-105">Dataset pull APIs</span></span>

<span data-ttu-id="2f3ce-106">***Tableau 1 : API d’extraction de jeux de données***</span><span class="sxs-lookup"><span data-stu-id="2f3ce-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="2f3ce-107">**API**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-107">**API**</span></span> | <span data-ttu-id="2f3ce-108">**Fonctionnalité**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2f3ce-109">Obtenir tous les jeux de données</span><span class="sxs-lookup"><span data-stu-id="2f3ce-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="2f3ce-110">Obtient tous les jeux de données disponibles.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-110">Gets all the available datasets.</span></span> <span data-ttu-id="2f3ce-111">Les jeux de données répertorient les tables, les colonnes, les métriques et les intervalles de temps.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="2f3ce-112">API de gestion des requêtes</span><span class="sxs-lookup"><span data-stu-id="2f3ce-112">Query management APIs</span></span>

<span data-ttu-id="2f3ce-113">***Tableau 2 : API de gestion des requêtes***</span><span class="sxs-lookup"><span data-stu-id="2f3ce-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="2f3ce-114">**API**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-114">**API**</span></span> | <span data-ttu-id="2f3ce-115">**Fonctionnalité**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2f3ce-116">Créer une requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="2f3ce-117">Crée des requêtes personnalisées qui définissent le jeu de données à partir duquel les colonnes et les métriques doivent être exportées.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="2f3ce-118">OBTENIR une requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="2f3ce-119">Obtient toutes les requêtes disponibles à utiliser dans les rapports.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="2f3ce-120">Obtient par défaut toutes les requêtes système et définies par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="2f3ce-121">SUPPRIMER la requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="2f3ce-122">Supprime les requêtes définies par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="2f3ce-123">API de gestion des rapports</span><span class="sxs-lookup"><span data-stu-id="2f3ce-123">Report management APIs</span></span>

<span data-ttu-id="2f3ce-124">***Tableau 3 : API de gestion des rapports***</span><span class="sxs-lookup"><span data-stu-id="2f3ce-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="2f3ce-125">**API**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-125">**API**</span></span> | <span data-ttu-id="2f3ce-126">**Fonctionnalité**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2f3ce-127">Créer un rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="2f3ce-128">Planifie l’exécution d’une requête à intervalles réguliers.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="2f3ce-129">TESTER la requête de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="2f3ce-130">Exécute une instruction de requête de rapport.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-130">Executes a Report query statement.</span></span> <span data-ttu-id="2f3ce-131">Renvoie uniquement 10 enregistrements qu’un partenaire peut utiliser pour vérifier si les données sont identiques à celles attendues.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="2f3ce-132">Obtenir le rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="2f3ce-133">Récupère tous les rapports planifiés.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="2f3ce-134">Mettre à jour le rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="2f3ce-135">Modifie un paramètre de rapport.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="2f3ce-136">Supprimer le rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="2f3ce-137">Supprime tous les enregistrements de rapport et d’exécution de rapport.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="2f3ce-138">Mettre en pause les exécutions de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="2f3ce-139">Met en pause l’exécution planifiée des rapports.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="2f3ce-140">Reprendre les exécutions de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="2f3ce-141">Reprend l’exécution planifiée d’un rapport mis en pause.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="2f3ce-142">API d’extraction d’exécution de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-142">Report execution pull APIs</span></span>

<span data-ttu-id="2f3ce-143">***Tableau 4 : API d’extraction d’exécution de rapport***</span><span class="sxs-lookup"><span data-stu-id="2f3ce-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="2f3ce-144">**API**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-144">**API**</span></span> | <span data-ttu-id="2f3ce-145">**Fonctionnalité**</span><span class="sxs-lookup"><span data-stu-id="2f3ce-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="2f3ce-146">Obtenir les exécutions de rapport</span><span class="sxs-lookup"><span data-stu-id="2f3ce-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="2f3ce-147">Obtient toutes les exécutions intervenues pour un rapport donné.</span><span class="sxs-lookup"><span data-stu-id="2f3ce-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="2f3ce-148">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="2f3ce-148">Next steps</span></span>

- <span data-ttu-id="2f3ce-149">Vous pouvez tester les API à l’aide de l’[URL d’API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="2f3ce-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>