---
title: supprimer l’API de rapport-données de Informations
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour supprimer un rapport dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375615"
---
# <a name="delete-report-api"></a>API Supprimer le rapport

Lors de son exécution, cette API supprime tous les enregistrements de rapport et d’exécution de rapport.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    Suppression    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    string    |    Non    |    ID du rapport en cours de suppression    |
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
|    ReportId     |    Identificateur unique universel (UUID) du rapport supprimé     |
|    ReportName     |    Nom donné au rapport lors de la création     |
|    Description     |    Description donnée lors de la création du rapport     |
|    QueryId     |    ID de requête passé au moment de la création du rapport     |
|    Requête     |    Texte de requête qui sera exécuté pour ce rapport     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer le rapport     |
|    CreatedTime     |    Heure de création du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ModifiedTime     |    Heure de dernière modification du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ExecuteNow     |    Indicateur ExecuteNow défini au moment de la création du rapport     |
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
