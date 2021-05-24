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
# <a name="create-user-accounts"></a><span data-ttu-id="6e481-104">Créer des comptes d'utilisateur</span><span class="sxs-lookup"><span data-stu-id="6e481-104">Create user accounts</span></span>  

<span data-ttu-id="6e481-105">**Rôles appropriés** : Administrateur de compte | Administrateur général | Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="6e481-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="6e481-106">Créez des comptes d’utilisateur pour les employés qui doivent accéder à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6e481-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="6e481-107">Ces tâches doivent être effectuées par l’administrateur de la gestion des utilisateurs, l’administrateur des comptes ou l’administrateur général. L’utilisateur qui effectue ces tâches doit aussi se voir attribuer les rôles Administrateur d’utilisateurs ou Administrateur général d’Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="6e481-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="6e481-108">Pour plus d’informations sur les rôles d’AAD, consultez [Autorisations des rôles d’administrateur dans Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="6e481-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="6e481-109">Ajouter un nouvel utilisateur</span><span class="sxs-lookup"><span data-stu-id="6e481-109">Add a new user</span></span>

1. <span data-ttu-id="6e481-110">À partir de l’icône **Paramètres** en haut à droite de l’Espace partenaires, sélectionnez **Paramètres de compte**, puis **Gestion des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="6e481-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="6e481-111">Sélectionnez **Ajouter un utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="6e481-111">Select **Add user**.</span></span>

3. <span data-ttu-id="6e481-112">Entrez le nom complet et l’adresse e-mail unique de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6e481-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="6e481-113">Sélectionnez le type d’agent et/ou le type d’administrateur que vous souhaitez attribuer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6e481-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="6e481-114">Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques.</span><span class="sxs-lookup"><span data-stu-id="6e481-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="6e481-115">Si des utilisateurs souhaitent se voir attribuer un rôle, ils peuvent trouver des administrateurs généraux à contacter en accédant à **Gestion des utilisateurs** et en filtrant sur Administrateur général.</span><span class="sxs-lookup"><span data-stu-id="6e481-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="6e481-116">Sélectionnez **Ajouter** pour créer le compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6e481-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="6e481-117">Confirmez les détails de l’utilisateur sur la page suivante.</span><span class="sxs-lookup"><span data-stu-id="6e481-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="6e481-118">Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page.</span><span class="sxs-lookup"><span data-stu-id="6e481-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="6e481-119">Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="6e481-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="6e481-120">L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire.</span><span class="sxs-lookup"><span data-stu-id="6e481-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="6e481-121">Lorsque l’utilisateur se connecte à l’Espace partenaires pour la première fois, il est invité à modifier son mot de passe.</span><span class="sxs-lookup"><span data-stu-id="6e481-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="6e481-122">Attribuer des rôles d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="6e481-122">Assign user roles</span></span>

<span data-ttu-id="6e481-123">Pour travailler dans l’Espace partenaires, un rôle doit vous être attribué.</span><span class="sxs-lookup"><span data-stu-id="6e481-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="6e481-124">Vous avez actuellement le choix entre des rôles de locataire Azure Active Directory, des rôles Fournisseur de solutions Cloud (CSP) et des rôles d’entreprise non-AAD.</span><span class="sxs-lookup"><span data-stu-id="6e481-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="6e481-125">Une entreprise individuelle peut avoir besoin de tous ces rôles.</span><span class="sxs-lookup"><span data-stu-id="6e481-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="6e481-126">Les individus doivent être listés dans votre locataire pour pouvoir accéder à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6e481-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="6e481-127">Les attributions de rôles fournissent un accès supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="6e481-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6e481-128">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6e481-128">Next steps</span></span>

- [<span data-ttu-id="6e481-129">Attribuer des rôles et des autorisations aux collaborateurs qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6e481-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
