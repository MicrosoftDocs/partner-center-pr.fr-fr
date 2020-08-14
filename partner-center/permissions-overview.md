---
title: Attribuer des rôles et des autorisations aux utilisateurs
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à identifier les rôles les mieux adaptés aux utilisateurs de votre entreprise qui gèrent les transactions commerciales, les références, les incentives ou les adhésions MPN dans l’Espace partenaires.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839184"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="b9465-103">Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="b9465-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="b9465-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b9465-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="b9465-105">Global admin</span></span>
- <span data-ttu-id="b9465-106">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b9465-106">User admin</span></span>
- <span data-ttu-id="b9465-107">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-107">MPN partner admin</span></span>

<span data-ttu-id="b9465-108">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="b9465-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="b9465-109">Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="b9465-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="b9465-110">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="b9465-111">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="b9465-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="b9465-112">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="b9465-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="b9465-113">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="b9465-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="b9465-114">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="b9465-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="b9465-115">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="b9465-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="b9465-116">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="b9465-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="b9465-117">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="b9465-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="b9465-118">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-118">**Role**</span></span>|<span data-ttu-id="b9465-119">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="b9465-120">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="b9465-120">Global admin</span></span>|<span data-ttu-id="b9465-121">\*    Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="b9465-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="b9465-122">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="b9465-123">\*    Voir les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="b9465-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="b9465-124">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="b9465-125">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="b9465-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="b9465-126">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b9465-126">User management admin</span></span>   | <span data-ttu-id="b9465-127">\*    Voir, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b9465-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="b9465-128">\*    Voir tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="b9465-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="b9465-129">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="b9465-130">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="b9465-130">Billing admin</span></span> | <span data-ttu-id="b9465-131">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="b9465-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="b9465-132">\*    Voir les prix</span><span class="sxs-lookup"><span data-stu-id="b9465-132">\*    View pricing</span></span>
|<span data-ttu-id="b9465-133">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="b9465-133">Default user</span></span>|  <span data-ttu-id="b9465-134">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="b9465-134">View My profile</span></span>   |
|<span data-ttu-id="b9465-135">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="b9465-135">Admin agent</span></span> | <span data-ttu-id="b9465-136">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="b9465-136">\*    Customer management</span></span>
||<span data-ttu-id="b9465-137">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="b9465-138">\*    Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="b9465-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="b9465-139">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="b9465-139">\*    Subscription management</span></span>
||<span data-ttu-id="b9465-140">\*    État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="b9465-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="b9465-141">\*    Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="b9465-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="b9465-142">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="b9465-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="b9465-143">\*    Facturation</span><span class="sxs-lookup"><span data-stu-id="b9465-143">\*    Billing</span></span>
||<span data-ttu-id="b9465-144">\*    Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="b9465-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="b9465-145">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="b9465-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="b9465-146">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="b9465-146">Sales agent</span></span> | <span data-ttu-id="b9465-147">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="b9465-147">\*    Customer management</span></span>
||<span data-ttu-id="b9465-148">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="b9465-149">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="b9465-149">\*    Subscription management</span></span>
||<span data-ttu-id="b9465-150">\*    Voir les tickets de support</span><span class="sxs-lookup"><span data-stu-id="b9465-150">\*    View support tickets</span></span>
||<span data-ttu-id="b9465-151">\*    Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="b9465-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="b9465-152">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="b9465-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="b9465-153">\*    Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="b9465-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="b9465-154">\*    Voir le contrat d’un client</span><span class="sxs-lookup"><span data-stu-id="b9465-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="b9465-155">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="b9465-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="b9465-156">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="b9465-156">Helpdesk agent</span></span>| <span data-ttu-id="b9465-157">\*    Rechercher et voir un client</span><span class="sxs-lookup"><span data-stu-id="b9465-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="b9465-158">\*    Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="b9465-158">\*    Edit customer details</span></span>
||<span data-ttu-id="b9465-159">\*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="b9465-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="b9465-160">\*    Demander un support pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="b9465-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="b9465-161">\*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="b9465-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="b9465-162">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="b9465-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="b9465-163">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="b9465-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="b9465-164">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b9465-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="b9465-165">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-165">**Role**</span></span>   |<span data-ttu-id="b9465-166">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="b9465-167">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="b9465-167">Global admin</span></span>| <span data-ttu-id="b9465-168">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="b9465-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="b9465-169">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="b9465-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="b9465-170">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="b9465-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="b9465-171">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="b9465-171">**Guest user**</span></span>   | <span data-ttu-id="b9465-172">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="b9465-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="b9465-173">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-173">MPN partner admin</span></span>|
||<span data-ttu-id="b9465-174">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="b9465-174">Accounts admin</span></span>|
||<span data-ttu-id="b9465-175">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="b9465-175">Incentives admin</span></span>|
||<span data-ttu-id="b9465-176">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="b9465-176">Business profile admin</span></span>|
||<span data-ttu-id="b9465-177">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="b9465-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="b9465-178">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="b9465-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="b9465-179">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-179">**Role**</span></span> | <span data-ttu-id="b9465-180">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="b9465-181">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-181">MPN partner admin</span></span>|<span data-ttu-id="b9465-182">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="b9465-183">\*    Voir les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="b9465-184">\*    Voir les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="b9465-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="b9465-185">\*    Voir les compétences</span><span class="sxs-lookup"><span data-stu-id="b9465-185">\*    View competencies</span></span>
||<span data-ttu-id="b9465-186">\*    Voir et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="b9465-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="b9465-187">\*    Voir et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="b9465-188">\*    Voir les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="b9465-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="b9465-189">\*    Voir les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="b9465-190">\*    Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="b9465-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="b9465-191">\*    Voir l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="b9465-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="b9465-192">\*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="b9465-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="b9465-193">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="b9465-193">Account admin</span></span>| <span data-ttu-id="b9465-194">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="b9465-194">Add locations</span></span>
|| <span data-ttu-id="b9465-195">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="b9465-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="b9465-196">\*    Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="b9465-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="b9465-197">\*    Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="b9465-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="b9465-198">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="b9465-198">Manage referrals</span></span> 

