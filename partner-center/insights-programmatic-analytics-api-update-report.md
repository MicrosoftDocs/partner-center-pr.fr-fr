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
# <a name="update-report-api"></a>API Mettre à jour le rapport

Cette API vous permet de modifier un paramètre de rapport.

**Syntaxe de la requête**

|    Méthode    |    URI de requête    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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

**Glossaire**

Ce tableau liste les définitions clés des éléments dans la réponse.

|    Paramètre    |    Obligatoire    |    Description    |    Valeurs autorisées    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Oui     |    Nom à assigner au rapport     |    String     |
|    Description     |    Non     |    Description du rapport créé     |    String     |
|    StartTime     |    Oui    |    Horodatage à partir duquel la génération du rapport commence     |    String     |
|    RecurrenceInterval     |    Non     |    Fréquence à laquelle le rapport doit être généré, en heures. La valeur minimale est 4     |    Integer     |
|    RecurrenceCount     |    Non     |    Nombre de rapports à générer. La valeur par défaut est indéfinie.     |    Integer     |
|    Format     |    Non    |    Format du fichier exporté. La valeur par défaut est CSV     |    CSV/TSV     |
|    CallbackURL     |    Non     |    URL de rappel HTTPS à appeler lors de la génération du rapport     |    String     |
|    CallbackMethod    |    Non    |    Méthode http à utiliser pour le rappel    |    RECEVOIR/POSTER    |
|        |        |        |        |


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
|    ReportId     |    Identificateur unique universel (UUID) du rapport en cours de mise à jour     |
|    ReportName     |    Nom donné au rapport dans la charge utile de la requête     |
|    Description     |    Description donnée au rapport dans la charge utile de la demande     |
|    QueryId     |    ID de requête passé au moment de la création du rapport     |
|    Requête     |    Texte de requête qui sera exécuté pour ce rapport     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer le rapport     |
|    CreatedTime     |    Heure de création du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ModifiedTime     |    Heure de dernière modification du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ExecuteNow     |    Indicateur ExecuteNow défini au moment de la création du rapport    |
|    StartTime     |    Heure de début de l’exécution du rapport. Le format d’heure est aaaa-MM-jjThh:mm:ssZ     |
|    ReportStatus     |    État d’exécution du rapport. Les valeurs possibles sont Paused, Active et Inactive.     |
|    RecurrenceInterval     |    Intervalle de récurrence fourni dans la charge utile de la demande     |
|    RecurrenceCount     |    Nombre de récurrences fourni dans la charge utile de la demande     |
|    CallbackUrl     |    URL de rappel fournie dans la requête     |
|    CallbackMethod    |    Méthode de rappel fournie dans la demande    |
|    Format     |    Format des fichiers de rapport     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |