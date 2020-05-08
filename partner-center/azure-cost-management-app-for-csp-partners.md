---
title: Azure Cost Management par Cloudyn pour les fournisseurs de services de chiffrement
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment inscrire l’application Web Cloudyn et utiliser une clé secrète pour celle-ci dans l’espace partenaires afin de pouvoir utiliser l’application pour suivre l’utilisation et les coûts d’Azure du client.
author: LauraBrenner
ms.author: labrenne
Keywords: Application Azure Cost Management, gérer les coûts, applications Web
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d88f37e0fe653c679df5729fa283336e4c7e144
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908373"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="1e6a8-104">Suivre l’utilisation et les coûts d’Azure des clients avec l’application Azure Cost Management pour les partenaires CSP</span><span class="sxs-lookup"><span data-stu-id="1e6a8-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="1e6a8-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="1e6a8-105">**Applies to**</span></span>

- <span data-ttu-id="1e6a8-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e6a8-106">Partner Center</span></span>
- <span data-ttu-id="1e6a8-107">Partenaires du programme Fournisseur de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="1e6a8-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="1e6a8-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="1e6a8-108">**Appropriate roles**</span></span>

- <span data-ttu-id="1e6a8-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="1e6a8-109">Global admin</span></span>
- <span data-ttu-id="1e6a8-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="1e6a8-110">Admin agent</span></span>

[<span data-ttu-id="1e6a8-111">Obtenir plus d’informations sur Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="1e6a8-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="1e6a8-112">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="1e6a8-112">Before you begin</span></span>
<span data-ttu-id="1e6a8-113">Avant de pouvoir utiliser Azure Cost Management, assurez-vous que vous remplissez les conditions suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e6a8-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="1e6a8-114">Vous êtes un partenaire dans le programme du fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="1e6a8-115">Vous avez la possibilité de créer une application Web d’API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="1e6a8-116">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="1e6a8-116">Overview</span></span>

<span data-ttu-id="1e6a8-117">Cloudyn est une application Web qui vous permet de suivre et de gérer l’utilisation d’Azure par vos clients, ainsi que les coûts de cette utilisation.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="1e6a8-118">Vous l’utilisez par le biais de l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="1e6a8-119">Inscrire votre application Web dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e6a8-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="1e6a8-120">Lorsque vous inscrivez une application Web Azure Active Directory dans l’espace partenaires, vous activez l’accès à l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="1e6a8-121">Connectez-vous à [l’espace partenaires](https://partnercenter.microsoft.com/pcv/dashboard/overview) à l’aide d’un [compte d’administrateur général ou d’agent d’administration](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="1e6a8-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="1e6a8-122">Dans l' **espace partenaires**, sélectionnez **paramètres** &gt; du compte **[gestion des applications](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="1e6a8-123">Dans la section **application Web** , cliquez sur **Ajouter une nouvelle application Web**.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="1e6a8-124">**Remarque**: Si vous avez déjà créé une application Web, vous pouvez ignorer l’étape 3.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="1e6a8-125">Copiez et enregistrez le GUID de l' **ID de commerce** et le GUID de l' **ID d’application** pour votre application Web.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="1e6a8-126">Vous aurez besoin des deux ID pour utiliser la version d’évaluation gratuite de 30 jours de l’application Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="1e6a8-127">Ajouter une clé secrète à votre application</span><span class="sxs-lookup"><span data-stu-id="1e6a8-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="1e6a8-128">Dans la liste déroulante en regard du bouton **Ajouter une clé** , sélectionnez une durée de 1 ou 2 ans.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="1e6a8-129">Cliquez sur **Ajouter une clé**.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="1e6a8-130">Copiez et enregistrez la valeur de la clé secrète.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-130">Copy and save the secret key value.</span></span> <span data-ttu-id="1e6a8-131">Vous en aurez besoin pour la version d’évaluation gratuite de 30 jours.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="1e6a8-132">Les clés secrètes de l’application sont semblables aux mots de passe avec des dates d’expiration plus longues.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="1e6a8-133">Enregistrez la valeur de clé dans un emplacement sécurisé pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1e6a8-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1e6a8-134">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1e6a8-134">Next steps</span></span>
<span data-ttu-id="1e6a8-135">Démarrez une [version d’évaluation gratuite de 30 jours](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="1e6a8-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="1e6a8-136">Vous avez besoin des informations suivantes pour commencer la version d’évaluation :</span><span class="sxs-lookup"><span data-stu-id="1e6a8-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="1e6a8-137">Informations d’identification de connexion de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e6a8-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="1e6a8-138">GUID de l’ID de commerce</span><span class="sxs-lookup"><span data-stu-id="1e6a8-138">Commerce ID GUID</span></span>
- <span data-ttu-id="1e6a8-139">GUID de l’ID d’application</span><span class="sxs-lookup"><span data-stu-id="1e6a8-139">App ID GUID</span></span>
- <span data-ttu-id="1e6a8-140">Valeur de clé secrète d’application</span><span class="sxs-lookup"><span data-stu-id="1e6a8-140">Application secret key value</span></span>
