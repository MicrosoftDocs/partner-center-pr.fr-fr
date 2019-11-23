---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a><span data-ttu-id="6ae1c-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="6ae1c-103">Understand charge types</span></span>

<span data-ttu-id="6ae1c-104">S'applique à :</span><span class="sxs-lookup"><span data-stu-id="6ae1c-104">Applies to:</span></span>

- <span data-ttu-id="6ae1c-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ae1c-105">Partner Center</span></span>
- <span data-ttu-id="6ae1c-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="6ae1c-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6ae1c-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="6ae1c-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="6ae1c-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="6ae1c-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="6ae1c-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="6ae1c-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="6ae1c-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="6ae1c-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="6ae1c-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="6ae1c-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="6ae1c-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="6ae1c-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="6ae1c-116">Frais basés sur la licence</span><span class="sxs-lookup"><span data-stu-id="6ae1c-116">License-based charges</span></span>

<span data-ttu-id="6ae1c-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="6ae1c-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="6ae1c-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6ae1c-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6ae1c-120">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-120">Activation fee</span></span> | <span data-ttu-id="6ae1c-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="6ae1c-122">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-122">Cancel fee</span></span> | <span data-ttu-id="6ae1c-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="6ae1c-124">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="6ae1c-124">Cycle fee</span></span> | <span data-ttu-id="6ae1c-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="6ae1c-126">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="6ae1c-126">Cycle instance prorate</span></span> | <span data-ttu-id="6ae1c-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="6ae1c-128">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-128">Prorate fees when cancel</span></span> | <span data-ttu-id="6ae1c-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="6ae1c-130">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="6ae1c-130">Prorate fees when purchase</span></span> | <span data-ttu-id="6ae1c-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="6ae1c-132">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="6ae1c-132">Purchase fee</span></span> | <span data-ttu-id="6ae1c-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="6ae1c-134">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="6ae1c-134">Prorate fee when renew</span></span> | <span data-ttu-id="6ae1c-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="6ae1c-136">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="6ae1c-136">Renew fee</span></span> | <span data-ttu-id="6ae1c-137">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="6ae1c-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="6ae1c-138">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-138">Prorate fees when activate</span></span> | <span data-ttu-id="6ae1c-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="6ae1c-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="6ae1c-140">One-time charges</span></span>

<span data-ttu-id="6ae1c-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="6ae1c-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="6ae1c-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6ae1c-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6ae1c-144">Nouveau</span><span class="sxs-lookup"><span data-stu-id="6ae1c-144">New</span></span> | <span data-ttu-id="6ae1c-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="6ae1c-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="6ae1c-146">addQuantity</span></span> | <span data-ttu-id="6ae1c-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="6ae1c-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="6ae1c-148">removeQuantity</span></span> | <span data-ttu-id="6ae1c-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="6ae1c-150">Annuler</span><span class="sxs-lookup"><span data-stu-id="6ae1c-150">Cancel</span></span> | <span data-ttu-id="6ae1c-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="6ae1c-152">Convertir</span><span class="sxs-lookup"><span data-stu-id="6ae1c-152">Convert</span></span> | <span data-ttu-id="6ae1c-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="6ae1c-154">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-154">Usage charges</span></span>

<span data-ttu-id="6ae1c-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="6ae1c-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="6ae1c-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6ae1c-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6ae1c-158">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="6ae1c-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="6ae1c-160">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="6ae1c-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="6ae1c-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="6ae1c-162">Crédits</span><span class="sxs-lookup"><span data-stu-id="6ae1c-162">Credits</span></span>

<span data-ttu-id="6ae1c-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="6ae1c-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="6ae1c-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="6ae1c-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="6ae1c-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="6ae1c-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6ae1c-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6ae1c-168">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="6ae1c-168">Offset a line item</span></span> | <span data-ttu-id="6ae1c-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="6ae1c-170">Remises basées sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-170">Usage-based discounts</span></span>

<span data-ttu-id="6ae1c-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="6ae1c-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="6ae1c-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="6ae1c-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="6ae1c-174">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="6ae1c-174">Activation discount</span></span> | <span data-ttu-id="6ae1c-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="6ae1c-176">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="6ae1c-176">Cycle discount</span></span> | <span data-ttu-id="6ae1c-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="6ae1c-178">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="6ae1c-178">Renew discount</span></span> | <span data-ttu-id="6ae1c-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="6ae1c-180">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="6ae1c-180">Cancel discount</span></span> | <span data-ttu-id="6ae1c-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="6ae1c-182">Remises basées sur la licence</span><span class="sxs-lookup"><span data-stu-id="6ae1c-182">License-based discounts</span></span>

<span data-ttu-id="6ae1c-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="6ae1c-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="6ae1c-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="6ae1c-184">*License-based discounts may be applied to multiple charge types.*</span></span>
