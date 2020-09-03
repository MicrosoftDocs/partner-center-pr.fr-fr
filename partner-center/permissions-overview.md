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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040765"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="20b3f-103">Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="20b3f-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="20b3f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="20b3f-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="20b3f-105">Global admin</span></span>
- <span data-ttu-id="20b3f-106">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="20b3f-106">User admin</span></span>
- <span data-ttu-id="20b3f-107">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-107">MPN partner admin</span></span>

<span data-ttu-id="20b3f-108">Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="20b3f-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="20b3f-109">Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.</span><span class="sxs-lookup"><span data-stu-id="20b3f-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="20b3f-110">Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="20b3f-111">Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez.</span><span class="sxs-lookup"><span data-stu-id="20b3f-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="20b3f-112">Les rôles sont liés aux programmes auxquels votre entreprise participe.</span><span class="sxs-lookup"><span data-stu-id="20b3f-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="20b3f-113">Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="20b3f-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="20b3f-114">Chaque programme est associé à des rôles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="20b3f-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="20b3f-115">Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="20b3f-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="20b3f-116">Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives.</span><span class="sxs-lookup"><span data-stu-id="20b3f-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="20b3f-117">Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)</span><span class="sxs-lookup"><span data-stu-id="20b3f-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="20b3f-118">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-118">**Role**</span></span>|<span data-ttu-id="20b3f-119">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="20b3f-120">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="20b3f-120">Global admin</span></span>|<span data-ttu-id="20b3f-121">\*    Accéder à tous les comptes/services Microsoft avec des privilèges complets</span><span class="sxs-lookup"><span data-stu-id="20b3f-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="20b3f-122">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-123">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="20b3f-124">\*    Voir les contrats, les listes de prix et les offres</span><span class="sxs-lookup"><span data-stu-id="20b3f-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="20b3f-125">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="20b3f-126">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="20b3f-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="20b3f-127">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="20b3f-127">User management admin</span></span>   | <span data-ttu-id="20b3f-128">\*    Voir, créer et gérer des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="20b3f-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="20b3f-129">\*    Voir tous les profils de partenaire</span><span class="sxs-lookup"><span data-stu-id="20b3f-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="20b3f-130">\*    Voir, créer et gérer les utilisateurs partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="20b3f-131">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-132">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="20b3f-133">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="20b3f-133">Billing admin</span></span> | <span data-ttu-id="20b3f-134">• Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="20b3f-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="20b3f-135">\*    Voir les prix</span><span class="sxs-lookup"><span data-stu-id="20b3f-135">\*    View pricing</span></span>
||<span data-ttu-id="20b3f-136">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-137">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="20b3f-138">Utilisateur par défaut</span><span class="sxs-lookup"><span data-stu-id="20b3f-138">Default user</span></span>|  <span data-ttu-id="20b3f-139">• Afficher son profil</span><span class="sxs-lookup"><span data-stu-id="20b3f-139">View My profile</span></span>   |
|<span data-ttu-id="20b3f-140">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="20b3f-140">Admin agent</span></span> | <span data-ttu-id="20b3f-141">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="20b3f-141">\*    Customer management</span></span>
||<span data-ttu-id="20b3f-142">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="20b3f-143">\*    Créer des profils et les appliquer aux appareils</span><span class="sxs-lookup"><span data-stu-id="20b3f-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="20b3f-144">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="20b3f-144">\*    Subscription management</span></span>
||<span data-ttu-id="20b3f-145">\*    État du service et demandes de service pour les clients</span><span class="sxs-lookup"><span data-stu-id="20b3f-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="20b3f-146">\*    Demander des privilèges d’administrateur délégué</span><span class="sxs-lookup"><span data-stu-id="20b3f-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="20b3f-147">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="20b3f-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="20b3f-148">\*    Facturation</span><span class="sxs-lookup"><span data-stu-id="20b3f-148">\*    Billing</span></span>
||<span data-ttu-id="20b3f-149">\*    Administrer au nom d’un client</span><span class="sxs-lookup"><span data-stu-id="20b3f-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="20b3f-150">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="20b3f-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="20b3f-151">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-152">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="20b3f-153">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="20b3f-153">Sales agent</span></span> | <span data-ttu-id="20b3f-154">\*    Gestion des clients</span><span class="sxs-lookup"><span data-stu-id="20b3f-154">\*    Customer management</span></span>
||<span data-ttu-id="20b3f-155">\*    Ajouter une liste d’appareils à l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="20b3f-156">\*    Gestion des abonnements</span><span class="sxs-lookup"><span data-stu-id="20b3f-156">\*    Subscription management</span></span>
||<span data-ttu-id="20b3f-157">\*    Voir les tickets de support</span><span class="sxs-lookup"><span data-stu-id="20b3f-157">\*    View support tickets</span></span>
||<span data-ttu-id="20b3f-158">\*    Demander une relation avec un client</span><span class="sxs-lookup"><span data-stu-id="20b3f-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="20b3f-159">\*    Voir les tarifs et les offres</span><span class="sxs-lookup"><span data-stu-id="20b3f-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="20b3f-160">\*    Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="20b3f-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="20b3f-161">\*    Voir le contrat d’un client</span><span class="sxs-lookup"><span data-stu-id="20b3f-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="20b3f-162">\*    Inscrire un revendeur à valeur ajoutée</span><span class="sxs-lookup"><span data-stu-id="20b3f-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="20b3f-163">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-164">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="20b3f-165">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="20b3f-165">Helpdesk agent</span></span>| <span data-ttu-id="20b3f-166">\*    Rechercher et voir un client</span><span class="sxs-lookup"><span data-stu-id="20b3f-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="20b3f-167">\*    Modifier les détails du client</span><span class="sxs-lookup"><span data-stu-id="20b3f-167">\*    Edit customer details</span></span>
||<span data-ttu-id="20b3f-168">\*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</span><span class="sxs-lookup"><span data-stu-id="20b3f-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="20b3f-169">\*    Demander un support pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="20b3f-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="20b3f-170">\*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients</span><span class="sxs-lookup"><span data-stu-id="20b3f-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="20b3f-171">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-172">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="20b3f-173">Fournisseur de panneau de contrôle (CPV)</span><span class="sxs-lookup"><span data-stu-id="20b3f-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="20b3f-174">(rôle Fournisseur de solutions Cloud et rôle non-AAD)</span><span class="sxs-lookup"><span data-stu-id="20b3f-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="20b3f-175">Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="20b3f-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="20b3f-176">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-176">**Role**</span></span>   |<span data-ttu-id="20b3f-177">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="20b3f-178">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="20b3f-178">Global admin</span></span>| <span data-ttu-id="20b3f-179">Voir et gérer votre profil de CPV</span><span class="sxs-lookup"><span data-stu-id="20b3f-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="20b3f-180">Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV</span><span class="sxs-lookup"><span data-stu-id="20b3f-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="20b3f-181">Utilisateur invité (doit être ajouté au locataire AAD)</span><span class="sxs-lookup"><span data-stu-id="20b3f-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="20b3f-182">**Utilisateur invité**</span><span class="sxs-lookup"><span data-stu-id="20b3f-182">**Guest user**</span></span>   | <span data-ttu-id="20b3f-183">**Rôles**</span><span class="sxs-lookup"><span data-stu-id="20b3f-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="20b3f-184">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-184">MPN partner admin</span></span>|
||<span data-ttu-id="20b3f-185">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="20b3f-185">Accounts admin</span></span>|
||<span data-ttu-id="20b3f-186">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="20b3f-186">Incentives admin</span></span>|
||<span data-ttu-id="20b3f-187">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="20b3f-187">Business profile admin</span></span>|
||<span data-ttu-id="20b3f-188">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="20b3f-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="20b3f-189">Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)</span><span class="sxs-lookup"><span data-stu-id="20b3f-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="20b3f-190">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-190">**Role**</span></span> | <span data-ttu-id="20b3f-191">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="20b3f-192">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-192">MPN partner admin</span></span>|<span data-ttu-id="20b3f-193">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="20b3f-194">\*    Voir les profils juridiques, d’entreprise, métier et MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="20b3f-195">\*    Voir les détails des utilisateurs et les données sur leurs compétences</span><span class="sxs-lookup"><span data-stu-id="20b3f-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="20b3f-196">\*    Voir les compétences</span><span class="sxs-lookup"><span data-stu-id="20b3f-196">\*    View competencies</span></span>
||<span data-ttu-id="20b3f-197">\*    Voir et gérer les revenus</span><span class="sxs-lookup"><span data-stu-id="20b3f-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="20b3f-198">\*    Voir et acheter les offres MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="20b3f-199">\*    Voir les factures et l’historique des commandes des offres MPN</span><span class="sxs-lookup"><span data-stu-id="20b3f-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="20b3f-200">\*    Voir les données des indicateurs de contribution des partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="20b3f-201">\*    Peut fonctionner dans l’outil de validation et d’échange de bons</span><span class="sxs-lookup"><span data-stu-id="20b3f-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="20b3f-202">\*    Voir l’analyse des données client</span><span class="sxs-lookup"><span data-stu-id="20b3f-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="20b3f-203">\*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles</span><span class="sxs-lookup"><span data-stu-id="20b3f-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="20b3f-204">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-205">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="20b3f-206">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="20b3f-206">Account admin</span></span>| <span data-ttu-id="20b3f-207">• Ajouter des emplacements</span><span class="sxs-lookup"><span data-stu-id="20b3f-207">Add locations</span></span>
|| <span data-ttu-id="20b3f-208">• Gérer les profils associés aux comptes dont vous êtes administrateur</span><span class="sxs-lookup"><span data-stu-id="20b3f-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="20b3f-209">\*    Affecter des rôles non-ADD aux utilisateurs dans le locataire</span><span class="sxs-lookup"><span data-stu-id="20b3f-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="20b3f-210">\*    Inscrire des emplacements dans des programmes</span><span class="sxs-lookup"><span data-stu-id="20b3f-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="20b3f-211">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-212">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="20b3f-213">Gérer les références</span><span class="sxs-lookup"><span data-stu-id="20b3f-213">Manage referrals</span></span> 

