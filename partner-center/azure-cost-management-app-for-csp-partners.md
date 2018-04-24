---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espacepartenaires
description: Azure Cost Management par Cloudyn requiert un accès fourni à l'API de l'Espace partenaires.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.openlocfilehash: 01553b850d5839d721de5406c3f1c63094f76bd6
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2018
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="f3d57-103">Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="f3d57-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="f3d57-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="f3d57-104">Applies to</span></span>**

-  <span data-ttu-id="f3d57-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f3d57-105">Partner Center</span></span>

[<span data-ttu-id="f3d57-106">Obtenez davantage d'informations sur Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="f3d57-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="f3d57-107">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="f3d57-107">Before you begin</span></span>
<span data-ttu-id="f3d57-108">Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies:</span><span class="sxs-lookup"><span data-stu-id="f3d57-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>
- <span data-ttu-id="f3d57-109">Vous êtes un partenaire du programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="f3d57-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="f3d57-110">Vous avez la possibilité de créer une application Web de l'API du Tableau de bord du partenaire.</span><span class="sxs-lookup"><span data-stu-id="f3d57-110">You have the ability to create a Partner Dashboard API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="f3d57-111">Vue d'ensemble</span><span class="sxs-lookup"><span data-stu-id="f3d57-111">Overview</span></span>

<span data-ttu-id="f3d57-112">Azure Cost Management by Cloudyn est une application Web qui vous permet de suivre et de gérer le degré d'utilisation d'Azure par vos clients et les coûts de cette utilisation.</span><span class="sxs-lookup"><span data-stu-id="f3d57-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="f3d57-113">Vous l'utilisez via l'API du Tableau de bord du partenaire.</span><span class="sxs-lookup"><span data-stu-id="f3d57-113">You use it through the Partner Dashboard API.</span></span>

## <a name="register-your-web-app-in-the-partner-dashboard"></a><span data-ttu-id="f3d57-114">Enregistrez votre application Web dans le Tableau de bord du partenaire</span><span class="sxs-lookup"><span data-stu-id="f3d57-114">Register your web app in the Partner Dashboard</span></span>
<span data-ttu-id="f3d57-115">Lorsque vous enregistrez une application Web Azure ActiveDirectory dans le Tableau de bord du partenaire, vous permettez l'accès à l'API du Tableau de bord du partenaire.</span><span class="sxs-lookup"><span data-stu-id="f3d57-115">When you register an Azure Active Directory web app in Partner Dashboard you enable access to the the Partner Dashboard API.</span></span> 
1.  <span data-ttu-id="f3d57-116">Connectez-vous au [Tableau de bord du partenaire](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="f3d57-116">Sign into [the Partner Dashboard](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="f3d57-117">Dans le **Tableau de bord**, sélectionnez **Paramètres du compte** &gt; **[Gestion des utilisateurs](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="f3d57-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="f3d57-118">Dans la section **Web App**, cliquez sur **Ajouter une application Web**.</span><span class="sxs-lookup"><span data-stu-id="f3d57-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="f3d57-119">**Remarque**: si vous avez déjà créé une application Web, vous pouvez ignorer l'étape3.</span><span class="sxs-lookup"><span data-stu-id="f3d57-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="f3d57-120">Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web.</span><span class="sxs-lookup"><span data-stu-id="f3d57-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="f3d57-121">Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30jours de l'application Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="f3d57-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="f3d57-122">Ajoutez une clé secrète à votre application</span><span class="sxs-lookup"><span data-stu-id="f3d57-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="f3d57-123">Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2ans.</span><span class="sxs-lookup"><span data-stu-id="f3d57-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="f3d57-124">Cliquez sur **Ajouter une clé**.</span><span class="sxs-lookup"><span data-stu-id="f3d57-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="f3d57-125">Copiez et enregistrez la valeur de la clé secrète.</span><span class="sxs-lookup"><span data-stu-id="f3d57-125">Copy and save the secret key value.</span></span> <span data-ttu-id="f3d57-126">Elle vous sera demandée pour la version d'évaluation gratuite de 30jours.</span><span class="sxs-lookup"><span data-stu-id="f3d57-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="f3d57-127">**Remarque**: les clés secrètes d'application sont semblables à des mots de passe avec des dates d'expiration plus longues.</span><span class="sxs-lookup"><span data-stu-id="f3d57-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="f3d57-128">Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f3d57-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f3d57-129">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="f3d57-129">Next steps</span></span>
<span data-ttu-id="f3d57-130">Démarrez une [version d'évaluation gratuite de 30jours](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="f3d57-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="f3d57-131">Les informations suivantes sont nécessaires pour démarrer la version d'évaluation:</span><span class="sxs-lookup"><span data-stu-id="f3d57-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="f3d57-132">Identifiants de connexion au Tableau de bord du partenaire</span><span class="sxs-lookup"><span data-stu-id="f3d57-132">Partner Dashboard sign in credentials</span></span>
- <span data-ttu-id="f3d57-133">GUID ID de commerce</span><span class="sxs-lookup"><span data-stu-id="f3d57-133">Commerce ID GUID</span></span>
- <span data-ttu-id="f3d57-134">GUID ID d'application</span><span class="sxs-lookup"><span data-stu-id="f3d57-134">App ID GUID</span></span>
- <span data-ttu-id="f3d57-135">Valeur de la clé secrète de l'application</span><span class="sxs-lookup"><span data-stu-id="f3d57-135">Application secret key value</span></span>
