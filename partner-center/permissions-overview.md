---
title: Attribuer des rôles et des autorisations aux utilisateurs
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à identifier les rôles les mieux adaptés aux utilisateurs de votre entreprise qui gèrent les transactions commerciales, les références, les incentives ou les adhésions MPN dans l’Espace partenaires.
author: hemas
ms.author: hemas
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f4ec3a1a14e6845f7b6079e286876d9bb1f3dd5
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948597"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="3dc69-104">Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="3dc69-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="3dc69-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3dc69-106">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="3dc69-106">Global admin</span></span>
- <span data-ttu-id="3dc69-107">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3dc69-107">User admin</span></span>
- <span data-ttu-id="3dc69-108">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-108">MPN partner admin</span></span>

<span data-ttu-id="3dc69-109">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="3dc69-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="3dc69-110">Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="3dc69-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="3dc69-111">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="3dc69-112">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="3dc69-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="3dc69-113">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="3dc69-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="3dc69-114">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="3dc69-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="3dc69-115">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="3dc69-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="3dc69-116">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="3dc69-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="3dc69-117">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="3dc69-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="3dc69-118">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="3dc69-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="3dc69-119">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-119">**Role**</span></span>|<span data-ttu-id="3dc69-120">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="3dc69-121">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="3dc69-121">Global admin</span></span>|<span data-ttu-id="3dc69-122">\*    Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="3dc69-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="3dc69-123">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dc69-124">\*    Voir les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="3dc69-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="3dc69-125">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="3dc69-126">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="3dc69-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="3dc69-127">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3dc69-127">User management admin</span></span>   | <span data-ttu-id="3dc69-128">\*    Voir, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3dc69-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="3dc69-129">\*    Voir tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="3dc69-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="3dc69-130">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="3dc69-131">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="3dc69-131">Billing admin</span></span> | <span data-ttu-id="3dc69-132">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="3dc69-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="3dc69-133">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="3dc69-133">Default user</span></span>|  <span data-ttu-id="3dc69-134">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="3dc69-134">View My profile</span></span>   |
|<span data-ttu-id="3dc69-135">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="3dc69-135">Admin agent</span></span> | <span data-ttu-id="3dc69-136">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="3dc69-136">\*    Customer management</span></span>
||<span data-ttu-id="3dc69-137">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="3dc69-138">\*    Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="3dc69-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="3dc69-139">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="3dc69-139">\*    Subscription management</span></span>
||<span data-ttu-id="3dc69-140">\*    État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="3dc69-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="3dc69-141">\*    Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="3dc69-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="3dc69-142">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="3dc69-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="3dc69-143">\*    Facturation</span><span class="sxs-lookup"><span data-stu-id="3dc69-143">\*    Billing</span></span>
||<span data-ttu-id="3dc69-144">\*    Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="3dc69-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="3dc69-145">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="3dc69-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="3dc69-146">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="3dc69-146">Sales agent</span></span> | <span data-ttu-id="3dc69-147">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="3dc69-147">\*    Customer management</span></span>
||<span data-ttu-id="3dc69-148">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="3dc69-149">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="3dc69-149">\*    Subscription management</span></span>
||<span data-ttu-id="3dc69-150">\*    Voir les tickets de support</span><span class="sxs-lookup"><span data-stu-id="3dc69-150">\*    View support tickets</span></span>
||<span data-ttu-id="3dc69-151">\*    Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="3dc69-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="3dc69-152">\*    Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="3dc69-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="3dc69-153">\*    Voir le contrat d’un client</span><span class="sxs-lookup"><span data-stu-id="3dc69-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="3dc69-154">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="3dc69-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="3dc69-155">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="3dc69-155">Helpdesk agent</span></span>| <span data-ttu-id="3dc69-156">\*    Rechercher et voir un client</span><span class="sxs-lookup"><span data-stu-id="3dc69-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="3dc69-157">\*    Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="3dc69-157">\*    Edit customer details</span></span>
||<span data-ttu-id="3dc69-158">\*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="3dc69-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="3dc69-159">\*    Demander un support pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="3dc69-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="3dc69-160">\*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="3dc69-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="3dc69-161">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="3dc69-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="3dc69-162">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="3dc69-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="3dc69-163">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="3dc69-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="3dc69-164">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-164">**Role**</span></span>   |<span data-ttu-id="3dc69-165">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="3dc69-166">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="3dc69-166">Global admin</span></span>| <span data-ttu-id="3dc69-167">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="3dc69-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="3dc69-168">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="3dc69-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="3dc69-169">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="3dc69-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="3dc69-170">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="3dc69-170">**Guest user**</span></span>   | <span data-ttu-id="3dc69-171">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="3dc69-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="3dc69-172">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-172">MPN partner admin</span></span>|
||<span data-ttu-id="3dc69-173">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="3dc69-173">Accounts admin</span></span>|
||<span data-ttu-id="3dc69-174">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="3dc69-174">Incentives admin</span></span>|
||<span data-ttu-id="3dc69-175">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="3dc69-175">Business profile admin</span></span>|
||<span data-ttu-id="3dc69-176">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="3dc69-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="3dc69-177">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="3dc69-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="3dc69-178">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-178">**Role**</span></span> | <span data-ttu-id="3dc69-179">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="3dc69-180">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-180">MPN partner admin</span></span>|<span data-ttu-id="3dc69-181">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="3dc69-182">\*    Voir les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="3dc69-183">\*    Voir les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="3dc69-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="3dc69-184">\*    Voir les compétences</span><span class="sxs-lookup"><span data-stu-id="3dc69-184">\*    View competencies</span></span>
||<span data-ttu-id="3dc69-185">\*    Voir et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="3dc69-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="3dc69-186">\*    Voir et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="3dc69-187">\*    Voir les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="3dc69-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="3dc69-188">\*    Voir les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="3dc69-189">\*    Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="3dc69-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="3dc69-190">\*    Voir l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="3dc69-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="3dc69-191">\*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="3dc69-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="3dc69-192">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="3dc69-192">Account admin</span></span>| <span data-ttu-id="3dc69-193">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="3dc69-193">Add locations</span></span>
|| <span data-ttu-id="3dc69-194">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="3dc69-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="3dc69-195">\*    Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="3dc69-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="3dc69-196">\*    Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="3dc69-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="3dc69-197">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="3dc69-197">Manage referrals</span></span> 

