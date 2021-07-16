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
# <a name="get-report-api"></a>API Obtenir le rapport

Cette API permet d’obtenir tous les rapports planifiés.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**En-tête de requête**

|    En-tête    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisation    |    string    |    Obligatoire. le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Paramètre de chemin**

Aucun

**Paramètre de requête.**

|    Nom du paramètre    |    Type    |    Obligatoire    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    Non    |    Filtre pour afficher uniquement les détails des rapports avec le reportId donné dans cet argument     |
|    reportName     |    string    |    Non    |    Filtre pour afficher uniquement les détails des rapports avec le rapport reportName fourni dans cet argument     |
|    queryId     |    string    |    Non    |    Filtre pour extraire uniquement les détails des rapports avec l’queryId donné dans cet argument     |
|        |        |        |        |


**Charge utile de demande**

Aucun

**Glossaire**

Aucune

**Réponse**

La charge utile de la réponse est structurée comme suit :

Code de réponse : 200, 400, 401, 403, 404, 500

Exemple de charge utile de réponse :

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

**Glossaire**

Ce tableau définit les éléments clés de la réponse :

|    Paramètre    |    Description    |
|    ----    |    ----    |
|    ReportId     |    UUID unique du rapport créé     |
|    ReportName     |    Nom donné au rapport dans la charge utile de la requête     |
|    Description     |    Description fournie lors de la création du rapport     |
|    QueryId     |    ID de requête passé au moment de la création du rapport     |
|    Requête     |    Texte de requête qui sera exécuté pour ce rapport     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer le rapport     |
|    CreatedTime     |    Heure de création du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ModifiedTime     |    Heure de dernière modification du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    executeNow     |    Indicateur ExecuteNow défini au moment de la création du rapport    |
|    StartTime     |    Heure de début de l’exécution. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ReportStatus     |    État d’exécution du rapport. Les valeurs possibles sont Paused, Active et Inactive.     |
|    RecurrenceInterval     |    Intervalle de périodicité fourni lors de la création du rapport     |
|    RecurrenceCount     |    Nombre de récurrences fourni lors de la création du rapport     |
|    CallbackUrl     |    URL de rappel fournie dans la requête     |
|    CallbackMethod    |    Méthode de rappel fournie dans la demande    |
|    Format     |    Format des fichiers de rapport     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |