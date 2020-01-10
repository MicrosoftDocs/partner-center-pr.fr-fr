---
title: Types de frais de fichier de réconciliation | Espace partenaires
ms.topic: article
ms.date: 01/06/2020
description: Types de frais (basés sur une licence, basés sur l’utilisation et exceptionnels), crédits et remises sur les fichiers de rapprochement de l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716870"
---
# <a name="understand-charge-types"></a><span data-ttu-id="5c1ce-103">Présentation des types de frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-103">Understand charge types</span></span>

<span data-ttu-id="5c1ce-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="5c1ce-104">**Applies to**</span></span>

- <span data-ttu-id="5c1ce-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5c1ce-105">Partner Center</span></span>
- <span data-ttu-id="5c1ce-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="5c1ce-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="5c1ce-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="5c1ce-107">**Appropriate roles**</span></span>

- <span data-ttu-id="5c1ce-108">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="5c1ce-108">Admin agent</span></span>
- <span data-ttu-id="5c1ce-109">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-109">Billing admin</span></span>
- <span data-ttu-id="5c1ce-110">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="5c1ce-110">Global admin</span></span>

<span data-ttu-id="5c1ce-111">Cette rubrique décrit les mappages entre une section de facture et les types de frais associés qui peuvent se trouver dans votre fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="5c1ce-112">Votre facture fournit un résumé des frais.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="5c1ce-113">Votre fichier de réconciliation fournit une répartition détaillée des transactions d’éléments de ligne, y compris les types de frais.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="5c1ce-114">Pour plus d’informations sur les fichiers de rapprochement, voir [How to use Reconciliation Files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="5c1ce-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="5c1ce-115">Les fichiers de [réconciliation basés sur l’utilisation](usage-based-recon-files.md) et les [fichiers de réconciliation basés sur des licences](license-based-recon-files.md) affichent uniquement les transactions et les frais liés à l’utilisation (unités consommées et frais connexes).</span><span class="sxs-lookup"><span data-stu-id="5c1ce-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="5c1ce-116">Les crédits uniques, les remises ou les remboursements qui apparaissent sur la facture en tant qu' **ajustements** ne sont pas affichés dans le fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="5c1ce-117">Mapper les types de frais aux frais de facture</span><span class="sxs-lookup"><span data-stu-id="5c1ce-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="5c1ce-118">Pour faire référence à des montants de frais entre votre facture et le fichier de réconciliation, utilisez les options de filtre dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="5c1ce-119">Filtrez par types de frais sur votre fichier de rapprochement pour mapper les frais de facture à un ensemble de répartitions de frais sur le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="5c1ce-120">Frais basés sur la licence</span><span class="sxs-lookup"><span data-stu-id="5c1ce-120">License-based charges</span></span>

<span data-ttu-id="5c1ce-121">Pour mapper ces frais basés sur des licences à votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="5c1ce-122">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5c1ce-123">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5c1ce-124">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-124">Activation fee</span></span> | <span data-ttu-id="5c1ce-125">Montant facturé au client lorsqu’il utilise l’abonnement après l’achat.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="5c1ce-126">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-126">Cancel fee</span></span> | <span data-ttu-id="5c1ce-127">Frais au prorata remboursés au client lors de la modification des sièges associés.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="5c1ce-128">Instance d'annulation au prorata</span><span class="sxs-lookup"><span data-stu-id="5c1ce-128">Cancel instance prorate</span></span> | <span data-ttu-id="5c1ce-129">Frais au prorata annulés lorsque l’abonnement du client avec abonnement mensuel est suspendu et que les sièges associés ont été modifiés au cours du même mois.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-129">Prorated charges cancelled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="5c1ce-130">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="5c1ce-130">Cycle fee</span></span> | <span data-ttu-id="5c1ce-131">Frais périodiques pour un abonnement.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="5c1ce-132">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="5c1ce-132">Cycle instance prorate</span></span> | <span data-ttu-id="5c1ce-133">Frais au prorata calculés par le client lors de la modification des sièges associés.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="5c1ce-134">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-134">Prorate fees when cancel</span></span> | <span data-ttu-id="5c1ce-135">Remboursement calculé au prorata pour la partie inutilisée du service lors de l’annulation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="5c1ce-136">Frais liés au prorata en cas de conversion hors de l’offre actuelle</span><span class="sxs-lookup"><span data-stu-id="5c1ce-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="5c1ce-137">Frais facturés au prorata après la conversion de l’abonnement mensuel actuel en abonnement annuel.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="5c1ce-138">Frais liés au prorata lors de la conversion vers une nouvelle offre</span><span class="sxs-lookup"><span data-stu-id="5c1ce-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="5c1ce-139">Frais au prorata après conversion d’un abonnement mensuel en nouvel abonnement annuel.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="5c1ce-140">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="5c1ce-140">Prorate fees when purchase</span></span> | <span data-ttu-id="5c1ce-141">Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="5c1ce-142">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="5c1ce-142">Purchase fee</span></span> | <span data-ttu-id="5c1ce-143">Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="5c1ce-144">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="5c1ce-144">Prorate fee when renew</span></span> | <span data-ttu-id="5c1ce-145">Frais au prorata lors du renouvellement de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="5c1ce-146">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="5c1ce-146">Renew fee</span></span> | <span data-ttu-id="5c1ce-147">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="5c1ce-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="5c1ce-148">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-148">Prorate fees when activate</span></span> | <span data-ttu-id="5c1ce-149">> des frais au prorata de l’activation jusqu’à la fin de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-149">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="5c1ce-150">Frais à usage unique</span><span class="sxs-lookup"><span data-stu-id="5c1ce-150">One-time charges</span></span>

<span data-ttu-id="5c1ce-151">Pour mapper ces frais à la fois sur votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="5c1ce-152">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5c1ce-153">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5c1ce-154">Nouveau</span><span class="sxs-lookup"><span data-stu-id="5c1ce-154">New</span></span> | <span data-ttu-id="5c1ce-155">Utilisé lors de la création d’un nouvel achat.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="5c1ce-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="5c1ce-156">addQuantity</span></span> | <span data-ttu-id="5c1ce-157">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une augmentation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="5c1ce-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="5c1ce-158">removeQuantity</span></span> | <span data-ttu-id="5c1ce-159">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une diminution.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="5c1ce-160">Annuler</span><span class="sxs-lookup"><span data-stu-id="5c1ce-160">Cancel</span></span> | <span data-ttu-id="5c1ce-161">Utilisé lors de l’annulation d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-161">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="5c1ce-162">Convertir</span><span class="sxs-lookup"><span data-stu-id="5c1ce-162">Convert</span></span> | <span data-ttu-id="5c1ce-163">Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="5c1ce-164">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-164">Usage charges</span></span>

<span data-ttu-id="5c1ce-165">Pour mapper ces frais d’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="5c1ce-166">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5c1ce-167">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5c1ce-168">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="5c1ce-169">Frais d’utilisation de l’accès en cas d’annulation pour utilisation impayée au cours de la période de facturation actuelle.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="5c1ce-170">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="5c1ce-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="5c1ce-171">Frais d’utilisation de l’accès pour la période de facturation en cours.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="5c1ce-172">Crédits</span><span class="sxs-lookup"><span data-stu-id="5c1ce-172">Credits</span></span>

<span data-ttu-id="5c1ce-173">Pour mapper ces crédits à votre facture :</span><span class="sxs-lookup"><span data-stu-id="5c1ce-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="5c1ce-174">Additionner le **TotalForCustomer** à partir du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="5c1ce-175">Totalisez la colonne **PostTaxTotal** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="5c1ce-176">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5c1ce-177">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5c1ce-178">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="5c1ce-178">Offset a line item</span></span> | <span data-ttu-id="5c1ce-179">Remboursement partiel ou entier sur un élément de ligne, y compris les taxes.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="5c1ce-180">Remises basées sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-180">Usage-based discounts</span></span>

<span data-ttu-id="5c1ce-181">Pour mapper ces remises basées sur l’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="5c1ce-182">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="5c1ce-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="5c1ce-183">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="5c1ce-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="5c1ce-184">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="5c1ce-184">Activation discount</span></span> | <span data-ttu-id="5c1ce-185">Remise appliquée lorsque l’abonnement est activé.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="5c1ce-186">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="5c1ce-186">Cycle discount</span></span> | <span data-ttu-id="5c1ce-187">Remise appliquée sur les frais périodiques.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="5c1ce-188">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="5c1ce-188">Renew discount</span></span> | <span data-ttu-id="5c1ce-189">Remise appliquée lorsque l’abonnement est renouvelé.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="5c1ce-190">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="5c1ce-190">Cancel discount</span></span> | <span data-ttu-id="5c1ce-191">Frais appliqués lors de l’annulation des remises.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-191">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="5c1ce-192">Remises basées sur la licence</span><span class="sxs-lookup"><span data-stu-id="5c1ce-192">License-based discounts</span></span>

<span data-ttu-id="5c1ce-193">Pour mapper les remises basées sur les licences à votre facture, faites la somme de la colonne **TotalOtherDiscount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="5c1ce-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="5c1ce-194">*Les remises basées sur une licence peuvent être appliquées à plusieurs types de frais.*</span><span class="sxs-lookup"><span data-stu-id="5c1ce-194">*License-based discounts may be applied to multiple charge types.*</span></span>
