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
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434318"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="5ff9e-103">Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="5ff9e-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5ff9e-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="5ff9e-105">Global admin</span></span>
- <span data-ttu-id="5ff9e-106">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5ff9e-106">User admin</span></span>
- <span data-ttu-id="5ff9e-107">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-107">MPN partner admin</span></span>

<span data-ttu-id="5ff9e-108">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="5ff9e-109">Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="5ff9e-110">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="5ff9e-111">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="5ff9e-112">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="5ff9e-113">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="5ff9e-114">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="5ff9e-115">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="5ff9e-116">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="5ff9e-117">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="5ff9e-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="5ff9e-118">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-118">**Role**</span></span>|<span data-ttu-id="5ff9e-119">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="5ff9e-120">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="5ff9e-120">Global admin</span></span>|<span data-ttu-id="5ff9e-121">\*    Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="5ff9e-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="5ff9e-122">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5ff9e-123">\*    Voir les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="5ff9e-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="5ff9e-124">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="5ff9e-125">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="5ff9e-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="5ff9e-126">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5ff9e-126">User management admin</span></span>   | <span data-ttu-id="5ff9e-127">\*    Voir, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5ff9e-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="5ff9e-128">\*    Voir tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="5ff9e-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="5ff9e-129">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="5ff9e-130">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="5ff9e-130">Billing admin</span></span> | <span data-ttu-id="5ff9e-131">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="5ff9e-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="5ff9e-132">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="5ff9e-132">Default user</span></span>|  <span data-ttu-id="5ff9e-133">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="5ff9e-133">View My profile</span></span>   |
|<span data-ttu-id="5ff9e-134">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="5ff9e-134">Admin agent</span></span> | <span data-ttu-id="5ff9e-135">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="5ff9e-135">\*    Customer management</span></span>
||<span data-ttu-id="5ff9e-136">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="5ff9e-137">\*    Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="5ff9e-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="5ff9e-138">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="5ff9e-138">\*    Subscription management</span></span>
||<span data-ttu-id="5ff9e-139">\*    État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="5ff9e-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="5ff9e-140">\*    Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="5ff9e-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="5ff9e-141">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="5ff9e-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="5ff9e-142">\*    Facturation</span><span class="sxs-lookup"><span data-stu-id="5ff9e-142">\*    Billing</span></span>
||<span data-ttu-id="5ff9e-143">\*    Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="5ff9e-144">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="5ff9e-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="5ff9e-145">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="5ff9e-145">Sales agent</span></span> | <span data-ttu-id="5ff9e-146">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="5ff9e-146">\*    Customer management</span></span>
||<span data-ttu-id="5ff9e-147">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="5ff9e-148">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="5ff9e-148">\*    Subscription management</span></span>
||<span data-ttu-id="5ff9e-149">\*    Voir les tickets de support</span><span class="sxs-lookup"><span data-stu-id="5ff9e-149">\*    View support tickets</span></span>
||<span data-ttu-id="5ff9e-150">\*    Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="5ff9e-151">\*    Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="5ff9e-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="5ff9e-152">\*    Voir le contrat d’un client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="5ff9e-153">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="5ff9e-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="5ff9e-154">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="5ff9e-154">Helpdesk agent</span></span>| <span data-ttu-id="5ff9e-155">\*    Rechercher et voir un client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="5ff9e-156">\*    Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-156">\*    Edit customer details</span></span>
||<span data-ttu-id="5ff9e-157">\*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="5ff9e-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="5ff9e-158">\*    Demander un support pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="5ff9e-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="5ff9e-159">\*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="5ff9e-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="5ff9e-160">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="5ff9e-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="5ff9e-161">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="5ff9e-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="5ff9e-162">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5ff9e-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="5ff9e-163">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-163">**Role**</span></span>   |<span data-ttu-id="5ff9e-164">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="5ff9e-165">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="5ff9e-165">Global admin</span></span>| <span data-ttu-id="5ff9e-166">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="5ff9e-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="5ff9e-167">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="5ff9e-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="5ff9e-168">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="5ff9e-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="5ff9e-169">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-169">**Guest user**</span></span>   | <span data-ttu-id="5ff9e-170">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="5ff9e-171">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-171">MPN partner admin</span></span>|
||<span data-ttu-id="5ff9e-172">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="5ff9e-172">Accounts admin</span></span>|
||<span data-ttu-id="5ff9e-173">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-173">Incentives admin</span></span>|
||<span data-ttu-id="5ff9e-174">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="5ff9e-174">Business profile admin</span></span>|
||<span data-ttu-id="5ff9e-175">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="5ff9e-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="5ff9e-176">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="5ff9e-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="5ff9e-177">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-177">**Role**</span></span> | <span data-ttu-id="5ff9e-178">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="5ff9e-179">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-179">MPN partner admin</span></span>|<span data-ttu-id="5ff9e-180">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="5ff9e-181">\*    Voir les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="5ff9e-182">\*    Voir les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="5ff9e-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="5ff9e-183">\*    Voir les compétences</span><span class="sxs-lookup"><span data-stu-id="5ff9e-183">\*    View competencies</span></span>
||<span data-ttu-id="5ff9e-184">\*    Voir et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="5ff9e-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="5ff9e-185">\*    Voir et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="5ff9e-186">\*    Voir les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="5ff9e-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="5ff9e-187">\*    Voir les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="5ff9e-188">\*    Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="5ff9e-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="5ff9e-189">\*    Voir l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="5ff9e-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="5ff9e-190">\*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="5ff9e-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="5ff9e-191">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="5ff9e-191">Account admin</span></span>| <span data-ttu-id="5ff9e-192">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="5ff9e-192">Add locations</span></span>
|| <span data-ttu-id="5ff9e-193">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="5ff9e-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="5ff9e-194">\*    Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="5ff9e-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="5ff9e-195">\*    Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="5ff9e-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="5ff9e-196">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="5ff9e-196">Manage referrals</span></span> 

