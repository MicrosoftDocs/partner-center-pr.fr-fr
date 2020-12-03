---
title: 'Démarrage rapide : gérer une place de marché Azure privée à l’aide de PowerShell'
description: Ce guide de démarrage rapide vous montre comment gérer les offres dans une place de marché Azure privée à l’aide de Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536078"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Démarrage rapide : gérer une place de marché Azure privée à l’aide de PowerShell

Cet article décrit comment vous pouvez gérer les offres dans une place de marché Azure privée à l’aide du module PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .

> [!IMPORTANT]
> La place de marché Azure privée est actuellement en version préliminaire publique. Cette préversion est fournie sans contrat de niveau de service. Il n’est pas recommandé pour les charges de travail de production. Certaines fonctionnalités peuvent être limitées ou non prises en charge. Pour plus d’informations, consultez [Conditions d’Utilisation Supplémentaires relatives aux Évaluations Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Spécifications

* Si vous n’avez pas d’abonnement Azure, créez un compte [gratuit](https://azure.microsoft.com/free/) avant de commencer.

* Si vous choisissez d’utiliser Azure PowerShell localement :
  * [Installez le module PowerShell Az](/powershell/azure/install-az-ps).
  * Connectez-vous à votre compte Azure à l’aide de la cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).
* Si vous choisissez d’utiliser Azure Cloud Shell :
  * Pour plus d’informations, consultez [Vue d’ensemble d’Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview).

  > [!IMPORTANT]
  > Tandis que le module PowerShell **AZ. Marketplace** est en version préliminaire, vous devez l’installer séparément à l’aide de l’applet de commande `Install-Module` . Une fois que ce module PowerShell sera en disponibilité générale, il fera partie intégrante des versions futures du module Az PowerShell et sera disponible par défaut dans Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Si vous avez plusieurs abonnements Azure, sélectionnez l’abonnement approprié dans lequel les ressources doivent être facturées. Sélectionnez un abonnement spécifique avec l’applet de commande [Set-AzContext](/powershell/module/az.accounts/set-azcontext).

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Répertorier les magasins privés

Pour récupérer une liste de magasins privés, vous utilisez l’applet de commande [AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) . L’exemple suivant répertorie les magasins privés qui ont été créés sous l’étendue du locataire.

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a>Ajouter une offre à une place de marché privée

Pour ajouter une offre à un magasin privé, vous utilisez l’applet de commande [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) . L’exemple suivant ajoute l’offre spécifiée à une place de marché privée pour un magasin privé créé sous l’étendue du locataire.

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a>Procurez-vous des offres de magasin privé

Pour obtenir une ou plusieurs offres de magasin privé, vous utilisez l’applet de commande [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) . L’exemple suivant obtient les offres associées au magasin privé spécifié qui ont été ajoutées sous l’étendue du locataire.

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a>Supprimer une offre

Pour supprimer une offre d’un magasin privé, vous utilisez l’applet de commande [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) . L’exemple suivant supprime une offre d’un magasin privé qui a été créé dans l’étendue du locataire.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Étapes suivantes

[Créer et gérer une place de marché Azure privée](create-manage-private-azure-marketplace.md).
