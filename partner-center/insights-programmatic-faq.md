---
title: Questions courantes sur l’accès par programme à Partner Insights
description: Recevez des réponses aux questions les plus fréquentes sur l’accès aux données de Partner Insights par le biais de l’API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375555"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Questions fréquentes sur l’accès programmatique aux données d’analyse

Cet article répond aux questions fréquemment posées sur la façon d’accéder par programmation aux données des informations des partenaires dans l’espace partenaires.

## <a name="api-responses"></a>Réponses de l’API

Quels sont les différents scénarios dans lesquels je peux recevoir une réponse de l’API autre que 200 (réussite) ?

Ce tableau décrit les réponses de l’API et la procédure à suivre si vous les recevez.

|    Description de l'erreur     |    Code d'erreur     |    Dépanner     |
|    ----    |    ----    |    ----    |
|    Non autorisé     |    401     |    Il s’agit d’une exception d’authentification. vérifiez l’exactitude du jeton Azure Active Directory (AAD). Le jeton AAD est valide pendant 60 minutes, après quoi vous auriez besoin de régénérer le jeton AAD.     |
|    Nom de table non valide     |    400     |    Le nom du jeu de données est incorrect. Revérifiez le nom du DataSet en appelant l’API « récupérer tous les jeux de données ».     |
|    Nom de colonne incorrect     |    400     |    Le nom de la colonne de la requête est incorrect. Revérifiez le nom de la colonne en appelant l’API « récupérer tous les jeux de données » ou reportez-vous aux noms des colonnes dans les définitions de données.    |
|    Valeur null ou manquante     |    400     |    Il se peut que des paramètres obligatoires soient absents de la charge utile de requête de l’API.     |
|    Paramètres de rapport non valides     |    400     |    Assurez-vous que les paramètres de rapport sont corrects. Par exemple, vous pouvez donner une valeur inférieure à 4 pour le paramètre RecurrenceInterval.     |
|    L’intervalle de récurrence doit être compris entre 4 et 2160     |    400     |    Assurez-vous que la valeur du paramètre de requête RecurrenceInterval est comprise entre 4 et 2160.     |
|    QueryId non valide     |    400     |    Revérifiez l’QueryId généré.     |
|    Paramètres de rapport non valides pour la création-l’heure de début du rapport doit être d’au moins 4 heures à partir de l’heure UTC actuelle     |    400     |    Le paramètre de l’heure de début dans le cadre de la charge utile de la requête ne doit pas être dans le passé. L’heure de début du rapport doit se situer à au moins 4 heures par rapport à l’heure UTC actuelle.     |
|    La valeur demandée’chaîne’est introuvable     |    400     |    Vérifiez si vous avez mis à jour les paramètres ou le format de la requête `callbackurl` .     |
|    Aucun élément n’a été trouvé avec les filtres spécifiés.     |    404     |    Vérifiez le paramètre reportID utilisé dans l’API d’extraction des exécutions de rapports.     |
|    Aucune exécution n’est intervenue pour les conditions de filtre données. Vérifiez à nouveau le reportId ou le executionId et recommencez l’API après l’exécution planifiée du rapport.     |    404     |    Assurez-vous que le reportId est correct. Réessayez l’API après l’heure d’exécution planifiée du rapport, comme indiqué dans la charge utile de la demande.     |
|    Une erreur interne s’est produite lors de la création du rapport. ID de corrélation <>     |    500     |    Assurez-vous que le format de date pour les champs *StartTime*, *QueryStartTime* et *QueryEndTime* est correct.     |
|    Service indisponible    |    500     |    Si vous recevez continuellement un service non disponible (erreur 5xx), ouvrez un ticket de support.    |
|        |        |        |

## <a name="no-records"></a>Aucun enregistrement

Je reçois une réponse d’API 200 lorsque je télécharge le rapport à partir de l’emplacement sécurisé. Pourquoi est-ce que je n’obtiens aucun enregistrement ?
Vérifiez que la chaîne de la requête présente une valeur autorisée pour l’en-tête de colonne. Par exemple, cette requête ne renvoie aucun résultat :

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

Dans cet exemple, les valeurs autorisées pour `IsDuplicateRowForPGA` sont 0 ou 1. Reportez-vous aux [définitions de données](insights-data-definitions.md) pour toutes les valeurs possibles des différentes colonnes.