|<span data-ttu-id="20b3f-214">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-214">**Role**</span></span>|<span data-ttu-id="20b3f-215">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="20b3f-216">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="20b3f-216">Referrals admin</span></span>       |<span data-ttu-id="20b3f-217">\*    Voir, créer et gérer les profils métier</span><span class="sxs-lookup"><span data-stu-id="20b3f-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="20b3f-218">\*    Recevoir et gérer les références</span><span class="sxs-lookup"><span data-stu-id="20b3f-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="20b3f-219">\* Voir, créer et gérer les références de covente</span><span class="sxs-lookup"><span data-stu-id="20b3f-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="20b3f-220">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="20b3f-221">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="20b3f-221">Business profile admin</span></span>   |<span data-ttu-id="20b3f-222">\* Voir, créer et gérer le profil métier</span><span class="sxs-lookup"><span data-stu-id="20b3f-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="20b3f-223">\*    Voir, créer et gérer les demandes de service des partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="20b3f-224">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-225">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="20b3f-226">Gérer les primes incitatives</span><span class="sxs-lookup"><span data-stu-id="20b3f-226">Manage incentives</span></span> 

|<span data-ttu-id="20b3f-227">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-227">**Role**</span></span> | <span data-ttu-id="20b3f-228">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="20b3f-229">Administrateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="20b3f-229">Incentives admin</span></span>|<span data-ttu-id="20b3f-230">\*    Lancer et gérer des incentives</span><span class="sxs-lookup"><span data-stu-id="20b3f-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="20b3f-231">\*    Voir et modifier tous les aspects des programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="20b3f-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="20b3f-232">\*    Voir et modifier les informations bancaires et fiscales</span><span class="sxs-lookup"><span data-stu-id="20b3f-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="20b3f-233">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="20b3f-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="20b3f-234">\*    Accéder au support</span><span class="sxs-lookup"><span data-stu-id="20b3f-234">\*    Access support</span></span>
||<span data-ttu-id="20b3f-235">\*    Contester des paiements d’incentives</span><span class="sxs-lookup"><span data-stu-id="20b3f-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="20b3f-236">Utilisateur de primes incitatives</span><span class="sxs-lookup"><span data-stu-id="20b3f-236">Incentives user</span></span>|<span data-ttu-id="20b3f-237">\*    Voir les programmes d’incentives</span><span class="sxs-lookup"><span data-stu-id="20b3f-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="20b3f-238">\*    Voir et lancer des revendications d’incentives</span><span class="sxs-lookup"><span data-stu-id="20b3f-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="20b3f-239">\*    Voir les remises et les revenus de coopération</span><span class="sxs-lookup"><span data-stu-id="20b3f-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="20b3f-240">\*    Créer des tickets de support pour l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="20b3f-241">\*    Voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="20b3f-242">Consulter les données des insights de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20b3f-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="20b3f-243">**Rôle**</span><span class="sxs-lookup"><span data-stu-id="20b3f-243">**Role**</span></span> | <span data-ttu-id="20b3f-244">**Ce qu’il peut faire**</span><span class="sxs-lookup"><span data-stu-id="20b3f-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="20b3f-245">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="20b3f-245">Executive report viewer</span></span>|<span data-ttu-id="20b3f-246">Accéder à tous les jeux de données de rapport, créer des tickets de support, voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="20b3f-247">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="20b3f-247">Report viewer</span></span>|<span data-ttu-id="20b3f-248">Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés, créer des tickets de support partenaire, voir les tickets de support partenaire que vous créez</span><span class="sxs-lookup"><span data-stu-id="20b3f-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
