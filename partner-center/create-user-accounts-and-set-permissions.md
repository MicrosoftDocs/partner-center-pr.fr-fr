---
title: Créer des comptes d’utilisateur et attribuer des rôles
description: Un rôle doit être attribué à chaque employé pour lui permettre d’accéder à l’Espace partenaires. Découvrez comment créer des comptes d’utilisateur, attribuer des rôles et définir des autorisations.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000433"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="e44b1-104">Créer des comptes d’utilisateur et attribuer des rôles et des autorisations</span><span class="sxs-lookup"><span data-stu-id="e44b1-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="e44b1-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="e44b1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e44b1-106">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="e44b1-106">Account admin</span></span>
- <span data-ttu-id="e44b1-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e44b1-107">Global admin</span></span>
- <span data-ttu-id="e44b1-108">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e44b1-108">User management admin</span></span>

<span data-ttu-id="e44b1-109">Créez des comptes d’utilisateur pour les employés qui doivent accéder à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e44b1-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="e44b1-110">Ces tâches doivent être effectuées par l’administrateur de la gestion des utilisateurs, l’administrateur des comptes ou l’administrateur général. L’utilisateur qui effectue ces tâches doit aussi se voir attribuer les rôles Administrateur d’utilisateurs ou Administrateur général d’Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="e44b1-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="e44b1-111">Pour plus d’informations sur les rôles d’AAD, consultez [Autorisations des rôles d’administrateur dans Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="e44b1-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="e44b1-112">Ajouter un nouvel utilisateur</span><span class="sxs-lookup"><span data-stu-id="e44b1-112">Add a new user</span></span>

1. <span data-ttu-id="e44b1-113">À partir de l’icône **Paramètres** en haut à droite de l’Espace partenaires, sélectionnez **Gestion des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="e44b1-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="e44b1-114">Sélectionnez **Ajouter un utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="e44b1-114">Select **Add user**.</span></span>

3. <span data-ttu-id="e44b1-115">Entrez le nom complet et l’adresse e-mail unique de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e44b1-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="e44b1-116">Sélectionnez le type d’agent et/ou le type d’administrateur que vous souhaitez attribuer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e44b1-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="e44b1-117">Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e44b1-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="e44b1-118">Si des utilisateurs souhaitent se voir attribuer un rôle, ils peuvent trouver des administrateurs généraux à contacter en accédant à **Gestion des utilisateurs** et en filtrant sur Administrateur général.</span><span class="sxs-lookup"><span data-stu-id="e44b1-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="e44b1-119">Sélectionnez **Ajouter** pour créer le compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e44b1-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="e44b1-120">Confirmez les détails de l’utilisateur sur la page suivante.</span><span class="sxs-lookup"><span data-stu-id="e44b1-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="e44b1-121">Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page.</span><span class="sxs-lookup"><span data-stu-id="e44b1-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="e44b1-122">Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="e44b1-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="e44b1-123">L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire.</span><span class="sxs-lookup"><span data-stu-id="e44b1-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="e44b1-124">Lorsque l’utilisateur se connecte à l’Espace partenaires pour la première fois, il est invité à modifier son mot de passe.</span><span class="sxs-lookup"><span data-stu-id="e44b1-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="e44b1-125">Rechercher le rôle qui vous a été attribué</span><span class="sxs-lookup"><span data-stu-id="e44b1-125">Find the role you've been assigned</span></span>

<span data-ttu-id="e44b1-126">Si votre administrateur général ne vous a rien dit, sachez que vous pouvez trouver le rôle que vous avez dans l’Espace partenaires en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="e44b1-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="e44b1-127">Connectez-vous au tableau de bord de l’Espace partenaires https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="e44b1-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="e44b1-128">Sélectionnez l’icône **Paramètres de compte**, puis **Mon profil**.</span><span class="sxs-lookup"><span data-stu-id="e44b1-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="e44b1-129">Sélectionnez l’onglet **Rôles et autorisations**. Vos rôles et autorisations s’affichent.</span><span class="sxs-lookup"><span data-stu-id="e44b1-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="e44b1-130">Si vous ne voyez pas de programme quand vous vous connectez, cela signifie généralement que vous ne disposez pas des autorisations appropriées pour travailler dans ce programme.</span><span class="sxs-lookup"><span data-stu-id="e44b1-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="e44b1-131">Par exemple, si vous ne voyez pas la page Incentives lorsque vous vous connectez, vous ne disposez pas des autorisations Incentives.</span><span class="sxs-lookup"><span data-stu-id="e44b1-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="e44b1-132">Votre administrateur général peut vous fournir les autorisations nécessaires.</span><span class="sxs-lookup"><span data-stu-id="e44b1-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="e44b1-133">Rechercher votre administrateur général</span><span class="sxs-lookup"><span data-stu-id="e44b1-133">Find your global admin</span></span>

<span data-ttu-id="e44b1-134">Parfois, un utilisateur peut être amené à changer de rôle ou un nouvel utilisateur peut souhaiter se voir attribuer un rôle spécifique.</span><span class="sxs-lookup"><span data-stu-id="e44b1-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="e44b1-135">Pour trouver un administrateur général qui peut effectuer des changements de rôle ou attribuer des rôles à un nouvel utilisateur, à partir de l’icône **Paramètres de compte** en haut à droite de l’Espace partenaires, sélectionnez **Gestion des utilisateurs** et filtrez sur l’administrateur général, ou accédez à **Mon profil**, sélectionnez **Rôles et autorisations** et consultez la liste des différents administrateurs qui peuvent vous aider à élever vos autorisations.</span><span class="sxs-lookup"><span data-stu-id="e44b1-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="e44b1-136">Nouvel administrateur général</span><span class="sxs-lookup"><span data-stu-id="e44b1-136">New global admin</span></span>

