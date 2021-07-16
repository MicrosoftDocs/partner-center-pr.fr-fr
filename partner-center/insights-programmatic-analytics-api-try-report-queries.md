---
title: API Essayer des requêtes de rapport
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour tester votre requête et valider les résultats dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375582"
---
# <a name="try-report-queries-api"></a>API Essayer des requêtes de rapport

Cette API exécute une instruction de requête de rapport. L’API retourne uniquement 100 enregistrements que vous pouvez utiliser comme partenaire pour vérifier si les données sont les mêmes que prévu.

> [!IMPORTANT]
> Cette API a un délai d’expiration d’exécution de requête de 100 secondes. Si vous remarquez que l’API prend plus de 100 secondes, il est très probable que la requête soit syntaxiquement correcte, sinon vous auriez reçu un code d’erreur autre que 200. La génération du rapport réussit si la syntaxe de la requête est correcte.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
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
|    exportQuery     |    string    |    Non    |    Chaîne de requête de rapport qui doit être exécutée     |
|    queryId     |    string    |    Non    |    ID de requête existant valide. S’exclut mutuellement avec la chaîne de requête spécifiée dans le paramètre exportQuery    |
|    startTime     |    string    |    Non    |    Heure de début à partir de laquelle les données doivent être recherchées. Elle remplace la période spécifiée dans la requête    |
|    endTime     |    string    |    Non    |    Heure de fin jusqu’à laquelle les données doivent être recherchées. Elle remplace la période spécifiée dans la requête    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |
