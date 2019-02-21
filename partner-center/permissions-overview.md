---
title: Attribuer des rôles d’utilisateurs et des autorisations | L’espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Tous les employés qui ont besoin de travailler dans l’espace partenaires doivent disposer d’un rôle.
author: labrenne
ms.author: labrenne
keywords: rôles, autorisations, administrateur, agent
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086727"
---
# <a name="assign-users-roles-and-permissions"></a>Affecter des rôles et des autorisations aux utilisateurs


Vous avez configuré votre profil de partenaire, y compris le nom légal et adresse, détails du support, d’exonération fiscale, informations bancaires et le contact principal pour votre entreprise. Étape suivante: demandez à vos utilisateurs configuré avec les rôles et les mots de passe afin qu’ils peuvent commencer à travailler dans l’espace partenaires avec vous.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés à travailler dans l’espace partenaires

Vous déterminez les types de vos utilisateurs ont vers l’espace partenaires par les rôles et autorisations que vous leur accordez un accès. Rôles sont liés aux répartis impliqué dans votre entreprise. Par exemple, si votre entreprise est une activité de fournisseur de solutions Cloud (CSP), pas seulement avoir Azure AD standard des rôles de gestion, tels qu’Administrateur général de client, mais devront rôles spécifiques au programme fournisseur de solutions cloud. Chaque programme possède des rôles spécifiques à celui-ci.

>[!Note]
> Rôles de client Azure Active Directory (AAD) incluent l’administrateur général, administrateur d’utilisateurs et les rôles de fournisseur de solutions cloud. Les rôles de non-AAD incluent administrateur MPN, administrateur de profil d’entreprise, administrateur des références, administrateur de primes incitatives et utilisateur de primes incitatives. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans l’espace partenaires (Azure AD et les rôles de fournisseur de solutions cloud)

|**Rôle**|**Ce qu’il peut faire**|
|----------------------------------|:---------------------------------|
|Administrateur général|• Peuvent accéder à tous les comptes/services Microsoft avec des privilèges complets
|      |• Créer des tickets de support pour l’espace partenaires
||• Afficher les contrats, listes de prix et offres
||• Afficher, créer et gérer les utilisateurs partenaires|
|Administrateur utilisateur   | • Afficher, créer et gérer des utilisateurs
||• Afficher tous les profils de partenaire
||• Afficher, créer et gérer les utilisateurs partenaires  |
|Utilisateur par défaut|  Afficher mon profil   |
|Agent d’administration | • Gestion des clients
||• Ajouter une liste d’appareil pour le Center< partenaire
||• Créer et appliquer des profils sur des appareils
||• Gestion des abonnements
||• Service health et demandes de service pour les clients
||• Demande des privilèges d’administrateur délégués
||• Vue tarification et offres
||• Facturation
||• Administrer au nom d’un client
||• Inscrire une valeur ajoutée revendeur|
|Commercial | • Gestion des clients
||• Ajouter une liste de l’appareil à l’espace partenaires
||• Gestion des abonnements
||• Afficher les tickets de support
||• Demander une relation avec un client
||• Gérer les prospects
||• Vue le contrat client
||• Inscrire un revendeur à valeur ajoutée|
|Agent du support technique| • Rechercher et afficher un client
||• Modifier les détails de client
||• Aide résoudre les problèmes client avec la gestion de facturation ou d’abonnement
||• Demande de prise en charge pour le compte de clients (Remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office 365)
||• Gérer les abonnements et de facturation des problèmes pour le compte de clients (Remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office 365)|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fournisseur du panneau contrôle (CPV). (Rôle de fournisseur de solutions cloud et non AAD)
CPVs développer des applications pour une utilisation par les partenaires de fournisseur de solutions Cloud (CSP) pour accroître leur intégrer leurs systèmes avec les API de l’espace partenaires. 

|**Rôle**   |**Ce que vous pouvez faire**|
|------------------------------|:----------------------------|
|Administrateur général| Afficher et gérer votre profil CPV|
||Afficher et gérer une de vos utilisateurs ont besoin d’accéder aux fonctionnalités CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Gérer l’adhésion au MPN et votre société (rôles non AAD)

|**Rôle** | **Ce que vous pouvez faire**|
|----------------------------|:----------------------------|
|Administrateur MPN|•CAN ajouter des utilisateurs non clients
||• Afficher, créer et gérer les demandes de service de l’espace
||• Vue juridiques, organisation, entreprise et des profils MPN
||• Afficher les détails utilisateur et les données sur leurs compétences
||• Afficher les compétences
||• Afficher et gérer les avantages
||Achat et • vue aux offres MPN
||• Vue MPN offre les factures et l’historique des commandes
||• Peut afficher des données de contribution partenaire
||• Utilisable dans l’outil de Validation de document|
|Administrateur de compte| • Peut ajouter des utilisateurs non clients
||• Ajouter ou supprimer des emplacements
||-Gérer les profils liés aux comptes de que vous êtes l’administrateur 
||• Affecter des rôles pour les utilisateurs de client aux rôles non AAD 
||• Inscrire des emplacements dans des programmes

## <a name="manage-referrals-non-aad-roles"></a>Gérer des références (rôles non AAD)

|**Rôle**|**Ce que vous pouvez faire**|
|-----------------------------|:------------------------|
|Administrateur des références       |• Afficher, créer et gérer les profils commerciaux
||• Recevoir et gérer des références
||• Afficher, créer et gérer les demandes de service de l’espace|
|Administrateur de profil d'entreprise   |•View, créer et gérer le profil d’entreprise 
||• Afficher, créer et gérer les demandes de service de l’espace|

## <a name="manage-incentives--non-aad-roles"></a>Gérer les primes (rôles non AAD)

|**Rôle** | **Ce que vous pouvez faire**|
|------------------------------|:-------------------------|
|Administrateur de primes incitatives|• Initie et gère les primes incitatives 
||• Peut afficher et modifier tous les aspects de programmes de primes incitatives
||• Peut afficher et modifier les informations bancaires et fiscaux
||• Vue remise et le mode coopération bénéfices
||• Accès prise en charge
||• Les paiements de primes incitatives litige|
|Utilisateur de primes incitatives|• Peut afficher les programmes de primes incitatives
||• Peut afficher et lancer des revendications de primes incitatives
||• Vue remise et le mode coopération bénéfices
||• Vue remise et le mode coopération bénéfices
||• Accès prise en charge