<span data-ttu-id="e44b1-137">Si votre administrateur général quitte l’organisation et qu’une autre personne doit endosser ce rôle, vous pouvez envoyer un ticket à l’équipe Azure ou Office 365.</span><span class="sxs-lookup"><span data-stu-id="e44b1-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="e44b1-138">Pour plus d’informations sur la façon de procéder, sélectionnez l’une des options ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e44b1-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="e44b1-139">Nouvel administrateur général pour Azure</span><span class="sxs-lookup"><span data-stu-id="e44b1-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="e44b1-140">Nouvel administrateur général pour Office 365</span><span class="sxs-lookup"><span data-stu-id="e44b1-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="e44b1-141">Attribuer des rôles d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="e44b1-141">Assign user roles</span></span>

<span data-ttu-id="e44b1-142">Pour travailler dans l’Espace partenaires, un rôle doit vous être attribué.</span><span class="sxs-lookup"><span data-stu-id="e44b1-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="e44b1-143">Vous avez actuellement le choix entre des rôles de locataire Azure Active Directory, des rôles Fournisseur de solutions Cloud (CSP) et des rôles d’entreprise non-AAD.</span><span class="sxs-lookup"><span data-stu-id="e44b1-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="e44b1-144">Une entreprise individuelle peut avoir besoin de tous ces rôles.</span><span class="sxs-lookup"><span data-stu-id="e44b1-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="e44b1-145">Les individus doivent être listés dans votre locataire pour pouvoir accéder à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e44b1-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="e44b1-146">Les attributions de rôles fournissent un accès supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="e44b1-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="e44b1-147">**Parmi les rôles de locataire AAD, citons :**</span><span class="sxs-lookup"><span data-stu-id="e44b1-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="e44b1-148">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e44b1-148">Global admin</span></span>
- <span data-ttu-id="e44b1-149">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e44b1-149">User admin</span></span>

<span data-ttu-id="e44b1-150">**Parmi les rôles CSP, citons :**</span><span class="sxs-lookup"><span data-stu-id="e44b1-150">**CSP roles include**:</span></span>
- <span data-ttu-id="e44b1-151">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="e44b1-151">Admin agent</span></span>
- <span data-ttu-id="e44b1-152">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="e44b1-152">Billing admin</span></span>
- <span data-ttu-id="e44b1-153">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="e44b1-153">Sales agent</span></span>
- <span data-ttu-id="e44b1-154">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="e44b1-154">Helpdesk agent</span></span>

<span data-ttu-id="e44b1-155">**Rôles qui gèrent l’adhésion au MPN et l’entreprise (non-AAD)**</span><span class="sxs-lookup"><span data-stu-id="e44b1-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="e44b1-156">Administrateur partenaire MPN</span><span class="sxs-lookup"><span data-stu-id="e44b1-156">MPN partner admin</span></span>
- <span data-ttu-id="e44b1-157">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="e44b1-157">Account admin</span></span>
- <span data-ttu-id="e44b1-158">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="e44b1-158">Referral admin</span></span>
- <span data-ttu-id="e44b1-159">Administrateur de profils métier</span><span class="sxs-lookup"><span data-stu-id="e44b1-159">Business profile admin</span></span>
- <span data-ttu-id="e44b1-160">Utilisateur et administrateur d’incentives</span><span class="sxs-lookup"><span data-stu-id="e44b1-160">Incentives admin and user</span></span>

<span data-ttu-id="e44b1-161">**Le fournisseur de panneau de contrôle est un rôle CSP et non-AAD**.</span><span class="sxs-lookup"><span data-stu-id="e44b1-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="e44b1-162">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e44b1-162">Global admin</span></span>

<span data-ttu-id="e44b1-163">L’**utilisateur invité** doit faire partie du locataire AAD et peut avoir n’importe quel rôle non-AAD.</span><span class="sxs-lookup"><span data-stu-id="e44b1-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="e44b1-164">Pour obtenir des informations spécifiques sur les rôles et ce qu’ils peuvent faire, consultez [Attribuer des autorisations aux utilisateurs](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e44b1-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="e44b1-165">Associer le compte Microsoft Learn d’un utilisateur dans l’Espace Partenaires</span><span class="sxs-lookup"><span data-stu-id="e44b1-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="e44b1-166">Pour que vous puissiez voir les parcours d’apprentissage et de formation suivis par vos utilisateurs pour acquérir des compétences, ils doivent associer leur ID MCP à leur compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e44b1-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="e44b1-167">En tant qu’administrateur général, quand vous ajoutez de nouveaux utilisateurs, veillez à leur rappeler d’associer leur ID MCP à leur compte.</span><span class="sxs-lookup"><span data-stu-id="e44b1-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="e44b1-168">Comment associer votre ID MCP à votre compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e44b1-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="e44b1-169">Dans le tableau de bord de l’Espace partenaires, sélectionnez l'icône **Votre compte** située dans le coin supérieur droit, puis **Mon profil**.</span><span class="sxs-lookup"><span data-stu-id="e44b1-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="e44b1-170">Sous **Votre formation**, vous pouvez associer votre compte Microsoft Learning et connecter votre compte Microsoft à l’Université des partenaires.</span><span class="sxs-lookup"><span data-stu-id="e44b1-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e44b1-171">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e44b1-171">Next steps</span></span>

- [<span data-ttu-id="e44b1-172">Attribuer des rôles et des autorisations aux utilisateurs d’une entreprise qui ont besoin de travailler dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e44b1-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)