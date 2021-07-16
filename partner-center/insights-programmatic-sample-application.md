---
title: Exemple d'application
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez l’exemple d’application pour créer votre propre application afin d’accéder par programme aux données des Insights de partenaire.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375061"
---
# <a name="sample-application"></a>Exemple d'application

Des exemples d’applications sont créés en langage C# et JAVA et sont disponibles sur [GitHub](https://github.com/partneranalytics)

- [Exemple d’application C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Exemple d’application JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Vous pouvez choisir de vous inspirer de l’exemple d’application et créer votre propre application dans n’importe quel langage.

L’exemple d’application atteint les objectifs suivants :

- génère un jeton Azure Active Directory (Azure AD).
- Obtention des jeux de données disponibles
- Crée des requêtes définies par l’utilisateur.
- Obtient les requêtes système et définies par l’utilisateur.
- Planification d’un rapport

L’exemple d’application ne couvre pas la méthode d’appel d’API pour d’autres fonctionnalités. Toutefois, le processus d’appel d’autres API reste le même que celui décrit ci-dessus.

## <a name="how-to-run-the-application"></a>Exécution de l’application

- Clonez le dépôt sur un système local à l’aide de la commande suivante :

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> pour plus d’instructions, reportez-vous au fichier ProgrammaticExportSampleAppMPN/README. md dans le [référentiel](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.

- Pour exécuter rapidement l’application, mettez à jour l’ID client et la clé secrète client dans le **appsettings.Development.jssur**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustration du développement de appSetting":::

L’exécution de l’application démarre un serveur web local et ouvre une page (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustration de l’interface utilisateur de l’exemple d’application":::

Cette page effectue des appels d’API au serveur web s’exécutant sur l’ordinateur local, qui à son tour effectue les appels d’API d’accès par programmation réels.

## <a name="code-snippets"></a>Extraits de code

La structure de base du code C# pour exécuter les appels d’API d’accès par programmation est la suivante :
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustration d’un extrait de code":::

## <a name="next-steps"></a>Étapes suivantes

[API permettant d’accéder aux données analytiques de Partner Insights](insights-programmatic-analytics-available-api.md)
