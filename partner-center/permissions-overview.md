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
# <a name="assign-users-roles-and-permissions"></a>Affecter des rôles et des autorisations aux utilisateurs


Vous avez configuré votre profil de partenaire, y compris le nom et l’adresse légaux, les détails du support, les exemptions de taxes de fichier, les informations bancaires et le contact principal de votre entreprise. Étape suivante: demandez à vos utilisateurs de configurer des mots de passe et des rôles pour qu’ils puissent commencer à travailler dans l’espace partenaires avec vous.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés pour qu’ils travaillent dans l’espace partenaires

Vous déterminez les types d’accès dont vos utilisateurs ont besoin dans l’espace partenaires par les rôles et les autorisations que vous leur donnez. Les rôles sont liés au (x) programme (s) dans lequel votre entreprise est impliquée. Par exemple, si votre entreprise est un fournisseur de solutions Cloud (CSP), vous n’aurez pas uniquement les rôles de gestion standard Azure AD locataires, tels que l’administrateur général, mais vous aurez besoin de rôles spécifiques au programme CSP. Chaque programme est associé à des rôles spécifiques.

>[!Note]
> Les rôles de locataire Azure Active Directory (AAD) incluent les rôles administrateur général, administrateur d’utilisateur et CSP. Les rôles non-AAD sont ceux qui ne gèrent pas le locataire. ils incluent l’administrateur MPN, l’administrateur du profil d’entreprise, l’administrateur de la référence, l’administrateur de l’incentive et l’utilisateur de l’incentive. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans l’espace partenaires (rôles Azure AD et CSP)

|**Actif**|**Ce qu’ils peuvent faire**|
|----------------------------------|:---------------------------------|
|Administrateur global|• Peut accéder à tous les compte Microsoft/Services avec des privilèges complets
|      |• Créer des tickets de support pour l’espace partenaires
||• Afficher les contrats, les tarifs et les offres
||• Afficher, créer et gérer des utilisateurs partenaires|
||  Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement
|Administrateur de la gestion des utilisateurs   | • Afficher, créer et gérer des utilisateurs
||• Afficher tous les profils de partenaires
||• Afficher, créer et gérer des utilisateurs partenaires  |
|Administration de facturation | -Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement|
|Utilisateur par défaut|  Afficher mon profil   |
|Agent d’administration | • Gestion des clients
||• Ajouter une liste d’appareils à l’espace partenaires
||• Créer et appliquer des profils à des appareils
||• Gestion des abonnements
||• Service de contrôle d’intégrité et de service pour les clients
||• Demander des privilèges d’administrateur délégué
||• Afficher la tarification et les offres
||• Facturation
||• Administrer au nom d’un client
||• Inscrire un revendeur à valeur ajoutée|
|Commercial | • Gestion des clients
||• Ajouter une liste d’appareils à l’espace partenaires
||• Gestion des abonnements
||• Afficher les listes de prix et les offres
||• Afficher les tickets de support
||• Demander une relation avec un client
||• Gérer les prospects client
||• Afficher le contrat du client
||• Inscrire un revendeur à valeur ajoutée|
|Agent du support technique| • Rechercher et afficher un client
||• Modifier les détails du client
||• Aider à résoudre les problèmes des clients avec la facturation ou la gestion des abonnements
||• Demande de support pour le compte des clients (Remarque: Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)
||• Gérer les abonnements et les problèmes de facturation pour le compte des clients (Remarque: Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fournisseur du panneau de configuration (CPV). (Rôle CSP et rôle non AAD)
CPVs développez des applications à utiliser par les partenaires fournisseurs de solutions Cloud (CSP) pour leur permettre d’intégrer leurs systèmes aux API de l’espace partenaires. 

|**Actif**   |**Ce que vous pouvez faire**|
|------------------------------|:----------------------------|
|Administrateur global| Afficher et gérer votre profil CPV|
||Afficher et gérer les utilisateurs qui ont besoin d’accéder aux fonctionnalités du CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Utilisateur invité (doit être ajouté au locataire AAD)

|**Utilisateur invité**   | **Rôles**|
|---------------------------|:--------------------|
||Administrateur partenaire MPN|
||Administration des comptes|
||Administrateur de primes incitatives|
||Administrateur de profil d'entreprise|
||Administration des références|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gérer l’appartenance MPN et votre entreprise (rôles non AAD: ces rôles gèrent l’entreprise de la société plutôt que le locataire)

|**Actif** | **Ce que vous pouvez faire**|
|----------------------------|:----------------------------|
|Administrateur partenaire MPN|• Afficher, créer et gérer les demandes de service partenaire||
||• Afficher les profils juridiques, de société, d’entreprise et MPN
||• Afficher les détails de l’utilisateur et leurs données de compétences
||• Afficher les compétences
||• Afficher et gérer les avantages
||• Afficher et acheter des offres MPN
||• View MPN propose des factures et l’historique des commandes
||• Afficher les données de l’indicateur de contribution partenaire
||• Peut fonctionner dans l’outil de validation de pièce justificative|
||-Afficher l’analyse des données client
|| Afficher d’autres rôles d’utilisateur au sein de la société, mais ne peut pas attribuer de rôles
|Administration de compte| Ajouter des emplacements
|| Gérer les profils associés aux comptes dont vous êtes l’administrateur 
||• Assigner des rôles pour les utilisateurs du locataire aux rôles non AAD 
||• Inscrire des emplacements dans des programmes


## <a name="manage-referrals"></a>Gérer les références 

|**Actif**|**Ce que vous pouvez faire**|
|-----------------------------|:------------------------|
|Administration des références       |• Afficher, créer et gérer des profils d’entreprise
||• Recevoir et gérer les références
||• Afficher, créer et gérer les références de covente|
||• Afficher, créer et gérer les demandes de service partenaire
|Administrateur de profil d'entreprise   |• Affichage, création et gestion d’un profil d’entreprise 
||• Afficher, créer et gérer les demandes de service partenaire|

## <a name="manage-incentives"></a>Gérer les incentives 

|**Actif** | **Ce que vous pouvez faire**|
|------------------------------|:-------------------------|
|Administrateur de primes incitatives|• Lance et gère les incentives 
||• Peut afficher et modifier tous les aspects des programmes d’incentives
||• Peut afficher et modifier les informations bancaires et fiscales
||• Afficher les bénéfices de la remise et du cofinancement
||• Prise en charge de l’accès
||• Paiements d’incentives pour les litiges|
|Utilisateur de primes incitatives|• Peut afficher des programmes d’incentives
||• Peut afficher et lancer des demandes d’incentives
||• Afficher les bénéfices de la remise et du cofinancement
||• Prise en charge de l’accès












