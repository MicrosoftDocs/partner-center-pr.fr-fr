---
title: "Créer des comptes d’utilisateur et définir des autorisations | Espace partenaires"
description: "L’administrateur crée un compte d’utilisateur pour chaque employé du partenaire devant accéder à l’Espace partenaires."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: bc699214c7919c7cff9788144d472063ba60ad10
ms.sourcegitcommit: 4a1cd51e5986f47badcde9412a7c7b22718500f0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Créer des comptes d’utilisateur et attribuer des autorisations

**S'applique à**

-  Espace partenaires

Créer des comptes d’utilisateur pour les employés qui doivent accéder à l'Espace partenaires. Ces tâches doivent être effectuées par un administrateur disposant de l’autorisation Administrateur de la gestion des utilisateurs. 

## <a name="add-a-new-user"></a>Ajouter un utilisateur

1. Dans le menu **Tableau de bord**, sélectionnez **Paramètres du compte > Gestion des utilisateurs**.

2.  Sélectionnez **Ajouter un utilisateur**.

3.  Entrez le nom complet et l’adresse de messagerie unique de l’utilisateur.

4.  Sélectionnez le type d’agent et le type d’administrateur. Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques. Pour plus d’informations sur ce que chaque rôle peut faire, voir la section [Affecter des autorisations utilisateur](#assignuserpermissions)

5.  Sélectionnez **Ajouter** pour créer le compte d’utilisateur. Confirmez les détails de l’utilisateur sur la page suivante.

>**Important**<br>
Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page. Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement. <br>

>L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire. Lorsque l’utilisateur se connecte à l'Espace partenaires pour la première fois, il est invité à modifier son mot de passe.    


### <a href="" id="assignuserpermissions"></a>Affecter des autorisations utilisateur

Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques. 

Pour chaque utilisateur, vous devez sélectionner deux niveaux d'autorisation:

-   Les autorisations d'agent contrôlent le type de données de client et d'informations de compte que l’utilisateur peut voir et modifier.

-   Les autorisations d’administrateur contrôlent le niveau d’accès de l’utilisateur aux fonctionnalités de l'Espace partenaires. Ce paramètre a un impact en dehors de l’Espace partenaires : un administrateur de facturation peut accéder aux factures pour tous les services Microsoft (même ceux non liés au fournisseur de solutions Cloud) et un administrateur global peut accéder aux comptes d’utilisateurs et aux comptes clients, indépendamment du fournisseur de solutions Cloud.

##<a name="assign-permissions-for-incentives-users"></a>Affecter des autorisations aux utilisateurs de primes incitatives
Lorsque vous configurez les utilisateurs de primes incitatives, vous pouvez leur attribuer le rôle d’administrateur ou d’utilisateur de primes incitatives.  Le rôle d’administrateur de primes incitatives permet de modifier les informations bancaires et fiscales, d’effectuer des demandes de paiement auprès de Microsoft, ainsi que de gérer les utilisateurs de primes incitatives. Le rôle d’utilisateur de primes incitatives permet de passer en revue les informations relatives aux programmes, ainsi que les informations bancaires et fiscales, sans toutefois pouvoir les modifier. Les utilisateurs dotés de ce rôle fournissent souvent les programmes de primes proprement dits aux clients. Les administrateurs et utilisateurs de primes incitatives peuvent avoir d’autres rôles pour votre entreprise dans l’Espace partenaires, mais pour travailler sur les programmes de primes incitatives, un utilisateur doit avoir le rôle d’administrateur ou d’utilisateur de primes incitatives.

>**Important** Le paramètre par défaut doit toujours être **Pas un administrateur**, sauf si le rôle de l’utilisateur requiert un accès supplémentaire pour effectuer des tâches et prendre en charge des clients.

Le tableau suivant explique ce que chaque rôle peut faire dans l'Espace partenaires.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rôle dans l’Espace Partenaires</strong></p></td>
<td><p><strong>Ce qu’il peut faire</strong></p></td>
<td><p><strong>Ce qu’il ne peut pas faire</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agent d’administration</strong></p></td>
<td><ul>
<li><p>Gestion des clients</p></li>
<li><p>Ajouter une liste d'appareils à l'Espace partenaires</p></li>
<p><li>Créer des profils et les appliquer aux appareils</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>État du service et demandes de service pour les clients</p></li>
<li><p>Demander des privilèges d’administrateur délégués</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Administrer au nom d’un client</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
<td><ul>
<li><p>Gestion des utilisateurs</p></li>
<li><p>Demandes de service pour l’Espace partenaires</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Commercial</strong></p></td>
<td><ul>
<li><p>Gestion des clients</p></li>
<li><p>Ajouter une liste d'appareils à l'Espace partenaires</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>Afficher les tickets de support</p></li>
<li><p>Demander une relation avec un client</p></li>
<li><p>Gérer les prospects</p></li>
<li><p>Afficher le contrat client</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
<td><ul>
<li><p>Créer des demandes de service pour des problèmes avec l'Espace partenaires</p></li>
<li><p>Résoudre les tickets de support</p></li>
<li><p>Afficher l’état du service</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Administrer au nom d’un client</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agent du support technique</strong></p></td>
<td><ul>
<li><p>Rechercher et afficher un client</p></li>
<li><p>Modifier les détails du client</p></li>
<li><p>Intégrité du service</p></li>
<li><p>Demander un support pour le compte de clients (remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office365)</p></li>
<li><p>Gérer les abonnements et les services pour le compte de clients (remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office365)</p></li>
</ul></td>
<td><ul>
<li><p>Afficher les profils de partenaire</p></li>
<li><p>Créer un compte client</p></li>
<li><p>Modifier les informations de facturation du client</p></li>
<li><p>Gérer les abonnements</p></li>
<li><p>Demander une relation avec un client</p></li>
<li><p>Gérer les prospects</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Afficher le contrat client</p></li>
<li><p>Facturation</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur global</strong></p></td>
<td><ul>
<li><p>Peut accéder à tous les comptes/services Microsoft avec des privilèges complets</p></li>
<li><p>Créer des tickets de support pour l’Espace partenaires</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Afficher, créer et gérer les utilisateurs partenaires</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administration de facturation</strong></p></td>
<td><ul>
<li><p>Peut accéder à toutes les factures émises par Microsoft avec des privilèges complets</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
<li><p>Facturation</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur de la gestion des utilisateurs</strong></p></td>
<td><ul>
<li><p>Afficher, créer et gérer des utilisateurs</p></li>
<li><p>Afficher tous les profils de partenaire</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrateur de primes incitatives</strong></p></td>
<td><ul>
<li><p>Afficher et gérer tous les programmes de primes incitatives</p></li>
<li><p>Modifier les profils bancaires et fiscaux pour les programmes de primes incitatives</p></li>
<LI><p>Gérer les utilisateurs de primes incitatives</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Utilisateur de primes incitatives</strong></p></td>
<td><ul>
<li><p>Afficher les programmes de primes incitatives</p></li>
<li><p>Afficher les profils bancaires et fiscaux</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



