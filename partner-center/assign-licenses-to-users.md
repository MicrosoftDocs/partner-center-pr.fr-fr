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
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149891"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="a9cc9-103">Gérer les utilisateurs et les licences utilisateur pour les comptes client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="a9cc9-104">**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="a9cc9-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="a9cc9-105">Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="a9cc9-106">Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="a9cc9-107">Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).</span><span class="sxs-lookup"><span data-stu-id="a9cc9-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="a9cc9-108">Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="a9cc9-109">La section **utilisateurs et licences** de l’onglet **client** affiche tous les utilisateurs créés dans le locataire d’un client spécifique, y compris les utilisateurs disposant de licences achetées auprès d’un autre partenaire CSP ou d’un autre canal d’achat.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="a9cc9-110">Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="a9cc9-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="a9cc9-111">Créer des comptes d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="a9cc9-112">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a9cc9-113">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a9cc9-114">Dans le menu client, sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="a9cc9-115">Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="a9cc9-116">**Enregistrez** les changements apportés.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-116">**Save** your changes.</span></span>

5. <span data-ttu-id="a9cc9-117">Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="a9cc9-118">Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="a9cc9-119">Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="a9cc9-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="a9cc9-120">Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="a9cc9-121">Ajouter ou supprimer des licences d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="a9cc9-122">Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="a9cc9-123">Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="a9cc9-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="a9cc9-124">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a9cc9-125">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a9cc9-126">Dans le menu client, sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="a9cc9-127">Choisissez un ou plusieurs utilisateurs dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-127">Choose one or more users from the list.</span></span> <span data-ttu-id="a9cc9-128">Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les affecter à des personnes qui n’en ont pas encore, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour trouver le groupe approprié.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="a9cc9-129">Sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-129">Select **Manage licenses**.</span></span> <span data-ttu-id="a9cc9-130">Apportez vos modifications, puis **Enregistrez**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="a9cc9-131">Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="a9cc9-132">Réinitialiser le mot de passe d’un utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="a9cc9-133">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a9cc9-134">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a9cc9-135">Dans le menu client, sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="a9cc9-136">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="a9cc9-137">En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="a9cc9-138">Envoyez le nouveau mot de passe temporaire à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="a9cc9-139">Supprimer les comptes d’utilisateur d’un client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="a9cc9-140">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="a9cc9-141">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="a9cc9-142">Dans le menu client, sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="a9cc9-143">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="a9cc9-144">Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="a9cc9-145">Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="a9cc9-146">Vous avez 30 jours pour restaurer un utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="a9cc9-147">Restaurer des comptes d’utilisateur supprimés</span><span class="sxs-lookup"><span data-stu-id="a9cc9-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="a9cc9-148">Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="a9cc9-149">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="a9cc9-150">Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="a9cc9-151">Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="a9cc9-152">Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="a9cc9-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9cc9-153">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a9cc9-153">Next steps</span></span>

- [<span data-ttu-id="a9cc9-154">Attribuer ou révoquer des licences pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a9cc9-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="a9cc9-155">Créer plusieurs utilisateurs pour un compte client</span><span class="sxs-lookup"><span data-stu-id="a9cc9-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)