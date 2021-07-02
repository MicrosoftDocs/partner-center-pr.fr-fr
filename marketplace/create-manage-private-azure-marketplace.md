---
title: Créer et gérer une place de marché Azure privée dans le Portail Azure
description: En savoir plus sur la création et la gestion de la place de marché Azure privée (version préliminaire) dans le Portail Azure. La place de marché Azure privée (version préliminaire) permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173691"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="00ebe-104">Créer et gérer une place de marché Azure privée dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="00ebe-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="00ebe-105">La place de marché Azure privée permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser.</span><span class="sxs-lookup"><span data-stu-id="00ebe-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="00ebe-106">Pour ce faire, il permet à l’utilisateur de déployer uniquement les offres approuvées par l’administrateur et de se conformer aux stratégies de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="00ebe-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="00ebe-107">Avec la place de marché Azure privée, les utilisateurs peuvent rechercher dans le magasin en ligne des offres conformes à acheter et à déployer.</span><span class="sxs-lookup"><span data-stu-id="00ebe-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="00ebe-108">En tant qu’administrateur de la place de marché (rôle affecté), vous allez commencer avec un magasin privé désactivé et vide où vous pouvez ajouter vos offres et plans approuvés.</span><span class="sxs-lookup"><span data-stu-id="00ebe-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="00ebe-109">Cet article explique comment attribuer le rôle nécessaire, créer un magasin privé, gérer des éléments, approuver des demandes d’utilisateur et activer la place de marché Azure privée pour vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="00ebe-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="00ebe-110">La place de marché Azure privée est au niveau du locataire, de sorte que tous les utilisateurs sous le locataire voient la même liste organisée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="00ebe-111">Toutes les solutions Microsoft (y compris les [distributions Linux approuvées](/azure/virtual-machines/linux/endorsed-distros)) sont automatiquement ajoutées à la place de marché Azure privée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="00ebe-112">Attribuer le rôle d’administrateur de la place de marché</span><span class="sxs-lookup"><span data-stu-id="00ebe-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="00ebe-113">L’administrateur général du locataire doit attribuer le rôle d’administrateur de la place de **marché** à l’administrateur Azure Marketplace privé qui gérera le magasin privé.</span><span class="sxs-lookup"><span data-stu-id="00ebe-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="00ebe-114">L’accès à la gestion de la place de marché Azure privée est uniquement disponible pour les administrateurs informatiques avec le rôle d’administrateur de la place de marché affecté.</span><span class="sxs-lookup"><span data-stu-id="00ebe-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="00ebe-115">Prérequis</span><span class="sxs-lookup"><span data-stu-id="00ebe-115">Prerequisites</span></span>

<span data-ttu-id="00ebe-116">Ces conditions préalables sont requises pour que vous puissiez attribuer le rôle d’administrateur de la place de marché à un utilisateur sur l’étendue du locataire :</span><span class="sxs-lookup"><span data-stu-id="00ebe-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="00ebe-117">Vous avez accès à un utilisateur **administrateur général** .</span><span class="sxs-lookup"><span data-stu-id="00ebe-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="00ebe-118">Le locataire a au moins un abonnement (peut être de n’importe quel type).</span><span class="sxs-lookup"><span data-stu-id="00ebe-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="00ebe-119">Le rôle **contributeur** ou supérieur est attribué à l’utilisateur administrateur général pour l’abonnement choisi.</span><span class="sxs-lookup"><span data-stu-id="00ebe-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="00ebe-120">Attribuer le rôle d’administrateur de la place de marché avec le contrôle d’accès (IAM)</span><span class="sxs-lookup"><span data-stu-id="00ebe-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="00ebe-121">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="00ebe-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="00ebe-122">Sélectionnez **tous les services** , puis **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="00ebe-123">Sélectionnez place de **marché privée** dans le menu de gauche.</span><span class="sxs-lookup"><span data-stu-id="00ebe-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Affiche l’option de menu place de marché privée sur le côté gauche de la place de marché.":::

1. <span data-ttu-id="00ebe-125">Sélectionnez **contrôle d’accès (IAM)** pour affecter le rôle d’administrateur de la place de marché.</span><span class="sxs-lookup"><span data-stu-id="00ebe-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Affiche l’écran de contrôle d’accès I A M.":::

