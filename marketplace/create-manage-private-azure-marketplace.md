---
title: Créer et gérer une place de marché Azure privée dans Portail Azure
description: En savoir plus sur la création et la gestion de la place de marché Azure privée (version préliminaire) dans le Portail Azure. La place de marché Azure privée (version préliminaire) permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439253"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="3964a-104">Créer et gérer une place de marché Azure privée (version préliminaire) dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="3964a-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="3964a-105">La place de marché Azure privée (version préliminaire) permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser.</span><span class="sxs-lookup"><span data-stu-id="3964a-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="3964a-106">Pour ce faire, il vous permet de déployer uniquement les offres que vous approuvez et qui sont conformes aux stratégies de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="3964a-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="3964a-107">Avec la place de marché Azure privée, vos utilisateurs peuvent rechercher des offres conformes à acheter et à déployer dans le magasin en ligne.</span><span class="sxs-lookup"><span data-stu-id="3964a-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="3964a-108">En tant qu’administrateur de la place de marché (rôle affecté), vous allez commencer avec un magasin privé désactivé et vide où vous pouvez ajouter vos offres et plans approuvés.</span><span class="sxs-lookup"><span data-stu-id="3964a-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="3964a-109">Cet article explique comment créer, gérer et activer la place de marché Azure privée pour vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="3964a-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="3964a-110">Remarques :</span><span class="sxs-lookup"><span data-stu-id="3964a-110">Notes:</span></span>

- <span data-ttu-id="3964a-111">La place de marché Azure privée est au niveau du locataire, de sorte que tous les utilisateurs sous le locataire voient la même liste organisée.</span><span class="sxs-lookup"><span data-stu-id="3964a-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="3964a-112">Toutes les solutions Microsoft sont automatiquement ajoutées à la place de marché Azure privée.</span><span class="sxs-lookup"><span data-stu-id="3964a-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="3964a-113">Attribuer le rôle d’administrateur de la place de marché</span><span class="sxs-lookup"><span data-stu-id="3964a-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="3964a-114">L’administrateur général du locataire doit attribuer le rôle d’administrateur de la place de **marché** à l’administrateur Azure Marketplace privé qui gérera le magasin privé.</span><span class="sxs-lookup"><span data-stu-id="3964a-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="3964a-115">L’accès à la gestion de la place de marché Azure privée est uniquement disponible pour les administrateurs informatiques avec le rôle d’administrateur de la place de marché affecté.</span><span class="sxs-lookup"><span data-stu-id="3964a-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="3964a-116">Prérequis</span><span class="sxs-lookup"><span data-stu-id="3964a-116">Prerequisites</span></span>

