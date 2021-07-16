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
# <a name="custom-query-specification"></a><span data-ttu-id="70a9d-103">Spécification de requête personnalisée</span><span class="sxs-lookup"><span data-stu-id="70a9d-103">Custom query specification</span></span>

<span data-ttu-id="70a9d-104">Les partenaires peuvent utiliser cette spécification de requête pour facilement formuler des requêtes personnalisées à des fins d’extraction de données à partir de tables analytiques.</span><span class="sxs-lookup"><span data-stu-id="70a9d-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="70a9d-105">Les requêtes peuvent être utilisées pour sélectionner uniquement les colonnes et les métriques souhaitées correspondant à un critère spécifique.</span><span class="sxs-lookup"><span data-stu-id="70a9d-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="70a9d-106">La spécification du langage repose sur la définition du jeu de données sur laquelle une requête personnalisée peut être écrite.</span><span class="sxs-lookup"><span data-stu-id="70a9d-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="70a9d-107">Groupes de données</span><span class="sxs-lookup"><span data-stu-id="70a9d-107">Datasets</span></span>

<span data-ttu-id="70a9d-108">De la même façon que certaines requêtes sont exécutées sur une base de données dotée de tables et de colonnes, une requête personnalisée fonctionne sur des jeux de données dotés de colonnes et de métriques.</span><span class="sxs-lookup"><span data-stu-id="70a9d-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="70a9d-109">La liste complète des jeux de données disponibles pour formuler une requête peut être obtenue à l’aide de l’API des jeux de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="70a9d-110">Voici un exemple de jeu de données affiché en tant que JSON :</span><span class="sxs-lookup"><span data-stu-id="70a9d-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="70a9d-111">Parties d’un jeu de données</span><span class="sxs-lookup"><span data-stu-id="70a9d-111">Parts of a dataset</span></span>

- <span data-ttu-id="70a9d-112">Un nom de jeu de données est similaire à un nom de table de base de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="70a9d-113">Par exemple, OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="70a9d-113">For example, OfficeUsage.</span></span> <span data-ttu-id="70a9d-114">Un DataSet contient une liste de colonnes qui peuvent être sélectionnées, par exemple CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="70a9d-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="70a9d-115">Un jeu de données possède également des métriques, qui s’apparentent aux fonctions d’agrégation d’une base de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="70a9d-116">Par exemple, TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="70a9d-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="70a9d-117">Il existe des intervalles de temps fixes au cours desquels les données peuvent être exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="70a9d-118">Formulation d’une requête sur un jeu de données</span><span class="sxs-lookup"><span data-stu-id="70a9d-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="70a9d-119">Voici quelques exemples de requêtes illustrant comment extraire différents types de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="70a9d-120">Requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-120">Query</span></span>|    <span data-ttu-id="70a9d-121">Description</span><span class="sxs-lookup"><span data-stu-id="70a9d-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="70a9d-122">**Sélectionnez** CustomerTenantId **, PaidAvailableUnits**</span><span class="sxs-lookup"><span data-stu-id="70a9d-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="70a9d-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="70a9d-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="70a9d-124">Cette requête obtiendra chaque CusotmerTenantID et ses PaidAvailableUnits correspondants au cours du dernier mois.</span><span class="sxs-lookup"><span data-stu-id="70a9d-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="70a9d-125">**Sélectionnez** CustomerTenantId **, PaidAvailableUnits**</span><span class="sxs-lookup"><span data-stu-id="70a9d-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="70a9d-126">OfficeUsage **classement** par PaidAvailableUnits, **limite** 10</span><span class="sxs-lookup"><span data-stu-id="70a9d-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="70a9d-127">Cette requête obtiendra les 10 principaux locataires client dans l’ordre décroissant du nombre d’unités disponibles payantes.</span><span class="sxs-lookup"><span data-stu-id="70a9d-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="70a9d-128">**Sélectionnez** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **de** OfficeUsage, **où** MONTHLYACTIVEUSERS > 100000 **commander par** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="70a9d-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="70a9d-129">Cette requête obtient les PaidAvailableUnits et les MonthlyActiveUsers de tous les clients dont le MonthlyActiveUsers est supérieur à 100 000.</span><span class="sxs-lookup"><span data-stu-id="70a9d-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="70a9d-130">**Sélectionnez** CustomerTenantId, month, MonthlyActiveUsers **from**</span><span class="sxs-lookup"><span data-stu-id="70a9d-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="70a9d-131">OfficeUsage **où** CustomerTpId (' 2a31c234-1f4e-4C60-909e-76d234f93161 ', ' 80780748-3f9a-11eb-B378-0242ac130002 ')</span><span class="sxs-lookup"><span data-stu-id="70a9d-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="70a9d-132">Cette requête obtiendra les CustomerTenantId et les utilisateurs actifs mensuels pour chaque mois par les deux valeurs CustomerTpId : « 2a31c234-1f4e-4C60-909e-76d234f93161 » et « 80780748-3f9a-11eb-B378-0242ac130002 ».</span><span class="sxs-lookup"><span data-stu-id="70a9d-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="70a9d-133">Spécification de requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-133">Query specification</span></span>

