---
title: Attribuer des rôles et des autorisations aux utilisateurs | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Tous les employés doivent fonctionner dans l’espace partenaires doivent avoir un rôle.
author: LauraBrenner
ms.author: labrenne
keywords: rôles, autorisations, administration, agent
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587742"
---
# <a name="assign-users-roles-and-permissions"></a>Affecter des rôles et des autorisations aux utilisateurs


Vous avez configuré votre profil de partenaire, y compris juridique nom et adresse, les détails de prise en charge, exonérations de fichier, les informations bancaires et le contact principal de votre entreprise. Étape suivante : configurer des mots de passe et des rôles, afin qu’ils peuvent commencer à travailler dans des partenaires avec vous de vos utilisateurs.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurer vos employés à travailler dans l’espace partenaires

Vous déterminez les types d’accès à que vos utilisateurs disposent de partenaires par les rôles et autorisations que vous leur donnez. Rôles associés à votre entreprise est impliqué dans l’ou les programmes. Par exemple, si votre entreprise est une entreprise de fournisseur de solutions Cloud (CSP), pas uniquement avoir l’Azure AD standard des rôles de gestion telles qu’Administrateur général du client, mais devez rôles spécifiques au programme CSP. Chaque programme possède des rôles spécifiques à celui-ci.

>[!Note]
> Rôles de locataire Azure Active Directory (AAD) incluent l’administrateur général, administrateur d’utilisateurs et rôles CSP. Rôles non-AAD incluent MPN admin, administrateur de profil d’entreprise, référence administrateur, administrateur offre incitative et offre incitative utilisateur. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gérer les transactions commerciales dans partenaires (Azure AD et les rôles CSP)

|**Role**|**Marche à suivre**|
|----------------------------------|:---------------------------------|
|Administrateur global|• Peuvent accéder à tous les comptes/services Microsoft avec privilèges complets
|      |• Créer des tickets de support pour l’espace partenaires
||• Afficher les contrats, des listes de prix et des offres
||• Afficher, créer et gérer des utilisateurs partenaires|
|Utilisateur Admin   | • Afficher, créer et gérer les utilisateurs
||• Afficher tous les profils de partenaires
||• Afficher, créer et gérer des utilisateurs partenaires  |
|Utilisateur par défaut|  Afficher mon profil   |
|Agent d’administration | • Gestion de client
||• Ajoutez la liste des appareils à l’espace partenaires <
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
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fournisseur de panneau de contrôle (CPV). (Rôle de fournisseur de services cryptographiques et rôle de non-AAD)
CPVs développer des applications pour une utilisation par les partenaires de fournisseur de solutions Cloud (CSP) pour leur permettre d’intégrer leurs systèmes avec les API Partner Center. 

|**Role**   |**Ce que vous pouvez faire**|
|------------------------------|:----------------------------|
|Administrateur global| Afficher et gérer votre profil CPV|
||Afficher et gérer des utilisateurs qui ont besoin d’accéder aux fonctionnalités CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Gérer l’appartenance au MPN et votre entreprise (rôles non AAD)

|**Role** | **Ce que vous pouvez faire**|
|----------------------------|:----------------------------|
|Administrateur partenaire MPN|•CAN ajouter les utilisateurs non client
||• Afficher, créer et gérer des demandes de service de partenaire
||• Vue juridique, organisation, entreprise et les profils MPN
||• Afficher les détails utilisateur et leurs données de compétences
||• Afficher les compétences
||• Afficher et gérer les avantages
||Achat et • vue Microsoft Partner Network
||• Affichage MPN offre des factures et l’historique des commandes
||• Afficher les données contribution partenaire
||• Peuvent fonctionner dans l’outil de Validation de document|
||-Afficher l’analytique des données client
|Administration de compte| • Peuvent ajouter des utilisateurs de non-client
||• Ajouter ou supprimer des emplacements
||-Gérer les profils associés aux comptes que vous êtes administrateur de 
||• Attribuer des rôles pour les utilisateurs du client de rôles non AAD 
||• Inscrire les emplacements dans des programmes

## <a name="manage-referrals-non-aad-roles"></a>Gérer les références (rôles non AAD)

|**Role**|**Ce que vous pouvez faire**|
|-----------------------------|:------------------------|
|Administrateur de références       |• Afficher, créer et gérer des profils d’entreprise
||• Recevoir et gérer les références
||• Afficher, créer et gérer des demandes de service de partenaire|
|Administrateur de profil d'entreprise   |•Afficher, créer et gérer le profil d’entreprise 
||• Afficher, créer et gérer des demandes de service de partenaire|

## <a name="manage-incentives--non-aad-roles"></a>Gérer des incitations (rôles non AAD)

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
||• Affichage rebate et co-op bénéfices
||• Accès prise en charge












