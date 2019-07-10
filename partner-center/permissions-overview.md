---
title: Attribuer des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 3/5/19
description: Tous les employés doivent fonctionner dans l’espace partenaires doivent avoir un rôle.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690839"
---
# <a name="assign-users-roles-and-permissions"></a>Affecter des rôles et des autorisations aux utilisateurs


Vous avez configuré votre profil de partenaire, y compris juridique nom et adresse, les détails de prise en charge, exonérations de fichier, les informations bancaires et le contact principal de votre entreprise. Étape suivante : configurer des mots de passe et des rôles, afin qu’ils peuvent commencer à travailler dans des partenaires avec vous de vos utilisateurs.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés à travailler dans l’espace partenaires

Vous déterminez les types d’accès à que vos utilisateurs disposent de partenaires par les rôles et autorisations que vous leur donnez. Rôles associés à votre entreprise est impliqué dans l’ou les programmes. Par exemple, si votre entreprise est une entreprise de fournisseur de solutions Cloud (CSP), pas uniquement avoir l’Azure AD standard des rôles de gestion telles qu’Administrateur général du client, mais devez rôles spécifiques au programme CSP. Chaque programme possède des rôles spécifiques à celui-ci.

>[!Note]
> Rôles de locataire Azure Active Directory (AAD) incluent l’administrateur général, administrateur d’utilisateurs et rôles CSP. Rôles non-AAD sont les rôles que vous ne gérez pas le client, et elles incluent MPN admin, administrateur de profil d’entreprise, référence administrateur, administrateur offre incitative et offre incitative utilisateur. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans partenaires (Azure AD et les rôles CSP)

|**Role**|**Marche à suivre**|
|----------------------------------|:---------------------------------|
|Administrateur global|• Peuvent accéder à tous les comptes/services Microsoft avec privilèges complets
|      |• Créer des tickets de support pour l’espace partenaires
||• Afficher les contrats, des listes de prix et des offres
||• Afficher, créer et gérer des utilisateurs partenaires|
||  Afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement
|Administrateur de la gestion des utilisateurs   | • Afficher, créer et gérer les utilisateurs
||• Afficher tous les profils de partenaires
||• Afficher, créer et gérer des utilisateurs partenaires  |
|Administration de facturation | -Permet d’afficher, créer et gérer la facturation, les factures et les fichiers de rapprochement|
|Utilisateur par défaut|  Afficher mon profil   |
|Agent d’administration | • Gestion de client
||• Ajoutez la liste des appareils à l’espace partenaires
||• Créer et appliquer des profils sur des appareils
||• Gestion des abonnements
||Demandes de service et l’intégrité de Service pour les clients •
||• Demande des privilèges d’administration déléguée
||• Affichage tarification et offres
||• Facturation
||• Administrer pour le compte d’un client
||Register • une valeur ajoutée de revendeur|
|Commercial | • Gestion de client
||• Ajoutez la liste des appareils à l’espace partenaires
||• Gestion des abonnements
||• Afficher le prix de répertorie et offre
||• Les tickets de support de vue
||• Demande une relation avec un client
||• Gestion des prospects
||• Afficher le contrat de client
||• Register un revendeur à valeur ajoutée|
|Agent du support technique| • Rechercher et afficher un client
||• Modifier les détails de client
||• Problèmes des clients aide résolution avec la gestion de facturation ou d’abonnement
||• Une demande de support pour le compte de clients (Remarque : Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)
||• Gérer les abonnements et la facturation des problèmes pour le compte de clients (Remarque : Vous devez être un agent d’administration pour effectuer cette tâche pour les abonnements Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fournisseur de panneau de contrôle (CPV). (Rôle de fournisseur de services cryptographiques et rôle de non-AAD)
CPVs développer des applications pour une utilisation par les partenaires de fournisseur de solutions Cloud (CSP) pour leur permettre d’intégrer leurs systèmes avec les API Partner Center. 

|**Role**   |**Ce que vous pouvez faire**|
|------------------------------|:----------------------------|
|Administrateur global| Afficher et gérer votre profil CPV|
||Afficher et gérer des utilisateurs qui ont besoin d’accéder aux fonctionnalités CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Utilisateur invité (doit être ajouté au locataire AAD)

|**Utilisateur invité**   | **Rôles**|
|---------------------------|:--------------------|
||Administrateur partenaire MPN|
||Comptes administrateur|
||Administrateur de primes incitatives|
||Administrateur de profil d'entreprise|
||Administrateur de références|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gérer l’appartenance au MPN et votre société (rôles non AAD : ces rôles de gérer l’activité de l’entreprise plutôt que le client)

|**Role** | **Ce que vous pouvez faire**|
|----------------------------|:----------------------------|
|Administrateur partenaire MPN|• Afficher, créer et gérer des demandes de service de partenaire||
||• Vue juridique, entreprise, entreprise et les profils MPN
||• Afficher les détails utilisateur et leurs données de compétences
||• Afficher les compétences
||• Afficher et gérer les avantages
||Achat et • vue Microsoft Partner Network
||• Affichage MPN offre des factures et l’historique des commandes
||• Affichage partenaire contribution indicateur des données
||• Peuvent fonctionner dans l’outil de Validation de document|
||-Afficher l’analytique des données client
|| Afficher d’autres rôles d’utilisateur au sein de l’entreprise, mais ne peut pas attribuer des rôles
|Administration de compte| Ajouter des emplacements
|| Gérer les profils associés aux comptes que vous êtes administrateur de 
||• Attribuer des rôles pour les utilisateurs du client de rôles non AAD 
||• Inscrire les emplacements dans des programmes


## <a name="manage-referrals"></a>Gérer les références 

|**Role**|**Ce que vous pouvez faire**|
|-----------------------------|:------------------------|
|Administrateur de références       |• Afficher, créer et gérer des profils d’entreprise
||• Recevoir et gérer les références
||• Afficher, créer et gérer les redirections de vente conjointe|
||• Afficher, créer et gérer des demandes de service de partenaire
|Administrateur de profil d'entreprise   |• Afficher, créer et gérer le profil d’entreprise 
||• Afficher, créer et gérer des demandes de service de partenaire|

## <a name="manage-incentives"></a>Gérer les primes 

|**Role** | **Ce que vous pouvez faire**|
|------------------------------|:-------------------------|
|Administrateur de primes incitatives|• Lance et gère les primes 
||• Peuvent afficher et modifier tous les aspects des programmes de primes
||• Peuvent afficher et modifier les informations fiscales et bancaires
||• Affichage rebate et co-op bénéfices
||• Accès prise en charge
||Paiements de primes litige •|
|Utilisateur de primes incitatives|• Peuvent afficher les programmes de primes
||• Peuvent afficher et lancer des revendications de primes
||• Affichage rebate et co-op bénéfices
||• Accès prise en charge












