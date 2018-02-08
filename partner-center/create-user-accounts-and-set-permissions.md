---
title: "Créer des comptes d’utilisateur et définir des autorisations | Espace partenaires"
description: "L’administrateur crée un compte d’utilisateur pour chaque employé du partenaire devant accéder à l’Espace partenaires."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
Keywords: roles, permissions,add user, assign role, admin, agent,
ms.openlocfilehash: 809641e488595e59beb63b0867b4758f3912106e
ms.sourcegitcommit: fc49a5e334ed37db4ff4c594ecf89a1527a3bd1d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2018
---
# <a name="create-user-accounts-and-assign-permissions"></a>Créer des comptes d’utilisateur et attribuer des autorisations

**S'applique à**

-  Espace partenaires

Créer des comptes d’utilisateur pour les employés qui doivent accéder à l'Espace partenaires. Ces tâches doivent être effectuées par un administrateur disposant de l’autorisation Administrateur de la gestion des utilisateurs. 

>**Remarque**<br> Vous avez désormais la possibilité d’attribuer aux utilisateurs de l'Espace partenaires trois nouveaux rôles qui vous aideront à gérer votre entreprise: Administrateur MPN, Administrateur de profil d'entreprise et Administrateur des références. Consultez la section Attribuer des autorisations aux utilisateurs ci-dessous pour connaître les détails de chaque rôle.


## <a name="add-a-new-user"></a>Ajouter un utilisateur

1. Dans le menu **Tableau de bord**, sélectionnez **Paramètres du compte > Gestion des utilisateurs**.

2.  Sélectionnez **Ajouter un utilisateur**.

3.  Saisissez le nom complet et l’adresse de messagerie unique de l’utilisateur.

4.  Sélectionnez le type d’agent et/ou le type d’administrateur que vous souhaitez attribuer à l’utilisateur. Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques. Pour en savoir plus sur les actions possibles pour chaque rôle, voir la section Attribuer des autorisations utilisateur, ci-dessous.

5.  Sélectionnez **Ajouter** pour créer le compte d’utilisateur. Confirmez les détails de l’utilisateur sur la page suivante.

>**Important**<br>
Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page. Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement. 

L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire. Lorsque l’utilisateur se connecte à l'Espace partenaires pour la première fois, il est invité à modifier son mot de passe. 

>**Remarque**<br> Si votre administrateur général a quitté votre organisation ou a été affecté à un autre rôle, et que vous devez ajouter un nouvel administrateur général, vous devez consigner une demande de service sur le [portail MPN](https://partner.microsoft.com/support). L’agent du support peut demander l’élévation d’un utilisateur au rôle d’administrateur général si votre demandeur est en mesure de fournir les informations d’identité personnelle nécessaires ainsi que des informations supplémentaires sur votre organisation.

## <a name="assign-user-permissions"></a>Attribuer des autorisations aux utilisateurs

L'accès à l'Espace partenaires est basé sur les rôles. Les autorisations attribuées à l'utilisateur personnalisent la vue accessible afin d'afficher uniquement les fonctionnalités dont l’utilisateur a besoin pour effectuer ses tâches spécifiques. 

Vous devez attribuer au moins un niveau d’autorisation à chaque utilisateur. L'un de ces niveaux peut être le niveau par défaut, c'est-à-dire **Manages your organization's account as**. Si vous n’affectez pas de rôle à un utilisateur, il ne pourra pas travailler dans l’Espace partenaires.

-   Les autorisations d'agent contrôlent le type de données client et d’informations de compte que l’utilisateur peut voir et modifier.

-   Les autorisations d’administrateur contrôlent le niveau d’accès de l’utilisateur aux fonctionnalités de l'Espace partenaires. Ce paramètre a un impact en dehors de l’Espace partenaires : un administrateur de facturation peut accéder aux factures pour tous les services Microsoft (même ceux non liés au fournisseur de solutions Cloud) et un administrateur global peut accéder aux comptes d’utilisateurs et aux comptes clients, indépendamment du fournisseur de solutions Cloud.

Les catégories générales des rôles sont: 

- Rôles d’administrateur
- Rôles d’agent
- Rôles pour primes incitatives
- Rôles pour les références et le marketing

Dans chacune de ces catégories générales, un utilisateur ne peut avoir qu'un seul rôle, mais il peut avoir également des rôles dans les autres catégories générales. 

>**Important** Si un utilisateur n’a pas besoin de rôle spécifique, laissez la désignation sur le paramètre par défaut: **Manages your organization's account as**. Les utilisateurs doivent disposer d’au moins un rôle pour travailler dans l’Espace partenaires.

Le tableau suivant explique ce que chaque rôle peut faire dans l’Espace partenaires. Lorsque vous réfléchissez à l'attribution des rôles, prenez en compte le travail qu'un utilisateur effectue dans votre organisation. Vous pouvez, par exemple, attribuer également à l’administrateur général le rôle d’agent d’administration. La personne responsable du marketing peut également être chargée de gérer le profil de l’entreprise.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rôle dans l’Espace partenaires</strong></p></td>
<td><p><strong>Ce qu’il peut faire</strong></p></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur général</strong></p></td>
<td><ul>
<li><p>Peut accéder à tous les comptes/services Microsoft avec des privilèges complets</p></li>
<li><p>Créer des tickets de support pour l’Espace partenaires</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Afficher, créer et gérer les utilisateurs partenaires</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administration de facturation</strong></p></td>
<td><ul>
<li><p>Peut accéder à toutes les factures émises par Microsoft avec des privilèges complets</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
<li><p>Facturation</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur de la gestion des utilisateurs</strong></p></td>
<td><ul>
<li><p>Afficher, créer et gérer des utilisateurs</p></li>
<li><p>Afficher tous les profils de partenaire</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrateur de profil d'entreprise</strong></p></td>
<td><ul>
<li><p>Affiche, crée et gère le profil de l'entreprise </p></li>
<li><p>Afficher, créer et gérer les demandes de service des partenaires</p></li>
</ul></td>
<tr class="odd">
<td><p><strong>Administrateur des références </strong></p></td>
<td><ul>
<li><p>Afficher, créer et gérer les profils commerciaux</p></li>
<li><p>Recevoir et gérer les références</p></li>
<li><p>Afficher, créer et gérer les demandes de service des partenaires</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Administrateur partenaire MPN</strong></p></td>
<td><ul>
<li><p>Afficher, créer et gérer les demandes de service des partenaires</p></li>
<li><p>Afficher les profils juridiques, d'entreprise, commerciaux et MPN</p></li>
<li><p>Afficher les détails des utilisateurs et les données sur leurs compétences</p></li>
<li><p>Afficher les compétences</p></li>
<li><p>Afficher et gérer les revenus</p></li>
<li><p>Afficher et acheter les offres MPN</p></li>
<li><p>Afficher les factures et l’historique des commandes des offres MPN</p></li>
</ul></td>
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
</tr>
<tr class="even">
<td><p><strong>Agent du support technique</strong></p></td>
<td><ul>
<li><p>Rechercher et afficher un client</p></li>
<li><p>Modifier les détails du client</p></li>
<li><p>Aider les clients à résoudre des problèmes de gestion de facturation ou d’abonnement</p></li>
<li><p>Demander un support pour le compte de clients (remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office365)</p></li>
<li><p>Gérer les problèmes d'abonnements et de facturation pour le compte de clients (remarque: vous devez être un agent administrateur pour effectuer cette tâche pour les abonnements Office365)</p></li>
</ul></td>
</tr>
 

 

 



