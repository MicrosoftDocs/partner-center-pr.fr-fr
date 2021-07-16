---
title: API d’extraction de tous les jeux de données-Informations données
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez cette API pour récupérer les détails de tous les jeux de données disponibles dans les Insights de l’espace partenaires.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375358"
---
# <a name="get-all-datasets-api"></a>API Obtenir tous les jeux de données

L’API Obtenir tous les jeux de données obtient tous les jeux de données disponibles. Les jeux de données listent les tables, les colonnes, les métriques et les intervalles de temps.

**Syntaxe de la requête**

|    Méthode    |    URI de demande    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    NomGroupeDonnées    |    string    |    Non    |    Filtrer pour afficher les détails d’un seul jeu de données    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Glossaire**

Ce tableau définit les éléments clés de la réponse :

|    Paramètre    |    Description    |
|    ----    |    ----    |
|    DatasetName     |    Nom du jeu de données défini par cet objet de tableau     |
|    SelectableColumns     |    Colonnes brutes qui peuvent être spécifiées dans les colonnes sélectionnées     |
|    AvailableMetrics     |    Noms des colonnes d’agrégation/métriques qui peuvent être spécifiées dans les colonnes sélectionnées     |
|    AvailableDateRanges     |    Plage de dates qui peut être utilisée dans les requêtes de rapport pour le jeu de données     |
|    minimumRecurrenceInterval     |    Valeur minimale de l’intervalle de récurrence     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    Message     |    Message d’état d’’exécution de l’API     |
|    StatusCode     |    Code de résultat. Les valeurs possibles sont 200, 400, 401, 403, 500     |
|        |        |
