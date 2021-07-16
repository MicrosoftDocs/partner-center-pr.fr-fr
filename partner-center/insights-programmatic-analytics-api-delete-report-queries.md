---
title: API de suppression des requêtes de rapport-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour supprimer une requête définie par l’utilisateur dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375379"
---
# <a name="delete-report-queries-api"></a>API Supprimer des requêtes de rapport

Cette API supprime les requêtes définies par l’utilisateur.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    Suppression    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
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
|    queryId     |    string     |    Non    |    Filtre permettant d’obtenir les détails des seules requêtes avec l’ID fourni dans l’argument     |
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
|    QueryId     |    UUID unique de la requête qui a été supprimée    |
|    Nom     |    Nom de la requête supprimée    |
|    Description     |    Description de la requête supprimée     |
|    Requête     |    Chaîne de requête de rapport de la requête supprimée    |
|    Type     |    Défini sur userDefined pour les requêtes créées par l’utilisateur     |
|    Utilisateur     |    ID de l’utilisateur qui a créé la requête     |
|    CreatedTime     |    Heure de création de la requête     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |
