---
title: Gérer les sites dans votre compte partenaire
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c6b0fc84636befedbc51aa0672ce19110eb4d9aa
ms.sourcegitcommit: 1719ff11409cd6953602b7798f8cfe821b8ea15e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/15/2020
ms.locfileid: "92100769"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="abaca-103">Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation</span><span class="sxs-lookup"><span data-stu-id="abaca-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="abaca-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="abaca-104">**Applies to**</span></span>

- <span data-ttu-id="abaca-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="abaca-105">Partner Center</span></span>

<span data-ttu-id="abaca-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="abaca-106">**Appropriate roles**</span></span>

- <span data-ttu-id="abaca-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="abaca-107">Global admin</span></span>
- <span data-ttu-id="abaca-108">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="abaca-108">Account admin</span></span>

<span data-ttu-id="abaca-109">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="abaca-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="abaca-110">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="abaca-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="abaca-111">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="abaca-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="abaca-112">Voici un scénario courant :</span><span class="sxs-lookup"><span data-stu-id="abaca-112">The following is a typical scenario:</span></span>

<span data-ttu-id="abaca-113">Contoso a son compte global de partenaire (PGA) au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="abaca-113">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="abaca-114">Il s’agit de leur activité légalement enregistrée et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="abaca-114">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="abaca-115">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="abaca-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="abaca-116">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="abaca-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="abaca-117">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="abaca-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="abaca-118">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="abaca-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="abaca-119">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="abaca-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="abaca-121">Prérequis pour pouvoir ajouter une nouvelle localisation pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="abaca-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="abaca-122">Pour ajouter une nouvelle localisation d’activité CSP, il y a plusieurs prérequis :</span><span class="sxs-lookup"><span data-stu-id="abaca-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="abaca-123">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité.</span><span class="sxs-lookup"><span data-stu-id="abaca-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="abaca-124">Vous avez besoin d’un nouveau locataire Azure AD dans la [région de l’activité](regional-authorization-overview.md), qui ne soit pas déjà inscrit dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="abaca-124">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="abaca-125">Créez cela quand vous vous inscrivez dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="abaca-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="abaca-126">Utilisez le nouveau locataire AAD pour vous inscrire au programme CSP dans la région.</span><span class="sxs-lookup"><span data-stu-id="abaca-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="abaca-127">Spécifiez les informations détaillées officielles de votre entreprise, comme le nom de la société, l’adresse et les coordonnées du contact principal.</span><span class="sxs-lookup"><span data-stu-id="abaca-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="abaca-128">Ce compte sera soumis à une vérification : veillez donc à ajouter des informations valides.</span><span class="sxs-lookup"><span data-stu-id="abaca-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="abaca-129">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="abaca-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="abaca-130">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="abaca-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="abaca-131">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="abaca-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="abaca-132">Ajouter un site MPN</span><span class="sxs-lookup"><span data-stu-id="abaca-132">Add an MPN location</span></span>

1. <span data-ttu-id="abaca-133">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="abaca-133">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="abaca-134">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="abaca-134">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="abaca-135">À partir de l’**icône de paramètres**, sélectionnez **Partner settings** (Paramètres partenaire).</span><span class="sxs-lookup"><span data-stu-id="abaca-135">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="abaca-136">Sélectionnez **Locations** (Sites).</span><span class="sxs-lookup"><span data-stu-id="abaca-136">Select **Locations.**</span></span>

3. <span data-ttu-id="abaca-137">Sélectionnez **Add a location** (Ajouter un site) et insérez les coordonnées du site que vous souhaitez ajouter à votre entreprise ainsi que son contact principal.</span><span class="sxs-lookup"><span data-stu-id="abaca-137">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="abaca-138">Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé.</span><span class="sxs-lookup"><span data-stu-id="abaca-138">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="abaca-139">Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="abaca-139">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="abaca-140">Changer la localisation du compte de partenaire global</span><span class="sxs-lookup"><span data-stu-id="abaca-140">Change Global partner account location</span></span>

1. <span data-ttu-id="abaca-141">Dans la page **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** (Sites), vérifiez que le site que vous voulez désigner comme entité légale figure bien dans la liste des sites.</span><span class="sxs-lookup"><span data-stu-id="abaca-141">On the **[Locations](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="abaca-142">Si ce n’est pas le cas, ajoutez-le.</span><span class="sxs-lookup"><span data-stu-id="abaca-142">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Structure des localisations MPN":::

2. <span data-ttu-id="abaca-144">Sélectionnez **Partner profile** (Profil partenaire), puis **Update legal business profile** (Mettre à jour le profil d’entreprise légale).</span><span class="sxs-lookup"><span data-stu-id="abaca-144">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Structure des localisations MPN":::

3. <span data-ttu-id="abaca-146">Sélectionnez la région et l’entité légale et choisissez **Submit** (Soumettre).</span><span class="sxs-lookup"><span data-stu-id="abaca-146">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Structure des localisations MPN":::

## <a name="next-steps"></a><span data-ttu-id="abaca-148">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="abaca-148">Next steps</span></span>

- <span data-ttu-id="abaca-149">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="abaca-149">Learn about the [verification process](verification-responses.md).</span></span>
