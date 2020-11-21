---
title: Créer et gérer une place de marché Azure privée dans Portail Azure
description: En savoir plus sur la création et la gestion de la place de marché Azure privée (version préliminaire) dans le Portail Azure.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006937"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Créer et gérer une place de marché Azure privée (version préliminaire) dans le Portail Azure

La place de marché Azure privée (version préliminaire) permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser. Pour ce faire, il vous permet de déployer uniquement les offres que vous approuvez et qui sont conformes aux stratégies de votre entreprise. Avec la place de marché Azure privée, vos utilisateurs peuvent rechercher des offres conformes à acheter et à déployer dans le magasin en ligne. 

En tant qu’administrateur de la place de marché (rôle affecté), vous allez commencer avec un magasin privé désactivé et vide où vous pouvez ajouter vos offres et plans approuvés. Cet article explique comment créer, gérer et activer la place de marché Azure privée pour vos utilisateurs.

Remarques :

- La place de marché Azure privée est au niveau du locataire, de sorte que tous les utilisateurs sous le locataire voient la même liste organisée.
- Toutes les solutions Microsoft sont automatiquement ajoutées à la place de marché Azure privée.

## <a name="assign-the-marketplace-admin-role"></a>Attribuer le rôle d’administrateur de la place de marché

L’administrateur général du locataire doit attribuer le rôle d’administrateur de la place de **marché** à l’administrateur Azure Marketplace privé qui gérera le magasin privé.

>[!IMPORTANT]
> L’accès à la gestion de la place de marché Azure privée est uniquement disponible pour les administrateurs informatiques avec le rôle d’administrateur de la place de marché affecté.

### <a name="prerequisites"></a>Prérequis

Vous devez respecter ces conditions préalables avant de pouvoir attribuer le rôle d’administrateur de la place de marché à un utilisateur sur l’étendue du locataire :

