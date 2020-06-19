---
title: Gérer les utilisateurs dans les comptes client
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à créer des comptes d’utilisateur pour un client, à ajouter ou supprimer des licences utilisateur, à réinitialiser les mots de passe utilisateur, à supprimer des comptes d’utilisateur ou à les restaurer.
author: LauraBrenner
ms.author: labrenne
Keywords: gestion des clients, compte, créer un compte, licences, attribuer une licence, gestion des utilisateurs, mot de passe, réinitialiser le mot de passe, modifier le mot de passe
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3fb55e341692e38250c4e751cf73f3120604c15a
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991031"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="986ce-104">Tâches de gestion des utilisateurs pour les comptes clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="986ce-104">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="986ce-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="986ce-105">**Applies to**</span></span>

- <span data-ttu-id="986ce-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="986ce-106">Partner Center</span></span>

<span data-ttu-id="986ce-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="986ce-107">**Appropriate roles**</span></span>

- <span data-ttu-id="986ce-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="986ce-108">Global admin</span></span>
- <span data-ttu-id="986ce-109">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="986ce-109">User management admin</span></span>
- <span data-ttu-id="986ce-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="986ce-110">Admin agent</span></span>
- <span data-ttu-id="986ce-111">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="986ce-111">Sales agent</span></span>
- <span data-ttu-id="986ce-112">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="986ce-112">Helpdesk agent</span></span>

<span data-ttu-id="986ce-113">Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="986ce-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="986ce-114">Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="986ce-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="986ce-115">Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).</span><span class="sxs-lookup"><span data-stu-id="986ce-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="986ce-116">Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.</span><span class="sxs-lookup"><span data-stu-id="986ce-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="986ce-117">Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="986ce-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="986ce-118">Créer des comptes d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="986ce-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="986ce-119">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="986ce-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="986ce-120">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="986ce-121">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="986ce-122">Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences.</span><span class="sxs-lookup"><span data-stu-id="986ce-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="986ce-123">**Enregistrez** les changements apportés.</span><span class="sxs-lookup"><span data-stu-id="986ce-123">**Save** your changes.</span></span>

5. <span data-ttu-id="986ce-124">Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="986ce-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="986ce-125">Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="986ce-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="986ce-126">Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="986ce-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="986ce-127">Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.</span><span class="sxs-lookup"><span data-stu-id="986ce-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="986ce-128">Ajouter ou supprimer des licences d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="986ce-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="986ce-129">Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="986ce-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="986ce-130">Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="986ce-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="986ce-131">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="986ce-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="986ce-132">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="986ce-133">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="986ce-134">Choisissez un ou plusieurs utilisateurs dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-134">Choose one or more users from the list.</span></span> <span data-ttu-id="986ce-135">Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les attribuer à des personnes qui en sont encore dépourvues, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour rechercher le groupe approprié.</span><span class="sxs-lookup"><span data-stu-id="986ce-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="986ce-136">Sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-136">Select **Manage licenses**.</span></span> <span data-ttu-id="986ce-137">Apportez vos modifications, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="986ce-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="986ce-138">Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.</span><span class="sxs-lookup"><span data-stu-id="986ce-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="986ce-139">Réinitialiser le mot de passe d’un utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="986ce-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="986ce-140">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="986ce-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="986ce-141">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="986ce-142">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="986ce-143">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="986ce-144">En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="986ce-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="986ce-145">Envoyez le nouveau mot de passe temporaire à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="986ce-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="986ce-146">Supprimer les comptes d’utilisateur d’un client</span><span class="sxs-lookup"><span data-stu-id="986ce-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="986ce-147">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="986ce-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="986ce-148">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="986ce-149">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="986ce-150">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="986ce-151">Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="986ce-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="986ce-152">Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client.</span><span class="sxs-lookup"><span data-stu-id="986ce-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="986ce-153">Vous avez 30 jours pour restaurer un utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="986ce-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="986ce-154">Restaurer des comptes d’utilisateur supprimés</span><span class="sxs-lookup"><span data-stu-id="986ce-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="986ce-155">Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="986ce-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="986ce-156">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="986ce-157">Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.</span><span class="sxs-lookup"><span data-stu-id="986ce-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="986ce-158">Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.</span><span class="sxs-lookup"><span data-stu-id="986ce-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="986ce-159">Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="986ce-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="986ce-160">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="986ce-160">Related topics</span></span>


[<span data-ttu-id="986ce-161">Attribuer ou révoquer des licences pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="986ce-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="986ce-162">Créer plusieurs utilisateurs pour un compte client</span><span class="sxs-lookup"><span data-stu-id="986ce-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)