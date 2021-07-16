---
title: paradigme d’accès par programme pour Informations données
description: Comprendre le flux général du modèle d’appel d’API pour l’analytique programmatique. Les API permettant d’accéder aux rapports analytiques de Partner Insights sont également couvertes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375382"
---
# <a name="programmatic-access-paradigm"></a>Paradigme de l’accès programmatique

Ce diagramme montre le modèle d’appel d’API utilisé pour créer un modèle de rapport, planifier le rapport personnalisé et récupérer les données d’échec.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Circuit de haut niveau":::
***Figure 1 : déroulement de haut niveau du modèle d’appel d’API***

Cette liste fournit plus de détails sur la Figure 1.

1. L’application cliente peut définir le schéma/modèle de rapport personnalisé en appelant l'[API Créer une requête de rapport](#create-report-query-api). Vous pouvez également choisir un modèle de rapport (QueryId) dans les exemples de la bibliothèque de modèles de rapport répertoriés [ici.](insights-programmatic-system-queries.md)
2. En cas de réussite, l’API de création de requête de rapport retourne l’QueryId.
3. L’application cliente doit ensuite appeler l' [API de création de rapport](#create-report-api) à l’aide du QueryId avec la date de début du rapport, l’intervalle de répétition, la récurrence et un URI de rappel facultatif.
4. En cas de réussite, l' [API de création de rapport](#create-report-api) retourne ReportID.
5. L’application cliente est notifiée à l’URL de rappel dès que les données du rapport sont prêtes à être téléchargées.
6. L’application cliente utilise ensuite l' [API obtenir des exécutions de rapport](#get-report-execution-api) pour interroger l’état du rapport avec l’ID de rapport et la plage de dates.
7. En cas de réussite, le lien de téléchargement du rapport est renvoyé et l’application peut lancer le téléchargement des données.

## <a name="report-query-language-specification"></a>Spécification du langage de requête de rapport