|<span data-ttu-id="3dc69-198">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-198">**Role**</span></span>|<span data-ttu-id="3dc69-199">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="3dc69-200">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="3dc69-200">Referrals admin</span></span>       |<span data-ttu-id="3dc69-201">\*    Voir, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="3dc69-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="3dc69-202">\*    Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="3dc69-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="3dc69-203">\* Voir, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="3dc69-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="3dc69-204">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="3dc69-205">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="3dc69-205">Business profile admin</span></span>   |<span data-ttu-id="3dc69-206">\* Voir, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="3dc69-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="3dc69-207">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="3dc69-208">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="3dc69-208">Manage incentives</span></span> 

|<span data-ttu-id="3dc69-209">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-209">**Role**</span></span> | <span data-ttu-id="3dc69-210">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="3dc69-211">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="3dc69-211">Incentives admin</span></span>|<span data-ttu-id="3dc69-212">\*    Lancer et gérer des incentives</span><span class="sxs-lookup"><span data-stu-id="3dc69-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="3dc69-213">\*    Voir et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="3dc69-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="3dc69-214">\*    Voir et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="3dc69-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="3dc69-215">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="3dc69-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="3dc69-216">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="3dc69-216">\*    Access support</span></span>
||<span data-ttu-id="3dc69-217">\*    Contester des paiements d’incentives</span><span class="sxs-lookup"><span data-stu-id="3dc69-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="3dc69-218">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="3dc69-218">Incentives user</span></span>|<span data-ttu-id="3dc69-219">\*    Voir les programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="3dc69-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="3dc69-220">\*    Voir et lancer des revendications d’incentives</span><span class="sxs-lookup"><span data-stu-id="3dc69-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="3dc69-221">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="3dc69-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="3dc69-222">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="3dc69-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="3dc69-223">Consulter les données des insights de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3dc69-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="3dc69-224">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="3dc69-224">**Role**</span></span> | <span data-ttu-id="3dc69-225">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="3dc69-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="3dc69-226">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="3dc69-226">Executive report viewer</span></span>|<span data-ttu-id="3dc69-227">Accéder à tous les jeux de données de rapport</span><span class="sxs-lookup"><span data-stu-id="3dc69-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="3dc69-228">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="3dc69-228">Report viewer</span></span>|<span data-ttu-id="3dc69-229">Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés</span><span class="sxs-lookup"><span data-stu-id="3dc69-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    