<span data-ttu-id="3964a-117">Vous devez respecter ces conditions préalables avant de pouvoir attribuer le rôle d’administrateur de la place de marché à un utilisateur sur l’étendue du locataire :</span><span class="sxs-lookup"><span data-stu-id="3964a-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="3964a-118">Vous avez accès à un utilisateur **administrateur général** .</span><span class="sxs-lookup"><span data-stu-id="3964a-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="3964a-119">Le locataire a au moins un abonnement (peut être de n’importe quel type).</span><span class="sxs-lookup"><span data-stu-id="3964a-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="3964a-120">Le rôle **contributeur** ou supérieur est attribué à l’utilisateur administrateur général pour l’abonnement choisi.</span><span class="sxs-lookup"><span data-stu-id="3964a-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="3964a-121">L’accès élevé à l’utilisateur administrateur général a la valeur **Oui** (voir [élever l’accès pour gérer tous les abonnements Azure et les groupes d’administration](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="3964a-121">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="3964a-122">Attribuer le rôle d’administrateur de la place de marché avec PowerShell</span><span class="sxs-lookup"><span data-stu-id="3964a-122">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="3964a-123">Utilisez le script PowerShell suivant pour attribuer le rôle d’administrateur de la place de marché. Il requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="3964a-123">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="3964a-124">**TenantId :** L’ID du locataire dans l’étendue (rôle d’administrateur de la place de marché est attribuable à l’étendue du locataire).</span><span class="sxs-lookup"><span data-stu-id="3964a-124">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="3964a-125">**SubscriptionId :** Un abonnement dont le rôle **collaborateur** ou supérieur est attribué à l’administrateur général.</span><span class="sxs-lookup"><span data-stu-id="3964a-125">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="3964a-126">**GlobalAdminUsername :** Nom d’utilisateur de l’administrateur général.</span><span class="sxs-lookup"><span data-stu-id="3964a-126">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="3964a-127">**UsernameToAssignRoleFor :** Nom d’utilisateur auquel le rôle d’administrateur de la place de marché sera attribué.</span><span class="sxs-lookup"><span data-stu-id="3964a-127">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="3964a-128">Pour les utilisateurs invités invités au locataire, la mise à disposition du rôle d’administrateur de la place de marché peut prendre jusqu’à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="3964a-128">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="3964a-129">Pour plus d’informations, consultez [propriétés d’un utilisateur Azure Active Directory B2B collaboration](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="3964a-129">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="3964a-130">Pour plus d’informations sur les applets de commande contenues dans le module PowerShell AZ. Portal, consultez [Microsoft Azure PowerShell : cmdlets du tableau de bord du portail](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="3964a-130">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="3964a-131">Créer une place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="3964a-131">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="3964a-132">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3964a-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3964a-133">Sélectionnez **tous les services** , puis **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="3964a-133">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portail Azure fenêtre principale.":::

3. <span data-ttu-id="3964a-135">Sélectionnez place de **marché privée** dans les options de gauche.</span><span class="sxs-lookup"><span data-stu-id="3964a-135">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Sélection de la place de marché privée dans la fenêtre principale de Portail Azure.":::

4. <span data-ttu-id="3964a-137">Sélectionnez **prise en main** pour créer une place de marché Azure privée (vous ne devez effectuer cette opération qu’une seule fois).</span><span class="sxs-lookup"><span data-stu-id="3964a-137">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Sélectionnez prise en main dans la fenêtre principale de Portail Azure.":::

    <span data-ttu-id="3964a-139">Si la place de marché Azure privée existe déjà pour ce locataire, l’option gérer la place de **marché** est sélectionnée par défaut.</span><span class="sxs-lookup"><span data-stu-id="3964a-139">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="3964a-140">Une fois l’opération terminée, vous disposez d’une place de marché Azure privée vide et désactivée.</span><span class="sxs-lookup"><span data-stu-id="3964a-140">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="L’écran place de marché Azure privé vide.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="3964a-142">Ajouter des éléments à partir de la Galerie</span><span class="sxs-lookup"><span data-stu-id="3964a-142">Add items from gallery</span></span>

<span data-ttu-id="3964a-143">Un élément est une combinaison d’une offre et d’un plan.</span><span class="sxs-lookup"><span data-stu-id="3964a-143">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="3964a-144">Vous pouvez rechercher et ajouter un élément dans la page gérer la place de marché.</span><span class="sxs-lookup"><span data-stu-id="3964a-144">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="3964a-145">Sélectionnez **Ajouter des éléments**.</span><span class="sxs-lookup"><span data-stu-id="3964a-145">Select **Add items**.</span></span>

2. <span data-ttu-id="3964a-146">Parcourez la **Galerie** ou utilisez le champ de recherche pour trouver l’élément de votre choix.</span><span class="sxs-lookup"><span data-stu-id="3964a-146">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navigation dans la galerie ou à l’aide du champ de recherche.":::

3. <span data-ttu-id="3964a-148">Par défaut, lors de l’ajout d’une nouvelle offre, tous les plans actuels sont ajoutés à la liste autorisée.</span><span class="sxs-lookup"><span data-stu-id="3964a-148">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="3964a-149">Pour modifier la sélection du plan avant d’ajouter les éléments sélectionnés, sélectionnez le menu déroulant dans la vignette de l’offre et mettez à jour les plans requis.</span><span class="sxs-lookup"><span data-stu-id="3964a-149">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mise à jour des plans requis.":::

4. <span data-ttu-id="3964a-151">Sélectionnez **terminé** en bas à gauche une fois que vous avez effectué vos sélections.</span><span class="sxs-lookup"><span data-stu-id="3964a-151">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="3964a-152">**Ajouter des éléments** à la place de marché sera disponible pour les offres non-Microsoft uniquement.</span><span class="sxs-lookup"><span data-stu-id="3964a-152">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="3964a-153">Les offres Microsoft sont autorisées par défaut.</span><span class="sxs-lookup"><span data-stu-id="3964a-153">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="3964a-154">Modifier les plans d’élément</span><span class="sxs-lookup"><span data-stu-id="3964a-154">Edit item plans</span></span>

<span data-ttu-id="3964a-155">Vous pouvez modifier les plans d’un élément dans la page gérer la place de marché.</span><span class="sxs-lookup"><span data-stu-id="3964a-155">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="3964a-156">Dans la colonne **plans** , passez en revue les plans disponibles dans le menu déroulant de cet élément.</span><span class="sxs-lookup"><span data-stu-id="3964a-156">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="3964a-157">Activez ou désactivez les cases à cocher pour choisir les plans à mettre à la disposition de vos utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="3964a-157">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Activez ou désactivez la case à cocher de l’élément requis.":::

> [!NOTE]
> <span data-ttu-id="3964a-159">Chaque offre doit avoir au moins un plan sélectionné pour que la mise à jour se produise.</span><span class="sxs-lookup"><span data-stu-id="3964a-159">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="3964a-160">Pour supprimer tous les plans associés à une offre, supprimez l’intégralité de l’offre (voir la section suivante).</span><span class="sxs-lookup"><span data-stu-id="3964a-160">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="3964a-161">Supprimer des offres</span><span class="sxs-lookup"><span data-stu-id="3964a-161">Delete offers</span></span>

<span data-ttu-id="3964a-162">Dans la page gérer le Marketplace, activez la case à cocher en regard du nom de l’offre (Voir l’écran ci-dessus), puis sélectionnez **Supprimer les éléments**.</span><span class="sxs-lookup"><span data-stu-id="3964a-162">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="3964a-163">Activer/désactiver la place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="3964a-163">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="3964a-164">Dans la page gérer la place de marché, vous verrez une de ces bannières, qui indiquent l’état actuel de la place de marché Azure privée :</span><span class="sxs-lookup"><span data-stu-id="3964a-164">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Bannière désactiver l’État":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Bannière activer l’État":::

<span data-ttu-id="3964a-167">Vous pouvez activer ou désactiver la place de marché Azure privée si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="3964a-167">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="3964a-168">S’il est désactivé, sélectionnez Activer la place de **marché privée** pour l’activer.</span><span class="sxs-lookup"><span data-stu-id="3964a-168">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="3964a-169">Si cette option est activée, sélectionnez Désactiver la place de **marché privée** pour la désactiver.</span><span class="sxs-lookup"><span data-stu-id="3964a-169">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="3964a-170">Navigation dans la place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="3964a-170">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="3964a-171">Lorsque la place de marché Azure privée est activée, les utilisateurs voient les plans que l’administrateur de la place de marché a autorisés.</span><span class="sxs-lookup"><span data-stu-id="3964a-171">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="3964a-172">Une notification **verte verte** indique une offre partenaire (non-Microsoft) qui est autorisée.</span><span class="sxs-lookup"><span data-stu-id="3964a-172">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="3964a-173">Un avis bleu **autorisé** indique une offre Microsoft autorisée.</span><span class="sxs-lookup"><span data-stu-id="3964a-173">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="3964a-174">Les utilisateurs peuvent filtrer les offres qui ne sont pas autorisées :</span><span class="sxs-lookup"><span data-stu-id="3964a-174">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Option de filtrage.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="3964a-176">Acheter ou déployer sur une place de marché Azure privée</span><span class="sxs-lookup"><span data-stu-id="3964a-176">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="3964a-177">Tandis que l’expérience de la page Détails du produit est similaire à la place de marché Azure publique, il existe trois scénarios spécifiques de la place de marché Azure privée.</span><span class="sxs-lookup"><span data-stu-id="3964a-177">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="3964a-178">Quand un utilisateur sélectionne un plan autorisé, le bouton **créer** est activé :</span><span class="sxs-lookup"><span data-stu-id="3964a-178">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Bannière d’offre : il est possible de créer un plan.":::

- <span data-ttu-id="3964a-180">Lorsqu’un utilisateur sélectionne un plan non autorisé, une bannière note que le plan n’est pas autorisé et que le bouton **créer** est désactivé.</span><span class="sxs-lookup"><span data-stu-id="3964a-180">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Bannière d’offre : il est impossible de créer un plan.":::

- <span data-ttu-id="3964a-182">Si une sélection de plan de produit n’apparaît pas dans la page Détails du produit mais que l’administrateur a approuvé un ou plusieurs plans, une bannière contient les plans autorisés et le bouton **créer** est activé :</span><span class="sxs-lookup"><span data-stu-id="3964a-182">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bannière de l’offre : il est possible de créer un plan et d’en présenter les plans disponibles.":::

## <a name="contact-support"></a><span data-ttu-id="3964a-184">Contactez le support technique</span><span class="sxs-lookup"><span data-stu-id="3964a-184">Contact support</span></span>

<span data-ttu-id="3964a-185">Pour obtenir de l’aide sur la place de marché Azure, visitez [le site Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="3964a-185">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
