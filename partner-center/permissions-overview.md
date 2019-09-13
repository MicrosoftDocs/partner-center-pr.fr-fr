---
title: Attribuer des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 3/5/2019
description: Chaque employé devant travailler dans l’espace partenaires doit se voir attribuer un rôle.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708868"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="91d6c-104">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="91d6c-104">Assign users roles and permissions</span></span>


<span data-ttu-id="91d6c-105">Vous avez configuré votre profil de partenaire, y compris le nom et l’adresse légaux, les détails du support, les exemptions de taxes de fichier, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="91d6c-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="91d6c-106">Étape suivante: demandez à vos utilisateurs de configurer des mots de passe et des rôles pour qu’ils puissent commencer à travailler dans l’espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="91d6c-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="91d6c-107">Configurer vos employés pour qu’ils travaillent dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="91d6c-108">Vous déterminez les types d’accès dont vos utilisateurs ont besoin dans l’espace partenaires par les rôles et les autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="91d6c-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="91d6c-109">Les rôles sont liés au (x) programme (s) dans lequel votre entreprise est impliquée.</span><span class="sxs-lookup"><span data-stu-id="91d6c-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="91d6c-110">Par exemple, si votre entreprise est un fournisseur de solutions Cloud (CSP), vous n’aurez pas uniquement les rôles de gestion standard Azure AD locataires, tels que l’administrateur général, mais vous aurez besoin de rôles spécifiques au programme CSP.</span><span class="sxs-lookup"><span data-stu-id="91d6c-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="91d6c-111">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="91d6c-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="91d6c-112">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles administrateur général, administrateur d’utilisateur et CSP.</span><span class="sxs-lookup"><span data-stu-id="91d6c-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="91d6c-113">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. ils incluent l’administrateur MPN, l’administrateur du profil d’entreprise, l’administrateur de la référence, l’administrateur de l’incentive et l’utilisateur de l’incentive.</span><span class="sxs-lookup"><span data-stu-id="91d6c-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="91d6c-114">Gérer les transactions commerciales dans l’espace partenaires (rôles Azure AD et CSP)</span><span class="sxs-lookup"><span data-stu-id="91d6c-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="91d6c-115">**Actif**</span><span class="sxs-lookup"><span data-stu-id="91d6c-115">**Role**</span></span>|<span data-ttu-id="91d6c-116">**Ce qu’ils peuvent faire**</span><span class="sxs-lookup"><span data-stu-id="91d6c-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="91d6c-117">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="91d6c-117">Global admin</span></span>|<span data-ttu-id="91d6c-118">• Peut accéder à tous les compte Microsoft/Services avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="91d6c-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="91d6c-119">• Créer des tickets de support pour l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="91d6c-120">• Afficher les contrats, les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="91d6c-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="91d6c-121">• Afficher, créer et gérer des utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="91d6c-122">Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="91d6c-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="91d6c-123">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="91d6c-123">User management admin</span></span>   | <span data-ttu-id="91d6c-124">• Afficher, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="91d6c-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="91d6c-125">• Afficher tous les profils de partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-125">• View all partner profiles</span></span>
||<span data-ttu-id="91d6c-126">• Afficher, créer et gérer des utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="91d6c-127">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="91d6c-127">Billing admin</span></span> | <span data-ttu-id="91d6c-128">-Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="91d6c-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="91d6c-129">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="91d6c-129">Default user</span></span>|  <span data-ttu-id="91d6c-130">Afficher mon profil</span><span class="sxs-lookup"><span data-stu-id="91d6c-130">View My profile</span></span>   |
|<span data-ttu-id="91d6c-131">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="91d6c-131">Admin agent</span></span> | <span data-ttu-id="91d6c-132">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="91d6c-132">•    Customer management</span></span>
||<span data-ttu-id="91d6c-133">• Ajouter une liste d’appareils à l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="91d6c-134">• Créer et appliquer des profils à des appareils</span><span class="sxs-lookup"><span data-stu-id="91d6c-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="91d6c-135">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="91d6c-135">• Subscription management</span></span>
||<span data-ttu-id="91d6c-136">• Service de contrôle d’intégrité et de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="91d6c-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="91d6c-137">• Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="91d6c-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="91d6c-138">• Afficher la tarification et les offres</span><span class="sxs-lookup"><span data-stu-id="91d6c-138">• View pricing and offers</span></span>
||<span data-ttu-id="91d6c-139">• Facturation</span><span class="sxs-lookup"><span data-stu-id="91d6c-139">• Billing</span></span>
||<span data-ttu-id="91d6c-140">• Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="91d6c-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="91d6c-141">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="91d6c-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="91d6c-142">Commercial</span><span class="sxs-lookup"><span data-stu-id="91d6c-142">Sales agent</span></span> | <span data-ttu-id="91d6c-143">• Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="91d6c-143">•    Customer management</span></span>
||<span data-ttu-id="91d6c-144">• Ajouter une liste d’appareils à l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="91d6c-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="91d6c-145">• Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="91d6c-145">• Subscription management</span></span>
||<span data-ttu-id="91d6c-146">• Afficher les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="91d6c-146">• View price lists and offers</span></span>
||<span data-ttu-id="91d6c-147">• Afficher les tickets de support</span><span class="sxs-lookup"><span data-stu-id="91d6c-147">• View support tickets</span></span>
||<span data-ttu-id="91d6c-148">• Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="91d6c-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="91d6c-149">• Gérer les prospects client</span><span class="sxs-lookup"><span data-stu-id="91d6c-149">• Manage customer leads</span></span>
||<span data-ttu-id="91d6c-150">• Afficher le contrat du client</span><span class="sxs-lookup"><span data-stu-id="91d6c-150">• View the customer agreement</span></span>
||<span data-ttu-id="91d6c-151">• Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="91d6c-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="91d6c-152">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="91d6c-152">Helpdesk agent</span></span>| <span data-ttu-id="91d6c-153">• Rechercher et afficher un client</span><span class="sxs-lookup"><span data-stu-id="91d6c-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="91d6c-154">• Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="91d6c-154">• Edit customer details</span></span>
||<span data-ttu-id="91d6c-155">• Aider à résoudre les problèmes des clients avec la facturation ou la gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="91d6c-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="91d6c-156">• Demande de support pour le compte des clients (Remarque: Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="91d6c-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="91d6c-157">• Gérer les abonnements et les problèmes de facturation pour le compte des clients (Remarque: Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)</span><span class="sxs-lookup"><span data-stu-id="91d6c-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="91d6c-158">Fournisseur du panneau de configuration (CPV).</span><span class="sxs-lookup"><span data-stu-id="91d6c-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="91d6c-159">(Rôle CSP et rôle non AAD)</span><span class="sxs-lookup"><span data-stu-id="91d6c-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="91d6c-160">CPVs développez des applications à utiliser par les partenaires fournisseurs de solutions Cloud (CSP) pour leur permettre d’intégrer leurs systèmes aux API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="91d6c-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="91d6c-161">**Actif**</span><span class="sxs-lookup"><span data-stu-id="91d6c-161">**Role**</span></span>   |<span data-ttu-id="91d6c-162">**Ce que vous pouvez faire**</span><span class="sxs-lookup"><span data-stu-id="91d6c-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="91d6c-163">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="91d6c-163">Global admin</span></span>| <span data-ttu-id="91d6c-164">Afficher et gérer votre profil CPV</span><span class="sxs-lookup"><span data-stu-id="91d6c-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="91d6c-165">Afficher et gérer les utilisateurs qui ont besoin d’accéder aux fonctionnalités du CPV</span><span class="sxs-lookup"><span data-stu-id="91d6c-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="91d6c-166">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="91d6c-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="91d6c-167">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="91d6c-167">**Guest user**</span></span>   | <span data-ttu-id="91d6c-168">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="91d6c-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="91d6c-169">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="91d6c-169">MPN partner admin</span></span>|
||<span data-ttu-id="91d6c-170">Administration des comptes</span><span class="sxs-lookup"><span data-stu-id="91d6c-170">Accounts admin</span></span>|
||<span data-ttu-id="91d6c-171">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="91d6c-171">Incentives admin</span></span>|
||<span data-ttu-id="91d6c-172">Administrateur de profil d'entreprise</span><span class="sxs-lookup"><span data-stu-id="91d6c-172">Business profile admin</span></span>|
||<span data-ttu-id="91d6c-173">Administration des références</span><span class="sxs-lookup"><span data-stu-id="91d6c-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="91d6c-174">Gérer l’appartenance MPN et votre entreprise (rôles non AAD: ces rôles gèrent l’entreprise de la société plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="91d6c-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="91d6c-175">**Actif**</span><span class="sxs-lookup"><span data-stu-id="91d6c-175">**Role**</span></span> | <span data-ttu-id="91d6c-176">**Ce que vous pouvez faire**</span><span class="sxs-lookup"><span data-stu-id="91d6c-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="91d6c-177">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="91d6c-177">MPN partner admin</span></span>|<span data-ttu-id="91d6c-178">• Afficher, créer et gérer les demandes de service partenaire</span><span class="sxs-lookup"><span data-stu-id="91d6c-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="91d6c-179">• Afficher les profils juridiques, de société, d’entreprise et MPN</span><span class="sxs-lookup"><span data-stu-id="91d6c-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="91d6c-180">• Afficher les détails de l’utilisateur et leurs données de compétences</span><span class="sxs-lookup"><span data-stu-id="91d6c-180">• View user details and their skills data</span></span>
||<span data-ttu-id="91d6c-181">• Afficher les compétences</span><span class="sxs-lookup"><span data-stu-id="91d6c-181">• View competencies</span></span>
||<span data-ttu-id="91d6c-182">• Afficher et gérer les avantages</span><span class="sxs-lookup"><span data-stu-id="91d6c-182">• View and manage benefits</span></span>
||<span data-ttu-id="91d6c-183">• Afficher et acheter des offres MPN</span><span class="sxs-lookup"><span data-stu-id="91d6c-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="91d6c-184">• View MPN propose des factures et l’historique des commandes</span><span class="sxs-lookup"><span data-stu-id="91d6c-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="91d6c-185">• Afficher les données de l’indicateur de contribution partenaire</span><span class="sxs-lookup"><span data-stu-id="91d6c-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="91d6c-186">• Peut fonctionner dans l’outil de validation de pièce justificative</span><span class="sxs-lookup"><span data-stu-id="91d6c-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="91d6c-187">-Afficher l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="91d6c-187">- View customer data analytics</span></span>
|| <span data-ttu-id="91d6c-188">Afficher d’autres rôles d’utilisateur au sein de la société, mais ne peut pas attribuer de rôles</span><span class="sxs-lookup"><span data-stu-id="91d6c-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="91d6c-189">Administration de compte</span><span class="sxs-lookup"><span data-stu-id="91d6c-189">Account admin</span></span>| <span data-ttu-id="91d6c-190">Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="91d6c-190">Add locations</span></span>
|| <span data-ttu-id="91d6c-191">Gérer les profils associés aux comptes dont vous êtes l’administrateur</span><span class="sxs-lookup"><span data-stu-id="91d6c-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="91d6c-192">• Assigner des rôles pour les utilisateurs du locataire aux rôles non AAD</span><span class="sxs-lookup"><span data-stu-id="91d6c-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="91d6c-193">• Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="91d6c-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="91d6c-194">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="91d6c-194">Manage referrals</span></span> 

