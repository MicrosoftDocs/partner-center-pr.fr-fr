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
# <a name="available-apis-for-partner-insights-analytics"></a>API disponibles pour l’analyse partenaire Insights

Voici la liste des API pour l’analytique Partner Insights et leurs fonctionnalités associées.

## <a name="dataset-pull-apis"></a>API d’extraction de jeux de données

***Tableau 1 : API d’extraction de jeux de données***

| **API** | **Fonctionnalité** |
| --- | --- |
| [Obtenir tous les jeux de données](insights-programmatic-analytics-api-get-dataset.md) | Obtient tous les jeux de données disponibles. Les jeux de données répertorient les tables, les colonnes, les métriques et les intervalles de temps. |
|||

## <a name="query-management-apis"></a>API de gestion des requêtes

***Tableau 2 : API de gestion des requêtes***

| **API** | **Fonctionnalité** |
| --- | --- |
| [Créer une requête de rapport](insights-programmatic-access-paradigm.md#create-report-query-api) | Crée des requêtes personnalisées qui définissent le jeu de données à partir duquel les colonnes et les métriques doivent être exportées. |
| [OBTENIR une requête de rapport](insights-programmatic-analytics-api-get-report-queries.md) | Obtient toutes les requêtes disponibles à utiliser dans les rapports. Obtient par défaut toutes les requêtes système et définies par l’utilisateur. |
| [SUPPRIMER la requête de rapport](insights-programmatic-analytics-api-delete-report-queries.md) | Supprime les requêtes définies par l’utilisateur. |
|||

## <a name="report-management-apis"></a>API de gestion des rapports

***Tableau 3 : API de gestion des rapports***

| **API** | **Fonctionnalité** |
| --- | --- |
| [Créer un rapport](insights-programmatic-access-paradigm.md#create-report-api) | Planifie l’exécution d’une requête à intervalles réguliers. |
| [TESTER la requête de rapport](insights-programmatic-analytics-api-try-report-queries.md) | Exécute une instruction de requête de rapport. Renvoie uniquement 10 enregistrements qu’un partenaire peut utiliser pour vérifier si les données sont identiques à celles attendues. |
| [Obtenir le rapport](insights-programmatic-analytics-api-get-report.md) | Récupère tous les rapports planifiés. |
| [Mettre à jour le rapport](insights-programmatic-analytics-api-update-report.md) | Modifie un paramètre de rapport. |
| [Supprimer le rapport](insights-programmatic-analytics-api-delete-report.md) | Supprime tous les enregistrements de rapport et d’exécution de rapport. |
| [Mettre en pause les exécutions de rapport](insights-programmatic-analytics-api-pause-report-executions.md) | Met en pause l’exécution planifiée des rapports. |
| [Reprendre les exécutions de rapport](insights-programmatic-analytics-api-resume-report-executions.md) | Reprend l’exécution planifiée d’un rapport mis en pause. |
|||

## <a name="report-execution-pull-apis"></a>API d’extraction d’exécution de rapport

***Tableau 4 : API d’extraction d’exécution de rapport***

| **API** | **Fonctionnalité** |
| --- | --- |
| [Obtenir les exécutions de rapport](insights-programmatic-access-paradigm.md#get-report-execution-api) | Obtient toutes les exécutions intervenues pour un rapport donné. |
|||

## <a name="next-steps"></a>Étapes suivantes

- Vous pouvez tester les API à l’aide de l’[URL d’API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).