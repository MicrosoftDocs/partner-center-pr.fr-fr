---
title: Attribuer des rôles et des autorisations aux utilisateurs
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à identifier les rôles les mieux adaptés aux utilisateurs de votre entreprise qui gèrent les transactions commerciales, les références, les incentives ou les adhésions MPN dans l’Espace partenaires.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565081"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires

**Rôles appropriés** : Administrateur général | Administrateur de la gestion des utilisateurs | Administrateur partenaire MPN

Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise. Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires

Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez. Les rôles sont liés aux programmes auxquels votre entreprise participe. Par exemple, si votre entreprise est un fournisseur de solutions cloud, vous avez non seulement besoin de rôles de gestion de locataire Azure Active Directory (Azure AD) standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques au programme CSP. Chaque programme est associé à des rôles spécifiques.

>[!Note]
> Les rôles de locataire Azure AD incluent les rôles d’administrateur général, d’administrateur des utilisateurs et de fournisseur de solutions cloud. Les rôles non-Azure AD sont ceux qui ne gèrent pas le locataire, comme l’administrateur des partenaires MPN (Microsoft Partner Network), l’administrateur de profils métier, l’administrateur des références, l’administrateur de primes incitatives et l’utilisateur de primes incitatives. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans l’Espace partenaires (rôles Azure AD et Fournisseur de solutions Microsoft Cloud)

|**Rôle**|**Ce qu’il peut faire**|**En savoir plus**|
|----------------------------------|---|:---------------------------------|
|Administrateur général|*    Accéder à tous les comptes/services Microsoft avec des privilèges complets|[Gérer votre compte dans l’Espace partenaires](partner-center-account-setup.md)
|      |*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez
||*    Voir les contrats, les listes de prix et les offres
||*    Voir, créer et gérer les utilisateurs partenaires|
||  • Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement
|Administrateur de la gestion des utilisateurs   | *    Voir, créer et gérer des utilisateurs|[Gérer les avantages et les offres de votre adhésion à Microsoft Partner Network dans l’Espace partenaires](manage-your-partner-network-benefits.md)
||*    Voir tous les profils de partenaire
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez
|Administrateur de la facturation | • Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement|[Lire votre facture](billing.md)
||*    Voir les prix
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez
|Utilisateur par défaut|  • Afficher son profil   |[Réinitialiser votre mot de passe](reset-my-pasword.md)
|Agent d’administration | *    Gestion des clients|[Se connecter à vos clients](connect-with-your-customers.md)
||*    Ajouter une liste d’appareils à l’Espace partenaires
||*    Créer des profils et les appliquer aux appareils
||*    Gestion des abonnements
||*    État du service et demandes de service pour les clients
||*    Demander des privilèges d’administrateur délégué
||*    Voir les tarifs et les offres
||*    Facturation
||*    Administrer au nom d’un client
||*    Inscrire un revendeur à valeur ajoutée
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez|
|Agent commercial | *    Gestion des clients|[Fournir du support sur la facturation à vos clients et aider à répondre à leurs questions sur la facturation](provide-billing-support.md)
||*    Ajouter une liste d’appareils à l’Espace partenaires
||*    Gestion des abonnements
||*    Voir les tickets de support
||*    Demander une relation avec un client
||*    Voir les tarifs et les offres
||*    Gérer les prospects
||*    Voir le contrat d’un client
||*    Inscrire un revendeur à valeur ajoutée
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez|
|Agent du support technique| *    Rechercher et voir un client|[Faire remonter les problèmes à Microsoft et découvrir les problèmes les plus adaptés à cette procédure](escalate-problems-to-microsoft.md)
||*    Modifier les détails du client
||*    Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement
||*    Demander un support pour le compte de clients 
||*    Gérer les problèmes d’abonnements et de facturation pour le compte de clients
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Fournisseur de panneau de contrôle (CPV) (rôle Fournisseur de solutions Cloud et rôle non-Azure AD)

Les CPV développent des applications utilisées par les partenaires CSP pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires. 

|**Rôle**   |**Ce qu’il peut faire**|**En savoir plus**|
|------------------------------|:----------------------------|----|
|Administrateur général| Afficher et gérer votre profil Fournisseur de panneau de contrôle (CPV)|[S’inscrire en tant que fournisseur de panneau de configuration pour faciliter l’intégration des systèmes de partenaires CSP aux API de l’Espace partenaires](enroll-as-cpv.md)
||Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Utilisateur invité (doit être ajouté au locataire Azure AD)

|**Utilisateur invité**   | **Rôles**|
|---------------------------|:--------------------|
||Administrateur partenaire MPN|
||Administrateur de profils métier|
||Administrateur des références|


## <a name="manage-mpn-membership-and-your-company"></a>Gérer l’appartenance MPN et votre entreprise 

Ces rôles ne sont pas des rôles Azure AD. Ces rôles gèrent l’activité de la société plutôt que le locataire.

