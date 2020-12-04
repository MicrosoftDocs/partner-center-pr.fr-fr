---
title: Gérer les utilisateurs pour les comptes client
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gérer les utilisateurs pour vos clients dans l’espace partenaires : créer des comptes d’utilisateur, ajouter ou supprimer des licences utilisateur, réinitialiser les mots de passe et supprimer ou restaurer des comptes d’utilisateur.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cea1ac8bff9690edfe4b257c910fc3c335d2836c
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570737"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="8f6c3-103">Gérer les utilisateurs et les licences utilisateur pour les comptes client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="8f6c3-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8f6c3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8f6c3-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="8f6c3-105">Global admin</span></span>
- <span data-ttu-id="8f6c3-106">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8f6c3-106">User management admin</span></span>
- <span data-ttu-id="8f6c3-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="8f6c3-107">Admin agent</span></span>


<span data-ttu-id="8f6c3-108">Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="8f6c3-109">Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="8f6c3-110">Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).</span><span class="sxs-lookup"><span data-stu-id="8f6c3-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="8f6c3-111">Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="8f6c3-112">Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="8f6c3-112">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="8f6c3-113">Créer des comptes d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-113">Create user accounts for a customer</span></span>

1. <span data-ttu-id="8f6c3-114">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-114">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8f6c3-115">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8f6c3-116">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-116">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="8f6c3-117">Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-117">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="8f6c3-118">**Enregistrez** les changements apportés.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-118">**Save** your changes.</span></span>

5. <span data-ttu-id="8f6c3-119">Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-119">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="8f6c3-120">Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-120">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="8f6c3-121">Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="8f6c3-121">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="8f6c3-122">Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-122">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="8f6c3-123">Ajouter ou supprimer des licences d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-123">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="8f6c3-124">Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-124">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="8f6c3-125">Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="8f6c3-125">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="8f6c3-126">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-126">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8f6c3-127">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-127">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8f6c3-128">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-128">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="8f6c3-129">Choisissez un ou plusieurs utilisateurs dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-129">Choose one or more users from the list.</span></span> <span data-ttu-id="8f6c3-130">Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les attribuer à des personnes qui en sont encore dépourvues, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour rechercher le groupe approprié.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-130">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="8f6c3-131">Sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-131">Select **Manage licenses**.</span></span> <span data-ttu-id="8f6c3-132">Apportez vos modifications, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-132">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="8f6c3-133">Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-133">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="8f6c3-134">Réinitialiser le mot de passe d’un utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-134">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="8f6c3-135">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-135">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="8f6c3-136">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-136">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="8f6c3-137">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-137">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="8f6c3-138">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-138">Choose the user from the list.</span></span>

4. <span data-ttu-id="8f6c3-139">En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-139">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="8f6c3-140">Envoyez le nouveau mot de passe temporaire à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-140">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="8f6c3-141">Supprimer les comptes d’utilisateur d’un client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-141">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="8f6c3-142">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-142">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="8f6c3-143">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-143">Choose the customer from the list.</span></span>

2. <span data-ttu-id="8f6c3-144">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-144">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="8f6c3-145">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-145">Choose the user from the list.</span></span>

3. <span data-ttu-id="8f6c3-146">Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-146">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="8f6c3-147">Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-147">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="8f6c3-148">Vous avez 30 jours pour restaurer un utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-148">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="8f6c3-149">Restaurer des comptes d’utilisateur supprimés</span><span class="sxs-lookup"><span data-stu-id="8f6c3-149">Restore deleted user accounts</span></span>

1. <span data-ttu-id="8f6c3-150">Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-150">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="8f6c3-151">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-151">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="8f6c3-152">Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-152">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="8f6c3-153">Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-153">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="8f6c3-154">Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8f6c3-154">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8f6c3-155">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8f6c3-155">Next steps</span></span>

- [<span data-ttu-id="8f6c3-156">Attribuer ou révoquer des licences pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8f6c3-156">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="8f6c3-157">Créer plusieurs utilisateurs pour un compte client</span><span class="sxs-lookup"><span data-stu-id="8f6c3-157">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)