---
title: Types de frais de fichier de réconciliation | Espace partenaires
ms.topic: article
ms.date: 08/26/2019
description: Types de frais (basés sur une licence, basés sur l’utilisation et exceptionnels), crédits et remises sur les fichiers de rapprochement de l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389807"
---
# <a name="understand-charge-types"></a><span data-ttu-id="41b0e-103">Présentation des types de frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-103">Understand charge types</span></span>

<span data-ttu-id="41b0e-104">S’applique à :</span><span class="sxs-lookup"><span data-stu-id="41b0e-104">Applies to:</span></span>

- <span data-ttu-id="41b0e-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="41b0e-105">Partner Center</span></span>
- <span data-ttu-id="41b0e-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="41b0e-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="41b0e-107">Cette rubrique décrit les mappages entre une section de facture et les types de frais associés qui peuvent se trouver dans votre fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="41b0e-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="41b0e-108">Votre facture fournit un résumé des frais.</span><span class="sxs-lookup"><span data-stu-id="41b0e-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="41b0e-109">Votre fichier de réconciliation fournit une répartition détaillée des transactions d’éléments de ligne, y compris les types de frais.</span><span class="sxs-lookup"><span data-stu-id="41b0e-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="41b0e-110">Pour plus d’informations sur les fichiers de rapprochement, voir [How to use Reconciliation Files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="41b0e-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="41b0e-111">Les fichiers de [réconciliation basés sur l’utilisation](usage-based-recon-files.md) et les [fichiers de réconciliation basés sur des licences](license-based-recon-files.md) affichent uniquement les transactions et les frais liés à l’utilisation (unités consommées et frais connexes).</span><span class="sxs-lookup"><span data-stu-id="41b0e-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="41b0e-112">Les crédits uniques, les remises ou les remboursements qui apparaissent sur la facture en tant qu' **ajustements** ne sont pas affichés dans le fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="41b0e-113">Mapper les types de frais aux frais de facture</span><span class="sxs-lookup"><span data-stu-id="41b0e-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="41b0e-114">Pour faire référence à des montants de frais entre votre facture et le fichier de réconciliation, utilisez les options de filtre dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="41b0e-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="41b0e-115">Filtrez par types de frais sur votre fichier de rapprochement pour mapper les frais de facture à un ensemble de répartitions de frais sur le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="41b0e-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="41b0e-116">Frais basés sur la licence</span><span class="sxs-lookup"><span data-stu-id="41b0e-116">License-based charges</span></span>

<span data-ttu-id="41b0e-117">Pour mapper ces frais basés sur des licences à votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="41b0e-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="41b0e-118">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="41b0e-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="41b0e-119">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="41b0e-120">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="41b0e-120">Activation fee</span></span> | <span data-ttu-id="41b0e-121">Montant facturé au client lorsqu’il utilise l’abonnement après l’achat.</span><span class="sxs-lookup"><span data-stu-id="41b0e-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="41b0e-122">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="41b0e-122">Cancel fee</span></span> | <span data-ttu-id="41b0e-123">Frais au prorata remboursés au client lors de la modification des sièges associés.</span><span class="sxs-lookup"><span data-stu-id="41b0e-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="41b0e-124">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="41b0e-124">Cycle fee</span></span> | <span data-ttu-id="41b0e-125">Frais périodiques pour un abonnement.</span><span class="sxs-lookup"><span data-stu-id="41b0e-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="41b0e-126">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="41b0e-126">Cycle instance prorate</span></span> | <span data-ttu-id="41b0e-127">Frais au prorata calculés par le client lors de la modification des sièges associés.</span><span class="sxs-lookup"><span data-stu-id="41b0e-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="41b0e-128">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="41b0e-128">Prorate fees when cancel</span></span> | <span data-ttu-id="41b0e-129">Remboursement calculé au prorata pour la partie inutilisée du service lors de l’annulation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="41b0e-130">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="41b0e-130">Prorate fees when purchase</span></span> | <span data-ttu-id="41b0e-131">Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle.</span><span class="sxs-lookup"><span data-stu-id="41b0e-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="41b0e-132">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="41b0e-132">Purchase fee</span></span> | <span data-ttu-id="41b0e-133">Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle.</span><span class="sxs-lookup"><span data-stu-id="41b0e-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="41b0e-134">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="41b0e-134">Prorate fee when renew</span></span> | <span data-ttu-id="41b0e-135">Frais au prorata lors du renouvellement de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="41b0e-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="41b0e-136">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="41b0e-136">Renew fee</span></span> | <span data-ttu-id="41b0e-137">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="41b0e-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="41b0e-138">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="41b0e-138">Prorate fees when activate</span></span> | <span data-ttu-id="41b0e-139">> des frais au prorata de l’activation jusqu’à la fin de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="41b0e-140">Frais à usage unique</span><span class="sxs-lookup"><span data-stu-id="41b0e-140">One-time charges</span></span>

