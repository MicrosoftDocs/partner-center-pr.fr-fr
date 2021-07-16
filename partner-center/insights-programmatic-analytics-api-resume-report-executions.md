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
# <a name="resume-report-executions-api"></a>API Reprendre les exécutions de rapport

À l’exécution, cette API reprend l’exécution planifiée d’un rapport suspendu.

**Syntaxe de la requête**

|    Méthode    |    URI de requête    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

**En-tête de requête**

|    En-tête    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisation    |    string    |    Obligatoire. le jeton d’accès Azure Active Directory (AAD) sous la forme`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Paramètre de chemin**

|    Nom du paramètre    |    Type    |    Obligatoire    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    Non    |    ID du rapport en cours de modification     |
|        |        |        |        |

**Paramètre de requête.**

Aucun

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

**Glossaire**

Ce tableau définit les éléments clés de la réponse :

|    Paramètre    |    Description    |
|    ----    |    ----    |
|    ReportId     |    Identificateur unique universel (UUID) du rapport dont la reprise a été effectuée     |
|    ReportName     |    Nom donné au rapport lors de la création     |
|    Description     |    Description donnée lors de la création du rapport     |
|    QueryId     |    ID de requête passé au moment de la création du rapport     |
|    Requête     |    Texte de requête qui sera exécuté pour ce rapport     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer le rapport     |
|    CreatedTime     |    Heure de création du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ModifiedTime     |    Heure de dernière modification du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ExecuteNow     |    Indicateur ExecuteNow défini au moment de la création du rapport    |
|    StartTime     |    Heure de début de l’exécution du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
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
