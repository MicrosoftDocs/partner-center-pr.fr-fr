---
title: Gérer les sites dans votre compte partenaire
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925036"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="33608-103">Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation</span><span class="sxs-lookup"><span data-stu-id="33608-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="33608-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="33608-104">**Appropriate roles**</span></span>

- <span data-ttu-id="33608-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="33608-105">Global admin</span></span>
- <span data-ttu-id="33608-106">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="33608-106">Account admin</span></span>

<span data-ttu-id="33608-107">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="33608-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="33608-108">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="33608-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="33608-109">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="33608-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="33608-110">Voici un scénario courant :</span><span class="sxs-lookup"><span data-stu-id="33608-110">The following is a typical scenario:</span></span>

<span data-ttu-id="33608-111">Contoso a son compte global de partenaire (PGA) au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="33608-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="33608-112">Il s’agit de leur activité légalement enregistrée et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="33608-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="33608-113">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="33608-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="33608-114">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="33608-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="33608-115">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="33608-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="33608-116">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="33608-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="33608-117">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="33608-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="33608-119">Prérequis pour l’ajout d’un nouveau compte pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="33608-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="33608-120">Pour ajouter un nouveau compte commercial CSP, commencez par veiller à remplir les prérequis.</span><span class="sxs-lookup"><span data-stu-id="33608-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="33608-121">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité CSP.</span><span class="sxs-lookup"><span data-stu-id="33608-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="33608-122">Pour créer une localisation MPN, consultez « Ajouter une localisation MPN » ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="33608-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="33608-123">Pour créer un nouvel abonnement CSP Indirect Reseller, lisez [Travailler avec des fournisseurs indirects](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="33608-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="33608-124">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** compte CSP.</span><span class="sxs-lookup"><span data-stu-id="33608-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="33608-125">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="33608-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="33608-126">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="33608-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="33608-127">Ajouter un site MPN</span><span class="sxs-lookup"><span data-stu-id="33608-127">Add an MPN location</span></span>

1. <span data-ttu-id="33608-128">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="33608-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="33608-129">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="33608-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="33608-130">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="33608-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="33608-131">À partir de l’**icône Paramètres**, sélectionnez **Paramètres du compte**, puis **Profil de l’organisation**.</span><span class="sxs-lookup"><span data-stu-id="33608-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="33608-132">Sélectionnez **Légal**, puis sous l’onglet **Partenaire**, sélectionnez **Localisations d’entreprise** et cliquez sur **Ajouter une localisation**.</span><span class="sxs-lookup"><span data-stu-id="33608-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="33608-133">Fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact pour la localisation que vous souhaitez ajouter à votre société.</span><span class="sxs-lookup"><span data-stu-id="33608-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="33608-134">Cliquez sur **Ajouter une localisation**.</span><span class="sxs-lookup"><span data-stu-id="33608-134">Click **Add location**.</span></span> <span data-ttu-id="33608-135">Un nouvel ID MPN est créé pour la nouvelle localisation que vous pouvez utiliser pour les transactions et incentives CSP.</span><span class="sxs-lookup"><span data-stu-id="33608-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Ajouter une nouvelle activité légale":::

> [!NOTE]
> <span data-ttu-id="33608-137">Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé.</span><span class="sxs-lookup"><span data-stu-id="33608-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="33608-138">Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="33608-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="33608-139">Changer le pays du compte global du partenaire</span><span class="sxs-lookup"><span data-stu-id="33608-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="33608-140">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="33608-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="33608-141">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="33608-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="33608-142">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="33608-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="33608-143">Sous l’onglet **Partenaire**, accédez à **Localisations d’entreprise** et vérifiez que la localisation que vous voulez désigner comme entité légale figure bien dans la liste.</span><span class="sxs-lookup"><span data-stu-id="33608-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="33608-144">Pour ajouter une localisation, cliquez sur **Ajouter une localisation**, puis dans le menu volant, fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact principal pour la localisation que vous souhaitez ajouter à votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="33608-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="33608-145">Sélectionnez **Changer votre pays** à côté de la liste déroulante **Pays/région** et suivez les étapes.</span><span class="sxs-lookup"><span data-stu-id="33608-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Menu volant des données de profil de l’entreprise légale":::

5. <span data-ttu-id="33608-147">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="33608-147">Click **Save**.</span></span>

6. <span data-ttu-id="33608-148">Le pays du compte global MPN sera remplacé par le nouveau pays légal.</span><span class="sxs-lookup"><span data-stu-id="33608-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="33608-149">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="33608-149">Next steps</span></span>

- <span data-ttu-id="33608-150">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="33608-150">Learn about the [verification process](verification-responses.md).</span></span>