|<span data-ttu-id="b9465-199">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-199">**Role**</span></span>|<span data-ttu-id="b9465-200">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="b9465-201">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="b9465-201">Referrals admin</span></span>       |<span data-ttu-id="b9465-202">\*    Voir, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="b9465-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="b9465-203">\*    Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="b9465-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="b9465-204">\* Voir, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="b9465-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="b9465-205">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="b9465-206">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="b9465-206">Business profile admin</span></span>   |<span data-ttu-id="b9465-207">\* Voir, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="b9465-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="b9465-208">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="b9465-209">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="b9465-209">Manage incentives</span></span> 

|<span data-ttu-id="b9465-210">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-210">**Role**</span></span> | <span data-ttu-id="b9465-211">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="b9465-212">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="b9465-212">Incentives admin</span></span>|<span data-ttu-id="b9465-213">\*    Lancer et gérer des incentives</span><span class="sxs-lookup"><span data-stu-id="b9465-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="b9465-214">\*    Voir et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="b9465-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="b9465-215">\*    Voir et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="b9465-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="b9465-216">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="b9465-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="b9465-217">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="b9465-217">\*    Access support</span></span>
||<span data-ttu-id="b9465-218">\*    Contester des paiements d’incentives</span><span class="sxs-lookup"><span data-stu-id="b9465-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="b9465-219">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="b9465-219">Incentives user</span></span>|<span data-ttu-id="b9465-220">\*    Voir les programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="b9465-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="b9465-221">\*    Voir et lancer des revendications d’incentives</span><span class="sxs-lookup"><span data-stu-id="b9465-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="b9465-222">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="b9465-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="b9465-223">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="b9465-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="b9465-224">Consulter les données des insights de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b9465-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="b9465-225">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="b9465-225">**Role**</span></span> | <span data-ttu-id="b9465-226">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="b9465-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="b9465-227">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="b9465-227">Executive report viewer</span></span>|<span data-ttu-id="b9465-228">Accéder à tous les jeux de données de rapport</span><span class="sxs-lookup"><span data-stu-id="b9465-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="b9465-229">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="b9465-229">Report viewer</span></span>|<span data-ttu-id="b9465-230">Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés</span><span class="sxs-lookup"><span data-stu-id="b9465-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
