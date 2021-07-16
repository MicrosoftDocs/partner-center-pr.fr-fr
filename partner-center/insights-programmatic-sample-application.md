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
# <a name="sample-application"></a><span data-ttu-id="f593b-103">Exemple d'application</span><span class="sxs-lookup"><span data-stu-id="f593b-103">Sample Application</span></span>

<span data-ttu-id="f593b-104">Des exemples d’applications sont créés en langage C# et JAVA et sont disponibles sur [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="f593b-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="f593b-105">Exemple d’application C#</span><span class="sxs-lookup"><span data-stu-id="f593b-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="f593b-106">Exemple d’application JAVA</span><span class="sxs-lookup"><span data-stu-id="f593b-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="f593b-107">Vous pouvez choisir de vous inspirer de l’exemple d’application et créer votre propre application dans n’importe quel langage.</span><span class="sxs-lookup"><span data-stu-id="f593b-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="f593b-108">L’exemple d’application atteint les objectifs suivants :</span><span class="sxs-lookup"><span data-stu-id="f593b-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="f593b-109">génère un jeton Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f593b-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="f593b-110">Obtention des jeux de données disponibles</span><span class="sxs-lookup"><span data-stu-id="f593b-110">Gets available datasets.</span></span>
- <span data-ttu-id="f593b-111">Crée des requêtes définies par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f593b-111">Creates user defined queries.</span></span>
- <span data-ttu-id="f593b-112">Obtient les requêtes système et définies par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f593b-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="f593b-113">Planification d’un rapport</span><span class="sxs-lookup"><span data-stu-id="f593b-113">Schedules a report.</span></span>

<span data-ttu-id="f593b-114">L’exemple d’application ne couvre pas la méthode d’appel d’API pour d’autres fonctionnalités.</span><span class="sxs-lookup"><span data-stu-id="f593b-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="f593b-115">Toutefois, le processus d’appel d’autres API reste le même que celui décrit ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="f593b-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="f593b-116">Exécution de l’application</span><span class="sxs-lookup"><span data-stu-id="f593b-116">How to run the application</span></span>

- <span data-ttu-id="f593b-117">Clonez le dépôt sur un système local à l’aide de la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="f593b-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="f593b-118">pour plus d’instructions, reportez-vous au fichier ProgrammaticExportSampleAppMPN/README. md dans le [référentiel](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.</span><span class="sxs-lookup"><span data-stu-id="f593b-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="f593b-119">Pour exécuter rapidement l’application, mettez à jour l’ID client et la clé secrète client dans le **appsettings.Development.jssur**</span><span class="sxs-lookup"><span data-stu-id="f593b-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustration du développement de appSetting":::

<span data-ttu-id="f593b-121">L’exécution de l’application démarre un serveur web local et ouvre une page (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span><span class="sxs-lookup"><span data-stu-id="f593b-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustration de l’interface utilisateur de l’exemple d’application":::

<span data-ttu-id="f593b-123">Cette page effectue des appels d’API au serveur web s’exécutant sur l’ordinateur local, qui à son tour effectue les appels d’API d’accès par programmation réels.</span><span class="sxs-lookup"><span data-stu-id="f593b-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="f593b-124">Extraits de code</span><span class="sxs-lookup"><span data-stu-id="f593b-124">Code Snippets</span></span>

<span data-ttu-id="f593b-125">La structure de base du code C# pour exécuter les appels d’API d’accès par programmation est la suivante :</span><span class="sxs-lookup"><span data-stu-id="f593b-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustration d’un extrait de code":::

## <a name="next-steps"></a><span data-ttu-id="f593b-127">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="f593b-127">Next steps</span></span>

[<span data-ttu-id="f593b-128">API permettant d’accéder aux données analytiques de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="f593b-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
