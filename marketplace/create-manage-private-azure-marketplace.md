---
title: Créer et gérer une place de marché Azure privée dans le Portail Azure
description: En savoir plus sur la création et la gestion de la place de marché Azure privée (version préliminaire) dans le Portail Azure. La place de marché Azure privée (version préliminaire) permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712764"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Créer et gérer une place de marché Azure privée dans le Portail Azure

La place de marché Azure privée permet aux administrateurs de gérer les solutions tierces que leurs utilisateurs peuvent utiliser. Pour ce faire, il permet à l’utilisateur de déployer uniquement les offres approuvées par l’administrateur et de se conformer aux stratégies de votre entreprise. Avec la place de marché Azure privée, les utilisateurs peuvent rechercher dans le magasin en ligne des offres conformes à acheter et à déployer.

En tant qu’administrateur de la place de marché (rôle affecté), vous allez commencer avec un magasin privé désactivé et vide où vous pouvez ajouter vos offres et plans approuvés. Cet article explique comment attribuer le rôle nécessaire, créer un magasin privé, gérer des éléments, approuver des demandes d’utilisateur et activer la place de marché Azure privée pour vos utilisateurs.

> [!NOTE]
> - La place de marché Azure privée est au niveau du locataire, de sorte que tous les utilisateurs sous le locataire voient la même liste organisée.
> - Toutes les solutions Microsoft (y compris les [distributions Linux approuvées](/azure/virtual-machines/linux/endorsed-distros)) sont automatiquement ajoutées à la place de marché Azure privée.

## <a name="assign-the-marketplace-admin-role"></a>Attribuer le rôle d’administrateur de la place de marché

L’administrateur général du locataire doit attribuer le rôle d’administrateur de la place de **marché** à l’administrateur Azure Marketplace privé qui gérera le magasin privé.

>[!IMPORTANT]
> L’accès à la gestion de la place de marché Azure privée est uniquement disponible pour les administrateurs informatiques avec le rôle d’administrateur de la place de marché affecté.

### <a name="prerequisites"></a>Prérequis

Ces conditions préalables sont requises pour que vous puissiez attribuer le rôle d’administrateur de la place de marché à un utilisateur sur l’étendue du locataire :

- Vous avez accès à un utilisateur **administrateur général** .
- Le locataire a au moins un abonnement (peut être de n’importe quel type).
- Le rôle **contributeur** ou supérieur est attribué à l’utilisateur administrateur général pour l’abonnement choisi.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Attribuer le rôle d’administrateur de la place de marché avec le contrôle d’accès (IAM)

