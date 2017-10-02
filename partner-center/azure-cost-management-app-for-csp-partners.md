---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espacepartenaires
description: "Azure Cost Management par Cloudyn requiert un accès fourni à l'API de l'Espace partenaires."
author: Janet
robots: 
ms.openlocfilehash: d9f0b3f0f8bd6d76f05dacba27cf7ee2ddc5071b
ms.sourcegitcommit: d9f3e4e8115c0ad44f97041d352b703cda7ba9e5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/28/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="e8086-103">Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="e8086-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="e8086-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="e8086-104">Applies to</span></span>**

-  <span data-ttu-id="e8086-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e8086-105">Partner Center</span></span>

[<span data-ttu-id="e8086-106">Obtenez davantage d'informations sur Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="e8086-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="e8086-107">Avant de commencer</span><span class="sxs-lookup"><span data-stu-id="e8086-107">Before you begin</span></span>
<span data-ttu-id="e8086-108">Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies:</span><span class="sxs-lookup"><span data-stu-id="e8086-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>
- <span data-ttu-id="e8086-109">Vous êtes un partenaire du programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="e8086-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="e8086-110">Vous avez la possibilité de créer une application Web de l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e8086-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="e8086-111">Vue d'ensemble</span><span class="sxs-lookup"><span data-stu-id="e8086-111">Overview</span></span>

<span data-ttu-id="e8086-112">Azure Cost Management by Cloudyn est une application Web qui vous permet de suivre et de gérer le degré d'utilisation d'Azure par vos clients et les coûts de cette utilisation.</span><span class="sxs-lookup"><span data-stu-id="e8086-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="e8086-113">Vous l'utilisez via l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e8086-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-partner-center"></a><span data-ttu-id="e8086-114">Enregistrez votre application Web dans l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e8086-114">Register your web app in Partner Center</span></span>
<span data-ttu-id="e8086-115">Lorsque vous enregistrez une application Web Azure ActiveDirectory dans l'Espace partenaires, vous permettez l'accès à l'API de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e8086-115">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="e8086-116">Connectez-vous à l'[Espace partenaires](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="e8086-116">Sign into [Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="e8086-117">Dans le **Tableau de bord**, sélectionnez **Paramètres du compte** &gt; **[Gestion des utilisateurs](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="e8086-117">From the **Dashboard**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="e8086-118">Dans la section **Web App**, cliquez sur **Ajouter une application Web**.</span><span class="sxs-lookup"><span data-stu-id="e8086-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="e8086-119">**Remarque**: si vous avez déjà créé une application Web, vous pouvez ignorer l'étape3.</span><span class="sxs-lookup"><span data-stu-id="e8086-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="e8086-120">Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web.</span><span class="sxs-lookup"><span data-stu-id="e8086-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="e8086-121">Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30jours de l'application Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="e8086-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="e8086-122">Ajoutez une clé secrète à votre application</span><span class="sxs-lookup"><span data-stu-id="e8086-122">Add a secret key to your app</span></span>
1.  <span data-ttu-id="e8086-123">Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2ans.</span><span class="sxs-lookup"><span data-stu-id="e8086-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2.  <span data-ttu-id="e8086-124">Cliquez sur **Ajouter une clé**.</span><span class="sxs-lookup"><span data-stu-id="e8086-124">Click **Add key**.</span></span> 
3.  <span data-ttu-id="e8086-125">Copiez et enregistrez la valeur de la clé secrète.</span><span class="sxs-lookup"><span data-stu-id="e8086-125">Copy and save the secret key value.</span></span> <span data-ttu-id="e8086-126">Elle vous sera demandée pour la version d'évaluation gratuite de 30jours.</span><span class="sxs-lookup"><span data-stu-id="e8086-126">You will need this for the 30-day free trial.</span></span>
<br><span data-ttu-id="e8086-127">**Remarque**: les clés secrètes d'application sont semblables à des mots de passe avec des dates d'expiration plus longues.</span><span class="sxs-lookup"><span data-stu-id="e8086-127">**Note**: The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="e8086-128">Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="e8086-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e8086-129">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e8086-129">Next steps</span></span>
<span data-ttu-id="e8086-130">Démarrez une [version d'évaluation gratuite de 30jours](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="e8086-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="e8086-131">Les informations suivantes sont nécessaires pour démarrer la version d'évaluation:</span><span class="sxs-lookup"><span data-stu-id="e8086-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="e8086-132">Identifiants de connexion à l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e8086-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="e8086-133">GUID ID de commerce</span><span class="sxs-lookup"><span data-stu-id="e8086-133">Commerce ID GUID</span></span>
- <span data-ttu-id="e8086-134">GUID ID d'application</span><span class="sxs-lookup"><span data-stu-id="e8086-134">App ID GUID</span></span>
- <span data-ttu-id="e8086-135">Valeur de la clé secrète de l'application</span><span class="sxs-lookup"><span data-stu-id="e8086-135">Application secret key value</span></span>
