---
title: Affecter des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 10/10/2019
description: Tous les employés qui ont besoin de travailler dans l’Espace partenaires doivent se voir attribuer un rôle.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: high
ms.openlocfilehash: 0bbc9af84b8a1464f255c17147fdc10a7504eb43
ms.sourcegitcommit: 1ccc27092949deb6f6404e64fd6a628fd7b5fd5c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/11/2019
ms.locfileid: "72276090"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="8f68d-104">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8f68d-104">Assign users roles and permissions</span></span>


<span data-ttu-id="8f68d-105">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="8f68d-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8f68d-106">Prochaine étape : demander à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="8f68d-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8f68d-107">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8f68d-108">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="8f68d-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8f68d-109">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="8f68d-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8f68d-110">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="8f68d-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8f68d-111">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="8f68d-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8f68d-112">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="8f68d-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8f68d-113">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="8f68d-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8f68d-114">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="8f68d-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="8f68d-115">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="8f68d-115">**Role**</span></span>|<span data-ttu-id="8f68d-116">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="8f68d-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8f68d-117">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="8f68d-117">Global admin</span></span>|<span data-ttu-id="8f68d-118">• Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="8f68d-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8f68d-119">• Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8f68d-120">• Afficher les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="8f68d-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8f68d-121">• Afficher, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="8f68d-122">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="8f68d-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="8f68d-123">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8f68d-123">User management admin</span></span>   | <span data-ttu-id="8f68d-124">• Afficher, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8f68d-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="8f68d-125">• Afficher tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="8f68d-125">• View all partner profiles</span></span>
||<span data-ttu-id="8f68d-126">• Afficher, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="8f68d-127">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="8f68d-127">Billing admin</span></span> | <span data-ttu-id="8f68d-128">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="8f68d-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="8f68d-129">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="8f68d-129">Default user</span></span>|  <span data-ttu-id="8f68d-130">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="8f68d-130">View My profile</span></span>   |
|<span data-ttu-id="8f68d-131">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="8f68d-131">Admin agent</span></span> | <span data-ttu-id="8f68d-132">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="8f68d-132">•    Customer management</span></span>
||<span data-ttu-id="8f68d-133">• Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8f68d-134">• Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="8f68d-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="8f68d-135">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="8f68d-135">• Subscription management</span></span>
||<span data-ttu-id="8f68d-136">• État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="8f68d-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="8f68d-137">• Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="8f68d-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="8f68d-138">• Afficher les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="8f68d-138">• View pricing and offers</span></span>
||<span data-ttu-id="8f68d-139">• Facturation</span><span class="sxs-lookup"><span data-stu-id="8f68d-139">• Billing</span></span>
||<span data-ttu-id="8f68d-140">• Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="8f68d-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="8f68d-141">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="8f68d-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="8f68d-142">Commercial</span><span class="sxs-lookup"><span data-stu-id="8f68d-142">Sales agent</span></span> | <span data-ttu-id="8f68d-143">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="8f68d-143">•    Customer management</span></span>
||<span data-ttu-id="8f68d-144">• Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8f68d-145">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="8f68d-145">• Subscription management</span></span>
||<span data-ttu-id="8f68d-146">• Afficher les tickets de support</span><span class="sxs-lookup"><span data-stu-id="8f68d-146">• View support tickets</span></span>
||<span data-ttu-id="8f68d-147">• Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="8f68d-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="8f68d-148">• Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="8f68d-148">• Manage customer leads</span></span>
||<span data-ttu-id="8f68d-149">• Afficher le contrat client</span><span class="sxs-lookup"><span data-stu-id="8f68d-149">• View the customer agreement</span></span>
||<span data-ttu-id="8f68d-150">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="8f68d-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="8f68d-151">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="8f68d-151">Helpdesk agent</span></span>| <span data-ttu-id="8f68d-152">• Rechercher et afficher un client</span><span class="sxs-lookup"><span data-stu-id="8f68d-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="8f68d-153">• Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="8f68d-153">• Edit customer details</span></span>
||<span data-ttu-id="8f68d-154">• Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="8f68d-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8f68d-155">• Demander un support pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="8f68d-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="8f68d-156">• Gérer les problèmes d’abonnements et de facturation pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="8f68d-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8f68d-157">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="8f68d-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8f68d-158">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="8f68d-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8f68d-159">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8f68d-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="8f68d-160">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="8f68d-160">**Role**</span></span>   |<span data-ttu-id="8f68d-161">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="8f68d-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="8f68d-162">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="8f68d-162">Global admin</span></span>| <span data-ttu-id="8f68d-163">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="8f68d-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8f68d-164">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="8f68d-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="8f68d-165">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="8f68d-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="8f68d-166">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="8f68d-166">**Guest user**</span></span>   | <span data-ttu-id="8f68d-167">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="8f68d-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="8f68d-168">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="8f68d-168">MPN partner admin</span></span>|
||<span data-ttu-id="8f68d-169">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="8f68d-169">Accounts admin</span></span>|
||<span data-ttu-id="8f68d-170">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-170">Incentives admin</span></span>|
||<span data-ttu-id="8f68d-171">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="8f68d-171">Business profile admin</span></span>|
||<span data-ttu-id="8f68d-172">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="8f68d-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="8f68d-173">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="8f68d-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="8f68d-174">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="8f68d-174">**Role**</span></span> | <span data-ttu-id="8f68d-175">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="8f68d-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="8f68d-176">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="8f68d-176">MPN partner admin</span></span>|<span data-ttu-id="8f68d-177">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="8f68d-178">• Afficher les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="8f68d-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="8f68d-179">• Afficher les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="8f68d-179">• View user details and their skills data</span></span>
||<span data-ttu-id="8f68d-180">• Afficher les compétences</span><span class="sxs-lookup"><span data-stu-id="8f68d-180">• View competencies</span></span>
||<span data-ttu-id="8f68d-181">• Afficher et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="8f68d-181">• View and manage benefits</span></span>
||<span data-ttu-id="8f68d-182">• Afficher et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="8f68d-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="8f68d-183">• Afficher les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="8f68d-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8f68d-184">• Afficher les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="8f68d-185">• Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="8f68d-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="8f68d-186">• Afficher l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="8f68d-186">- View customer data analytics</span></span>
|| <span data-ttu-id="8f68d-187">• Afficher d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="8f68d-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="8f68d-188">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="8f68d-188">Account admin</span></span>| <span data-ttu-id="8f68d-189">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="8f68d-189">Add locations</span></span>
|| <span data-ttu-id="8f68d-190">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="8f68d-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8f68d-191">• Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="8f68d-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8f68d-192">• Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="8f68d-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="8f68d-193">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="8f68d-193">Manage referrals</span></span> 

