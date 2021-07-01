---
title: Gérer les localisations dans votre compte partenaire
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276822"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="93d03-103">Gérer les localisations dans votre compte MPN et ajouter (supprimer) une localisation</span><span class="sxs-lookup"><span data-stu-id="93d03-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="93d03-104">**Rôles appropriés** : Administrateur général | Administrateur de compte</span><span class="sxs-lookup"><span data-stu-id="93d03-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="93d03-105">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="93d03-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="93d03-106">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="93d03-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="93d03-107">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="93d03-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="93d03-108">Le scénario suivant est très courant :</span><span class="sxs-lookup"><span data-stu-id="93d03-108">The following scenario is typical:</span></span>

<span data-ttu-id="93d03-109">Contoso a son compte global de partenaire (PGA) au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="93d03-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="93d03-110">Il s’agit de leur activité légalement enregistrée, et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="93d03-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="93d03-111">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="93d03-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="93d03-112">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="93d03-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="93d03-113">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="93d03-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="93d03-114">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="93d03-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="93d03-115">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="93d03-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="93d03-117">Prérequis pour l’ajout d’un nouveau compte pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="93d03-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="93d03-118">Pour ajouter un nouveau compte commercial CSP, commencez par veiller à remplir les prérequis.</span><span class="sxs-lookup"><span data-stu-id="93d03-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="93d03-119">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité CSP.</span><span class="sxs-lookup"><span data-stu-id="93d03-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="93d03-120">Pour créer une localisation MPN, consultez « Ajouter une localisation MPN » ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="93d03-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="93d03-121">Pour créer un nouvel abonnement CSP Indirect Reseller, lisez [Travailler avec des fournisseurs indirects](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="93d03-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="93d03-122">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** compte CSP.</span><span class="sxs-lookup"><span data-stu-id="93d03-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="93d03-123">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="93d03-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="93d03-124">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="93d03-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="93d03-125">Si vous souhaitez vous inscrire en tant que Direct Bill Partner, lisez les [Conditions requises qui s’y rattachent](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="93d03-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="93d03-126">Afficher et mettre à jour vos localisations MPN</span><span class="sxs-lookup"><span data-stu-id="93d03-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="93d03-127">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/home) de l’Espace partenaires avec vos informations d’identification de compte MPN.</span><span class="sxs-lookup"><span data-stu-id="93d03-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="93d03-128">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="93d03-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="93d03-129">À partir de l’icône **Paramètres**, sélectionnez **Paramètres du compte**, **Profil de l’organisation**, puis **Légal**.</span><span class="sxs-lookup"><span data-stu-id="93d03-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="93d03-130">Sous l’onglet **Partenaire**, vérifiez qu’aucune bannière de message d’erreur ne vous invite à corriger les localisations migrées à partir de PMC.</span><span class="sxs-lookup"><span data-stu-id="93d03-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="93d03-131">Si vos localisations n’ont pas été correctement définies dans PMC et n’ont pas encore transité vers un PC, vous devez les mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="93d03-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Capture d’écran montrant comment mettre à jour une localisation.":::
 
4.  <span data-ttu-id="93d03-133">Dans l’écran **Vérifier les localisations PMC**, sélectionnez **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="93d03-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="93d03-134">Mettez à jour les champs suivants :</span><span class="sxs-lookup"><span data-stu-id="93d03-134">Update the following fields:</span></span>