1. Connectez-vous au [portail Azure](https://portal.azure.com/).
1. Sélectionnez **tous les services** , puis **Marketplace**.
1. Sélectionnez place de **marché privée** dans le menu de gauche.

    [![Affiche l’option de menu place de marché privée sur le côté gauche de la place de marché.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Sélectionnez **contrôle d’accès (IAM)** pour affecter le rôle d’administrateur de la place de marché.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Affiche l’écran de contrôle d’accès I A M.":::

1. Sélectionnez **+ Ajouter** > **Ajouter une attribution de rôle**.
1. Sous **rôle**, choisissez **administrateur** de la place de marché.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Affiche le menu attribution de rôle.":::

1. Sélectionnez l’utilisateur souhaité dans la liste déroulante, puis sélectionnez **terminé**.

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

Pour plus d’informations sur les applets de commande contenues dans le module PowerShell AZ. Portal, consultez [Microsoft Azure PowerShell : cmdlets du tableau de bord du portail](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Créer une place de marché Azure privée

1. Connectez-vous au [portail Azure](https://portal.azure.com/).
2. Sélectionnez **tous les services** , puis **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Affiche la fenêtre principale de Portail Azure.":::

3. Sélectionnez place de **marché privée** dans le menu de gauche.

4. Sélectionnez **prise en main** pour créer une place de marché Azure privée (vous ne devez effectuer cette opération qu’une seule fois).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Montre comment sélectionner la fenêtre principale « prise en main de la Portail Azure ».":::

    Si la place de marché Azure privée existe déjà pour ce locataire, l’option gérer la place de **marché** est sélectionnée par défaut.

5. Une fois l’opération terminée, vous disposez d’une place de marché Azure privée vide et désactivée.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Affiche l’écran de la place de marché Azure privée vide.":::

## <a name="add-items-from-gallery"></a>Ajouter des éléments à partir de la Galerie

Un élément est une combinaison d’une offre et d’un plan. Vous pouvez rechercher et ajouter des éléments sur la page gérer la place de marché.

1. Sélectionnez **Ajouter des éléments**.

2. Parcourez la **Galerie** ou utilisez le champ de recherche pour trouver l’élément de votre choix.

    [![Montre comment parcourir la galerie ou utiliser le champ de recherche.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Par défaut, lors de l’ajout d’une nouvelle offre, tous les plans actuels sont ajoutés à la liste approuvée. Pour modifier la sélection du plan avant d’ajouter les éléments sélectionnés, sélectionnez le menu déroulant dans la vignette de l’offre et mettez à jour les plans requis.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Montre comment mettre à jour les plans requis.":::

4. Sélectionnez **terminé** en bas à gauche une fois que vous avez effectué vos sélections.

>[!Note]
> **Ajouter des éléments** à la place de marché sera disponible pour les offres non-Microsoft uniquement. Les solutions Microsoft (y compris les [distributions Linux](/azure/virtual-machines/linux/endorsed-distros)approuvées) sont marquées comme « approuvées par défaut » et ne peuvent pas être gérées dans la place de marché privée.

## <a name="edit-items-plans"></a>Modifier les plans de l’élément

Vous pouvez modifier les plans d’un élément sur la page gérer la place de marché.

1. Dans la colonne **plans** , passez en revue les plans disponibles dans le menu déroulant de cet élément.
2. Activez ou désactivez les cases à cocher pour choisir les plans à mettre à la disposition de vos utilisateurs.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Montre comment activer ou désactiver la case à cocher pour l’élément requis.":::

> [!NOTE]
> Chaque offre doit avoir au moins un plan sélectionné pour que la mise à jour se produise. Pour supprimer tous les plans associés à une offre, supprimez l’intégralité de l’offre (voir la section suivante).

## <a name="delete-offers"></a>Supprimer des offres

Dans la page gérer le Marketplace, activez la case à cocher en regard du nom de l’offre (Voir l’écran ci-dessus), puis sélectionnez **Supprimer les éléments**.

## <a name="enabledisable-private-azure-marketplace"></a>Activer/désactiver la place de marché Azure privée

Dans la page gérer la place de marché, vous verrez une de ces bannières, qui indiquent l’état actuel de la place de marché Azure privée :

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Affiche la bannière « désactiver l’État ».":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Affiche la bannière « activer l’État ».":::

Vous pouvez activer ou désactiver la place de marché Azure privée si nécessaire.

- S’il est désactivé, sélectionnez Activer la place de **marché privée** pour l’activer.
- Si cette option est activée, sélectionnez Désactiver la place de **marché privée** pour la désactiver.

## <a name="private-azure-marketplace-notification-center"></a>Centre de notifications de la place de marché Azure privé

Le centre de notifications se compose de trois types de notifications et permet à l’administrateur de la place de marché d’effectuer des actions en fonction de la notification :

- Demandes d’approbation des utilisateurs pour les éléments qui ne figurent pas dans la liste approuvée (consultez la [demande d’ajout d’offres ou de plans](#request-to-add-offers-or-plans) ci-dessous).
- Nouvelles notifications de plan pour les offres qui disposent déjà d’un ou plusieurs plans dans la liste approuvée.
- Suppression des notifications de plan pour les éléments qui se trouvent dans la liste approuvée, mais qui ont été supprimés de la place de marché Azure globale.

Pour accéder au centre de notifications :

1. Sélectionnez **notifications** dans le menu de gauche.

    [![Affiche le menu notifications.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Sélectionnez le menu de points de suspension pour plus d’actions.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Affiche les résultats du menu plus d’options.":::

1. Pour les demandes de plan, **afficher les demandes** ouvre le formulaire de demande d’approbation dans lequel vous pouvez consulter toutes les demandes d’utilisateur pour l’offre spécifique.
1. Sélectionnez **approuver** ou **rejeter**.

    [![Affiche les options approuver et rejeter.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Sélectionnez le plan à approuver dans le menu déroulant.
1. Ajoutez un commentaire et sélectionnez **Envoyer**.

## <a name="browsing-private-azure-marketplace"></a>Navigation dans la place de marché Azure privée

Lorsque la place de marché Azure privée est activée, les utilisateurs voient les plans approuvés par l’administrateur de la place de marché.

- Une notification verte **approuvée** indique une offre partenaire (non-Microsoft) approuvée.
- Une notification bleue **approuvée** indique une offre Microsoft (y compris les [distributions Linux](/azure/virtual-machines/linux/endorsed-distros)approuvées) approuvée.

Les utilisateurs peuvent filtrer les offres qui ne sont pas approuvées :

[![Affiche l’option de filtrage.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Acheter ou déployer sur une place de marché Azure privée

Bien que l’expérience de la page Détails du produit soit similaire à la place de marché Azure mondiale, il existe trois scénarios spécifiques à Azure Marketplace.

- Quand un utilisateur sélectionne un plan approuvé, le bouton **créer** est activé :

    [![Affiche la bannière d’offre indiquant qu’un plan peut être créé.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Si une sélection de plan de produit n’apparaît pas dans la page Détails du produit mais que l’administrateur a approuvé un ou plusieurs plans, une bannière indique les plans qui sont approuvés et le bouton **créer** est activé :

    [![Affiche la bannière d’offre indiquant qu’un plan peut être créé et afficher les plans disponibles.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Lorsqu’un utilisateur sélectionne un plan non approuvé, une bannière note le plan comme non approuvé et le bouton **créer** est désactivé. L’utilisateur peut toujours demander à ajouter le plan à la liste approuvée (voir la section suivante).

## <a name="request-to-add-offers-or-plans"></a>Demande d’ajout d’offres ou de plans

Vous pouvez demander à ajouter une offre ou un plan public qui n’est pas actuellement approuvé dans la place de marché Azure privée.

1. Sélectionnez **demander à ajouter** dans la bannière pour ouvrir le **formulaire de demande d’accès**.

    [![Affiche la bannière avec le lien « demander à ajouter ».](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Affiche le formulaire de demande d’accès pour les offres ou les plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Sélectionnez les plans à ajouter à la demande (**tout plan** indique à l’administrateur de la place de marché que vous n’avez pas de préférence pour un plan dans une offre).

1. Ajoutez une **Justification** et sélectionnez **demander** pour envoyer votre demande.
  
    [![Affiche le formulaire de demande d’accès pour les offres ou les plans avec des exemples d’entrées.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Une indication pour une demande en attente apparaît dans le formulaire de demande d’accès avec une option de retrait de la **demande**.

    [![Affiche la liste des plans approuvés ou en attente avec le lien de demande de retrait.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Une fois soumis, le formulaire de demande d’approbation est envoyé au [Centre de notifications](#private-azure-marketplace-notification-center) pour que l’administrateur de la place de marché examine la demande et effectue une action.

## <a name="frequently-asked-questions-faqs"></a>Forum Aux Questions (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Je bloque déjà l’application tierce de la place de marché via Azure Policy. En quoi cela diffère-t-il ?

Il existe actuellement deux façons de limiter les services tiers dans la place de marché :

1. Via le portail EA ou le Portail Azure, désactivez les services tiers ou limitez-les uniquement à des références SKU libres ou BYOL.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Montre comment restreindre les services de la Portail Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Montre comment restreindre les services dans le portail E A.":::

2. Créez une stratégie Azure pour autoriser uniquement des machines virtuelles spécifiques. Pour plus d’informations sur la façon d’appliquer une stratégie à des machines virtuelles Windows, consultez [appliquer des stratégies à des machines virtuelles Windows avec Azure Resource Manager](/azure/virtual-machines/windows/policy).

La place de marché Azure privée offre davantage de souplesse pour limiter et autoriser des offres et des plans spécifiques. Il informe les utilisateurs finaux sur la disponibilité du déploiement dans la Galerie de la place de marché même avant d’essayer de déployer des services tiers. Pour autoriser le déploiement de services tiers, définissez la place de marché Azure sur activé/activé dans le portail EA et le Portail Azure.

- La place de marché Azure privée peut organiser des solutions de partenaires non limitées aux machines virtuelles.
- La place de marché Azure privée peut être organisée au niveau du plan et peut également définir le « plan actuel et futur ».
- La place de marché Azure privée peut informer les utilisateurs finaux sur ce qui peut et ne peut pas être déployé.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Quelle est la différence entre une offre privée et une place de marché Azure privée ?

Une **offre privée** permet aux éditeurs de créer des plans qui sont uniquement visibles par les clients ciblés. Cela leur permet de partager en privé des solutions personnalisées avec la tarification négociée, les conditions générales et les configurations spécialisées. Pour plus d’informations, consultez [les offres privées dans le Marketplace commercial](/azure/marketplace/private-offers).

La place de **marché Azure privée** dans le portail Azure permet aux administrateurs de préapprouver les solutions tierces que leurs utilisateurs peuvent déployer. Avec une place de marché Azure privée, les utilisateurs peuvent profiter des avantages de la place de marché Azure en recherchant, en achetant et en déployant des offres conformes. Pour gérer les offres privées basées sur un abonnement dans la place de marché privé, l’administrateur de la place de marché doit avoir au minimum le rôle de « lecture » sur l’abonnement spécifique.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>J’ai ajouté une offre privée à la place de marché Azure privée, pourquoi ne s’est-elle pas affichée dans l’onglet gérer la place de marché ?

Les offres privées basées sur un abonnement sont visibles uniquement pour les abonnements répertoriés dans les paramètres de l’offre privée. Pour afficher l’offre privée, assurez-vous que le filtre d’abonnement global affiche tous les abonnements.

[![Affiche le filtre place de marché privé.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Pouvez-vous inclure des images personnalisées dans la place de marché Azure privée ?

Non. La place de marché Azure privée permet à n’importe quel administrateur informatique de gérer et d’organiser des solutions tierces à partir de la place de marché Azure mondiale. Étant donné que les images personnalisées ne se trouvent pas sur la place de marché Azure globale, l’administrateur informatique ne peut pas choisir vos images personnalisées. Si vous souhaitez partager des images personnalisées, utilisez la [Galerie d’images partagées](/azure/virtual-machines/shared-image-galleries).

1. Guide pas à pas de création d’une bibliothèque d’images partagées (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Créer une définition d’image dans un SIG. Le client doit choisir **généralisée** pour le champ de l’état du système d’exploitation. ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Placez l’image managée dans la Galerie d’images partagées ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Les images de machine virtuelle SIG se trouvent dans un seul abonnement. Pour le rendre disponible pour d’autres abonnements, utilisez une inscription d’application ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Pourquoi certaines offres sont-elles **approuvées par défaut,** même si le serveur de publication n’est pas Microsoft ?

Microsoft prend en charge les technologies Linux et open source dans Azure. Les [distributions Linux approuvées](/azure/virtual-machines/linux/endorsed-distros) sont prises en charge sur Azure et le prix est intégré aux machines virtuelles. Étant donné que l’agent Linux Azure est déjà préinstallé sur la place de marché Azure, il est traité comme une offre Microsoft. Étant donné que les offres Microsoft sont approuvées par défaut, les distributions Linux approuvées ne peuvent pas être gérées dans la place de marché Azure privée et sont approuvées par défaut.

## <a name="contact-support"></a>Contacter le support technique

- Pour obtenir de l’aide sur la place de marché Azure, visitez [le site Microsoft Q&A](/answers/products/).