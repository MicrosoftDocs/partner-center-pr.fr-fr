---
title: Affecter des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 03/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les rôles les mieux adaptés à vos utilisateurs qui gèrent des transactions commerciales, des références, des incentives ou les adhésions MPN de votre entreprise.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: high
ms.openlocfilehash: fbff7f353a0055aa645467fccaa049b598b4c880
ms.sourcegitcommit: f9c5c11258d5c827bb6fbbb31bc26ba70c346f11
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2020
ms.locfileid: "80296396"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="7a205-104">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="7a205-104">Assign users roles and permissions</span></span>

<span data-ttu-id="7a205-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="7a205-105">**Appropriate roles**</span></span>
-    <span data-ttu-id="7a205-106">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="7a205-106">Global admin</span></span>
-    <span data-ttu-id="7a205-107">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="7a205-107">User admin</span></span>
-    <span data-ttu-id="7a205-108">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-108">MPN partner admin</span></span>

<span data-ttu-id="7a205-109">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="7a205-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7a205-110">Prochaine étape : demander à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="7a205-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7a205-111">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7a205-112">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="7a205-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7a205-113">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="7a205-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7a205-114">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="7a205-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7a205-115">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="7a205-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7a205-116">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="7a205-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7a205-117">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="7a205-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7a205-118">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="7a205-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7a205-119">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-119">**Role**</span></span>|<span data-ttu-id="7a205-120">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7a205-121">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="7a205-121">Global admin</span></span>|<span data-ttu-id="7a205-122">\*    Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="7a205-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7a205-123">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7a205-124">\*    Voir les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="7a205-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7a205-125">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7a205-126">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="7a205-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7a205-127">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="7a205-127">User management admin</span></span>   | <span data-ttu-id="7a205-128">\*    Voir, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="7a205-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="7a205-129">\*    Voir tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="7a205-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="7a205-130">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7a205-131">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="7a205-131">Billing admin</span></span> | <span data-ttu-id="7a205-132">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="7a205-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="7a205-133">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="7a205-133">Default user</span></span>|  <span data-ttu-id="7a205-134">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="7a205-134">View My profile</span></span>   |
|<span data-ttu-id="7a205-135">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="7a205-135">Admin agent</span></span> | <span data-ttu-id="7a205-136">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="7a205-136">\*    Customer management</span></span>
||<span data-ttu-id="7a205-137">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7a205-138">\*    Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="7a205-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="7a205-139">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="7a205-139">\*    Subscription management</span></span>
||<span data-ttu-id="7a205-140">\*    État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="7a205-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="7a205-141">\*    Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="7a205-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="7a205-142">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="7a205-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="7a205-143">\*    Facturation</span><span class="sxs-lookup"><span data-stu-id="7a205-143">\*    Billing</span></span>
||<span data-ttu-id="7a205-144">\*    Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="7a205-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="7a205-145">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="7a205-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="7a205-146">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="7a205-146">Sales agent</span></span> | <span data-ttu-id="7a205-147">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="7a205-147">\*    Customer management</span></span>
||<span data-ttu-id="7a205-148">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7a205-149">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="7a205-149">\*    Subscription management</span></span>
||<span data-ttu-id="7a205-150">\*    Voir les tickets de support</span><span class="sxs-lookup"><span data-stu-id="7a205-150">\*    View support tickets</span></span>
||<span data-ttu-id="7a205-151">\*    Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="7a205-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="7a205-152">\*    Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="7a205-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="7a205-153">\*    Voir le contrat d’un client</span><span class="sxs-lookup"><span data-stu-id="7a205-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="7a205-154">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="7a205-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="7a205-155">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="7a205-155">Helpdesk agent</span></span>| <span data-ttu-id="7a205-156">\*    Rechercher et voir un client</span><span class="sxs-lookup"><span data-stu-id="7a205-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="7a205-157">\*    Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="7a205-157">\*    Edit customer details</span></span>
||<span data-ttu-id="7a205-158">\*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="7a205-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7a205-159">\*    Demander un support pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="7a205-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="7a205-160">\*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="7a205-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7a205-161">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="7a205-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7a205-162">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="7a205-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7a205-163">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="7a205-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7a205-164">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-164">**Role**</span></span>   |<span data-ttu-id="7a205-165">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7a205-166">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="7a205-166">Global admin</span></span>| <span data-ttu-id="7a205-167">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="7a205-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7a205-168">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="7a205-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7a205-169">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="7a205-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7a205-170">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="7a205-170">**Guest user**</span></span>   | <span data-ttu-id="7a205-171">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="7a205-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7a205-172">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-172">MPN partner admin</span></span>|
||<span data-ttu-id="7a205-173">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="7a205-173">Accounts admin</span></span>|
||<span data-ttu-id="7a205-174">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="7a205-174">Incentives admin</span></span>|
||<span data-ttu-id="7a205-175">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="7a205-175">Business profile admin</span></span>|
||<span data-ttu-id="7a205-176">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="7a205-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7a205-177">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="7a205-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7a205-178">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-178">**Role**</span></span> | <span data-ttu-id="7a205-179">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7a205-180">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-180">MPN partner admin</span></span>|<span data-ttu-id="7a205-181">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7a205-182">\*    Voir les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7a205-183">\*    Voir les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="7a205-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="7a205-184">\*    Voir les compétences</span><span class="sxs-lookup"><span data-stu-id="7a205-184">\*    View competencies</span></span>
||<span data-ttu-id="7a205-185">\*    Voir et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="7a205-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="7a205-186">\*    Voir et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="7a205-187">\*    Voir les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="7a205-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7a205-188">\*    Voir les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="7a205-189">\*    Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="7a205-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7a205-190">\*    Voir l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="7a205-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="7a205-191">\*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="7a205-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7a205-192">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="7a205-192">Account admin</span></span>| <span data-ttu-id="7a205-193">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="7a205-193">Add locations</span></span>
|| <span data-ttu-id="7a205-194">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="7a205-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7a205-195">\*    Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="7a205-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7a205-196">\*    Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="7a205-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7a205-197">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="7a205-197">Manage referrals</span></span> 