- <span data-ttu-id="93d03-135">**Champ du nom** : Assurez-vous que le nom de la localisation de la société est correcte.</span><span class="sxs-lookup"><span data-stu-id="93d03-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="93d03-136">Si une erreur de doublon s’affiche, essayez de remplacer Contoso par Contoso SARL, par exemple.</span><span class="sxs-lookup"><span data-stu-id="93d03-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="93d03-137">**Champ de l’entité juridique** : Assurez-vous d’avoir choisi l’entité juridique à laquelle la localisation est liée.</span><span class="sxs-lookup"><span data-stu-id="93d03-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="93d03-138">**Champs des lignes d’adresse 1 et 2** : Vérifiez que l’adresse est correcte.</span><span class="sxs-lookup"><span data-stu-id="93d03-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="93d03-139">**Champs des ville et département/province** : Assurez-vous que la combinaison entre la ville et le département/la province est correcte.</span><span class="sxs-lookup"><span data-stu-id="93d03-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="93d03-140">Certains pays ont un menu déroulant pour choisir le département/la province, alors que d’autres ont un champ qui doit être renseigné manuellement.</span><span class="sxs-lookup"><span data-stu-id="93d03-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="93d03-141">**Champ du code postal** : Assurez-vous que le champ du code postal correspond au pays, à la région, à la ville ou à l’adresse indiqué(e).</span><span class="sxs-lookup"><span data-stu-id="93d03-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="93d03-142">**Champs des informations du contact principal** : Assurez-vous que les champs du nom et du prénom sont remplis et que l’adresse e-mail indiquée est une adresse e-mail professionnelle et non personnelle (par exemple, @outlook.com @live.com, etc.)</span><span class="sxs-lookup"><span data-stu-id="93d03-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="93d03-143">**Champ du numéro de téléphone** : Assurez-vous que le numéro de téléphone n’inclut PAS de caractères spéciaux, d’espaces ou d’indicatif.</span><span class="sxs-lookup"><span data-stu-id="93d03-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="93d03-144">La valeur entrée dans le champ du numéro de téléphone contient toujours un maximum de 10 caractères.</span><span class="sxs-lookup"><span data-stu-id="93d03-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="93d03-145">Si aucun message d’erreur ne s’affiche, dans **Paramètres**, sélectionnez **Paramètres de compte**, **Profil de l’organisation** et **Identificateurs**.</span><span class="sxs-lookup"><span data-stu-id="93d03-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="93d03-146">Recherchez l’ID MPN avec le type « localisation » correspondant au pays de ce compte CSP et utilisez-le pour procéder à l’association.</span><span class="sxs-lookup"><span data-stu-id="93d03-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="93d03-147">Si vous ne trouvez pas l’ID MPN de localisation correspondant au compte CSP que vous souhaitez utiliser, vous pouvez ajouter une nouvelle localisation qui créera un nouvel ID MPN.</span><span class="sxs-lookup"><span data-stu-id="93d03-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="93d03-148">Consultez **Ajouter une localisation MPN** ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="93d03-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="93d03-149">Ajouter une localisation MPN</span><span class="sxs-lookup"><span data-stu-id="93d03-149">Add an MPN location</span></span>

1. <span data-ttu-id="93d03-150">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="93d03-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="93d03-151">(Vos informations d’identification MPN peuvent être différentes de celles de votre fournisseur de services de chiffrement) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="93d03-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="93d03-152">À partir de l’**icône Paramètres**, sélectionnez **Paramètres du compte**, puis **Profil de l’organisation**.</span><span class="sxs-lookup"><span data-stu-id="93d03-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="93d03-153">Sélectionnez **Légal**. Sous l’onglet **Partenaire**, sélectionnez **Localisations d’entreprise** puis sélectionnez **Ajouter une localisation**.</span><span class="sxs-lookup"><span data-stu-id="93d03-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="93d03-154">Fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact pour la localisation que vous souhaitez ajouter à votre société.</span><span class="sxs-lookup"><span data-stu-id="93d03-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="93d03-155">Sélectionnez **Ajouter un emplacement**.</span><span class="sxs-lookup"><span data-stu-id="93d03-155">Select **Add location**.</span></span> <span data-ttu-id="93d03-156">Un nouvel ID MPN est créé pour la nouvelle localisation que vous pouvez utiliser pour les transactions et incentives CSP.</span><span class="sxs-lookup"><span data-stu-id="93d03-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Ajouter une nouvelle activité légale.":::

> [!NOTE]
> <span data-ttu-id="93d03-158">Une fois que vous ajoutez une localisation dans l’Espace partenaires, vous ne pouvez plus la supprimer.</span><span class="sxs-lookup"><span data-stu-id="93d03-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="93d03-159">Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="93d03-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="93d03-160">Ajouter le numéro d’identification d’inscription</span><span class="sxs-lookup"><span data-stu-id="93d03-160">Add the registration number ID</span></span>