<span data-ttu-id="70a9d-134">Cette section décrit la définition et la structure de la requête.</span><span class="sxs-lookup"><span data-stu-id="70a9d-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="70a9d-135">Référence de grammaire</span><span class="sxs-lookup"><span data-stu-id="70a9d-135">Grammar reference</span></span>

<span data-ttu-id="70a9d-136">Ce tableau décrit les symboles utilisés dans les requêtes.</span><span class="sxs-lookup"><span data-stu-id="70a9d-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="70a9d-137">Requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-137">Query</span></span>    |    <span data-ttu-id="70a9d-138">Description</span><span class="sxs-lookup"><span data-stu-id="70a9d-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="70a9d-139">Facultatif</span><span class="sxs-lookup"><span data-stu-id="70a9d-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="70a9d-140">Zéro ou plus</span><span class="sxs-lookup"><span data-stu-id="70a9d-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="70a9d-141">Un ou plus</span><span class="sxs-lookup"><span data-stu-id="70a9d-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="70a9d-142">Ou/une des listes</span><span class="sxs-lookup"><span data-stu-id="70a9d-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="70a9d-143">Définition de la requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-143">Query definition</span></span>

<span data-ttu-id="70a9d-144">L’instruction de requête contient les clauses suivantes : SelectClause, FromClause, WhereClause, OrderClause, LimitClause et TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="70a9d-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="70a9d-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="70a9d-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="70a9d-146">**ColumOrMetricName** : colonnes et métriques définies dans le jeu de données</span><span class="sxs-lookup"><span data-stu-id="70a9d-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="70a9d-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="70a9d-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="70a9d-148">**DatasetName**: nom du jeu de données défini dans le jeu de données</span><span class="sxs-lookup"><span data-stu-id="70a9d-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="70a9d-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="70a9d-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="70a9d-150">**FilterCondition**: valeur de l’opérateur ColumOrMetricName</span><span class="sxs-lookup"><span data-stu-id="70a9d-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="70a9d-151">**Opérateur**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="70a9d-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="70a9d-152">**Valeur** : nombre | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="70a9d-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="70a9d-153">**Nombre**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="70a9d-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="70a9d-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="70a9d-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="70a9d-155">**MultiNumberList**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="70a9d-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="70a9d-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="70a9d-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="70a9d-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="70a9d-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="70a9d-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="70a9d-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="70a9d-159">**LimitClause**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="70a9d-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="70a9d-160">**Intervalle** de durée : `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="70a9d-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="70a9d-161">Structure de la requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-161">Query Structure</span></span>

