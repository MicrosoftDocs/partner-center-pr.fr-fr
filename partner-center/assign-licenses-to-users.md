---
title: Gérer les utilisateurs dans les comptes client
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à créer des comptes d’utilisateur pour un client, à ajouter ou supprimer des licences utilisateur, à réinitialiser les mots de passe utilisateur, à supprimer des comptes d’utilisateur ou à les restaurer.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527675"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="621f0-103">Tâches de gestion des utilisateurs pour les comptes clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="621f0-103">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="621f0-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="621f0-104">**Applies to**</span></span>

- <span data-ttu-id="621f0-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="621f0-105">Partner Center</span></span>

<span data-ttu-id="621f0-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="621f0-106">**Appropriate roles**</span></span>

- <span data-ttu-id="621f0-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="621f0-107">Global admin</span></span>
- <span data-ttu-id="621f0-108">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="621f0-108">User management admin</span></span>
- <span data-ttu-id="621f0-109">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="621f0-109">Admin agent</span></span>
- <span data-ttu-id="621f0-110">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="621f0-110">Sales agent</span></span>
- <span data-ttu-id="621f0-111">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="621f0-111">Helpdesk agent</span></span>

<span data-ttu-id="621f0-112">Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="621f0-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="621f0-113">Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="621f0-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="621f0-114">Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).</span><span class="sxs-lookup"><span data-stu-id="621f0-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="621f0-115">Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.</span><span class="sxs-lookup"><span data-stu-id="621f0-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="621f0-116">Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="621f0-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="621f0-117">Créer des comptes d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="621f0-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="621f0-118">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="621f0-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="621f0-119">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-119">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="621f0-120">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-120">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="621f0-121">Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences.</span><span class="sxs-lookup"><span data-stu-id="621f0-121">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="621f0-122">**Enregistrez** les changements apportés.</span><span class="sxs-lookup"><span data-stu-id="621f0-122">**Save** your changes.</span></span>

5. <span data-ttu-id="621f0-123">Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="621f0-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="621f0-124">Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="621f0-124">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="621f0-125">Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="621f0-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="621f0-126">Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.</span><span class="sxs-lookup"><span data-stu-id="621f0-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="621f0-127">Ajouter ou supprimer des licences d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="621f0-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="621f0-128">Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="621f0-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="621f0-129">Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="621f0-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="621f0-130">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="621f0-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="621f0-131">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-131">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="621f0-132">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-132">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="621f0-133">Choisissez un ou plusieurs utilisateurs dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-133">Choose one or more users from the list.</span></span> <span data-ttu-id="621f0-134">Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les attribuer à des personnes qui en sont encore dépourvues, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour rechercher le groupe approprié.</span><span class="sxs-lookup"><span data-stu-id="621f0-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="621f0-135">Sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-135">Select **Manage licenses**.</span></span> <span data-ttu-id="621f0-136">Apportez vos modifications, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="621f0-136">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="621f0-137">Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.</span><span class="sxs-lookup"><span data-stu-id="621f0-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="621f0-138">Réinitialiser le mot de passe d’un utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="621f0-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="621f0-139">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="621f0-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="621f0-140">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-140">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="621f0-141">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-141">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="621f0-142">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="621f0-143">En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="621f0-143">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="621f0-144">Envoyez le nouveau mot de passe temporaire à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="621f0-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="621f0-145">Supprimer les comptes d’utilisateur d’un client</span><span class="sxs-lookup"><span data-stu-id="621f0-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="621f0-146">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="621f0-146">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="621f0-147">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="621f0-148">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-148">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="621f0-149">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="621f0-150">Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="621f0-150">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="621f0-151">Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client.</span><span class="sxs-lookup"><span data-stu-id="621f0-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="621f0-152">Vous avez 30 jours pour restaurer un utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="621f0-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="621f0-153">Restaurer des comptes d’utilisateur supprimés</span><span class="sxs-lookup"><span data-stu-id="621f0-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="621f0-154">Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="621f0-154">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="621f0-155">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-155">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="621f0-156">Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.</span><span class="sxs-lookup"><span data-stu-id="621f0-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="621f0-157">Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.</span><span class="sxs-lookup"><span data-stu-id="621f0-157">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="621f0-158">Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="621f0-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="621f0-159">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="621f0-159">Related topics</span></span>


[<span data-ttu-id="621f0-160">Attribuer ou révoquer des licences pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="621f0-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="621f0-161">Créer plusieurs utilisateurs pour un compte client</span><span class="sxs-lookup"><span data-stu-id="621f0-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)