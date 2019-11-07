---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Cost Management par Cloudyn requiert un accès fourni à l'API de l'Espace partenaires.
author: Janet
ms.author: janet
Keywords: Application Azure Cost Management, gérer les coûts, applications Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: a746522d3470a8b97b845ed723fae87455e33e5e
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653869"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="542e1-104">Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="542e1-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="542e1-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="542e1-105">**Applies to**</span></span>

-  <span data-ttu-id="542e1-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="542e1-106">Partner Center</span></span>

[<span data-ttu-id="542e1-107">Obtenir plus d’informations sur Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="542e1-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="542e1-108">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="542e1-108">Before you begin</span></span>
<span data-ttu-id="542e1-109">Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies :</span><span class="sxs-lookup"><span data-stu-id="542e1-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="542e1-110">Vous êtes un partenaire du programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="542e1-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="542e1-111">Vous avez la possibilité de créer une application Web de l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="542e1-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="542e1-112">Vue d'ensemble</span><span class="sxs-lookup"><span data-stu-id="542e1-112">Overview</span></span>

<span data-ttu-id="542e1-113">Cloudyn est une application Web qui vous permet de suivre et de gérer l’utilisation d’Azure par vos clients, ainsi que les coûts de cette utilisation.</span><span class="sxs-lookup"><span data-stu-id="542e1-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="542e1-114">Vous l'utilisez via l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="542e1-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="542e1-115">Enregistrez votre application Web dans l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="542e1-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="542e1-116">Lorsque vous enregistrez une application Web Azure Active Directory dans l'Espace partenaires, vous permettez l'accès à l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="542e1-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="542e1-117">Connectez-vous à l'[Espace partenaires](https://partnercenter.microsoft.com/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="542e1-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="542e1-118">Dans l' **espace partenaires**, sélectionnez **paramètres de compte** &gt; **[gestion des applications](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="542e1-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="542e1-119">Dans la section **Web App**, cliquez sur **Ajouter une application Web**.</span><span class="sxs-lookup"><span data-stu-id="542e1-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="542e1-120">**Remarque** : si vous avez déjà créé une application Web, vous pouvez ignorer l'étape 3.</span><span class="sxs-lookup"><span data-stu-id="542e1-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="542e1-121">Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web.</span><span class="sxs-lookup"><span data-stu-id="542e1-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="542e1-122">Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30 jours de l'application Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="542e1-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="542e1-123">Ajoutez une clé secrète à votre application</span><span class="sxs-lookup"><span data-stu-id="542e1-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="542e1-124">Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2 ans.</span><span class="sxs-lookup"><span data-stu-id="542e1-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="542e1-125">Cliquez sur **Ajouter une clé**.</span><span class="sxs-lookup"><span data-stu-id="542e1-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="542e1-126">Copiez et enregistrez la valeur de la clé secrète.</span><span class="sxs-lookup"><span data-stu-id="542e1-126">Copy and save the secret key value.</span></span> <span data-ttu-id="542e1-127">Elle vous sera demandée pour la version d'évaluation gratuite de 30 jours.</span><span class="sxs-lookup"><span data-stu-id="542e1-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="542e1-128">Les clés secrètes de l’application sont semblables aux mots de passe avec des dates d’expiration plus longues.</span><span class="sxs-lookup"><span data-stu-id="542e1-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="542e1-129">Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="542e1-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="542e1-130">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="542e1-130">Next steps</span></span>
<span data-ttu-id="542e1-131">Démarrez une [version d'évaluation gratuite de 30 jours](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="542e1-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="542e1-132">Les informations suivantes sont nécessaires pour démarrer la version d'évaluation :</span><span class="sxs-lookup"><span data-stu-id="542e1-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="542e1-133">Identifiants de connexion à l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="542e1-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="542e1-134">GUID ID de commerce</span><span class="sxs-lookup"><span data-stu-id="542e1-134">Commerce ID GUID</span></span>
- <span data-ttu-id="542e1-135">GUID ID d'application</span><span class="sxs-lookup"><span data-stu-id="542e1-135">App ID GUID</span></span>
- <span data-ttu-id="542e1-136">Valeur de la clé secrète de l'application</span><span class="sxs-lookup"><span data-stu-id="542e1-136">Application secret key value</span></span>