<span data-ttu-id="41b0e-141">Pour mapper ces frais à la fois sur votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="41b0e-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="41b0e-142">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="41b0e-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="41b0e-143">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="41b0e-144">Nouveau</span><span class="sxs-lookup"><span data-stu-id="41b0e-144">New</span></span> | <span data-ttu-id="41b0e-145">Utilisé lors de la création d’un nouvel achat.</span><span class="sxs-lookup"><span data-stu-id="41b0e-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="41b0e-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="41b0e-146">addQuantity</span></span> | <span data-ttu-id="41b0e-147">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une augmentation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="41b0e-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="41b0e-148">removeQuantity</span></span> | <span data-ttu-id="41b0e-149">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une diminution.</span><span class="sxs-lookup"><span data-stu-id="41b0e-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="41b0e-150">Cancel</span><span class="sxs-lookup"><span data-stu-id="41b0e-150">Cancel</span></span> | <span data-ttu-id="41b0e-151">Utilisé lors de l’annulation d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="41b0e-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="41b0e-152">Convertir</span><span class="sxs-lookup"><span data-stu-id="41b0e-152">Convert</span></span> | <span data-ttu-id="41b0e-153">Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé.</span><span class="sxs-lookup"><span data-stu-id="41b0e-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="41b0e-154">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="41b0e-154">Usage charges</span></span>

<span data-ttu-id="41b0e-155">Pour mapper ces frais d’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="41b0e-156">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="41b0e-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="41b0e-157">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="41b0e-158">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="41b0e-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="41b0e-159">Frais d’utilisation de l’accès en cas d’annulation pour une utilisation sans paiement durant la période de facturation actuelle.</span><span class="sxs-lookup"><span data-stu-id="41b0e-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="41b0e-160">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="41b0e-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="41b0e-161">Frais d’utilisation de l’accès pour la période de facturation actuelle.</span><span class="sxs-lookup"><span data-stu-id="41b0e-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="41b0e-162">Crédits</span><span class="sxs-lookup"><span data-stu-id="41b0e-162">Credits</span></span>

<span data-ttu-id="41b0e-163">Pour mapper ces crédits à votre facture :</span><span class="sxs-lookup"><span data-stu-id="41b0e-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="41b0e-164">Additionner le **TotalForCustomer** à partir du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="41b0e-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="41b0e-165">Totalisez la colonne **PostTaxTotal** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="41b0e-166">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="41b0e-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="41b0e-167">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="41b0e-168">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="41b0e-168">Offset a line item</span></span> | <span data-ttu-id="41b0e-169">Remboursement partiel ou entier à un article de ligne, y compris les taxes.</span><span class="sxs-lookup"><span data-stu-id="41b0e-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="41b0e-170">Remises basées sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="41b0e-170">Usage-based discounts</span></span>

<span data-ttu-id="41b0e-171">Pour mapper ces remises basées sur l’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="41b0e-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="41b0e-172">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="41b0e-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="41b0e-173">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="41b0e-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="41b0e-174">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="41b0e-174">Activation discount</span></span> | <span data-ttu-id="41b0e-175">Remise appliquée lorsque l’abonnement est activé.</span><span class="sxs-lookup"><span data-stu-id="41b0e-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="41b0e-176">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="41b0e-176">Cycle discount</span></span> | <span data-ttu-id="41b0e-177">Remise appliquée sur les frais périodiques.</span><span class="sxs-lookup"><span data-stu-id="41b0e-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="41b0e-178">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="41b0e-178">Renew discount</span></span> | <span data-ttu-id="41b0e-179">Remise appliquée lorsque l’abonnement est renouvelé.</span><span class="sxs-lookup"><span data-stu-id="41b0e-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="41b0e-180">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="41b0e-180">Cancel discount</span></span> | <span data-ttu-id="41b0e-181">Frais appliqués lors de l’annulation des remises.</span><span class="sxs-lookup"><span data-stu-id="41b0e-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="41b0e-182">Remises basées sur la licence</span><span class="sxs-lookup"><span data-stu-id="41b0e-182">License-based discounts</span></span>

<span data-ttu-id="41b0e-183">Pour mapper les remises basées sur les licences à votre facture, faites la somme de la colonne **TotalOtherDiscount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="41b0e-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="41b0e-184">*Les remises basées sur une licence peuvent être appliquées à plusieurs types de frais.*</span><span class="sxs-lookup"><span data-stu-id="41b0e-184">*License-based discounts may be applied to multiple charge types.*</span></span>