<span data-ttu-id="70a9d-162">Une requête de rapport est composée de plusieurs parties :</span><span class="sxs-lookup"><span data-stu-id="70a9d-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="70a9d-163">Chaque partie est décrite ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="70a9d-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="70a9d-164">Cette partie de la requête spécifie les colonnes qui seront exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="70a9d-165">Les colonnes qui peuvent être sélectionnées sont les champs répertoriés dans les sections *selectableColumns* et *availableMetrics* d’un jeu de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="70a9d-166">Si vous le souhaitez, le `DISTINCT` mot clé peut être spécifié après `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="70a9d-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="70a9d-167">Si `DISTINCT` est spécifié, les dernières lignes exportées contiennent toujours des valeurs distinctes des colonnes sélectionnées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="70a9d-168">Les mesures sont calculées pour chaque combinaison distincte des colonnes sélectionnées. par conséquent, `DISTINCT` le mot clé n’est pas requis quand une colonne métrique est incluse dans la liste Sélectionner une colonne.</span><span class="sxs-lookup"><span data-stu-id="70a9d-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="70a9d-169">**Exemple :**</span><span class="sxs-lookup"><span data-stu-id="70a9d-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="70a9d-170">Cette partie de la requête indique le jeu de données à partir duquel les données doivent être exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="70a9d-171">Le nom du jeu de données spécifié ici doit correspondre à un nom de jeu de données valide renvoyé par l’API des jeux de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="70a9d-172">**Exemple :**</span><span class="sxs-lookup"><span data-stu-id="70a9d-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="70a9d-173">Cette partie de la requête est utilisée pour spécifier les conditions de filtre du jeu de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="70a9d-174">Seules les lignes correspondant à toutes les conditions répertoriées dans cette clause sont présentes dans le fichier exporté final.</span><span class="sxs-lookup"><span data-stu-id="70a9d-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="70a9d-175">La condition de filtre peut figurer dans l’une des colonnes listées dans *selectableColumns* et *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="70a9d-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="70a9d-176">Les valeurs spécifiées dans la condition de filtre peuvent correspondre à une liste de nombres ou une liste de chaînes uniquement lorsque l’opérateur est `IN` ou `NOT IN`.</span><span class="sxs-lookup"><span data-stu-id="70a9d-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="70a9d-177">Les valeurs peuvent toujours être spécifiées sous forme de chaîne littérale et sont converties en types natifs de colonnes.</span><span class="sxs-lookup"><span data-stu-id="70a9d-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="70a9d-178">Plusieurs conditions de filtre doivent être séparées par une opération AND.</span><span class="sxs-lookup"><span data-stu-id="70a9d-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="70a9d-179">**Exemple :**</span><span class="sxs-lookup"><span data-stu-id="70a9d-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="70a9d-180">Cette partie de la requête spécifie les critères de tri des lignes exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="70a9d-181">Les colonnes sur lesquelles le classement peut être défini doivent provenir de *selectableColumns* et *availableMetrics* du DataSet.</span><span class="sxs-lookup"><span data-stu-id="70a9d-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="70a9d-182">Si aucun sens de tri n’est spécifié, la valeur par défaut est DESC sur la colonne.</span><span class="sxs-lookup"><span data-stu-id="70a9d-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="70a9d-183">Le tri peut être défini sur plusieurs colonnes en séparant les critères par une virgule.</span><span class="sxs-lookup"><span data-stu-id="70a9d-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="70a9d-184">**Exemple :**</span><span class="sxs-lookup"><span data-stu-id="70a9d-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="70a9d-185">Cette partie de la requête spécifie le nombre de lignes qui seront exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="70a9d-186">Le nombre que vous spécifiez doit être un entier positif non nul.</span><span class="sxs-lookup"><span data-stu-id="70a9d-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="70a9d-187">Cette partie de la requête spécifie la durée pendant laquelle les données doivent être exportées.</span><span class="sxs-lookup"><span data-stu-id="70a9d-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="70a9d-188">Les valeurs possibles doivent provenir du champ *availableDateRanges* dans la définition du jeu de données.</span><span class="sxs-lookup"><span data-stu-id="70a9d-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="70a9d-189">Respect de la casse dans la spécification de requête</span><span class="sxs-lookup"><span data-stu-id="70a9d-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="70a9d-190">La spécification ne respecte pas la casse.</span><span class="sxs-lookup"><span data-stu-id="70a9d-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="70a9d-191">Les mots clés prédéfinis, les noms de colonnes et les valeurs peuvent être spécifiés en majuscules ou en minuscules.</span><span class="sxs-lookup"><span data-stu-id="70a9d-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70a9d-192">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="70a9d-192">Next steps</span></span>

- [<span data-ttu-id="70a9d-193">Liste des requêtes système</span><span class="sxs-lookup"><span data-stu-id="70a9d-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="70a9d-194">Liste des exemples de requêtes</span><span class="sxs-lookup"><span data-stu-id="70a9d-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)