|<span data-ttu-id="7a205-198">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-198">**Role**</span></span>|<span data-ttu-id="7a205-199">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7a205-200">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="7a205-200">Referrals admin</span></span>       |<span data-ttu-id="7a205-201">\*    Voir, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="7a205-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="7a205-202">\*    Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="7a205-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="7a205-203">\* Voir, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="7a205-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7a205-204">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7a205-205">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="7a205-205">Business profile admin</span></span>   |<span data-ttu-id="7a205-206">\* Voir, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="7a205-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="7a205-207">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7a205-208">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="7a205-208">Manage incentives</span></span> 

|<span data-ttu-id="7a205-209">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-209">**Role**</span></span> | <span data-ttu-id="7a205-210">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7a205-211">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="7a205-211">Incentives admin</span></span>|<span data-ttu-id="7a205-212">\*    Lancer et gérer des incentives</span><span class="sxs-lookup"><span data-stu-id="7a205-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="7a205-213">\*    Voir et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="7a205-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7a205-214">\*    Voir et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="7a205-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7a205-215">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="7a205-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7a205-216">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="7a205-216">\*    Access support</span></span>
||<span data-ttu-id="7a205-217">\*    Contester des paiements d’incentives</span><span class="sxs-lookup"><span data-stu-id="7a205-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="7a205-218">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="7a205-218">Incentives user</span></span>|<span data-ttu-id="7a205-219">\*    Voir les programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="7a205-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="7a205-220">\*    Voir et lancer des revendications d’incentives</span><span class="sxs-lookup"><span data-stu-id="7a205-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7a205-221">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="7a205-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7a205-222">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="7a205-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="7a205-223">Consulter les données des insights de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="7a205-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="7a205-224">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="7a205-224">**Role**</span></span> | <span data-ttu-id="7a205-225">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="7a205-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7a205-226">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="7a205-226">Executive report viewer</span></span>|<span data-ttu-id="7a205-227">Accéder à tous les jeux de données de rapport</span><span class="sxs-lookup"><span data-stu-id="7a205-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="7a205-228">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="7a205-228">Report viewer</span></span>|<span data-ttu-id="7a205-229">Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés</span><span class="sxs-lookup"><span data-stu-id="7a205-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    