---
title: Affecter des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 10/10/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les rôles les mieux adaptés à vos utilisateurs qui gèrent des transactions commerciales, des référencements, des incentives ou les adhésions MPN de votre entreprise.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: high
ms.openlocfilehash: e0f53e2f1aae51a1287a2e347fa9014b5d75ea03
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004128"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="5fee5-104">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5fee5-104">Assign users roles and permissions</span></span>

<span data-ttu-id="5fee5-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="5fee5-105">**Appropriate roles**</span></span>
-   <span data-ttu-id="5fee5-106">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="5fee5-106">Global admin</span></span>
-   <span data-ttu-id="5fee5-107">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5fee5-107">User admin</span></span>
-   <span data-ttu-id="5fee5-108">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-108">MPN partner admin</span></span>

<span data-ttu-id="5fee5-109">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="5fee5-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="5fee5-110">Prochaine étape : demander à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="5fee5-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="5fee5-111">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="5fee5-112">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="5fee5-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="5fee5-113">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="5fee5-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="5fee5-114">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="5fee5-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="5fee5-115">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="5fee5-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="5fee5-116">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="5fee5-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="5fee5-117">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="5fee5-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="5fee5-118">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="5fee5-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="5fee5-119">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5fee5-119">**Role**</span></span>|<span data-ttu-id="5fee5-120">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5fee5-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="5fee5-121">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="5fee5-121">Global admin</span></span>|<span data-ttu-id="5fee5-122">• Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="5fee5-122">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="5fee5-123">• Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-123">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5fee5-124">• Afficher les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="5fee5-124">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="5fee5-125">• Afficher, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-125">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="5fee5-126">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="5fee5-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="5fee5-127">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5fee5-127">User management admin</span></span>   | <span data-ttu-id="5fee5-128">• Afficher, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5fee5-128">•    View, create, and manage users</span></span>
||<span data-ttu-id="5fee5-129">• Afficher tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="5fee5-129">• View all partner profiles</span></span>
||<span data-ttu-id="5fee5-130">• Afficher, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-130">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="5fee5-131">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="5fee5-131">Billing admin</span></span> | <span data-ttu-id="5fee5-132">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="5fee5-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="5fee5-133">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="5fee5-133">Default user</span></span>|  <span data-ttu-id="5fee5-134">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="5fee5-134">View My profile</span></span>   |
|<span data-ttu-id="5fee5-135">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="5fee5-135">Admin agent</span></span> | <span data-ttu-id="5fee5-136">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="5fee5-136">•    Customer management</span></span>
||<span data-ttu-id="5fee5-137">• Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-137">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="5fee5-138">• Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="5fee5-138">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="5fee5-139">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="5fee5-139">• Subscription management</span></span>
||<span data-ttu-id="5fee5-140">• État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="5fee5-140">• Service health and service requests for customers</span></span>
||<span data-ttu-id="5fee5-141">• Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="5fee5-141">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="5fee5-142">• Afficher les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="5fee5-142">• View pricing and offers</span></span>
||<span data-ttu-id="5fee5-143">• Facturation</span><span class="sxs-lookup"><span data-stu-id="5fee5-143">• Billing</span></span>
||<span data-ttu-id="5fee5-144">• Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="5fee5-144">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="5fee5-145">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="5fee5-145">• Register a value added reseller</span></span>|
|<span data-ttu-id="5fee5-146">Commercial</span><span class="sxs-lookup"><span data-stu-id="5fee5-146">Sales agent</span></span> | <span data-ttu-id="5fee5-147">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="5fee5-147">•    Customer management</span></span>
||<span data-ttu-id="5fee5-148">• Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-148">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="5fee5-149">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="5fee5-149">• Subscription management</span></span>
||<span data-ttu-id="5fee5-150">• Afficher les tickets de support</span><span class="sxs-lookup"><span data-stu-id="5fee5-150">• View support tickets</span></span>
||<span data-ttu-id="5fee5-151">• Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="5fee5-151">• Request a relationship with a customer</span></span>
||<span data-ttu-id="5fee5-152">• Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="5fee5-152">• Manage customer leads</span></span>
||<span data-ttu-id="5fee5-153">• Afficher le contrat client</span><span class="sxs-lookup"><span data-stu-id="5fee5-153">• View the customer agreement</span></span>
||<span data-ttu-id="5fee5-154">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="5fee5-154">• Register a value-added reseller</span></span>|
|<span data-ttu-id="5fee5-155">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="5fee5-155">Helpdesk agent</span></span>| <span data-ttu-id="5fee5-156">• Rechercher et afficher un client</span><span class="sxs-lookup"><span data-stu-id="5fee5-156">•  Search for and view a customer</span></span>
||<span data-ttu-id="5fee5-157">• Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="5fee5-157">• Edit customer details</span></span>
||<span data-ttu-id="5fee5-158">• Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="5fee5-158">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="5fee5-159">• Demander un support pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="5fee5-159">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="5fee5-160">• Gérer les problèmes d’abonnements et de facturation pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="5fee5-160">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="5fee5-161">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="5fee5-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="5fee5-162">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="5fee5-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="5fee5-163">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5fee5-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="5fee5-164">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5fee5-164">**Role**</span></span>   |<span data-ttu-id="5fee5-165">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5fee5-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="5fee5-166">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="5fee5-166">Global admin</span></span>| <span data-ttu-id="5fee5-167">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="5fee5-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="5fee5-168">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="5fee5-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="5fee5-169">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="5fee5-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="5fee5-170">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="5fee5-170">**Guest user**</span></span>   | <span data-ttu-id="5fee5-171">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="5fee5-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="5fee5-172">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-172">MPN partner admin</span></span>|
||<span data-ttu-id="5fee5-173">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="5fee5-173">Accounts admin</span></span>|
||<span data-ttu-id="5fee5-174">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-174">Incentives admin</span></span>|
||<span data-ttu-id="5fee5-175">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="5fee5-175">Business profile admin</span></span>|
||<span data-ttu-id="5fee5-176">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="5fee5-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="5fee5-177">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="5fee5-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="5fee5-178">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5fee5-178">**Role**</span></span> | <span data-ttu-id="5fee5-179">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5fee5-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="5fee5-180">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-180">MPN partner admin</span></span>|<span data-ttu-id="5fee5-181">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-181">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="5fee5-182">• Afficher les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-182">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="5fee5-183">• Afficher les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="5fee5-183">• View user details and their skills data</span></span>
||<span data-ttu-id="5fee5-184">• Afficher les compétences</span><span class="sxs-lookup"><span data-stu-id="5fee5-184">• View competencies</span></span>
||<span data-ttu-id="5fee5-185">• Afficher et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="5fee5-185">• View and manage benefits</span></span>
||<span data-ttu-id="5fee5-186">• Afficher et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-186">• View and purchase MPN offers</span></span>
||<span data-ttu-id="5fee5-187">• Afficher les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="5fee5-187">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="5fee5-188">• Afficher les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-188">• View partner contribution indicator data</span></span>
||<span data-ttu-id="5fee5-189">• Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="5fee5-189">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="5fee5-190">• Afficher l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="5fee5-190">- View customer data analytics</span></span>
|| <span data-ttu-id="5fee5-191">• Afficher d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="5fee5-191">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="5fee5-192">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="5fee5-192">Account admin</span></span>| <span data-ttu-id="5fee5-193">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="5fee5-193">Add locations</span></span>
|| <span data-ttu-id="5fee5-194">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="5fee5-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="5fee5-195">• Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="5fee5-195">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="5fee5-196">• Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="5fee5-196">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="5fee5-197">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="5fee5-197">Manage referrals</span></span> 

