---
title: Gérer les sites dans votre compte partenaire
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773426"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="567a6-103">Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation</span><span class="sxs-lookup"><span data-stu-id="567a6-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="567a6-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="567a6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="567a6-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="567a6-105">Global admin</span></span>
- <span data-ttu-id="567a6-106">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="567a6-106">Account admin</span></span>

<span data-ttu-id="567a6-107">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="567a6-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="567a6-108">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="567a6-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="567a6-109">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="567a6-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="567a6-110">Voici un scénario courant :</span><span class="sxs-lookup"><span data-stu-id="567a6-110">The following is a typical scenario:</span></span>

<span data-ttu-id="567a6-111">Contoso a son compte global de partenaire (PGA) au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="567a6-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="567a6-112">Il s’agit de leur activité légalement enregistrée et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="567a6-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="567a6-113">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="567a6-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="567a6-114">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="567a6-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="567a6-115">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="567a6-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="567a6-116">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="567a6-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="567a6-117">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="567a6-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="567a6-119">Prérequis pour l’ajout d’une nouvelle localisation de compte pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="567a6-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="567a6-120">Pour ajouter une nouvelle localisation d’activité CSP, il y a plusieurs prérequis :</span><span class="sxs-lookup"><span data-stu-id="567a6-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="567a6-121">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité.</span><span class="sxs-lookup"><span data-stu-id="567a6-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="567a6-122">Vous avez besoin d’un nouveau locataire Azure AD dans la [région de l’activité](regional-authorization-overview.md), qui ne soit pas déjà inscrit dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="567a6-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="567a6-123">Créez cela quand vous vous inscrivez dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="567a6-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="567a6-124">Utilisez le nouveau locataire AAD pour vous inscrire au programme CSP dans la région.</span><span class="sxs-lookup"><span data-stu-id="567a6-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="567a6-125">Spécifiez les informations détaillées officielles de votre entreprise, comme le nom de la société, l’adresse et les coordonnées du contact principal.</span><span class="sxs-lookup"><span data-stu-id="567a6-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="567a6-126">Ce compte sera soumis à une vérification : veillez donc à ajouter des informations valides.</span><span class="sxs-lookup"><span data-stu-id="567a6-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="567a6-127">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="567a6-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="567a6-128">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="567a6-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="567a6-129">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="567a6-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="567a6-130">Ajouter un site MPN</span><span class="sxs-lookup"><span data-stu-id="567a6-130">Add an MPN location</span></span>

1. <span data-ttu-id="567a6-131">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="567a6-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="567a6-132">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="567a6-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="567a6-133">À partir de l’**icône de paramètres**, sélectionnez **Organization settings** (Paramètres de l’organisation).</span><span class="sxs-lookup"><span data-stu-id="567a6-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="567a6-134">Sélectionnez **Legal**, puis **Locations** (Sites).</span><span class="sxs-lookup"><span data-stu-id="567a6-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="567a6-135">Sélectionnez **Add a location** (Ajouter un site) et insérez les coordonnées du site que vous souhaitez ajouter à votre entreprise ainsi que son contact principal.</span><span class="sxs-lookup"><span data-stu-id="567a6-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="567a6-136">Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé.</span><span class="sxs-lookup"><span data-stu-id="567a6-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="567a6-137">Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="567a6-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="567a6-138">Changer la localisation du compte de partenaire global</span><span class="sxs-lookup"><span data-stu-id="567a6-138">Change Global partner account location</span></span>

1. <span data-ttu-id="567a6-139">Dans **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** (Sites commerciaux), vérifiez que le site que vous voulez désigner comme entité légale figure bien dans la liste.</span><span class="sxs-lookup"><span data-stu-id="567a6-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="567a6-140">Si ce n’est pas le cas, ajoutez-le.</span><span class="sxs-lookup"><span data-stu-id="567a6-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Capture d’écran de la page Emplacements des comptes de l’Espace partenaires, avec la liste de tous les emplacements actuels.":::

2. <span data-ttu-id="567a6-142">Sélectionnez **Legal**, puis **Update legal business profile** (Mettre à jour le profil d’entreprise légale).</span><span class="sxs-lookup"><span data-stu-id="567a6-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="567a6-143">Sélectionnez la région et l’entité légale et choisissez **Submit** (Soumettre).</span><span class="sxs-lookup"><span data-stu-id="567a6-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="567a6-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="567a6-144">Next steps</span></span>

- <span data-ttu-id="567a6-145">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="567a6-145">Learn about the [verification process](verification-responses.md).</span></span>