|<span data-ttu-id="8f68d-194">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="8f68d-194">**Role**</span></span>|<span data-ttu-id="8f68d-195">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="8f68d-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="8f68d-196">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="8f68d-196">Referrals admin</span></span>       |<span data-ttu-id="8f68d-197">• Afficher, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="8f68d-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="8f68d-198">• Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="8f68d-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="8f68d-199">• Afficher, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="8f68d-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="8f68d-200">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="8f68d-201">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="8f68d-201">Business profile admin</span></span>   |<span data-ttu-id="8f68d-202">• Afficher, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="8f68d-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="8f68d-203">• Afficher, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="8f68d-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="8f68d-204">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-204">Manage incentives</span></span> 

|<span data-ttu-id="8f68d-205">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="8f68d-205">**Role**</span></span> | <span data-ttu-id="8f68d-206">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="8f68d-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8f68d-207">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-207">Incentives admin</span></span>|<span data-ttu-id="8f68d-208">• Lancer et gérer des primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="8f68d-209">• Afficher et modifier tous les aspects des programmes de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8f68d-210">• Afficher et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="8f68d-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8f68d-211">• Afficher les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="8f68d-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8f68d-212">• Accéder au support</span><span class="sxs-lookup"><span data-stu-id="8f68d-212">• Access support</span></span>
||<span data-ttu-id="8f68d-213">• Contester des paiements de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="8f68d-214">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-214">Incentives user</span></span>|<span data-ttu-id="8f68d-215">• Afficher les programmes de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="8f68d-216">• Afficher et lancer des revendications de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="8f68d-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8f68d-217">• Afficher les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="8f68d-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8f68d-218">• Accéder au support</span><span class="sxs-lookup"><span data-stu-id="8f68d-218">• Access support</span></span>












