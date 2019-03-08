---
title: Créer des comptes d’utilisateur et définir des autorisations (Partner Center géré par 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Comment créer des comptes d’utilisateur pour les employés qui ont besoin d’accéder à des partenaires.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: a96c7fedacbb177c93ae19c5ff4f1a241905be4b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584442"
---
# <a name="create-user-accounts-and-set-permissions"></a>Créer des comptes d’utilisateurs et définir des autorisations


**S’applique à**

-   Espace partenaires géré par 21Vianet


Créer des comptes d’utilisateur pour vos employés ont besoin pour effectuer des tâches sur les partenaires. Global uniquement ou administrateurs de gestion d’utilisateur peuvent ajouter des utilisateurs et attribuer des rôles. Dans **comptable** &gt; **gestion des utilisateurs**, vous pouvez ajouter des comptes d’utilisateur et affecter ou modifier les autorisations.

**Ajouter un nouvel utilisateur**

1.  Dans le centre de partenaires, accédez au menu Tableau de bord &gt; **paramètres du compte** &gt; **gestion des utilisateurs**.

2.  Sélectionnez **Ajouter un utilisateur**.

3.  Tapez le nom complet et l’adresse de messagerie unique de l’utilisateur.

4.  Sélectionnez le rôle et le niveau d’accès de l’employé. Autorisations et l’accès des partenaires sont basées sur des rôles, ce qui vous permet de contrôler les tâches spécifiques que chaque employé peut effectuer. Pour plus d’informations sur le rôle de chaque rôle, consultez [définir les autorisations utilisateur](#setuserpermissions).

5.  Sélectionnez **Ajouter** pour créer le compte d’utilisateur. La page de confirmation apparaît, affichant les autorisations et les informations de connexion, y compris un mot de passe temporaire du nouvel utilisateur.

    >**Important**<br>Lorsque de nouveaux utilisateurs se connecter à des partenaires pour la première fois, il doivent se connecter avec leur mot de passe temporaire. Veillez à noter de mot de passe temporaire du nouvel utilisateur afin de pouvoir l’envoyer plus tard. Il se peut que vous ne pourrez pas accéder à ces informations à nouveau. 

### <a href="" id="setuserpermissions"></a>Définir des autorisations utilisateur

Accès des partenaires est en fonction du rôle, ce qui signifie que vous pouvez restreindre l’affichage de l’utilisateur pour afficher uniquement les fonctionnalités et fonctions dont un utilisateur a besoin pour effectuer des tâches spécifiques. Pour chaque utilisateur, vous devez sélectionner deux paramètres :

-   Le **agent** paramètre détermine le type de données client et société de l’utilisateur peut voir.

-   Le **administrateur** paramètre détermine le degré d’accès l’utilisateur dispose de fonctionnalités de partenaires, les fonctions et les données. 

    >**Remarque**<br>Le paramètre par défaut doit être **aucun administrateur** dans la plupart des cas, sauf si l’employé a besoin d’autorisations pour effectuer des tâches administratives spécifiques.

####<a name="partner-center-roles-and-associated-permissions"></a>Rôles de partenaires et les autorisations associées

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rôle dans l’espace partenaires</strong></p></td>
<td><p><strong>Marche à suivre</strong></p></td>
<td><p><strong>Ce qu’ils ne peuvent pas faire</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agent d’administration</strong></p></td>
<td><ul>
<li><p>Gestion des clients</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>Intégrité de service d’accès pour les clients</p></li>
<li><p>Demander des privilèges d’administrateur délégués</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Afficher et télécharger les factures et les fichiers de réconciliation</p></li>
<li><p>Administrer au nom d’un client</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
<td><ul>
<li><p>Gestion des utilisateurs</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agent commercial</strong></p></td>
<td><ul>
<li><p>Gestion des clients</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>Demander une relation de revendeur avec un client</p></li>
<li><p>Afficher le contrat client</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
<td><ul>
<li><p>Créer des demandes de support avec 21Vianet pour les problèmes avec les services ou les partenaires</p></li>
<li><p>Afficher l’état du service</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Afficher et télécharger les factures et les fichiers de réconciliation</p></li>
<li><p>Administrer au nom d’un client</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agent de support technique</strong></p></td>
<td><ul>
<li><p>Rechercher des clients et d’afficher les détails de client</p></li>
<li><p>Modifier les détails du client</p></li>
<li><p>Intégrité de service d’accès pour les clients</p></li>
<li><p>Administrer au nom d’un client</p></li>
</ul></td>
<td><ul>
<li><p>Afficher les profils de partenaire</p></li>
<li><p>Créer un compte client</p></li>
<li><p>Modifier les informations de facturation client</p></li>
<li><p>Gestion des abonnements</p></li>
<li><p>Demander une relation de revendeur avec un client</p></li>
<li><p>Afficher les tarifs et les offres</p></li>
<li><p>Afficher le contrat client</p></li>
<li><p>Afficher et télécharger les factures et les fichiers de réconciliation</p></li>
<li><p>Inscrire un revendeur à valeur ajoutée</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur général</strong></p></td>
<td><ul>
<li><p>Peut accéder à tous les comptes et les services avec privilèges complets</p></li>
<li><p>Créer des demandes de support avec 21Vianet pour les problèmes de partenaires</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
<li><p>Afficher et télécharger les factures et les fichiers de réconciliation</p></li>
<li><p>Afficher, créer et gérer les utilisateurs de votre entreprise</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrateur de facturation</strong></p></td>
<td><ul>
<li><p>Peut accéder à toutes les factures et les fichiers de rapprochement avec privilèges complets</p></li>
<li><p>Afficher les contrats, les listes de prix et les offres</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrateur de gestion des utilisateurs</strong></p></td>
<td><ul>
<li><p>Afficher, créer et gérer les utilisateurs de votre entreprise</p></li>
<li><p>Afficher tous les profils de partenaire</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