|**Rôle** | **Ce qu’il peut faire**|**En savoir plus**|
|----------------------------|:----------------------------|-----|
|Administrateur partenaire MPN|*    Voir, créer et gérer les demandes de service des partenaires|[Premier achat ou renouvellement d’un abonnement Microsoft Action Pack ou de compétences Silver et Gold](mpn-get-action-pack.md)
||*    Voir les profils juridiques, d’entreprise, métier et MPN
||*    Voir les détails des utilisateurs et les données sur leurs compétences
||*    Voir les compétences
||*    Voir et gérer les revenus
||*    Voir et acheter les offres MPN
||*    Voir les factures et l’historique des commandes des offres MPN
||*    Voir les données des indicateurs de contribution des partenaires
||*    Peut fonctionner dans l’outil de validation et d’échange de bons|
||*    Voir l’analyse des données client
||*    Voir d’autres rôles d’utilisateur au sein de l’entreprise, sans pouvoir affecter de rôles
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez
|Administrateur des comptes| • Ajouter des emplacements|[Gérer des sites](manage-locations.md)
|| • Gérer les profils associés aux comptes dont vous êtes administrateur 
||*    Affecter des rôles non-Azure AD aux utilisateurs dans le locataire 
||*    Inscrire des emplacements dans des programmes
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez

## <a name="manage-referrals"></a>Gérer les références

|**Rôle** | **Ce qu’il peut faire**|**En savoir plus**
|------------------------------|:-------------------------|---|
|Administrateur des références|Créer et gérer tous les éléments sous l’onglet Références dans l’Espace partenaires|[Gérer les opportunités de co-vente](manage-co-sell-opportunities.md)
||    Peut afficher et modifier l’ensemble des prospects et opportunités de co-vente
||    Peut affecter des membres d’une équipe à une transaction
||    Peut consulter et modifier des profils métier
||    Peut consulter et inscrire des transactions pour les opportunités marquées comme conclues et éligibles à l’inscription de transactions
||    Peut créer et consulter des tickets de support
|Utilisateur Références|Créer et gérer des opportunités de co-vente uniquement s’il fait partie de l’équipe |[Gérer les opportunités de co-vente](manage-co-sell-opportunities.md)
||    Peut créer des opportunités de co-vente pour les emplacements où le rôle leur est attribué.
||    Peut consulter et inscrire des transactions pour les opportunités marquées comme conclues et éligibles à l’inscription de transactions s’il est membre d’une équipe.
||    Peut créer et consulter des tickets de support
|Administrateur de profils métier|Créer et gérer les profils métier | [Gérer des profils métier](create-a-marketing-profile.md)
||    Peut créer et consulter des tickets de support

Avec le nouveau rôle utilisateur Références, nous introduisons également la portée de l’emplacement pour les transactions. Le tableau ci-dessous décrit l’accès aux transactions en fonction de l’emplacement.

|**Étendue** | **Ce qu’il peut faire** |
|------------------------------|:-------------------------|
|Toute l’entreprise | Aussi bien les administrateurs que les utilisateurs ont accès aux opérations de création de transactions pour n’importe quel emplacement de leur entreprise|
|| L’administrateur des références a accès à la consultation et à la modification de toutes les transactions |
|| Les utilisateurs de références ont accès à l’affichage et à la modification de toutes les transactions uniquement s’ils font partie de l’équipe |
|Un ou plusieurs emplacements | Aussi bien les administrateurs que les utilisateurs ont accès aux opérations de création de transactions pour l’emplacement affecté de leur entreprise|
|| L’administrateur des références a accès à la consultation et à la modification de toutes les transactions appartenant aux emplacements affectés|
|| L’administrateur des références a accès à la consultation et à la modification de toutes les transactions appartenant aux emplacements affectés s’ils font partie de l’équipe|

## <a name="manage-incentives"></a>Gérer les primes incitatives

|**Rôle** | **Ce qu’il peut faire**|**En savoir plus**
|------------------------------|:-------------------------|---|
|Administrateur de primes incitatives|*    Lancer et gérer des incentives |[Utilisez ces ressources pour bien démarrer avec les incentives](incentives-get-started-intro.md)
||*    Voir et modifier tous les aspects des programmes d’incentives
||*    Voir et modifier les informations bancaires et fiscales
||*    Voir les remises et les revenus de coopération
||*    Accéder au support
||*    Contester des paiements d’incentives|
|Utilisateur de primes incitatives|*    Voir les programmes d’incentives
||*    Voir et lancer des revendications d’incentives
||*    Voir les remises et les revenus de coopération
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez

## <a name="view-partner-center-insights-data"></a>Consulter les données des insights de l’Espace partenaires

|**Rôle** | **Ce qu’il peut faire**|**En savoir plus**|
|------------------------------|:-------------------------|---|
|Visionneuse de rapports de la direction|Accéder à tous les jeux de données de rapport, créer des tickets de support, voir les tickets de support partenaire que vous créez|[Vue d’ensemble des rapports de tableau de bord disponibles dans les insights de l’Espace partenaires](pci-overview-report.md)
|Visionneuse de rapports|Accéder aux rapports de données, à l’exception des revenus et des données personnelles des clients et des employés, créer des tickets de support partenaire, voir les tickets de support partenaire que vous créez|

## <a name="next-steps"></a>Étapes suivantes

- [Créer des comptes d’utilisateur et attribuer des rôles et des autorisations](create-user-accounts-and-set-permissions.md)
- [Vérifier les informations de votre compte lors de votre inscription à un nouveau programme de l’Espace partenaires](verification-responses.md)