|<span data-ttu-id="91d6c-195">**Actif**</span><span class="sxs-lookup"><span data-stu-id="91d6c-195">**Role**</span></span>|<span data-ttu-id="91d6c-196">**Ce que vous pouvez faire**</span><span class="sxs-lookup"><span data-stu-id="91d6c-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="91d6c-197">Administration des références</span><span class="sxs-lookup"><span data-stu-id="91d6c-197">Referrals admin</span></span>       |<span data-ttu-id="91d6c-198">• Afficher, créer et gérer des profils d’entreprise</span><span class="sxs-lookup"><span data-stu-id="91d6c-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="91d6c-199">• Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="91d6c-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="91d6c-200">• Afficher, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="91d6c-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="91d6c-201">• Afficher, créer et gérer les demandes de service partenaire</span><span class="sxs-lookup"><span data-stu-id="91d6c-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="91d6c-202">Administrateur de profil d'entreprise</span><span class="sxs-lookup"><span data-stu-id="91d6c-202">Business profile admin</span></span>   |<span data-ttu-id="91d6c-203">• Affichage, création et gestion d’un profil d’entreprise</span><span class="sxs-lookup"><span data-stu-id="91d6c-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="91d6c-204">• Afficher, créer et gérer les demandes de service partenaire</span><span class="sxs-lookup"><span data-stu-id="91d6c-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="91d6c-205">Gérer les incentives</span><span class="sxs-lookup"><span data-stu-id="91d6c-205">Manage incentives</span></span> 

