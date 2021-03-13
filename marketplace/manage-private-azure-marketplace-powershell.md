---
title: 'Démarrage rapide : gérer une place de marché Azure privée à l’aide de PowerShell'
description: Ce guide de démarrage rapide vous montre comment gérer les offres dans une place de marché Azure privée à l’aide de Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412452"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="05e9d-103">Démarrage rapide : gérer une place de marché Azure privée à l’aide de PowerShell</span><span class="sxs-lookup"><span data-stu-id="05e9d-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="05e9d-104">Cet article décrit comment vous pouvez gérer les offres dans une place de marché Azure privée à l’aide du module PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="05e9d-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="05e9d-105">La place de marché Azure privée est actuellement en version préliminaire publique.</span><span class="sxs-lookup"><span data-stu-id="05e9d-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="05e9d-106">Cette préversion est fournie sans contrat de niveau de service.</span><span class="sxs-lookup"><span data-stu-id="05e9d-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="05e9d-107">Il n’est pas recommandé pour les charges de travail de production.</span><span class="sxs-lookup"><span data-stu-id="05e9d-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="05e9d-108">Certaines fonctionnalités peuvent être limitées ou non prises en charge.</span><span class="sxs-lookup"><span data-stu-id="05e9d-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="05e9d-109">Pour plus d’informations, consultez [Conditions d’Utilisation Supplémentaires relatives aux Évaluations Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="05e9d-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="05e9d-110">Spécifications</span><span class="sxs-lookup"><span data-stu-id="05e9d-110">Requirements</span></span>

* <span data-ttu-id="05e9d-111">Si vous n’avez pas d’abonnement Azure, créez un compte [gratuit](https://azure.microsoft.com/free/) avant de commencer.</span><span class="sxs-lookup"><span data-stu-id="05e9d-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="05e9d-112">Si vous choisissez d’utiliser Azure PowerShell localement :</span><span class="sxs-lookup"><span data-stu-id="05e9d-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="05e9d-113">[Installez le module PowerShell Az](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="05e9d-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="05e9d-114">Connectez-vous à votre compte Azure à l’aide de la cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="05e9d-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="05e9d-115">Si vous choisissez d’utiliser Azure Cloud Shell :</span><span class="sxs-lookup"><span data-stu-id="05e9d-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="05e9d-116">Pour plus d’informations, consultez [Vue d’ensemble d’Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="05e9d-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="05e9d-117">Tandis que le module PowerShell **AZ. Marketplace** est en version préliminaire, vous devez l’installer séparément à l’aide de l’applet de commande `Install-Module` .</span><span class="sxs-lookup"><span data-stu-id="05e9d-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="05e9d-118">Une fois que ce module PowerShell sera en disponibilité générale, il fera partie intégrante des versions futures du module Az PowerShell et sera disponible par défaut dans Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="05e9d-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="05e9d-119">Si vous avez plusieurs abonnements Azure, sélectionnez l’abonnement approprié dans lequel les ressources doivent être facturées.</span><span class="sxs-lookup"><span data-stu-id="05e9d-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="05e9d-120">Sélectionnez un abonnement spécifique avec l’applet de commande [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="05e9d-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="05e9d-121">Répertorier les magasins privés</span><span class="sxs-lookup"><span data-stu-id="05e9d-121">List private stores</span></span>

<span data-ttu-id="05e9d-122">Pour récupérer une liste de magasins privés, vous utilisez l’applet de commande [AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="05e9d-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="05e9d-123">L’exemple suivant répertorie les magasins privés qui ont été créés sous l’étendue du locataire.</span><span class="sxs-lookup"><span data-stu-id="05e9d-123">The following example lists private stores that were created under the tenant scope.</span></span>

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

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="05e9d-124">Ajouter une offre à une place de marché privée</span><span class="sxs-lookup"><span data-stu-id="05e9d-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="05e9d-125">Pour ajouter une offre à un magasin privé, vous utilisez l’applet de commande [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="05e9d-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="05e9d-126">L’exemple suivant ajoute l’offre spécifiée à une place de marché privée pour un magasin privé créé sous l’étendue du locataire.</span><span class="sxs-lookup"><span data-stu-id="05e9d-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

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

## <a name="get-private-store-offers"></a><span data-ttu-id="05e9d-127">Procurez-vous des offres de magasin privé</span><span class="sxs-lookup"><span data-stu-id="05e9d-127">Get private store offers</span></span>

<span data-ttu-id="05e9d-128">Pour obtenir une ou plusieurs offres de magasin privé, vous utilisez l’applet de commande [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="05e9d-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="05e9d-129">L’exemple suivant obtient les offres associées au magasin privé spécifié qui ont été ajoutées sous l’étendue du locataire.</span><span class="sxs-lookup"><span data-stu-id="05e9d-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

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

## <a name="remove-an-offer"></a><span data-ttu-id="05e9d-130">Supprimer une offre</span><span class="sxs-lookup"><span data-stu-id="05e9d-130">Remove an offer</span></span>

<span data-ttu-id="05e9d-131">Pour supprimer une offre d’un magasin privé, vous utilisez l’applet de commande [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="05e9d-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="05e9d-132">L’exemple suivant supprime une offre d’un magasin privé qui a été créé dans l’étendue du locataire.</span><span class="sxs-lookup"><span data-stu-id="05e9d-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="05e9d-133">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="05e9d-133">Next steps</span></span>

<span data-ttu-id="05e9d-134">[Créer et gérer une place de marché Azure privée](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="05e9d-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>