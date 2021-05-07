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
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702890"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="a488f-103">Gérer les localisations dans votre compte MPN et ajouter (supprimer) une localisation</span><span class="sxs-lookup"><span data-stu-id="a488f-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="a488f-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="a488f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a488f-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="a488f-105">Global admin</span></span>
- <span data-ttu-id="a488f-106">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="a488f-106">Account admin</span></span>

<span data-ttu-id="a488f-107">L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="a488f-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="a488f-108">Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales.</span><span class="sxs-lookup"><span data-stu-id="a488f-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="a488f-109">L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.</span><span class="sxs-lookup"><span data-stu-id="a488f-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="a488f-110">Le scénario suivant est très courant :</span><span class="sxs-lookup"><span data-stu-id="a488f-110">The following scenario is typical:</span></span>

<span data-ttu-id="a488f-111">Contoso a son compte global de partenaire (PGA) au Royaume-Uni.</span><span class="sxs-lookup"><span data-stu-id="a488f-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="a488f-112">Il s’agit de leur activité légalement enregistrée et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions.</span><span class="sxs-lookup"><span data-stu-id="a488f-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="a488f-113">Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis.</span><span class="sxs-lookup"><span data-stu-id="a488f-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="a488f-114">Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques.</span><span class="sxs-lookup"><span data-stu-id="a488f-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="a488f-115">Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives.</span><span class="sxs-lookup"><span data-stu-id="a488f-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="a488f-116">Les règlements sont associés à des sites spécifiques.</span><span class="sxs-lookup"><span data-stu-id="a488f-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="a488f-117">Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.</span><span class="sxs-lookup"><span data-stu-id="a488f-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="a488f-119">Prérequis pour l’ajout d’un nouveau compte pour une activité CSP</span><span class="sxs-lookup"><span data-stu-id="a488f-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="a488f-120">Pour ajouter un nouveau compte commercial CSP, commencez par veiller à remplir les prérequis.</span><span class="sxs-lookup"><span data-stu-id="a488f-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="a488f-121">Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité CSP.</span><span class="sxs-lookup"><span data-stu-id="a488f-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="a488f-122">Pour créer une localisation MPN, consultez « Ajouter une localisation MPN » ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a488f-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="a488f-123">Pour créer un nouvel abonnement CSP Indirect Reseller, lisez [Travailler avec des fournisseurs indirects](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="a488f-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="a488f-124">N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** compte CSP.</span><span class="sxs-lookup"><span data-stu-id="a488f-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="a488f-125">N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.</span><span class="sxs-lookup"><span data-stu-id="a488f-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="a488f-126">Acceptez le Contrat Partenaire Microsoft et activez le compte.</span><span class="sxs-lookup"><span data-stu-id="a488f-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="a488f-127">Si vous souhaitez vous inscrire en tant que Direct Bill Partner, lisez les [Conditions requises qui s’y rattachent](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="a488f-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="a488f-128">Afficher et mettre à jour vos localisations MPN</span><span class="sxs-lookup"><span data-stu-id="a488f-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="a488f-129">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/home) de l’Espace partenaires avec vos informations d’identification de compte MPN.</span><span class="sxs-lookup"><span data-stu-id="a488f-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="a488f-130">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="a488f-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="a488f-131">À partir de l’icône **Paramètres**, sélectionnez **Paramètres du compte**, **Profil de l’organisation**, puis **Légal**.</span><span class="sxs-lookup"><span data-stu-id="a488f-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="a488f-132">Sous l’onglet **Partenaire**, vérifiez qu’aucune bannière de message d’erreur ne vous invite à corriger les localisations migrées à partir de PMC.</span><span class="sxs-lookup"><span data-stu-id="a488f-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="a488f-133">Si vos localisations n’ont pas été correctement définies dans PMC et n’ont pas encore transité vers un PC, vous devez les mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="a488f-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Capture d’écran montrant comment mettre à jour une localisation.":::
 
4.  <span data-ttu-id="a488f-135">Dans l’écran **Vérifier les localisations PMC**, sélectionnez **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="a488f-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="a488f-136">Mettez à jour les champs suivants :</span><span class="sxs-lookup"><span data-stu-id="a488f-136">Update the following fields:</span></span>

- <span data-ttu-id="a488f-137">**Champ du nom** : Assurez-vous que le nom de la localisation de la société est correcte.</span><span class="sxs-lookup"><span data-stu-id="a488f-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="a488f-138">Si une erreur de doublon s’affiche, essayez de remplacer Contoso par Contoso SARL, par exemple.</span><span class="sxs-lookup"><span data-stu-id="a488f-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="a488f-139">**Champ de l’entité juridique** : Assurez-vous d’avoir choisi l’entité juridique à laquelle la localisation est liée.</span><span class="sxs-lookup"><span data-stu-id="a488f-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="a488f-140">**Champs des lignes d’adresse 1 et 2** : Vérifiez que l’adresse est correcte.</span><span class="sxs-lookup"><span data-stu-id="a488f-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="a488f-141">**Champs des ville et département/province** : Assurez-vous que la combinaison entre la ville et le département/la province est correcte.</span><span class="sxs-lookup"><span data-stu-id="a488f-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="a488f-142">Certains pays ont un menu déroulant pour choisir le département/la province, alors que d’autres ont un champ qui doit être renseigné manuellement.</span><span class="sxs-lookup"><span data-stu-id="a488f-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="a488f-143">**Champ du code postal** : Assurez-vous que le champ du code postal correspond au pays, à la région, à la ville ou à l’adresse indiqué(e).</span><span class="sxs-lookup"><span data-stu-id="a488f-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="a488f-144">**Champs des informations du contact principal** : Assurez-vous que les champs du nom et du prénom sont remplis et que l’adresse e-mail indiquée est une adresse e-mail professionnelle et non personnelle (par exemple, @outlook.com @live.com, etc.)</span><span class="sxs-lookup"><span data-stu-id="a488f-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="a488f-145">**Champ du numéro de téléphone** : Assurez-vous que le numéro de téléphone n’inclut PAS de caractères spéciaux, d’espaces ou d’indicatif.</span><span class="sxs-lookup"><span data-stu-id="a488f-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="a488f-146">La valeur entrée dans le champ du numéro de téléphone contient toujours un maximum de 10 caractères.</span><span class="sxs-lookup"><span data-stu-id="a488f-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="a488f-147">Si aucun message d’erreur ne s’affiche, dans **Paramètres**, sélectionnez **Paramètres de compte**, **Profil de l’organisation** et **Identificateurs**.</span><span class="sxs-lookup"><span data-stu-id="a488f-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="a488f-148">Recherchez l’ID MPN avec le type « localisation » correspondant au pays de ce compte CSP et utilisez-le pour procéder à l’association.</span><span class="sxs-lookup"><span data-stu-id="a488f-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="a488f-149">Si vous ne trouvez pas l’ID MPN de localisation correspondant au compte CSP que vous souhaitez utiliser, vous pouvez ajouter une nouvelle localisation qui créera un nouvel ID MPN.</span><span class="sxs-lookup"><span data-stu-id="a488f-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="a488f-150">Consultez **Ajouter une localisation MPN** ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a488f-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="a488f-151">Ajouter une localisation MPN</span><span class="sxs-lookup"><span data-stu-id="a488f-151">Add an MPN location</span></span>

1. <span data-ttu-id="a488f-152">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a488f-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a488f-153">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="a488f-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a488f-154">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="a488f-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="a488f-155">À partir de l’**icône Paramètres**, sélectionnez **Paramètres du compte**, puis **Profil de l’organisation**.</span><span class="sxs-lookup"><span data-stu-id="a488f-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="a488f-156">Sélectionnez **Légal**, puis sous l’onglet **Partenaire**, sélectionnez **Localisations d’entreprise** et cliquez sur **Ajouter une localisation**.</span><span class="sxs-lookup"><span data-stu-id="a488f-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="a488f-157">Fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact pour la localisation que vous souhaitez ajouter à votre société.</span><span class="sxs-lookup"><span data-stu-id="a488f-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="a488f-158">Cliquez sur **Ajouter une localisation**.</span><span class="sxs-lookup"><span data-stu-id="a488f-158">Click **Add location**.</span></span> <span data-ttu-id="a488f-159">Un nouvel ID MPN est créé pour la nouvelle localisation que vous pouvez utiliser pour les transactions et incentives CSP.</span><span class="sxs-lookup"><span data-stu-id="a488f-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Ajouter une nouvelle activité légale":::

> [!NOTE]
> <span data-ttu-id="a488f-161">Une fois que vous ajoutez une localisation dans l’Espace partenaires, vous ne pouvez plus la supprimer.</span><span class="sxs-lookup"><span data-stu-id="a488f-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="a488f-162">Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="a488f-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="a488f-163">Ajouter le numéro d’identification d’inscription</span><span class="sxs-lookup"><span data-stu-id="a488f-163">Add the registration number ID</span></span>

<span data-ttu-id="a488f-164">Si vous êtes fournisseur indirect, partenaire à facturation directe ou revendeur indirect et que vous travaillez avec des clients nouveaux ou existants dans les pays suivants, vous devez fournir les numéros d’identification d’inscription de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="a488f-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="a488f-165">Si le pays avec lequel vous travaillez ne figure pas dans la liste ci-dessous, le numéro d’inscription est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a488f-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="a488f-166">Arménie</span><span class="sxs-lookup"><span data-stu-id="a488f-166">Armenia</span></span> 
- <span data-ttu-id="a488f-167">Azerbaïdjan</span><span class="sxs-lookup"><span data-stu-id="a488f-167">Azerbaijan</span></span> 
- <span data-ttu-id="a488f-168">Bélarus</span><span class="sxs-lookup"><span data-stu-id="a488f-168">Belarus</span></span> 
- <span data-ttu-id="a488f-169">Brésil</span><span class="sxs-lookup"><span data-stu-id="a488f-169">Brazil</span></span> 
- <span data-ttu-id="a488f-170">Hongrie</span><span class="sxs-lookup"><span data-stu-id="a488f-170">Hungary</span></span> 
- <span data-ttu-id="a488f-171">Inde</span><span class="sxs-lookup"><span data-stu-id="a488f-171">India</span></span> 
- <span data-ttu-id="a488f-172">Irak</span><span class="sxs-lookup"><span data-stu-id="a488f-172">Iraq</span></span> 
- <span data-ttu-id="a488f-173">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="a488f-173">Kazakhstan</span></span> 
- <span data-ttu-id="a488f-174">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="a488f-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="a488f-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="a488f-175">Moldova</span></span> 
- <span data-ttu-id="a488f-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="a488f-176">Myanmar</span></span> 
- <span data-ttu-id="a488f-177">Pologne</span><span class="sxs-lookup"><span data-stu-id="a488f-177">Poland</span></span> 
- <span data-ttu-id="a488f-178">Russie</span><span class="sxs-lookup"><span data-stu-id="a488f-178">Russia</span></span> 
- <span data-ttu-id="a488f-179">Arabie Saoudite</span><span class="sxs-lookup"><span data-stu-id="a488f-179">Saudi Arabia</span></span> 
- <span data-ttu-id="a488f-180">Afrique du Sud</span><span class="sxs-lookup"><span data-stu-id="a488f-180">South Africa</span></span> 
- <span data-ttu-id="a488f-181">Soudan du Sud</span><span class="sxs-lookup"><span data-stu-id="a488f-181">South Sudan</span></span>  
- <span data-ttu-id="a488f-182">Tadjikistan</span><span class="sxs-lookup"><span data-stu-id="a488f-182">Tajikistan</span></span> 
- <span data-ttu-id="a488f-183">Thaïlande</span><span class="sxs-lookup"><span data-stu-id="a488f-183">Thailand</span></span>
- <span data-ttu-id="a488f-184">Turquie</span><span class="sxs-lookup"><span data-stu-id="a488f-184">Turkey</span></span> 
- <span data-ttu-id="a488f-185">Ukraine</span><span class="sxs-lookup"><span data-stu-id="a488f-185">Ukraine</span></span> 
- <span data-ttu-id="a488f-186">Émirats arabes unis</span><span class="sxs-lookup"><span data-stu-id="a488f-186">United Arab Emirates</span></span> 
- <span data-ttu-id="a488f-187">Ouzbékistan</span><span class="sxs-lookup"><span data-stu-id="a488f-187">Uzbekistan</span></span> 
- <span data-ttu-id="a488f-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="a488f-188">Venezuela</span></span>
- <span data-ttu-id="a488f-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="a488f-189">Vietnam</span></span> 


<span data-ttu-id="a488f-190">Pour plus d’informations, consultez [Informations sur les numéros d’identification d’inscription](reg-number-id.md).</span><span class="sxs-lookup"><span data-stu-id="a488f-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="a488f-191">Supprimer une localisation</span><span class="sxs-lookup"><span data-stu-id="a488f-191">Delete a location</span></span>

<span data-ttu-id="a488f-192">Pour supprimer une localisation de votre compte, vous devez contacter [le support de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="a488f-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="a488f-193">Veillez à bien comprendre l’impact de cette action.</span><span class="sxs-lookup"><span data-stu-id="a488f-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="a488f-194">Les localisations supprimées ne peuvent pas être récupérées et tout ce qui est lié à cet ID MPN spécifique n’est plus reconnu ni actif pour votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="a488f-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="a488f-195">Changer le pays du compte global du partenaire</span><span class="sxs-lookup"><span data-stu-id="a488f-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="a488f-196">Connectez-vous avec le compte MPN dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a488f-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a488f-197">(Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.)</span><span class="sxs-lookup"><span data-stu-id="a488f-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a488f-198">Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte.</span><span class="sxs-lookup"><span data-stu-id="a488f-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="a488f-199">Sous l’onglet **Partenaire**, accédez à **Localisations d’entreprise** et vérifiez que la localisation que vous voulez désigner comme entité légale figure bien dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a488f-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="a488f-200">Pour ajouter une localisation, cliquez sur **Ajouter une localisation**, puis dans le menu volant, fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact principal pour la localisation que vous souhaitez ajouter à votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="a488f-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="a488f-201">Sélectionnez **Changer votre pays** à côté de la liste déroulante **Pays/région** et suivez les étapes.</span><span class="sxs-lookup"><span data-stu-id="a488f-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Menu volant des données de profil de l’entreprise légale":::

5. <span data-ttu-id="a488f-203">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="a488f-203">Click **Save**.</span></span>

6. <span data-ttu-id="a488f-204">Le pays du compte global MPN sera remplacé par le nouveau pays légal.</span><span class="sxs-lookup"><span data-stu-id="a488f-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="a488f-205">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a488f-205">Next steps</span></span>

- <span data-ttu-id="a488f-206">Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="a488f-206">Learn about the [verification process](verification-responses.md).</span></span>