|<span data-ttu-id="91d6c-206">**Actif**</span><span class="sxs-lookup"><span data-stu-id="91d6c-206">**Role**</span></span> | <span data-ttu-id="91d6c-207">**Ce que vous pouvez faire**</span><span class="sxs-lookup"><span data-stu-id="91d6c-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="91d6c-208">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="91d6c-208">Incentives admin</span></span>|<span data-ttu-id="91d6c-209">• Lance et gère les incentives</span><span class="sxs-lookup"><span data-stu-id="91d6c-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="91d6c-210">• Peut afficher et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="91d6c-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="91d6c-211">• Peut afficher et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="91d6c-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="91d6c-212">• Afficher les bénéfices de la remise et du cofinancement</span><span class="sxs-lookup"><span data-stu-id="91d6c-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="91d6c-213">• Prise en charge de l’accès</span><span class="sxs-lookup"><span data-stu-id="91d6c-213">• Access support</span></span>
||<span data-ttu-id="91d6c-214">• Paiements d’incentives pour les litiges</span><span class="sxs-lookup"><span data-stu-id="91d6c-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="91d6c-215">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="91d6c-215">Incentives user</span></span>|<span data-ttu-id="91d6c-216">• Peut afficher des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="91d6c-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="91d6c-217">• Peut afficher et lancer des demandes d’incentives</span><span class="sxs-lookup"><span data-stu-id="91d6c-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="91d6c-218">• Afficher les bénéfices de la remise et du cofinancement</span><span class="sxs-lookup"><span data-stu-id="91d6c-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="91d6c-219">• Prise en charge de l’accès</span><span class="sxs-lookup"><span data-stu-id="91d6c-219">• Access support</span></span>












