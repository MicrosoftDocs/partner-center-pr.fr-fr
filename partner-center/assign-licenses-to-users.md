---
title: Gérer les utilisateurs pour les comptes client
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gérer les utilisateurs pour vos clients dans l’espace partenaires : créer des comptes d’utilisateur, ajouter ou supprimer des licences utilisateur, réinitialiser les mots de passe et supprimer ou restaurer des comptes d’utilisateur.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756078"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gérer les utilisateurs et les licences utilisateur pour les comptes client 

**Rôles appropriés**

- Administrateur général
- Administrateur de la gestion des utilisateurs
- Agent d’administration


Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client. Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression. Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).

Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.  

>[!NOTE]
>La section **utilisateurs et licences** de l’onglet **client** affiche tous les utilisateurs créés dans le locataire d’un client spécifique, y compris les utilisateurs disposant de licences achetées auprès d’un autre partenaire CSP ou d’un autre canal d’achat.

Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Créer des comptes d’utilisateur pour un client

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Dans le menu client, sélectionnez **Utilisateurs et licences**.

4. Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences. **Enregistrez** les changements apportés.

5. Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.

6. Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.

7. Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md). Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Ajouter ou supprimer des licences d’utilisateur pour un client

Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft. Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Dans le menu client, sélectionnez **Utilisateurs et licences**.

4. Choisissez un ou plusieurs utilisateurs dans la liste. Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les attribuer à des personnes qui en sont encore dépourvues, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour rechercher le groupe approprié.

5. Sélectionnez **Gérer les licences**. Apportez vos modifications, puis sélectionnez **Enregistrer**.

> [!NOTE]
> Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Réinitialiser le mot de passe d’un utilisateur pour un client

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Dans le menu client, sélectionnez **Utilisateurs et licences**. Sélectionnez l’utilisateur dans la liste.

4. En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**. 

5. Envoyez le nouveau mot de passe temporaire à l’utilisateur.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Supprimer les comptes d’utilisateur d’un client

1. Dans le menu **espace partenaires** , sélectionnez **clients**. Sélectionnez le client dans la liste.

2. Dans le menu client, sélectionnez **Utilisateurs et licences**. Sélectionnez l’utilisateur dans la liste.

3. Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.

Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client. Vous avez 30 jours pour restaurer un utilisateur supprimé.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurer des comptes d’utilisateur supprimés

1. Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.

2. Sélectionnez **utilisateurs et licences**.

3. Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.

4. Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.

    Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.

## <a name="next-steps"></a>Étapes suivantes

- [Attribuer ou révoquer des licences pour plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md)

- [Créer plusieurs utilisateurs pour un compte client](adding-multiple-users-to-a-customer-account.md)