1. <span data-ttu-id="00ebe-127">Sélectionnez **+ Ajouter** > **Ajouter une attribution de rôle**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="00ebe-128">Sous **rôle**, choisissez **administrateur** de la place de marché.</span><span class="sxs-lookup"><span data-stu-id="00ebe-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Affiche le menu attribution de rôle.":::

1. <span data-ttu-id="00ebe-130">Sélectionnez l’utilisateur souhaité dans la liste déroulante, puis sélectionnez **terminé**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="00ebe-131">Attribuer le rôle d’administrateur de la place de marché avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="00ebe-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="00ebe-132">Utilisez le script PowerShell suivant pour attribuer le rôle d’administrateur de la place de marché. Il requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="00ebe-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="00ebe-133">**TenantId :** L’ID du locataire dans l’étendue (rôle d’administrateur de la place de marché est attribuable à l’étendue du locataire).</span><span class="sxs-lookup"><span data-stu-id="00ebe-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="00ebe-134">**SubscriptionId :** Un abonnement dont le rôle **collaborateur** ou supérieur est attribué à l’administrateur général.</span><span class="sxs-lookup"><span data-stu-id="00ebe-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="00ebe-135">**GlobalAdminUsername :** Nom d’utilisateur de l’administrateur général.</span><span class="sxs-lookup"><span data-stu-id="00ebe-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="00ebe-136">**UsernameToAssignRoleFor :** Nom d’utilisateur auquel le rôle d’administrateur de la place de marché sera attribué.</span><span class="sxs-lookup"><span data-stu-id="00ebe-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="00ebe-137">Pour les utilisateurs invités invités au locataire, la mise à disposition du rôle d’administrateur de la place de marché peut prendre jusqu’à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="00ebe-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="00ebe-138">pour plus d’informations, consultez [propriétés d’un utilisateur Azure Active Directory B2B collaboration](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="00ebe-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="00ebe-139">pour plus d’informations sur les applets de commande contenues dans le module PowerShell Az. portal, consultez [Microsoft Azure PowerShell : cmdlets du tableau de bord du portail](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="00ebe-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="00ebe-140">Créer une place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="00ebe-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="00ebe-141">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="00ebe-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="00ebe-142">Sélectionnez **tous les services** , puis **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Affiche la fenêtre principale de Portail Azure.":::

3. <span data-ttu-id="00ebe-144">Sélectionnez place de **marché privée** dans le menu de gauche.</span><span class="sxs-lookup"><span data-stu-id="00ebe-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="00ebe-145">sélectionnez **Prise en main** pour créer une place de marché Azure privée (vous ne devez effectuer cette opération qu’une seule fois).</span><span class="sxs-lookup"><span data-stu-id="00ebe-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="montre comment sélectionner la Prise en main dans la fenêtre principale de Portail Azure.":::

    <span data-ttu-id="00ebe-147">Si la place de marché Azure privée existe déjà pour ce locataire, l’option gérer la place de **marché** est sélectionnée par défaut.</span><span class="sxs-lookup"><span data-stu-id="00ebe-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="00ebe-148">Une fois l’opération terminée, vous disposez d’une place de marché Azure privée vide et désactivée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Affiche l’écran de la place de marché Azure privée vide.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="00ebe-150">Ajouter des éléments à partir de la Galerie</span><span class="sxs-lookup"><span data-stu-id="00ebe-150">Add items from gallery</span></span>

<span data-ttu-id="00ebe-151">Un élément est une combinaison d’une offre et d’un plan.</span><span class="sxs-lookup"><span data-stu-id="00ebe-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="00ebe-152">Vous pouvez rechercher et ajouter des éléments sur la page gérer la place de marché.</span><span class="sxs-lookup"><span data-stu-id="00ebe-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="00ebe-153">Sélectionnez **Ajouter des éléments**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-153">Select **Add items**.</span></span>

2. <span data-ttu-id="00ebe-154">Parcourez la **Galerie** ou utilisez le champ de recherche pour trouver l’élément de votre choix.</span><span class="sxs-lookup"><span data-stu-id="00ebe-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Montre comment parcourir la galerie ou utiliser le champ de recherche.":::

3. <span data-ttu-id="00ebe-156">Par défaut, lors de l’ajout d’une nouvelle offre, tous les plans actuels sont ajoutés à la liste approuvée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="00ebe-157">Pour modifier la sélection du plan avant d’ajouter les éléments sélectionnés, sélectionnez le menu déroulant dans la vignette de l’offre et mettez à jour les plans requis.</span><span class="sxs-lookup"><span data-stu-id="00ebe-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Montre comment mettre à jour les plans requis.":::

4. <span data-ttu-id="00ebe-159">Sélectionnez **terminé** en bas à gauche une fois que vous avez effectué vos sélections.</span><span class="sxs-lookup"><span data-stu-id="00ebe-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="00ebe-160">**Ajouter des éléments** à la place de marché sera disponible pour les offres non-Microsoft uniquement.</span><span class="sxs-lookup"><span data-stu-id="00ebe-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="00ebe-161">Les solutions Microsoft (y compris les [distributions Linux](/azure/virtual-machines/linux/endorsed-distros)approuvées) sont marquées comme « approuvées par défaut » et ne peuvent pas être gérées dans la place de marché privée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="00ebe-162">Modifier les plans de l’élément</span><span class="sxs-lookup"><span data-stu-id="00ebe-162">Edit item's plans</span></span>

<span data-ttu-id="00ebe-163">Vous pouvez modifier les plans d’un élément sur la page gérer la place de marché.</span><span class="sxs-lookup"><span data-stu-id="00ebe-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="00ebe-164">Dans la colonne **plans** , passez en revue les plans disponibles dans le menu déroulant de cet élément.</span><span class="sxs-lookup"><span data-stu-id="00ebe-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="00ebe-165">Activez ou désactivez les cases à cocher pour choisir les plans à mettre à la disposition de vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="00ebe-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Montre comment activer ou désactiver la case à cocher pour l’élément requis.":::

   > [!NOTE]
   > <span data-ttu-id="00ebe-167">Chaque offre doit avoir au moins un plan sélectionné pour que la mise à jour se produise.</span><span class="sxs-lookup"><span data-stu-id="00ebe-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="00ebe-168">Pour supprimer tous les plans associés à une offre, supprimez l’intégralité de l’offre (voir la section suivante).</span><span class="sxs-lookup"><span data-stu-id="00ebe-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="00ebe-169">Supprimer des offres</span><span class="sxs-lookup"><span data-stu-id="00ebe-169">Delete offers</span></span>

<span data-ttu-id="00ebe-170">Dans la page gérer le Marketplace, activez la case à cocher en regard du nom de l’offre (Voir l’écran ci-dessus), puis sélectionnez **Supprimer les éléments**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="00ebe-171">Activer/désactiver la place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="00ebe-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="00ebe-172">Dans la page gérer la place de marché, vous verrez une de ces bannières, qui indiquent l’état actuel de la place de marché Azure privée :</span><span class="sxs-lookup"><span data-stu-id="00ebe-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Affiche la bannière « désactiver l’État ».":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Affiche la bannière « activer l’État ».":::

<span data-ttu-id="00ebe-175">Vous pouvez activer ou désactiver la place de marché Azure privée si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="00ebe-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="00ebe-176">S’il est désactivé, sélectionnez Activer la place de **marché privée** pour l’activer.</span><span class="sxs-lookup"><span data-stu-id="00ebe-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="00ebe-177">Si cette option est activée, sélectionnez Désactiver la place de **marché privée** pour la désactiver.</span><span class="sxs-lookup"><span data-stu-id="00ebe-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="00ebe-178">Centre de notifications de la place de marché Azure privé</span><span class="sxs-lookup"><span data-stu-id="00ebe-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="00ebe-179">Le centre de notifications se compose de trois types de notifications et permet à l’administrateur de la place de marché d’effectuer des actions en fonction de la notification :</span><span class="sxs-lookup"><span data-stu-id="00ebe-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="00ebe-180">Demandes d’approbation des utilisateurs pour les éléments qui ne figurent pas dans la liste approuvée (consultez la [demande d’ajout d’offres ou de plans](#request-to-add-offers-or-plans) ci-dessous).</span><span class="sxs-lookup"><span data-stu-id="00ebe-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="00ebe-181">Nouvelles notifications de plan pour les offres qui disposent déjà d’un ou plusieurs plans dans la liste approuvée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="00ebe-182">Suppression des notifications de plan pour les éléments qui se trouvent dans la liste approuvée, mais qui ont été supprimés de la place de marché Azure globale.</span><span class="sxs-lookup"><span data-stu-id="00ebe-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="00ebe-183">Pour accéder au centre de notifications :</span><span class="sxs-lookup"><span data-stu-id="00ebe-183">To access the notification center:</span></span>

1. <span data-ttu-id="00ebe-184">Sélectionnez **notifications** dans le menu de gauche.</span><span class="sxs-lookup"><span data-stu-id="00ebe-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Affiche le menu notifications.":::

1. <span data-ttu-id="00ebe-186">Sélectionnez le menu de points de suspension pour plus d’actions.</span><span class="sxs-lookup"><span data-stu-id="00ebe-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Affiche les résultats du menu plus d’options.":::

1. <span data-ttu-id="00ebe-188">Pour les demandes de plan, **afficher les demandes** ouvre le formulaire de demande d’approbation dans lequel vous pouvez consulter toutes les demandes d’utilisateur pour l’offre spécifique.</span><span class="sxs-lookup"><span data-stu-id="00ebe-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="00ebe-189">Sélectionnez **approuver** ou **rejeter**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Affiche les options approuver et rejeter.":::

1. <span data-ttu-id="00ebe-191">Sélectionnez le plan à approuver dans le menu déroulant.</span><span class="sxs-lookup"><span data-stu-id="00ebe-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="00ebe-192">Ajoutez un commentaire et sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="00ebe-193">Navigation dans la place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="00ebe-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="00ebe-194">Lorsque la place de marché Azure privée est activée, les utilisateurs voient les plans approuvés par l’administrateur de la place de marché.</span><span class="sxs-lookup"><span data-stu-id="00ebe-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="00ebe-195">Une notification verte **approuvée** indique une offre partenaire (non-Microsoft) approuvée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="00ebe-196">Une notification bleue **approuvée** indique une offre Microsoft (y compris les [distributions Linux](/azure/virtual-machines/linux/endorsed-distros)approuvées) approuvée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="00ebe-197">Les utilisateurs peuvent filtrer les offres qui ne sont pas approuvées :</span><span class="sxs-lookup"><span data-stu-id="00ebe-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Affiche l’option de filtrage.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="00ebe-199">Acheter ou déployer sur une place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="00ebe-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="00ebe-200">Bien que l’expérience de la page Détails du produit soit similaire à la place de marché Azure mondiale, il existe trois scénarios spécifiques à Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="00ebe-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="00ebe-201">Quand un utilisateur sélectionne un plan approuvé, le bouton **créer** est activé :</span><span class="sxs-lookup"><span data-stu-id="00ebe-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Affiche la bannière d’offre indiquant qu’un plan peut être créé.":::

- <span data-ttu-id="00ebe-203">Si une sélection de plan de produit n’apparaît pas dans la page Détails du produit mais que l’administrateur a approuvé un ou plusieurs plans, une bannière indique les plans qui sont approuvés et le bouton **créer** est activé :</span><span class="sxs-lookup"><span data-stu-id="00ebe-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Affiche la bannière d’offre indiquant qu’un plan peut être créé et afficher les plans disponibles.":::

- <span data-ttu-id="00ebe-205">Lorsqu’un utilisateur sélectionne un plan non approuvé, une bannière note le plan comme non approuvé et le bouton **créer** est désactivé.</span><span class="sxs-lookup"><span data-stu-id="00ebe-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="00ebe-206">L’utilisateur peut toujours demander à ajouter le plan à la liste approuvée (voir la section suivante).</span><span class="sxs-lookup"><span data-stu-id="00ebe-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="00ebe-207">Demande d’ajout d’offres ou de plans</span><span class="sxs-lookup"><span data-stu-id="00ebe-207">Request to add offers or plans</span></span>

<span data-ttu-id="00ebe-208">Vous pouvez demander à ajouter une offre ou un plan public qui n’est pas actuellement approuvé dans la place de marché Azure privée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="00ebe-209">Sélectionnez **demander à ajouter** dans la bannière pour ouvrir le **formulaire de demande d’accès**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Affiche la bannière avec le lien « demander à ajouter ».":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Affiche le formulaire de demande d’accès pour les offres ou les plans.":::

1. <span data-ttu-id="00ebe-212">Sélectionnez les plans à ajouter à la demande (**tout plan** indique à l’administrateur de la place de marché que vous n’avez pas de préférence pour un plan dans une offre).</span><span class="sxs-lookup"><span data-stu-id="00ebe-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="00ebe-213">Ajoutez une **Justification** et sélectionnez **demander** pour envoyer votre demande.</span><span class="sxs-lookup"><span data-stu-id="00ebe-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Affiche le formulaire de demande d’accès pour les offres ou les plans avec des exemples d’entrées.":::

1. <span data-ttu-id="00ebe-215">Une indication pour une demande en attente apparaît dans le formulaire de demande d’accès avec une option de retrait de la **demande**.</span><span class="sxs-lookup"><span data-stu-id="00ebe-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Affiche la liste des plans approuvés ou en attente avec le lien de demande de retrait.":::

> [!NOTE]
> <span data-ttu-id="00ebe-217">Une fois soumis, le formulaire de demande d’approbation est envoyé au [Centre de notifications](#private-azure-marketplace-notification-center) pour que l’administrateur de la place de marché examine la demande et effectue une action.</span><span class="sxs-lookup"><span data-stu-id="00ebe-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="00ebe-218">L’approbation sur la place de marché privée n’indique pas l’approvisionnement d’une solution.</span><span class="sxs-lookup"><span data-stu-id="00ebe-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="00ebe-219">Forum Aux Questions (FAQ)</span><span class="sxs-lookup"><span data-stu-id="00ebe-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="00ebe-220">Je bloque déjà l’application tierce de la place de marché via Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="00ebe-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="00ebe-221">En quoi cela diffère-t-il ?</span><span class="sxs-lookup"><span data-stu-id="00ebe-221">How is this different?</span></span>

<span data-ttu-id="00ebe-222">Il existe actuellement deux façons de limiter les services tiers dans la place de marché :</span><span class="sxs-lookup"><span data-stu-id="00ebe-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="00ebe-223">Via le portail EA ou le Portail Azure, désactivez les services tiers ou limitez-les uniquement à des références SKU libres ou BYOL.</span><span class="sxs-lookup"><span data-stu-id="00ebe-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Montre comment restreindre les services de la Portail Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Montre comment restreindre les services dans le portail E A.":::

2. <span data-ttu-id="00ebe-226">Créez une stratégie Azure pour autoriser uniquement des machines virtuelles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="00ebe-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="00ebe-227">pour plus d’informations sur la façon d’appliquer une stratégie à Windows des machines virtuelles, consultez [appliquer des stratégies à des machines virtuelles Windows avec Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="00ebe-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="00ebe-228">La place de marché Azure privée offre davantage de souplesse pour limiter et autoriser des offres et des plans spécifiques.</span><span class="sxs-lookup"><span data-stu-id="00ebe-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="00ebe-229">Il informe les utilisateurs finaux sur la disponibilité du déploiement dans la Galerie de la place de marché même avant d’essayer de déployer des services tiers.</span><span class="sxs-lookup"><span data-stu-id="00ebe-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="00ebe-230">Pour autoriser le déploiement de services tiers, définissez la place de marché Azure sur activé/activé dans le portail EA et le Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="00ebe-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="00ebe-231">La place de marché Azure privée peut organiser des solutions de partenaires non limitées aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="00ebe-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="00ebe-232">La place de marché Azure privée peut être organisée au niveau du plan et peut également définir le « plan actuel et futur ».</span><span class="sxs-lookup"><span data-stu-id="00ebe-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="00ebe-233">La place de marché Azure privée peut informer les utilisateurs finaux sur ce qui peut et ne peut pas être déployé.</span><span class="sxs-lookup"><span data-stu-id="00ebe-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="00ebe-234">Quelle est la différence entre une offre privée et une place de marché Azure privée ?</span><span class="sxs-lookup"><span data-stu-id="00ebe-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="00ebe-235">Une **offre privée** permet aux éditeurs de créer des plans qui sont uniquement visibles par les clients ciblés.</span><span class="sxs-lookup"><span data-stu-id="00ebe-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="00ebe-236">Cela leur permet de partager en privé des solutions personnalisées avec la tarification négociée, les conditions générales et les configurations spécialisées.</span><span class="sxs-lookup"><span data-stu-id="00ebe-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="00ebe-237">Pour plus d’informations, consultez [les offres privées dans le Marketplace commercial](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="00ebe-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="00ebe-238">La place de **marché Azure privée** dans le portail Azure permet aux administrateurs de préapprouver les solutions tierces que leurs utilisateurs peuvent déployer.</span><span class="sxs-lookup"><span data-stu-id="00ebe-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="00ebe-239">Avec une place de marché Azure privée, les utilisateurs peuvent profiter des avantages de la place de marché Azure en recherchant, en achetant et en déployant des offres conformes.</span><span class="sxs-lookup"><span data-stu-id="00ebe-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="00ebe-240">Pour gérer les offres privées basées sur un abonnement dans la place de marché privé, l’administrateur de la place de marché doit avoir au minimum le rôle de « lecture » sur l’abonnement spécifique.</span><span class="sxs-lookup"><span data-stu-id="00ebe-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="00ebe-241">J’ai ajouté une offre privée à la place de marché Azure privée, pourquoi ne s’est-elle pas affichée dans l’onglet gérer la place de marché ?</span><span class="sxs-lookup"><span data-stu-id="00ebe-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="00ebe-242">Les offres privées basées sur un abonnement sont visibles uniquement pour les abonnements répertoriés dans les paramètres de l’offre privée.</span><span class="sxs-lookup"><span data-stu-id="00ebe-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="00ebe-243">Pour afficher l’offre privée, assurez-vous que le filtre d’abonnement global affiche tous les abonnements.</span><span class="sxs-lookup"><span data-stu-id="00ebe-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Affiche le filtre place de marché privé.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="00ebe-245">Pouvez-vous inclure des images personnalisées dans la place de marché Azure privée ?</span><span class="sxs-lookup"><span data-stu-id="00ebe-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="00ebe-246">Non.</span><span class="sxs-lookup"><span data-stu-id="00ebe-246">No.</span></span> <span data-ttu-id="00ebe-247">La place de marché Azure privée permet à n’importe quel administrateur informatique de gérer et d’organiser des solutions tierces à partir de la place de marché Azure mondiale.</span><span class="sxs-lookup"><span data-stu-id="00ebe-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="00ebe-248">Étant donné que les images personnalisées ne se trouvent pas sur la place de marché Azure globale, l’administrateur informatique ne peut pas choisir vos images personnalisées.</span><span class="sxs-lookup"><span data-stu-id="00ebe-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="00ebe-249">Si vous souhaitez partager des images personnalisées, utilisez la [Galerie d’images partagées](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="00ebe-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="00ebe-250">Guide pas à pas de création d’une bibliothèque d’images partagées (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="00ebe-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="00ebe-251">Créer une définition d’image dans un SIG.</span><span class="sxs-lookup"><span data-stu-id="00ebe-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="00ebe-252">Le client doit choisir **généralisée** pour le champ de l’état du système d’exploitation.</span><span class="sxs-lookup"><span data-stu-id="00ebe-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="00ebe-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="00ebe-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="00ebe-254">Placez l’image managée dans la Galerie d’images partagées ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="00ebe-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="00ebe-255">Les images de machine virtuelle SIG se trouvent dans un seul abonnement.</span><span class="sxs-lookup"><span data-stu-id="00ebe-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="00ebe-256">Pour le rendre disponible pour d’autres abonnements, utilisez une inscription d’application ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="00ebe-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="00ebe-257">Pourquoi certaines offres sont-elles **approuvées par défaut,** même si le serveur de publication n’est pas Microsoft ?</span><span class="sxs-lookup"><span data-stu-id="00ebe-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="00ebe-258">Microsoft prend en charge les technologies Linux et open source dans Azure.</span><span class="sxs-lookup"><span data-stu-id="00ebe-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="00ebe-259">Les [distributions Linux approuvées](/azure/virtual-machines/linux/endorsed-distros) sont prises en charge sur Azure et le prix est intégré aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="00ebe-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="00ebe-260">Étant donné que l’agent Linux Azure est déjà préinstallé sur la place de marché Azure, il est traité comme une offre Microsoft.</span><span class="sxs-lookup"><span data-stu-id="00ebe-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="00ebe-261">Étant donné que les offres Microsoft sont approuvées par défaut, les distributions Linux approuvées ne peuvent pas être gérées dans la place de marché Azure privée et sont approuvées par défaut.</span><span class="sxs-lookup"><span data-stu-id="00ebe-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="00ebe-262">Contacter le support technique</span><span class="sxs-lookup"><span data-stu-id="00ebe-262">Contact support</span></span>

- <span data-ttu-id="00ebe-263">Pour obtenir de l’aide sur la place de marché Azure, visitez [le site Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="00ebe-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>