Alors que nous fournissons des [requêtes système](insights-programmatic-system-queries.md) que vous pouvez utiliser pour créer des rapports, vous pouvez également créer vos propres requêtes en fonction des besoins de votre entreprise. Pour en savoir plus sur les requêtes personnalisées, consultez [spécification de requête personnalisée](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>API Créer une requête de rapport

L’API permet de créer des requêtes personnalisées qui définissent le jeu de données à partir duquel les colonnes et les mesures doivent être exportées. L’API offre la flexibilité nécessaire pour créer un nouveau modèle de rapport basé sur les besoins de votre entreprise.  

Vous pouvez également utiliser les [requêtes système](insights-programmatic-system-queries.md) que nous fournissons. Lorsque des modèles de rapport personnalisés ne sont pas nécessaires, vous pouvez appeler l' [API de création de rapports](#create-report-api) directement à l’aide de la QueryIds des requêtes système fournies.  

L’exemple suivant montre comment créer une requête personnalisée pour obtenir les 10 premiers clients par revenu pour le mois dernier.

### <a name="request-syntax"></a>Syntaxe de la requête

|    Méthode     |    URI de demande     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>En-tête de requête

|    En-tête     |    Type     |    Description     |
|-------|-----|------|
|    Autorisation     |    string |Obligatoire. Jeton d’accès Azure Active Directory (Azure AD). Le format est  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Paramètre de chemin

Aucune

### <a name="query-parameter"></a>Paramètre de requête.

Aucune

### <a name="sample-request-payload"></a>Exemple de charge utile de demande

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glossaire

Ce tableau fournit les définitions clés des éléments dans la charge utile de requête.

|Paramètre|    Obligatoire     |    Description     |    Valeurs autorisées     |
|-----|    -----    |    -----    |    -----    |
|Nom |    Oui     |    Nom convivial de la requête     |    string     |
|    Description     |    Non     |    Description de ce que la requête renvoie     |    string     |
|    Requête     |    Oui     |    Chaîne de requête de rapport     |    Type de données : chaîne <br> [Requête personnalisée](insights-programmatic-custom-query.md) basée sur les besoins de l’entreprise |
|        |        |        |        |

> [!Note]
> Pour obtenir des exemples de requêtes personnalisées, consultez [exemples d’exemples de requêtes.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Exemple de réponse

La charge utile de la réponse est structurée comme suit :

Codes de réponse : 200, 400, 401, 403, 500

Exemple de charge utile de réponse :

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Glossaire

Ce tableau fournit les définitions clés des éléments dans la charge utile de requête.

|    Paramètre     |    Description     |
|    ----    |    ----    |
|    QueryId     |    Identificateur unique universel (UUID) de la requête créée     |
|    Nom     |    Nom convivial donné à la requête dans la charge utile de requête     |
|    Description     |    Description donnée lors de la création de la requête     |
|    Requête     |    Requête de rapport transmise en tant qu’entrée lors de la création de la requête     |
|    Type     |    Paramètre à définir sur `userDefined`     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer la requête     |
|    CreatedTime     |    Heure UTC de création de la requête au format suivant : aaaa-MM-jjThh:mm:ssZ     |
|    TotalCount     |    Nombre de jeux de données dans le tableau de valeurs     |
|    StatusCode     |    Code de résultat <br> Les valeurs possibles sont 200, 400, 401, 403, 500     |
|    message     |    Message d’état d’’exécution de l’API     |
|        |        |

## <a name="create-report-api"></a>API Créer un rapport

Lors de la création d’un modèle de rapport personnalisé avec succès et la réception de l’élément QueryID dans le cadre de la réponse à la [requête de création de rapport](#create-report-query-api) , cette API peut être appelée pour planifier l’exécution d’une requête à intervalles réguliers. Vous pouvez définir une fréquence et une planification pour le rapport à remettre.
Pour les requêtes système que nous fournissons, l’API Créer un rapport peut également être appelée avec [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>Callback URL (URL de rappel)

L’API de création de rapport accepte une URL de rappel. Cette URL sera appelée une fois la génération du rapport réussie. L’URL de rappel doit être publiquement accessible. En plus de l’URL, une méthode de rappel peut également être donnée. La méthode de rappel peut uniquement être « obtient » ou « poster ». La méthode par défaut si aucune valeur n’est passée est « poster ». Le reportId dont la génération est terminée sera toujours renvoyé pendant le rappel.

Rappel de publication : si l’URL transmise était `https://www.contosso.com/callback` , l’URL d’arrière-plan sera `https://www.contosso.com/callback/<reportID>` 

Obtient le rappel : si l’URL passée était `https://www.contosso.com/callback` , l’URL d’arrière-plan appelée sera `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Rapports ExecuteNow

Il existe une provision pour générer un rapport sans planification. La charge utile de l’API de création de rapport peut accepter un paramètre `ExecuteNow` , qui met en file d’attente le rapport à générer dès que l’API est appelée. Lorsque `ExecuteNow` a la valeur true, les champs : `StartTime` , `RecurrenceCount` , `RecurrenceInterval` sont ignorés, car ces rapports ne sont pas planifiés.

Deux champs supplémentaires peuvent être passés lorsque `ExecuteNow` a la valeur true, `QueryStartTime` et `QueryEndTime` . Ces deux champs remplacent le `TIMESPAN` champ dans la requête. Ces champs ne s’appliquent pas aux rapports planifiés, car les données sont générées en continu pendant une période fixe qui ne change pas.

### <a name="request-syntax"></a>Syntaxe de la requête

|    Méthode     |    URI de demande     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>En-tête de requête

|    En-tête     |    Type     |    Description     |
|-------|-----|------|
|    Autorisation     |    string |Obligatoire. Jeton d’accès Azure Active Directory (Azure AD). Le format est  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Paramètre Path

Aucune

### <a name="query-parameter"></a>Paramètre de requête

Aucune

### <a name="sample-request-payload"></a>Exemple de charge utile de demande

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Glossaire

Les définitions de clé des éléments dans la charge utile de la demande sont articulées ci-dessous :

|    Paramètre     |    Obligatoire     |    Description     |    Valeurs autorisées     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Oui     |    Nom à assigner au rapport     |    string     |
|    Description     |    Non     |    Description du rapport créé     |    string     |
|    QueryId     |    Oui     |    ID de equête de rapport     |    string     |
|    StartTime     |    Oui     |    Horodatage UTC à partir duquel la génération du rapport commence. <br> Le format doit être : aaaaa-MM-jjTHH:mm:ssZ       |    string     |
|    ExecuteNow     |    Non     |    Ce paramètre doit être utilisé pour créer un rapport à exécution unique. `StartTime`, `RecurrenceInterval` et `RecurrenceCount` sont ignorés si cette propriété a la valeur true. Le rapport est exécuté immédiatement de manière asynchrone     |    true/false     |
|    QueryStartTime     |    Non     |    (Facultatif) Spécifie l’heure de début de la requête qui extrait les données. Ce paramètre s’applique uniquement à un rapport d’exécution unique dont la propriété a la valeur `ExecuteNow` true. La définition de ce paramètre se substitue `TIMESPAN` à la valeur fournie dans la requête. Le format doit être aaaa-MM-jjTHH:mm:ssZ     |    Timestamp sous forme de chaîne     |
|    QueryEndTime     |    Non     |    (Facultatif) Spécifie l’heure de fin de la requête qui extrait les données. Ce paramètre s’applique uniquement à un rapport d’exécution unique dont la propriété a la valeur `ExecuteNow` true. La définition de ce paramètre se substitue `TIMESPAN` à la valeur fournie dans la requête. Le format doit être aaaa-MM-jjTHH:mm:ssZ     |    Timestamp sous forme de chaîne     |
|    RecurrenceInterval     |    Oui     |    Fréquence en heures à laquelle le rapport doit être généré. <br> La valeur minimale est 4 et la valeur maximale est 2160.      |    entier     |
|    RecurrenceCount     |    Non     |    Nombre de rapports à générer.     |    entier     |
|    Format     |    Non     |    Format du fichier exporté. <br> La valeur par défaut est CSV.    |    « CSV »/« TSV »     |
|    CallbackUrl     |    Non     |    URL publiquement accessible qui peut éventuellement être configurée en tant que destination de rappel     |    Chaîne (URL http)     |
|    CallbackMethod     |    Non     |    Méthode à utiliser pour le rappel     |    RECEVOIR/POSTER     |
|        |        |        |        |

### <a name="sample-response"></a>Exemple de réponse

La charge utile de la réponse est structurée comme suit :

Codes de réponse : 200, 400, 401, 403, 404, 500

Exemple de charge utile de réponse :

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Glossaire

Les définitions de clé des éléments de la réponse sont articulées ci-dessous :

|    Paramètre     |    Description     |
|    ----    |    ----    |
|    ReportId     |    Identificateur unique universel (UUID) du rapport créé     |
|    ReportName     |    Nom donné au rapport dans la charge utile de la requête     |
|    Description     |    Description donnée lors de la création du rapport     |
|    QueryId     |    ID de requête transmis au moment où vous avez créé le rapport     |
|    Requête     |    Texte de requête qui sera exécuté pour ce rapport     |
|    Utilisateur     |    ID d’utilisateur utilisé pour créer le rapport     |
|    CreatedTime     |    Heure UTC de création du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ     |
|    ModifiedTime     |    Heure UTC de dernière modification du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` indicateur défini au moment de la création du rapport     |
|    StartTime     |    Heure UTC de début d’exécution du rapport au format suivant : aaaa-MM-jjTHH:mm:ssZ     |
|    ReportStatus     |    État d’exécution du rapport. Les valeurs possibles sont `Paused` , `Active` et `Inactive`     |
|    RecurrenceInterval     |    Intervalle de périodicité fourni lors de la création du rapport     |
|    RecurrenceCount     |    Nombre de récurrences fourni lors de la création du rapport      |
|    CallbackUrl     |    URL de rappel fournie dans la requête     |
|    CallbackMethod     |    Méthode de rappel fournie dans la demande     |
|    Format     |    Format des fichiers de rapport Les valeurs possibles sont `CSV` ou `TSV` .     |
|    TotalCount     |    Nombre d’enregistrements dans le tableau de valeurs     |
|    StatusCode     |    Code de résultat     |
|    message     |    Les valeurs possibles sont 200, 400, 401, 403, 500. Message d’état d’’exécution de l’API     |
|        |        |

## <a name="get-report-execution-api"></a>Obtient l’API d’exécution de rapport

Vous pouvez utiliser cette méthode pour interroger l’état d’une exécution de rapport à l’aide du ReportId reçu à partir de l' [API de création de rapport](#create-report-api). La méthode renvoie le lien de téléchargement du rapport si le rapport est prêt à être téléchargé. Sinon, la méthode renvoie l’état. Vous pouvez également utiliser cette API pour obtenir toutes les exécutions intervenues pour un rapport donné.  

>[!IMPORTANT]
>Les paramètres de requête par défaut de cette API sont définis pour `executionStatus=Completed` et `getLatestExecution=true` . Par conséquent, l’appel de l’API avant la première exécution réussie du rapport renvoie 404. Les exécutions en attente peuvent être obtenues en définissant `executionStatus=Pending`.

### <a name="request-syntax"></a>Syntaxe de la requête

|    Méthode     |    URI de demande     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>En-tête de requête

|    En-tête     |    Type     |    Description     |
|-------|-----|------|
|    Autorisation     |    string |Obligatoire. Jeton d’accès Azure Active Directory (Azure AD). Le format est  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Paramètre de chemin

|    Nom du paramètre    |    Obligatoire    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Oui    |    string    |    Filtre pour récupérer les détails de l’exécution des rapports uniquement avec le reportId donné dans cet argument. Plusieurs reportIds peuvent être spécifiés en les séparant par un point-virgule « ; ».    |
|        |        |        |        |

### <a name="query-parameter"></a>Paramètre de requête.

|    Nom du paramètre    |    Obligatoire    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    Non    |    string    |    Filtre pour extraire uniquement les détails des rapports avec le executionId donné dans cet argument. Plusieurs executionIds peuvent être spécifiés en les séparant par un point-virgule « ; ».    |
|    executionStatus    |    Non    |    Chaîne/enum    |    Filtre pour extraire uniquement les détails des rapports avec le executionStatus donné dans cet argument. <br> Les valeurs valides sont les suivantes : `Pending` , `Running` `Paused` et `Completed` . <br> La valeur par défaut est `Completed`. <br> Plusieurs États peuvent être spécifiés en les séparant par un point-virgule « ; ».    |
|    getLatestExecution    |    Non    |    boolean    |    L’API retourne les détails de l’exécution la plus récente. Par défaut, ce paramètre a la valeur true.<br> Si vous choisissez de passer la valeur de ce paramètre comme false, l’API retourne les dernières instances d’exécution de 90 jours.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Exemple de charge utile de demande

Aucune

### <a name="sample-response"></a>Exemple de réponse

La charge utile de la réponse est structurée comme suit :

Codes de réponse : 200, 400, 401, 403, 404, 500

Exemple de charge utile de réponse :

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Une fois l’exécution du rapport terminée, l’état d’exécution `Completed` est affiché. Vous pouvez télécharger le rapport en sélectionnant l’URL dans le `reportAccessSecureLink`.

### <a name="glossary"></a>Glossaire

Définitions clés des éléments dans la réponse.

|    Paramètre    |    Description    |
|    ----    |    ----    |
|    ExecutionId    |    Identificateur unique universel (UUID) de l’instance d’exécution    |
|    ReportId    |    ID de rapport associé à l’instance d’exécution    |
|    RecurrenceInterval    |    Intervalle de périodicité fourni lors de la création du rapport    |
|    RecurrenceCount    |    Nombre de récurrences fourni lors de la création du rapport    |
|    CallbackUrl    |    URL de rappel associée à l’instance d’exécution    |
|    CallbackMethod    |    Méthode de rappel associée à l’instance d’exécution    |
|    Format    |    Format du fichier généré à la fin de l’exécution    |
|    ExecutionStatus    |    État de l’instance d’exécution du rapport. <br> Les valeurs valides sont `Pending`, `Running`, `Paused` et `Completed`.    |
|    ReportAccessSecureLink    |Lien permettant d’accéder en toute sécurité au rapport        |
|    ReportExpiryTime    |    Heure UTC après laquelle le lien du rapport expire au format suivant : aaaa-MM-jjTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Heure UTC à laquelle le rapport a été généré au format suivant : aaaa-MM-jjTHH:mm:ssZ    |
|    TotalCount    |    Nombre de jeux de données dans le tableau de valeurs    |
|    StatusCode    |    Code de résultat <br> Les valeurs possibles sont 200, 400, 401, 403, 404 et 500.    |
|    message    |    Message d’état d’’exécution de l’API    |
|        |        |

## <a name="next-steps"></a>Étapes suivantes

- Tester les API par le biais de l’URL de l' [API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Effectuer votre premier appel d’API](insights-programmatic-first-api-call.md)