|<span data-ttu-id="5fee5-198">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5fee5-198">**Role**</span></span>|<span data-ttu-id="5fee5-199">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5fee5-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="5fee5-200">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="5fee5-200">Referrals admin</span></span>       |<span data-ttu-id="5fee5-201">• Afficher, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="5fee5-201">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="5fee5-202">• Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="5fee5-202">• Receive and manage referrals</span></span>
||<span data-ttu-id="5fee5-203">• Afficher, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="5fee5-203">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="5fee5-204">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-204">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="5fee5-205">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="5fee5-205">Business profile admin</span></span>   |<span data-ttu-id="5fee5-206">• Afficher, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="5fee5-206">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="5fee5-207">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5fee5-207">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="5fee5-208">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-208">Manage incentives</span></span> 

|<span data-ttu-id="5fee5-209">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5fee5-209">**Role**</span></span> | <span data-ttu-id="5fee5-210">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5fee5-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="5fee5-211">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-211">Incentives admin</span></span>|<span data-ttu-id="5fee5-212">• Lancer et gérer des primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-212">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="5fee5-213">• Afficher et modifier tous les aspects des programmes de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-213">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="5fee5-214">• Afficher et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="5fee5-214">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="5fee5-215">• Afficher les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="5fee5-215">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="5fee5-216">• Accéder au support</span><span class="sxs-lookup"><span data-stu-id="5fee5-216">• Access support</span></span>
||<span data-ttu-id="5fee5-217">• Contester des paiements de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-217">• Dispute incentives payments</span></span>|
|<span data-ttu-id="5fee5-218">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-218">Incentives user</span></span>|<span data-ttu-id="5fee5-219">• Afficher les programmes de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-219">•  Can view incentives programs</span></span>
||<span data-ttu-id="5fee5-220">• Afficher et lancer des revendications de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5fee5-220">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="5fee5-221">• Afficher les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="5fee5-221">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="5fee5-222">• Accéder au support</span><span class="sxs-lookup"><span data-stu-id="5fee5-222">• Access support</span></span>