- Vous avez accès à un utilisateur **administrateur général** .
- Le locataire a au moins un abonnement (peut être de n’importe quel type).
- Le rôle **contributeur** ou supérieur est attribué à l’utilisateur administrateur général pour l’abonnement choisi.
- L’accès élevé à l’utilisateur administrateur général a la valeur **Oui** (voir [élever l’accès pour gérer tous les abonnements Azure et les groupes d’administration](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Attribuer le rôle d’administrateur de la place de marché avec PowerShell

Utilisez le script PowerShell suivant pour attribuer le rôle d’administrateur de la place de marché. Il requiert les paramètres suivants :

- **TenantId :** L’ID du locataire dans l’étendue (rôle d’administrateur de la place de marché est attribuable à l’étendue du locataire).
- **SubscriptionId :** Un abonnement dont le rôle **collaborateur** ou supérieur est attribué à l’administrateur général.
- **GlobalAdminUsername :** Nom d’utilisateur de l’administrateur général.
- **UsernameToAssignRoleFor :** Nom d’utilisateur auquel le rôle d’administrateur de la place de marché sera attribué.

> [!NOTE]
> Pour les utilisateurs invités invités au locataire, la mise à disposition du rôle d’administrateur de la place de marché peut prendre jusqu’à 48 heures. Pour plus d’informations, consultez [propriétés d’un utilisateur Azure Active Directory B2B collaboration](/azure/active-directory/b2b/user-properties).

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

Pour plus d’informations sur les applets de commande contenues dans le module PowerShell AZ. Portal, consultez [Microsoft Azure PowerShell : cmdlets du tableau de bord du portail](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Créer une place de marché Azure privée

1. Connectez-vous au [portail Azure](https://portal.azure.com/).
2. Sélectionnez **tous les services** , puis **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portail Azure fenêtre principale.":::

3. Sélectionnez place de **marché privée** dans les options de gauche.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Sélection de la place de marché privée dans la fenêtre principale de Portail Azure.":::

4. Sélectionnez **prise en main** pour créer une place de marché Azure privée (vous ne devez effectuer cette opération qu’une seule fois).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Sélectionnez prise en main dans la fenêtre principale de Portail Azure.":::

    Si la place de marché Azure privée existe déjà pour ce locataire, l’option gérer la place de **marché** est sélectionnée par défaut.

5. Une fois l’opération terminée, vous disposez d’une place de marché Azure privée vide et désactivée.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="L’écran place de marché Azure privé vide.":::

## <a name="add-items-from-gallery"></a>Ajouter des éléments à partir de la Galerie

Un élément est une combinaison d’une offre et d’un plan. Vous pouvez rechercher et ajouter un élément dans la page gérer la place de marché.

1. Sélectionnez **Ajouter des éléments**.

2. Parcourez la **Galerie** ou utilisez le champ de recherche pour trouver l’élément de votre choix.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Navigation dans la galerie ou à l’aide du champ de recherche.":::

3. Par défaut, lors de l’ajout d’une nouvelle offre, tous les plans actuels sont ajoutés à la liste autorisée. Pour modifier la sélection du plan avant d’ajouter les éléments sélectionnés, sélectionnez le menu déroulant dans la vignette de l’offre et mettez à jour les plans requis.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Mise à jour des plans requis.":::

4. Sélectionnez **terminé** en bas à gauche une fois que vous avez effectué vos sélections.

>[!Note]
> **Ajouter des éléments** à la place de marché sera disponible pour les offres non-Microsoft uniquement. Les offres Microsoft sont autorisées par défaut.

## <a name="edit-item-plans"></a>Modifier les plans d’élément

Vous pouvez modifier les plans d’un élément dans la page gérer la place de marché.

1. Dans la colonne **plans** , passez en revue les plans disponibles dans le menu déroulant de cet élément.
2. Activez ou désactivez les cases à cocher pour choisir les plans à mettre à la disposition de vos utilisateurs.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Activez ou désactivez la case à cocher de l’élément requis.":::

> [!NOTE]
> Chaque offre doit avoir au moins un plan sélectionné pour que la mise à jour se produise. Pour supprimer tous les plans associés à une offre, supprimez l’intégralité de l’offre (voir la section suivante).

## <a name="delete-offers"></a>Supprimer des offres

Dans la page gérer le Marketplace, activez la case à cocher en regard du nom de l’offre (Voir l’écran ci-dessus), puis sélectionnez **Supprimer les éléments**.

## <a name="enabledisable-private-azure-marketplace"></a>Activer/désactiver la place de marché Azure privée

Dans la page gérer la place de marché, vous verrez une de ces bannières, qui indiquent l’état actuel de la place de marché Azure privée :

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Bannière désactiver l’État":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Bannière activer l’État":::

Vous pouvez activer ou désactiver la place de marché Azure privée si nécessaire.

1. S’il est désactivé, sélectionnez Activer la place de **marché privée** pour l’activer.
2. Si cette option est activée, sélectionnez Désactiver la place de **marché privée** pour la désactiver.

## <a name="browsing-private-azure-marketplace"></a>Navigation dans la place de marché Azure privée

Lorsque la place de marché Azure privée est activée, les utilisateurs voient les plans que l’administrateur de la place de marché a autorisés.

- Une notification **verte verte** indique une offre partenaire (non-Microsoft) qui est autorisée.
- Un avis bleu **autorisé** indique une offre Microsoft autorisée.

Les utilisateurs peuvent filtrer les offres qui ne sont pas autorisées :

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Option de filtrage.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Acheter ou déployer sur une place de marché Azure privée

Tandis que l’expérience de la page Détails du produit est similaire à la place de marché Azure publique, il existe trois scénarios spécifiques de la place de marché Azure privée.

- Quand un utilisateur sélectionne un plan autorisé, le bouton **créer** est activé :

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Bannière d’offre : il est possible de créer un plan.":::

- Lorsqu’un utilisateur sélectionne un plan non autorisé, une bannière note que le plan n’est pas autorisé et que le bouton **créer** est désactivé.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Bannière d’offre : il est impossible de créer un plan.":::

- Si une sélection de plan de produit n’apparaît pas dans la page Détails du produit mais que l’administrateur a approuvé un ou plusieurs plans, une bannière contient les plans autorisés et le bouton **créer** est activé :

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Bannière de l’offre : il est possible de créer un plan et d’en présenter les plans disponibles.":::

## <a name="contact-support"></a>Contacter le support technique

Pour obtenir de l’aide sur la place de marché Azure, visitez [le site Microsoft Q&A](/answers/products/). 
