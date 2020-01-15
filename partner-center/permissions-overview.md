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
ms.openlocfilehash: bf7b1d2b029f2ce4558a2b24c3e1f12a63813339
ms.sourcegitcommit: bd76d42044ed4e3266395455a1956b2f9ccece76
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/09/2020
ms.locfileid: "75776500"
---
# <a name="assign-users-roles-and-permissions"></a>Affecter des rôles et des autorisations aux utilisateurs

**Rôles appropriés**
-   Administrateur général
-   Administrateur des utilisateurs
-   Administrateur partenaire MPN

Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise. Prochaine étape : demander à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires

Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez. Les rôles sont liés aux programmes auxquels votre entreprise participe. Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous n’avez pas uniquement besoin des rôle de gestion de locataire Azure AD standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques du programme des fournisseurs de solutions Cloud. Chaque programme est associé à des rôles spécifiques.

>[!Note]
> Les rôles de locataire Azure Active Directory (AAD) incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud. Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. Ils incluent l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)

|**Rôle**|**Ce qu’il peut faire**|
|----------------------------------|:---------------------------------|
|Administrateur général|• Accéder à tous les comptes/services Microsoft avec des privilèges complets
|      |• Créer des tickets de support pour l’Espace partenaires
||• Afficher les contrats, les listes de prix et les offres
||• Afficher, créer et gérer les utilisateurs partenaires|
||  • Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement
|Administrateur de la gestion des utilisateurs   | • Afficher, créer et gérer des utilisateurs
||• Afficher tous les profils de partenaire
||• Afficher, créer et gérer les utilisateurs partenaires  |
|Administrateur de la facturation | • Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement|
|Utilisateur par défaut|  • Afficher son profil   |
|Agent d’administration | • Gestion des clients
||• Ajouter une liste d’appareils à l’Espace partenaires
||• Créer des profils et les appliquer aux appareils
||• Gestion des abonnements
||• État du service et demandes de service pour les clients
||• Demander des privilèges d’administrateur délégué
||• Afficher les tarifs et les offres
||• Facturation
||• Administrer au nom d’un client
||• Inscrire un revendeur à valeur ajoutée|
|Agent commercial | • Gestion des clients
||• Ajouter une liste d’appareils à l’Espace partenaires
||• Gestion des abonnements
||• Afficher les tickets de support
||• Demander une relation avec un client
||• Gérer les prospects
||• Afficher le contrat client
||• Inscrire un revendeur à valeur ajoutée|
|Agent du support technique| • Rechercher et afficher un client
||• Modifier les détails du client
||• Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement
||• Demander un support pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)
||• Gérer les problèmes d’abonnements et de facturation pour le compte de clients (remarque : vous devez être agent administrateur pour effectuer cette tâche pour les abonnements Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fournisseur de panneau de contrôle (CPV) (rôle Fournisseur de solutions Cloud et rôle non-AAD)
Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires. 

|**Rôle**   |**Ce qu’il peut faire**|
|------------------------------|:----------------------------|
|Administrateur général| Voir et gérer votre profil de CPV|
||Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Utilisateur invité (doit être ajouté au locataire AAD)

|**Utilisateur invité**   | **Rôles**|
|---------------------------|:--------------------|
||Administrateur partenaire MPN|
||Administrateur des comptes|
||Administrateur de primes incitatives|
||Administrateur de profils métier|
||Administrateur des références|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gérer l’appartenance MPN et votre entreprise (rôles non-AAD : ces rôles gèrent l’activité de l’entreprise plutôt que le locataire)

|**Rôle** | **Ce qu’il peut faire**|
|----------------------------|:----------------------------|
|Administrateur partenaire MPN|• Afficher, créer et gérer les demandes de service des partenaires||
||• Afficher les profils juridiques, d’entreprise, métier et MPN
||• Afficher les détails des utilisateurs et les données sur leurs compétences
||• Afficher les compétences
||• Afficher et gérer les revenus
||• Afficher et acheter les offres MPN
||• Afficher les factures et l’historique des commandes des offres MPN
||• Afficher les données des indicateurs de contribution des partenaires
||• Peut fonctionner dans l’outil de validation et d’échange de bons|
||• Afficher l’analyse des données client
|| • Afficher d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles
|Administrateur des comptes| • Ajouter des emplacements
|| • Gérer les profils associés aux comptes dont vous êtes administrateur 
||• Affecter des rôles non-ADD aux utilisateurs dans le locataire 
||• Inscrire des emplacements dans des programmes


## <a name="manage-referrals"></a>Gérer les références 

|**Rôle**|**Ce qu’il peut faire**|
|-----------------------------|:------------------------|
|Administrateur des références       |• Afficher, créer et gérer les profils métier
||• Recevoir et gérer les références
||• Afficher, créer et gérer les références de covente|
||• Afficher, créer et gérer les demandes de service des partenaires
|Administrateur de profils métier   |• Afficher, créer et gérer le profil métier 
||• Afficher, créer et gérer les demandes de service des partenaires|

## <a name="manage-incentives"></a>Gérer les primes incitatives 

|**Rôle** | **Ce qu’il peut faire**|
|------------------------------|:-------------------------|
|Administrateur de primes incitatives|• Lancer et gérer des primes incitatives 
||• Afficher et modifier tous les aspects des programmes de primes incitatives
||• Afficher et modifier les informations bancaires et fiscales
||• Afficher les remises et les revenus de coopération
||• Accéder au support
||• Contester des paiements de primes incitatives|
|Utilisateur de primes incitatives|• Afficher les programmes de primes incitatives
||• Afficher et lancer des revendications de primes incitatives
||• Afficher les remises et les revenus de coopération
||• Accéder au support

## <a name="view-partner-center-insights-data"></a>Consulter les données des insights de l’Espace partenaires

|**Rôle** | **Ce qu’il peut faire**|
|------------------------------|:-------------------------|
|Visionneuse de rapports de la direction|Accéder à tous les jeux de données de rapport|
|Visionneuse de rapports|Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés|












