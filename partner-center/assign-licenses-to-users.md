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
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="fe59d-103">Gérer les utilisateurs et les licences utilisateur pour les comptes client</span><span class="sxs-lookup"><span data-stu-id="fe59d-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="fe59d-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="fe59d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fe59d-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="fe59d-105">Global admin</span></span>
- <span data-ttu-id="fe59d-106">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fe59d-106">User management admin</span></span>
- <span data-ttu-id="fe59d-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="fe59d-107">Admin agent</span></span>


<span data-ttu-id="fe59d-108">Vous pouvez créer et supprimer de nouveaux utilisateurs dans le compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="fe59d-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="fe59d-109">Vous pouvez également restaurer un ou plusieurs comptes d’utilisateur que vous avez précédemment supprimés dans les 30 jours suivant la suppression.</span><span class="sxs-lookup"><span data-stu-id="fe59d-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="fe59d-110">Les anciens abonnements attribués à l’utilisateur seront également restaurés (en supposant que ces informations soient disponibles).</span><span class="sxs-lookup"><span data-stu-id="fe59d-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="fe59d-111">Lorsque vous achetez de nouveaux abonnements pour un client, le client doit vous fournir une liste de tous les utilisateurs qui auront besoin de comptes, de leurs autorisations utilisateur et des services dont chaque utilisateur a besoin.</span><span class="sxs-lookup"><span data-stu-id="fe59d-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="fe59d-112">La section **utilisateurs et licences** de l’onglet **client** affiche tous les utilisateurs créés dans le locataire d’un client spécifique, y compris les utilisateurs disposant de licences achetées auprès d’un autre partenaire CSP ou d’un autre canal d’achat.</span><span class="sxs-lookup"><span data-stu-id="fe59d-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="fe59d-113">Vous pouvez [affecter des abonnements à plusieurs utilisateurs](bulk-license-provisioning-for-multiple-users.md) à la fois en important les noms à l’aide d’un [fichier de feuille de calcul. csv compatible avec Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="fe59d-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="fe59d-114">Créer des comptes d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="fe59d-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="fe59d-115">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fe59d-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fe59d-116">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="fe59d-117">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="fe59d-118">Pour chaque utilisateur que vous ajoutez, sélectionnez **Ajouter un abonnement**, puis renseignez les informations, notamment les autorisations et les licences.</span><span class="sxs-lookup"><span data-stu-id="fe59d-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="fe59d-119">**Enregistrez** les changements apportés.</span><span class="sxs-lookup"><span data-stu-id="fe59d-119">**Save** your changes.</span></span>

5. <span data-ttu-id="fe59d-120">Veillez à enregistrer le nom d’utilisateur et le mot de passe temporaire à envoyer à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fe59d-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="fe59d-121">Si vous ajoutez plusieurs utilisateurs, un à la fois, utilisez **Ajouter un autre utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="fe59d-122">Vous pouvez également ajouter plusieurs utilisateurs à la fois en [important un fichier de feuille de calcul. csv compatible Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="fe59d-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="fe59d-123">Vous pouvez attendre la fin de l’ensemble de l’ensemble avant de l’envoyer par courrier électronique ou d’imprimer les noms et les mots de passe à partir de l’écran de confirmation.</span><span class="sxs-lookup"><span data-stu-id="fe59d-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="fe59d-124">Ajouter ou supprimer des licences d’utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="fe59d-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="fe59d-125">Les étapes suivantes s’appliquent à l’ajout ou à la suppression de licences utilisateur pour les produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fe59d-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="fe59d-126">Pour ajouter ou supprimer des licences utilisateur pour les abonnements SaaS basés sur une licence dans le Marketplace commercial, consultez [Ajouter ou supprimer des licences pour un abonnement Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="fe59d-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="fe59d-127">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fe59d-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fe59d-128">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="fe59d-129">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="fe59d-130">Choisissez un ou plusieurs utilisateurs dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-130">Choose one or more users from the list.</span></span> <span data-ttu-id="fe59d-131">Si, par exemple, le client vient d’acheter de nouvelles licences et que vous souhaitez les attribuer à des personnes qui en sont encore dépourvues, vous pouvez utiliser l’option **Filtrer les utilisateurs par...** pour rechercher le groupe approprié.</span><span class="sxs-lookup"><span data-stu-id="fe59d-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="fe59d-132">Sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-132">Select **Manage licenses**.</span></span> <span data-ttu-id="fe59d-133">Apportez vos modifications, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="fe59d-134">Pour les produits de la place de [marché Azure](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit.</span><span class="sxs-lookup"><span data-stu-id="fe59d-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="fe59d-135">Réinitialiser le mot de passe d’un utilisateur pour un client</span><span class="sxs-lookup"><span data-stu-id="fe59d-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="fe59d-136">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="fe59d-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="fe59d-137">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="fe59d-138">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="fe59d-139">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="fe59d-140">En bas de l’écran, sélectionnez **Réinitialiser le mot de passe**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="fe59d-141">Envoyez le nouveau mot de passe temporaire à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fe59d-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="fe59d-142">Supprimer les comptes d’utilisateur d’un client</span><span class="sxs-lookup"><span data-stu-id="fe59d-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="fe59d-143">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="fe59d-144">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="fe59d-145">Dans le menu client, sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="fe59d-146">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="fe59d-147">Au bas de l’écran, sélectionnez **Supprimer le compte utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="fe59d-148">Si vous devez restaurer ce compte, vous pouvez le trouver sous l’onglet **utilisateurs supprimés** de la liste **utilisateurs et licences** du client.</span><span class="sxs-lookup"><span data-stu-id="fe59d-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="fe59d-149">Vous avez 30 jours pour restaurer un utilisateur supprimé.</span><span class="sxs-lookup"><span data-stu-id="fe59d-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="fe59d-150">Restaurer des comptes d’utilisateur supprimés</span><span class="sxs-lookup"><span data-stu-id="fe59d-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="fe59d-151">Dans le menu **espace partenaires** , sélectionnez **clients**, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="fe59d-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="fe59d-152">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="fe59d-153">Sélectionnez l’onglet **utilisateurs supprimés ()** . Elle doit être lue **(1)** ou supérieure quand des utilisateurs supprimés peuvent être restaurés.</span><span class="sxs-lookup"><span data-stu-id="fe59d-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="fe59d-154">Activez une ou plusieurs cases à cocher correspondant aux utilisateurs supprimés, puis sélectionnez **Restaurer**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="fe59d-155">Tous les comptes d’utilisateur sélectionnés réapparaissent dans la page **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="fe59d-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fe59d-156">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fe59d-156">Next steps</span></span>

- [<span data-ttu-id="fe59d-157">Attribuer ou révoquer des licences pour plusieurs utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fe59d-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="fe59d-158">Créer plusieurs utilisateurs pour un compte client</span><span class="sxs-lookup"><span data-stu-id="fe59d-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)