|<span data-ttu-id="5ff9e-197">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-197">**Role**</span></span>|<span data-ttu-id="5ff9e-198">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="5ff9e-199">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="5ff9e-199">Referrals admin</span></span>       |<span data-ttu-id="5ff9e-200">\*    Voir, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="5ff9e-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="5ff9e-201">\*    Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="5ff9e-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="5ff9e-202">\* Voir, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="5ff9e-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="5ff9e-203">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="5ff9e-204">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="5ff9e-204">Business profile admin</span></span>   |<span data-ttu-id="5ff9e-205">\* Voir, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="5ff9e-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="5ff9e-206">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="5ff9e-207">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-207">Manage incentives</span></span> 

|<span data-ttu-id="5ff9e-208">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-208">**Role**</span></span> | <span data-ttu-id="5ff9e-209">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="5ff9e-210">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-210">Incentives admin</span></span>|<span data-ttu-id="5ff9e-211">\*    Lancer et gérer des incentives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="5ff9e-212">\*    Voir et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="5ff9e-213">\*    Voir et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="5ff9e-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="5ff9e-214">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="5ff9e-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="5ff9e-215">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="5ff9e-215">\*    Access support</span></span>
||<span data-ttu-id="5ff9e-216">\*    Contester des paiements d’incentives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="5ff9e-217">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-217">Incentives user</span></span>|<span data-ttu-id="5ff9e-218">\*    Voir les programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="5ff9e-219">\*    Voir et lancer des revendications d’incentives</span><span class="sxs-lookup"><span data-stu-id="5ff9e-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="5ff9e-220">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="5ff9e-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="5ff9e-221">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="5ff9e-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="5ff9e-222">Consulter les données des insights de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5ff9e-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="5ff9e-223">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-223">**Role**</span></span> | <span data-ttu-id="5ff9e-224">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="5ff9e-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="5ff9e-225">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="5ff9e-225">Executive report viewer</span></span>|<span data-ttu-id="5ff9e-226">Accéder à tous les jeux de données de rapport</span><span class="sxs-lookup"><span data-stu-id="5ff9e-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="5ff9e-227">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="5ff9e-227">Report viewer</span></span>|<span data-ttu-id="5ff9e-228">Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés</span><span class="sxs-lookup"><span data-stu-id="5ff9e-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    