<span data-ttu-id="93d03-161">Si vous êtes fournisseur indirect, partenaire à facturation directe ou revendeur indirect et que vous travaillez avec des clients nouveaux ou existants dans les pays suivants, vous devez fournir les numéros d’identification d’inscription de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="93d03-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="93d03-162">Si le pays avec lequel vous travaillez ne figure pas dans la liste ci-dessous, l’ID d’inscription est facultatif.</span><span class="sxs-lookup"><span data-stu-id="93d03-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="93d03-163">Arménie</span><span class="sxs-lookup"><span data-stu-id="93d03-163">Armenia</span></span> 
- <span data-ttu-id="93d03-164">Azerbaïdjan</span><span class="sxs-lookup"><span data-stu-id="93d03-164">Azerbaijan</span></span> 
- <span data-ttu-id="93d03-165">Bélarus</span><span class="sxs-lookup"><span data-stu-id="93d03-165">Belarus</span></span> 
- <span data-ttu-id="93d03-166">Brésil</span><span class="sxs-lookup"><span data-stu-id="93d03-166">Brazil</span></span> 
- <span data-ttu-id="93d03-167">Hongrie</span><span class="sxs-lookup"><span data-stu-id="93d03-167">Hungary</span></span> 
- <span data-ttu-id="93d03-168">Inde</span><span class="sxs-lookup"><span data-stu-id="93d03-168">India</span></span> 
- <span data-ttu-id="93d03-169">Irak</span><span class="sxs-lookup"><span data-stu-id="93d03-169">Iraq</span></span> 
- <span data-ttu-id="93d03-170">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="93d03-170">Kazakhstan</span></span> 
- <span data-ttu-id="93d03-171">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="93d03-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="93d03-172">Moldova</span><span class="sxs-lookup"><span data-stu-id="93d03-172">Moldova</span></span> 
- <span data-ttu-id="93d03-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="93d03-173">Myanmar</span></span> 
- <span data-ttu-id="93d03-174">Pologne</span><span class="sxs-lookup"><span data-stu-id="93d03-174">Poland</span></span> 
- <span data-ttu-id="93d03-175">Russie</span><span class="sxs-lookup"><span data-stu-id="93d03-175">Russia</span></span> 
- <span data-ttu-id="93d03-176">Arabie Saoudite</span><span class="sxs-lookup"><span data-stu-id="93d03-176">Saudi Arabia</span></span> 
- <span data-ttu-id="93d03-177">Afrique du Sud</span><span class="sxs-lookup"><span data-stu-id="93d03-177">South Africa</span></span> 
- <span data-ttu-id="93d03-178">Soudan du Sud</span><span class="sxs-lookup"><span data-stu-id="93d03-178">South Sudan</span></span>  
- <span data-ttu-id="93d03-179">Tadjikistan</span><span class="sxs-lookup"><span data-stu-id="93d03-179">Tajikistan</span></span> 
- <span data-ttu-id="93d03-180">Thaïlande</span><span class="sxs-lookup"><span data-stu-id="93d03-180">Thailand</span></span>
- <span data-ttu-id="93d03-181">Turquie</span><span class="sxs-lookup"><span data-stu-id="93d03-181">Turkey</span></span> 
- <span data-ttu-id="93d03-182">Ukraine</span><span class="sxs-lookup"><span data-stu-id="93d03-182">Ukraine</span></span> 
- <span data-ttu-id="93d03-183">Émirats arabes unis</span><span class="sxs-lookup"><span data-stu-id="93d03-183">United Arab Emirates</span></span> 
- <span data-ttu-id="93d03-184">Ouzbékistan</span><span class="sxs-lookup"><span data-stu-id="93d03-184">Uzbekistan</span></span> 
- <span data-ttu-id="93d03-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="93d03-185">Venezuela</span></span>
- <span data-ttu-id="93d03-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="93d03-186">Vietnam</span></span> 


<span data-ttu-id="93d03-187">Pour plus d’informations, consultez [Informations sur les numéros d’identification d’inscription](reg-number-id.md).</span><span class="sxs-lookup"><span data-stu-id="93d03-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="93d03-188">Supprimer une localisation</span><span class="sxs-lookup"><span data-stu-id="93d03-188">Delete a location</span></span>

<span data-ttu-id="93d03-189">Pour supprimer une localisation de votre compte, vous devez contacter [le support de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="93d03-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="93d03-190">Veillez à bien comprendre l’impact de cette action.</span><span class="sxs-lookup"><span data-stu-id="93d03-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="93d03-191">Les localisations supprimées ne peuvent pas être récupérées, et tout ce qui est lié à cet ID MPN n’est plus reconnu ni actif pour votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="93d03-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="93d03-192">Changer le pays du compte global du partenaire</span><span class="sxs-lookup"><span data-stu-id="93d03-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="93d03-193">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="93d03-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="93d03-194">(Vos informations d’identification MPN peuvent être différentes de celles de votre fournisseur de services de chiffrement) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="93d03-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="93d03-195">Sous l’onglet **Partenaire**, accédez à **Localisations d’entreprise** et vérifiez que la localisation que vous voulez désigner comme entité légale figure bien dans la liste.</span><span class="sxs-lookup"><span data-stu-id="93d03-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="93d03-196">Pour ajouter une localisation, cliquez sur **Ajouter une localisation**, puis dans le menu volant, fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact principal pour la localisation que vous souhaitez ajouter à votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="93d03-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="93d03-197">Sélectionnez **Changer votre pays** à côté de la liste déroulante **Pays/région** et suivez les étapes.</span><span class="sxs-lookup"><span data-stu-id="93d03-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Menu volant des données de profil de l’entreprise légale.":::

5. <span data-ttu-id="93d03-199">Sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="93d03-199">Select **Save**.</span></span>

6. <span data-ttu-id="93d03-200">Le pays du compte global MPN sera remplacé par le nouveau pays légal.</span><span class="sxs-lookup"><span data-stu-id="93d03-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="93d03-201">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="93d03-201">Next steps</span></span>

- <span data-ttu-id="93d03-202">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="93d03-202">Learn about the [verification process](verification-responses.md).</span></span>
