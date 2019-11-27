---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espace partenaires
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment inscrire l’application Web Cloudyn et utiliser une clé secrète pour celle-ci dans l’espace partenaires afin de pouvoir utiliser l’application pour suivre l’utilisation et les coûts d’Azure du client.
author: Janet
ms.author: janet
Keywords: Application Azure Cost Management, gérer les coûts, applications Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253297"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="a723c-104">Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="a723c-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="a723c-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="a723c-105">**Applies to**</span></span>

- <span data-ttu-id="a723c-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a723c-106">Partner Center</span></span>
- <span data-ttu-id="a723c-107">Partenaires du programme Fournisseur de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="a723c-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="a723c-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="a723c-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a723c-109">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="a723c-109">Global admin</span></span>
- <span data-ttu-id="a723c-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="a723c-110">Admin agent</span></span>

[<span data-ttu-id="a723c-111">Obtenir plus d’informations sur Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="a723c-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="a723c-112">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="a723c-112">Before you begin</span></span>
<span data-ttu-id="a723c-113">Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies :</span><span class="sxs-lookup"><span data-stu-id="a723c-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="a723c-114">Vous êtes un partenaire du programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="a723c-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="a723c-115">Vous avez la possibilité de créer une application Web de l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a723c-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="a723c-116">Présentation</span><span class="sxs-lookup"><span data-stu-id="a723c-116">Overview</span></span>

<span data-ttu-id="a723c-117">Cloudyn est une application Web qui vous permet de suivre et de gérer l’utilisation d’Azure par vos clients, ainsi que les coûts de cette utilisation.</span><span class="sxs-lookup"><span data-stu-id="a723c-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="a723c-118">Vous l'utilisez via l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a723c-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="a723c-119">Enregistrez votre application Web dans l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a723c-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="a723c-120">Lorsque vous enregistrez une application Web Azure Active Directory dans l'Espace partenaires, vous permettez l'accès à l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a723c-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="a723c-121">Connectez-vous à l'[Espace partenaires](https://partnercenter.microsoft.com/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="a723c-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="a723c-122">Dans l' **espace partenaires**, sélectionnez **paramètres de compte** &gt; **[gestion des applications](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="a723c-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="a723c-123">Dans la section **Web App**, cliquez sur **Ajouter une application Web**.</span><span class="sxs-lookup"><span data-stu-id="a723c-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="a723c-124">**Remarque** : si vous avez déjà créé une application Web, vous pouvez ignorer l'étape 3.</span><span class="sxs-lookup"><span data-stu-id="a723c-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="a723c-125">Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web.</span><span class="sxs-lookup"><span data-stu-id="a723c-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="a723c-126">Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30 jours de l'application Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="a723c-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="a723c-127">Ajoutez une clé secrète à votre application</span><span class="sxs-lookup"><span data-stu-id="a723c-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="a723c-128">Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2 ans.</span><span class="sxs-lookup"><span data-stu-id="a723c-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="a723c-129">Cliquez sur **Ajouter une clé**.</span><span class="sxs-lookup"><span data-stu-id="a723c-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="a723c-130">Copiez et enregistrez la valeur de la clé secrète.</span><span class="sxs-lookup"><span data-stu-id="a723c-130">Copy and save the secret key value.</span></span> <span data-ttu-id="a723c-131">Elle vous sera demandée pour la version d'évaluation gratuite de 30 jours.</span><span class="sxs-lookup"><span data-stu-id="a723c-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="a723c-132">Les clés secrètes de l’application sont semblables aux mots de passe avec des dates d’expiration plus longues.</span><span class="sxs-lookup"><span data-stu-id="a723c-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="a723c-133">Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="a723c-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a723c-134">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a723c-134">Next steps</span></span>
<span data-ttu-id="a723c-135">Démarrez une [version d'évaluation gratuite de 30 jours](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="a723c-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="a723c-136">Les informations suivantes sont nécessaires pour démarrer la version d'évaluation :</span><span class="sxs-lookup"><span data-stu-id="a723c-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="a723c-137">Identifiants de connexion à l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a723c-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="a723c-138">GUID ID de commerce</span><span class="sxs-lookup"><span data-stu-id="a723c-138">Commerce ID GUID</span></span>
- <span data-ttu-id="a723c-139">GUID ID d'application</span><span class="sxs-lookup"><span data-stu-id="a723c-139">App ID GUID</span></span>
- <span data-ttu-id="a723c-140">Valeur de la clé secrète de l'application</span><span class="sxs-lookup"><span data-stu-id="a723c-140">Application secret key value</span></span>
