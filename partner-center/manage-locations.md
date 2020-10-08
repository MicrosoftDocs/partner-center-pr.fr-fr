---
title: Gérer les sites dans votre compte partenaire
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663893"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="da14f-103">Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation</span><span class="sxs-lookup"><span data-stu-id="da14f-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="da14f-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="da14f-104">**Applies to**</span></span>

- <span data-ttu-id="da14f-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="da14f-105">Partner Center</span></span>

<span data-ttu-id="da14f-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="da14f-106">**Appropriate roles**</span></span>

- <span data-ttu-id="da14f-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="da14f-107">Global admin</span></span>
- <span data-ttu-id="da14f-108">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="da14f-108">Account admin</span></span>

<span data-ttu-id="da14f-109">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="da14f-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="da14f-110">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="da14f-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="da14f-111">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="da14f-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="da14f-112">Voici un scénario courant :</span><span class="sxs-lookup"><span data-stu-id="da14f-112">The following is a typical scenario:</span></span>

<span data-ttu-id="da14f-113">Contoso a comme localisation de son compte global de partenaire (PGA) le Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="da14f-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="da14f-114">Il s’agit de leur activité légalement enregistrée et elle a un ID MPN utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="da14f-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="da14f-115">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="da14f-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="da14f-116">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="da14f-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="da14f-117">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="da14f-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="da14f-118">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="da14f-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="da14f-119">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="da14f-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="da14f-121">Prérequis pour pouvoir ajouter une nouvelle localisation pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="da14f-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="da14f-122">Pour ajouter une nouvelle localisation d’activité CSP, il y a plusieurs prérequis :</span><span class="sxs-lookup"><span data-stu-id="da14f-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="da14f-123">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité.</span><span class="sxs-lookup"><span data-stu-id="da14f-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="da14f-124">Vous avez besoin d’un nouveau locataire Azure AD dans la région de l’activité, qui ne soit pas déjà inscrit dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="da14f-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="da14f-125">Créez cela quand vous vous inscrivez dans le programme CSP.</span><span class="sxs-lookup"><span data-stu-id="da14f-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="da14f-126">Utilisez le nouveau locataire AAD pour vous inscrire au programme CSP dans la région.</span><span class="sxs-lookup"><span data-stu-id="da14f-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="da14f-127">Spécifiez les informations détaillées officielles de votre entreprise, comme le nom de la société, l’adresse et les coordonnées du contact principal.</span><span class="sxs-lookup"><span data-stu-id="da14f-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="da14f-128">Ce compte sera soumis à une vérification : veillez donc à ajouter des informations valides.</span><span class="sxs-lookup"><span data-stu-id="da14f-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="da14f-129">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da14f-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="da14f-130">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="da14f-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="da14f-131">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="da14f-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="da14f-132">Ajouter une localisation</span><span class="sxs-lookup"><span data-stu-id="da14f-132">Add a location</span></span>

1. <span data-ttu-id="da14f-133">À partir de l’**icône de paramètres**, sélectionnez **Partner settings** (Paramètres partenaire).</span><span class="sxs-lookup"><span data-stu-id="da14f-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="da14f-134">Sélectionnez **Locations** (Sites).</span><span class="sxs-lookup"><span data-stu-id="da14f-134">Select **Locations.**</span></span>

3. <span data-ttu-id="da14f-135">Sélectionnez **Add a location** (Ajouter un site).</span><span class="sxs-lookup"><span data-stu-id="da14f-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="da14f-136">Dans la page **Add a location** (Ajouter un site), insérez les coordonnées du site que vous souhaitez ajouter à votre entreprise ainsi que son contact principal.</span><span class="sxs-lookup"><span data-stu-id="da14f-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="da14f-137">Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé.</span><span class="sxs-lookup"><span data-stu-id="da14f-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="da14f-138">Changer la localisation du compte de partenaire global</span><span class="sxs-lookup"><span data-stu-id="da14f-138">Change Global partner account location</span></span>

1. <span data-ttu-id="da14f-139">Dans la page **Locations** (Sites), vérifiez que le site que vous voulez désigner comme entité légale figure bien dans la liste des sites.</span><span class="sxs-lookup"><span data-stu-id="da14f-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="da14f-140">Si ce n’est pas le cas, ajoutez-le.</span><span class="sxs-lookup"><span data-stu-id="da14f-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Structure des localisations MPN":::

2. <span data-ttu-id="da14f-142">Sélectionnez **Partner profile** (Profil partenaire), puis **Update legal business profile** (Mettre à jour le profil d’entreprise légale).</span><span class="sxs-lookup"><span data-stu-id="da14f-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Structure des localisations MPN":::

3. <span data-ttu-id="da14f-144">Sélectionnez la région et l’entité légale et choisissez **Submit** (Soumettre).</span><span class="sxs-lookup"><span data-stu-id="da14f-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Structure des localisations MPN":::

## <a name="next-steps"></a><span data-ttu-id="da14f-146">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="da14f-146">Next steps</span></span>

- <span data-ttu-id="da14f-147">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="da14f-147">Learn about the [verification process](verification-responses.md).</span></span>
