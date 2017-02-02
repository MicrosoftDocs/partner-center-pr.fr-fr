---
title: "Créer des comptes d’utilisateur et définir des autorisations | Espace partenaires"
description: "L’administrateur crée un compte d’utilisateur pour chaque employé du partenaire devant accéder à l’Espace partenaires."
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: e1825890f208a90b9b5694f4000ac06687ac87ab
ms.openlocfilehash: a755c9375c7bd5e61345d7d7e1ab27e00af3fe4d

---

# Créer des comptes d’utilisateurs et définir des autorisations

**S'applique à**

-  Espace partenaires

L’administrateur crée un compte d’utilisateur pour chaque employé du partenaire devant accéder à l’Espace partenaires. Ces tâches doivent être effectuées par un administrateur disposant de l’autorisation **Administrateur global** ou **Administrateur de la gestion des utilisateurs**. Dans **Paramètres du compte** &gt; **Gestion des utilisateurs**, vous pouvez ajouter des comptes et définir ou mettre à jour les autorisations.

**Ajouter un utilisateur**

1.  Dans l’Espace partenaires, accédez au menu Tableau de bord &gt; **Paramètres du compte** &gt; **Gestion des utilisateurs**.
2.  Choisissez **Ajouter un utilisateur**.

3.  Tapez le nom complet de l’utilisateur et créez-lui une adresse électronique unique.

4.  Sélectionnez le type d’agent et le type d’administrateur. L’accès à l'Espace partenaires dépendant des rôles, les sélections effectuées à cette étape personnalisent l’affichage en n'incluant que les fonctionnalités nécessaires. Pour plus d’informations sur les actions de chaque rôle, voir la section [Définir les autorisations utilisateur](#setuserpermissions)

5.  Ajoutez l’utilisateur. Vous verrez un écran de confirmation avec un mot de passe temporaire pour la nouvelle connexion. Vous devez le copier et l’envoyer au nouvel utilisateur. Il n’est plus accessible une fois que vous quittez l’écran. Lors de sa première connexion, l’utilisateur devra mettre à jour le mot de passe.

### <a href="" id="setuserpermissions"></a>Définir les autorisations de l’utilisateur

Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez personnaliser l’affichage afin de n'inclure que les fonctionnalités nécessaires à l’utilisateur dans le cadre de son travail. Pour chaque utilisateur, vous devez sélectionner deux paramètres :

-   Le paramètre **agent** détermine le type de données clients et le type d’informations Microsoft que l’utilisateur peut voir.

-   Le paramètre **admin** détermine le contrôle de l’utilisateur sur l’environnement de l’Espace partenaires et sur tous les autres services Microsoft (comptes, profils et tickets de support). Ce paramètre a un impact en dehors de l’Espace partenaires : un administrateur de facturation peut accéder à toutes les factures pour tous les services Microsoft (même ceux non liés au fournisseur de solutions Cloud) et un administrateur global peut accéder aux comptes d’utilisateurs et aux comptes clients, indépendamment du fournisseur de solutions Cloud.

    Le paramètre par défaut doit toujours être **Pas un administrateur**, sauf si le rôle de l’utilisateur requiert un accès supplémentaire pour effectuer des tâches et prendre en charge des clients.

Le tableau suivant détaille l’ensemble complet des activités que chaque rôle peut effectuer dans l’Espace partenaires.

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
<li><p>Gestion des abonnements</p></li>
<li><p>État du service et demandes de service pour les clients</p></li>
<li><p>Demander des privilèges d’administrateur délégués</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Administrateur pour le compte de</p></li>
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
<li><p>Gestion des abonnements</p></li>
<li><p>Afficher les tickets de support</p></li>
<li><p>Demander une relation</p></li>
<li><p>Gérer les prospects</p></li>
<li><p>Afficher le contrat client</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
<td><ul>
<li><p>Créer des tickets de support pour les services ou l’Espace partenaires</p></li>
<li><p>Résoudre les tickets de support</p></li>
<li><p>Afficher l’état du service</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Facturation</p></li>
<li><p>Administrateur pour le compte de</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agent du support technique</strong></p></td>
<td><ul>
<li><p>Rechercher et afficher un client</p></li>
<li><p>Modifier les détails du client</p></li>
<li><p>Intégrité du service</p></li>
<li><p>Créer des tickets de support pour les clients</p></li>
<li><p>Administrer les services au nom des clients</p></li>
</ul></td>
<td><ul>
<li><p>Afficher les profils de partenaire</p></li>
<li><p>Créer une liste de clients</p></li>
<li><p>Modifier les informations de facturation du client</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>Demander une relation</p></li>
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
</tbody>
</table>

 

 

 






<!--HONumber=Jan17_HO2-->


