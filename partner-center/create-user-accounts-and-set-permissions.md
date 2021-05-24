---
title: Créer des comptes d’utilisateur et attribuer des rôles
description: Un rôle doit être attribué à chaque employé pour lui permettre d’accéder à l’Espace partenaires. Découvrez comment créer des comptes d’utilisateur, attribuer des rôles et définir des autorisations.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148140"
---
# <a name="create-user-accounts"></a>Créer des comptes d'utilisateur  

**Rôles appropriés** : Administrateur de compte | Administrateur général | Administrateur de la gestion des utilisateurs

Créez des comptes d’utilisateur pour les employés qui doivent accéder à l’Espace partenaires. Ces tâches doivent être effectuées par l’administrateur de la gestion des utilisateurs, l’administrateur des comptes ou l’administrateur général. L’utilisateur qui effectue ces tâches doit aussi se voir attribuer les rôles Administrateur d’utilisateurs ou Administrateur général d’Azure Active Directory (AAD). Pour plus d’informations sur les rôles d’AAD, consultez [Autorisations des rôles d’administrateur dans Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Ajouter un nouvel utilisateur

1. À partir de l’icône **Paramètres** en haut à droite de l’Espace partenaires, sélectionnez **Paramètres de compte**, puis **Gestion des utilisateurs**.

2. Sélectionnez **Ajouter un utilisateur**.

3. Entrez le nom complet et l’adresse e-mail unique de l’utilisateur.

4. Sélectionnez le type d’agent et/ou le type d’administrateur que vous souhaitez attribuer à l’utilisateur. Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques.  Si des utilisateurs souhaitent se voir attribuer un rôle, ils peuvent trouver des administrateurs généraux à contacter en accédant à **Gestion des utilisateurs** et en filtrant sur Administrateur général.

5. Sélectionnez **Ajouter** pour créer le compte d’utilisateur. Confirmez les détails de l’utilisateur sur la page suivante.

> [!IMPORTANT]  
> Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page. Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement. 

L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire. Lorsque l’utilisateur se connecte à l’Espace partenaires pour la première fois, il est invité à modifier son mot de passe.

## <a name="assign-user-roles"></a>Attribuer des rôles d’utilisateur

Pour travailler dans l’Espace partenaires, un rôle doit vous être attribué.  Vous avez actuellement le choix entre des rôles de locataire Azure Active Directory, des rôles Fournisseur de solutions Cloud (CSP) et des rôles d’entreprise non-AAD. Une entreprise individuelle peut avoir besoin de tous ces rôles.

>[!Important]
>Les individus doivent être listés dans votre locataire pour pouvoir accéder à l’Espace partenaires. Les attributions de rôles fournissent un accès supplémentaire.

## <a name="next-steps"></a>Étapes suivantes

- [Attribuer des rôles et des autorisations aux collaborateurs qui ont besoin de travailler dans l’Espace partenaires](permissions-overview.md)
