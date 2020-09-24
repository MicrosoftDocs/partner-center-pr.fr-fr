---
title: Attribuer des rôles et des autorisations aux utilisateurs
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à identifier les rôles les mieux adaptés aux utilisateurs de votre entreprise qui gèrent les transactions commerciales, les références, les incentives ou les adhésions MPN dans l’Espace partenaires.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 391602651976500576f13824bfebc6e06fec40a2
ms.sourcegitcommit: 9359f92fb7d3965374eb095ebf68fd6a94ec4943
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/21/2020
ms.locfileid: "90832112"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires

**Rôles appropriés**

- Administrateur général
- Administrateur des utilisateurs
- Administrateur partenaire MPN

Vous avez configuré votre profil de partenaire, notamment le nom légal, l’adresse officielle, les détails du support, les exonérations fiscales, les informations bancaires et le contact principal de votre entreprise. Étape suivante : Demandez à vos utilisateurs de configurer des mots de passe et des rôles pour pouvoir commencer à travailler dans l’Espace partenaires avec vous.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés pour qu’ils travaillent dans l’Espace partenaires

Vous déterminez les types d’accès que vos utilisateurs ont dans l’Espace partenaires à l’aide des rôles et autorisations que vous leur donnez. Les rôles sont liés aux programmes auxquels votre entreprise participe. Par exemple, si votre entreprise est un fournisseur de solutions Cloud, vous avez non seulement besoin de rôles de gestion de locataire Azure Active Directory standard, comme celui de l’administrateur général, mais aussi de rôles spécifiques au programme CSP. Chaque programme est associé à des rôles spécifiques.

>[!Note]
> Les rôles de locataire Azure Active Directory incluent les rôles d’administrateur général, d’administrateur d’utilisateurs et de fournisseur de solutions Cloud. Les rôles non-Azure Active Directory sont ceux qui ne gèrent pas le locataire, comme l’administrateur MPN, l’administrateur de profils métier, l’administrateur des références, l’administrateur d’incentives et l’utilisateur d’incentives. 

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
|Agent d’administration | *    Gestion des clients|[Configuration et gestion des comptes clients pour les partenaires revendeurs dans l’Espace partenaires](customer-accounts.md)
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

Les CPV développent des applications utilisées par les partenaires fournisseurs de solutions Cloud pour leur permettre d’intégrer leurs systèmes aux API de l’Espace partenaires. 

|**Rôle**   |**Ce qu’il peut faire**|**En savoir plus**|
|------------------------------|:----------------------------|----|
|Administrateur général| Voir et gérer votre profil de CPV|[S’inscrire en tant que fournisseur de panneau de configuration pour faciliter l’intégration des systèmes de partenaires CSP aux API de l’Espace partenaires](enroll-as-cpv.md)
||Voir et gérer vos utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Utilisateur invité (doit être ajouté au locataire Azure Active Directory)

|**Utilisateur invité**   | **Rôles**|
|---------------------------|:--------------------|
||Administrateur partenaire MPN|
||Administrateur des comptes|
||Administrateur de primes incitatives|
||Administrateur de profils métier|
||Administrateur des références|


## <a name="manage-mpn-membership-and-your-company"></a>Gérer l’appartenance MPN et votre entreprise 

Ces rôles ne sont pas des rôles Azure Active Directory. Ces rôles gèrent l’activité de la société plutôt que le locataire.

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
||*    Affecter des rôles non-Azure Active Directory aux utilisateurs dans le locataire 
||*    Inscrire des emplacements dans des programmes
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez


## <a name="manage-referrals"></a>Gérer les références 

|**Rôle**|**Ce qu’il peut faire**|**En savoir plus**|
|-----------------------------|:------------------------|---|
|Administrateur des références       |*    Voir, créer et gérer les profils métier|[Gérer différents prospects, comme les demandes des clients, des prospects qualifiés par le marketing et des prospects qualifiés par les commerciaux](manage-leads.md)
||*    Recevoir et gérer les références
||* Voir, créer et gérer les références de covente|
||*    Voir, créer et gérer les demandes de service des partenaires
|Administrateur de profils métier   |* Voir, créer et gérer le profil métier |[Créer un profil professionnel](create-a-marketing-profile.md)
||*    Voir, créer et gérer les demandes de service des partenaires
||*    Créer des tickets de support pour l’Espace partenaires
||*    Voir les tickets de support partenaire que vous créez|

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
