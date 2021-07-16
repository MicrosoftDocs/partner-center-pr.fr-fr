---
title: Conditions préalables à l’accès programmatique aux données d’analyse
description: Conditions préalables à l’accès programmatique aux données d’analyse
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375068"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="8b21b-103">Conditions préalables à l’accès programmatique aux données d’analyse</span><span class="sxs-lookup"><span data-stu-id="8b21b-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="8b21b-104">**Rôles appropriés :** Administrateur général | Administrateur MPN</span><span class="sxs-lookup"><span data-stu-id="8b21b-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="8b21b-105">Avant de pouvoir accéder par programme aux données analytiques de Partner Insights, vous devez remplir les conditions suivantes.</span><span class="sxs-lookup"><span data-stu-id="8b21b-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="8b21b-106">Inscription au programme MPN</span><span class="sxs-lookup"><span data-stu-id="8b21b-106">MPN Program enrollment</span></span>

<span data-ttu-id="8b21b-107">Pour accéder par programme à des données analytiques d’analyse partenaire, vous devez être inscrit au programme MPN et disposer d’un compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8b21b-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="8b21b-108">Pour en savoir plus, consultez [créer un compte MPN dans l’espace partenaires](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="8b21b-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="8b21b-109">créer une application Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="8b21b-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="8b21b-110">les informations d’identification de l’utilisateur standard ne peuvent pas être utilisées pour l’accès par programme aux données du partenaire Informations Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b21b-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="8b21b-111">une application Azure Active Directory (AAD) doit être créée avec un secret (application + accès utilisateur) pour accéder aux api d’accès par programme.</span><span class="sxs-lookup"><span data-stu-id="8b21b-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="8b21b-112">pour savoir comment créer une application AAD et une clé secrète, consultez [démarrage rapide : inscrire une application avec le Plateforme d’identités Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Une autorisation est requise pour accéder à l’API partenaire Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b21b-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="8b21b-113">Pour savoir comment ajouter une autorisation, consultez [Partner API Authentication-Partner](/partner/develop/api-authentication#application-and-user-access) .</span><span class="sxs-lookup"><span data-stu-id="8b21b-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="8b21b-114">Attribuer le rôle ERV (Executive Report Viewer) à l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="8b21b-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="8b21b-115">Pour accéder par programme à des données analytiques d’analyse partenaire, vous devez disposer d’une visionneuse de rapports (ERV).</span><span class="sxs-lookup"><span data-stu-id="8b21b-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="8b21b-116">pour savoir comment attribuer le rôle ERV à l’utilisateur, consultez [espace partenaires Informations accès en fonction du rôle-espace partenaires](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="8b21b-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="8b21b-117">Générer un jeton AAD</span><span class="sxs-lookup"><span data-stu-id="8b21b-117">Generate an AAD token</span></span>

<span data-ttu-id="8b21b-118">Vous devez générer un jeton AAD à l’aide de l’ID d’application (client), de la clé secrète client, de votre ID d’utilisateur et de votre mot de passe. Pour savoir comment générer un jeton AAD, cliquez   [ici](insights-programmatic-first-api-call.md#token-generation) .</span><span class="sxs-lookup"><span data-stu-id="8b21b-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="8b21b-119">Ce jeton est valide une heure.</span><span class="sxs-lookup"><span data-stu-id="8b21b-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8b21b-120">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8b21b-120">Next steps</span></span>
[<span data-ttu-id="8b21b-121">Paradigme de l’accès programmatique</span><span class="sxs-lookup"><span data-stu-id="8b21b-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)