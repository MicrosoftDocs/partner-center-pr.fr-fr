---
title: API d’extraction de requêtes de rapport-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour obtenir toutes les requêtes disponibles à utiliser dans l’API de rapport.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375606"
---
# <a name="get-report-queries-api"></a>API Obtenir des requêtes de rapport

L’API obtenir des requêtes de rapport obtient toutes les requêtes qui peuvent être utilisées dans les rapports. Elle obtient toutes les requêtes système et définies par l’utilisateur par défaut.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    queryId     |    string     |    Non    |    Filtre permettant d’obtenir les détails des seules requêtes avec l’ID fourni dans l’argument     |
|    NomRequête     |    string     |    Non    |    Filtre permettant d’obtenir les détails des seules requête avec le nom founi dans l’argument     |
|    IncludeSystemQueries     |    boolean     |    Non    |    Inclure les requêtes système prédéfinies dans la réponse     |
|    IncludeOnlySystemQueries     |    boolean     |    Non    |    Inclure uniquement les requêtes système dans la réponse     |
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
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    QueryId     |    UUID unique de la requête     |
|    Nom     |    Nom donné à la requête au moment de sa création     |
|    Description     |    Description donnée lors de la création de la requête     |
|    Requête     |    Chaîne de requête de rapport     |
|    Type     |    Défini sur userDefined pour les requêtes créées par l’utilisateur et système pour les requêtes système prédéfinies     |
|    Utilisateur     |    ID de l’utilisateur qui a créé la requête     |
|    CreatedTime     |    Heure de création de la requête     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |
