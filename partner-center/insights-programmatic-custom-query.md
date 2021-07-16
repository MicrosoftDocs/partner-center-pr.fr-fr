---
title: Spécification de requête personnalisée
description: Découvrez comment créer des requêtes personnalisées pour l’extraction de données à partir de tables analytiques.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375564"
---
# <a name="custom-query-specification"></a>Spécification de requête personnalisée

Les partenaires peuvent utiliser cette spécification de requête pour facilement formuler des requêtes personnalisées à des fins d’extraction de données à partir de tables analytiques. Les requêtes peuvent être utilisées pour sélectionner uniquement les colonnes et les métriques souhaitées correspondant à un critère spécifique. La spécification du langage repose sur la définition du jeu de données sur laquelle une requête personnalisée peut être écrite.

## <a name="datasets"></a>Groupes de données

De la même façon que certaines requêtes sont exécutées sur une base de données dotée de tables et de colonnes, une requête personnalisée fonctionne sur des jeux de données dotés de colonnes et de métriques. La liste complète des jeux de données disponibles pour formuler une requête peut être obtenue à l’aide de l’API des jeux de données.

Voici un exemple de jeu de données affiché en tant que JSON :

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Parties d’un jeu de données

- Un nom de jeu de données est similaire à un nom de table de base de données. Par exemple, OfficeUsage. Un DataSet contient une liste de colonnes qui peuvent être sélectionnées, par exemple CustomerTenantId.
- Un jeu de données possède également des métriques, qui s’apparentent aux fonctions d’agrégation d’une base de données. Par exemple, TotalMonthlyActiveUsers.
- Il existe des intervalles de temps fixes au cours desquels les données peuvent être exportées.

## <a name="formulating-a-query-on-a-dataset"></a>Formulation d’une requête sur un jeu de données

Voici quelques exemples de requêtes illustrant comment extraire différents types de données.

|Requête|    Description    |
|----|    ----    |
|**Sélectionnez** CustomerTenantId **, PaidAvailableUnits** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Cette requête obtiendra chaque CusotmerTenantID et ses PaidAvailableUnits correspondants au cours du dernier mois.    |
|**Sélectionnez** CustomerTenantId **, PaidAvailableUnits** <br>OfficeUsage **classement** par PaidAvailableUnits, **limite** 10|    Cette requête obtiendra les 10 principaux locataires client dans l’ordre décroissant du nombre d’unités disponibles payantes.     |
|**Sélectionnez** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **de** OfficeUsage, **où** MONTHLYACTIVEUSERS > 100000 **commander par** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Cette requête obtient les PaidAvailableUnits et les MonthlyActiveUsers de tous les clients dont le MonthlyActiveUsers est supérieur à 100 000.     |
|**Sélectionnez** CustomerTenantId, month, MonthlyActiveUsers **from** <br>OfficeUsage **où** CustomerTpId (' 2a31c234-1f4e-4C60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-B378-0242ac130002 ') |    Cette requête obtiendra les CustomerTenantId et les utilisateurs actifs mensuels pour chaque mois par les deux valeurs CustomerTpId : « 2a31c234-1f4e-4C60-909e-76d234f93161 » et « 80780748-3f9a-11eb-B378-0242ac130002 ».     |
|        |        |

## <a name="query-specification"></a>Spécification de requête

Cette section décrit la définition et la structure de la requête.

## <a name="grammar-reference"></a>Référence de grammaire

Ce tableau décrit les symboles utilisés dans les requêtes.

|    Requête    |    Description    |
|    ----    |    ----    |
|    `?`    |    Facultatif    |
|    `*`    |    Zéro ou plus    |
|    `+`    |    Un ou plus    |
|    `\|`    |    Ou/une des listes    |
|        |        |

## <a name="query-definition"></a>Définition de la requête

L’instruction de requête contient les clauses suivantes : SelectClause, FromClause, WhereClause, OrderClause, LimitClause et TimeSpan.

- **SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName** : colonnes et métriques définies dans le jeu de données
- **FromClause**: `FROM DatasetName`
    - **DatasetName**: nom du jeu de données défini dans le jeu de données
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: valeur de l’opérateur ColumOrMetricName
        - **Opérateur**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Valeur** : nombre | StringLiteral | MultiNumberList | MultiStringList
            - **Nombre**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList**: `(Number (,Number)*)`
            - **MultiStringList**: `(StringLiteral (,StringLiteral)*)`
- **OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition**: `ColumOrMetricName (ASC | DESC)*`
- **LimitClause**: `LIMIT [0-9]+`
- **Intervalle** de durée : `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Structure de la requête

Une requête de rapport est composée de plusieurs parties :
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Chaque partie est décrite ci-dessous.

### `SELECT`

Cette partie de la requête spécifie les colonnes qui seront exportées. Les colonnes qui peuvent être sélectionnées sont les champs répertoriés dans les sections *selectableColumns* et *availableMetrics* d’un jeu de données.

Si vous le souhaitez, le `DISTINCT` mot clé peut être spécifié après `SELECT` . Si `DISTINCT` est spécifié, les dernières lignes exportées contiennent toujours des valeurs distinctes des colonnes sélectionnées. Les mesures sont calculées pour chaque combinaison distincte des colonnes sélectionnées. par conséquent, `DISTINCT` le mot clé n’est pas requis quand une colonne métrique est incluse dans la liste Sélectionner une colonne.

**Exemple :**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Cette partie de la requête indique le jeu de données à partir duquel les données doivent être exportées. Le nom du jeu de données spécifié ici doit correspondre à un nom de jeu de données valide renvoyé par l’API des jeux de données.

**Exemple :**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Cette partie de la requête est utilisée pour spécifier les conditions de filtre du jeu de données. Seules les lignes correspondant à toutes les conditions répertoriées dans cette clause sont présentes dans le fichier exporté final. La condition de filtre peut figurer dans l’une des colonnes listées dans *selectableColumns* et *availableMetrics*. Les valeurs spécifiées dans la condition de filtre peuvent correspondre à une liste de nombres ou une liste de chaînes uniquement lorsque l’opérateur est `IN` ou `NOT IN`. Les valeurs peuvent toujours être spécifiées sous forme de chaîne littérale et sont converties en types natifs de colonnes. Plusieurs conditions de filtre doivent être séparées par une opération AND.

**Exemple :**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Cette partie de la requête spécifie les critères de tri des lignes exportées. Les colonnes sur lesquelles le classement peut être défini doivent provenir de *selectableColumns* et *availableMetrics* du DataSet. Si aucun sens de tri n’est spécifié, la valeur par défaut est DESC sur la colonne. Le tri peut être défini sur plusieurs colonnes en séparant les critères par une virgule.

**Exemple :**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Cette partie de la requête spécifie le nombre de lignes qui seront exportées. Le nombre que vous spécifiez doit être un entier positif non nul.

### `TIMESPAN`

Cette partie de la requête spécifie la durée pendant laquelle les données doivent être exportées. Les valeurs possibles doivent provenir du champ *availableDateRanges* dans la définition du jeu de données.

### <a name="case-sensitivity-in-query-specification"></a>Respect de la casse dans la spécification de requête

La spécification ne respecte pas la casse. Les mots clés prédéfinis, les noms de colonnes et les valeurs peuvent être spécifiés en majuscules ou en minuscules.

## <a name="next-steps"></a>Étapes suivantes

- [Liste des requêtes système](insights-programmatic-system-queries.md)
- [Liste des exemples de requêtes](insights-programmatic-sample-queries.md)