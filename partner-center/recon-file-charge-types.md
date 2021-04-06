---
title: Types de frais de fichier de rapprochement
ms.topic: article
ms.date: 06/05/2020
description: Découvrez les types de frais (par exemple, basés sur une licence, basés sur l’utilisation et une fois), les crédits et les remises dans les fichiers de rapprochement de l’espace partenaires.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441592"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="58dce-103">Comprendre les différents types de frais dans les fichiers de rapprochement de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="58dce-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="58dce-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="58dce-104">**Applies to**</span></span>

- <span data-ttu-id="58dce-105">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="58dce-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="58dce-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="58dce-106">**Appropriate roles**</span></span>

- <span data-ttu-id="58dce-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="58dce-107">Admin agent</span></span>
- <span data-ttu-id="58dce-108">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="58dce-108">Billing admin</span></span>
- <span data-ttu-id="58dce-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="58dce-109">Global admin</span></span>

<span data-ttu-id="58dce-110">Cet article décrit les mappages entre une section de facture et les types de frais associés qui peuvent se trouver dans votre fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="58dce-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="58dce-111">Votre facture fournit un résumé des frais.</span><span class="sxs-lookup"><span data-stu-id="58dce-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="58dce-112">Votre fichier de réconciliation fournit une répartition détaillée des transactions d’éléments de ligne, y compris les types de frais.</span><span class="sxs-lookup"><span data-stu-id="58dce-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="58dce-113">Pour plus d’informations sur les fichiers de rapprochement, voir [How to use Reconciliation Files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="58dce-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="58dce-114">Les fichiers de [réconciliation basés sur l’utilisation](usage-based-recon-files.md) et les [fichiers de réconciliation basés sur des licences](license-based-recon-files.md) affichent uniquement les transactions et les frais liés à l’utilisation (unités consommées et frais connexes).</span><span class="sxs-lookup"><span data-stu-id="58dce-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="58dce-115">Les crédits uniques, les remises ou les remboursements qui apparaissent sur la facture en tant qu' **ajustements** ne sont pas affichés dans le fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="58dce-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="58dce-116">Mapper les types de frais aux frais de facture</span><span class="sxs-lookup"><span data-stu-id="58dce-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="58dce-117">Pour faire référence à des montants de frais entre votre facture et le fichier de réconciliation, utilisez les options de filtre dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="58dce-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="58dce-118">Filtrez par types de frais sur votre fichier de rapprochement pour mapper les frais de facture à un ensemble de répartitions de frais sur le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="58dce-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="58dce-119">Frais basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="58dce-119">License-based charges</span></span>

<span data-ttu-id="58dce-120">Pour mapper ces frais basés sur des licences à votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="58dce-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="58dce-121">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="58dce-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="58dce-122">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="58dce-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="58dce-123">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="58dce-123">Activation fee</span></span> | <span data-ttu-id="58dce-124">Montant facturé au client lorsqu’il utilise l’abonnement après l’achat.</span><span class="sxs-lookup"><span data-stu-id="58dce-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="58dce-125">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="58dce-125">Cancel fee</span></span> | <span data-ttu-id="58dce-126">Frais au prorata remboursés au client lors de la modification des licences associées.</span><span class="sxs-lookup"><span data-stu-id="58dce-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="58dce-127">Annuler le taux d’instance</span><span class="sxs-lookup"><span data-stu-id="58dce-127">Cancel instance prorate</span></span> | <span data-ttu-id="58dce-128">Frais au prorata annulés lorsque l’abonnement du client avec abonnement mensuel est suspendu et que les licences associées ont été modifiées dans le même mois.</span><span class="sxs-lookup"><span data-stu-id="58dce-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="58dce-129">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="58dce-129">Cycle fee</span></span> | <span data-ttu-id="58dce-130">Frais périodiques pour un abonnement.</span><span class="sxs-lookup"><span data-stu-id="58dce-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="58dce-131">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="58dce-131">Cycle instance prorate</span></span> | <span data-ttu-id="58dce-132">Frais au prorata calculés par le client lors de la modification des licences associées.</span><span class="sxs-lookup"><span data-stu-id="58dce-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="58dce-133">Frais liés au prorata en cas d’annulation</span><span class="sxs-lookup"><span data-stu-id="58dce-133">Prorate fees when cancel</span></span> | <span data-ttu-id="58dce-134">Remboursement calculé au prorata pour la partie inutilisée du service lors de l’annulation.</span><span class="sxs-lookup"><span data-stu-id="58dce-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="58dce-135">Frais liés au prorata en cas de conversion hors de l’offre actuelle</span><span class="sxs-lookup"><span data-stu-id="58dce-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="58dce-136">Frais facturés au prorata après la conversion de l’abonnement mensuel actuel en abonnement annuel.</span><span class="sxs-lookup"><span data-stu-id="58dce-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="58dce-137">Frais liés au prorata lors de la conversion vers une nouvelle offre</span><span class="sxs-lookup"><span data-stu-id="58dce-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="58dce-138">Frais au prorata après conversion d’un abonnement mensuel en nouvel abonnement annuel.</span><span class="sxs-lookup"><span data-stu-id="58dce-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="58dce-139">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="58dce-139">Prorate fees when purchase</span></span> | <span data-ttu-id="58dce-140">Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle ou annuelle.</span><span class="sxs-lookup"><span data-stu-id="58dce-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="58dce-141">Frais liés au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="58dce-141">Prorate fee when renew</span></span> | <span data-ttu-id="58dce-142">Frais au prorata lors du renouvellement de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="58dce-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="58dce-143">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="58dce-143">Renew fee</span></span> | <span data-ttu-id="58dce-144">Facturation pour le renouvellement d’un abonnement</span><span class="sxs-lookup"><span data-stu-id="58dce-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="58dce-145">Frais de prorata lors de l’activation</span><span class="sxs-lookup"><span data-stu-id="58dce-145">Prorate fees when activate</span></span> | <span data-ttu-id="58dce-146">Frais au prorata de l’activation jusqu’à la fin de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="58dce-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="58dce-147">Frais à usage unique</span><span class="sxs-lookup"><span data-stu-id="58dce-147">One-time charges</span></span>

<span data-ttu-id="58dce-148">Pour mapper ces frais à la fois sur votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="58dce-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="58dce-149">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="58dce-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="58dce-150">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="58dce-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="58dce-151">Nouveau</span><span class="sxs-lookup"><span data-stu-id="58dce-151">New</span></span> | <span data-ttu-id="58dce-152">Utilisé lors de la création d’un nouvel achat.</span><span class="sxs-lookup"><span data-stu-id="58dce-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="58dce-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="58dce-153">addQuantity</span></span> | <span data-ttu-id="58dce-154">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une augmentation.</span><span class="sxs-lookup"><span data-stu-id="58dce-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="58dce-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="58dce-155">removeQuantity</span></span> | <span data-ttu-id="58dce-156">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une diminution.</span><span class="sxs-lookup"><span data-stu-id="58dce-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="58dce-157">Annuler</span><span class="sxs-lookup"><span data-stu-id="58dce-157">Cancel</span></span> | <span data-ttu-id="58dce-158">Utilisé lorsqu’un abonnement est annulé.</span><span class="sxs-lookup"><span data-stu-id="58dce-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="58dce-159">Convertir</span><span class="sxs-lookup"><span data-stu-id="58dce-159">Convert</span></span> | <span data-ttu-id="58dce-160">Utilisé lors de la mise à niveau d’une licence, mais le nombre de licences reste inchangé.</span><span class="sxs-lookup"><span data-stu-id="58dce-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="58dce-161">Frais d'utilisation</span><span class="sxs-lookup"><span data-stu-id="58dce-161">Usage charges</span></span>

<span data-ttu-id="58dce-162">Pour mapper ces frais d’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="58dce-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="58dce-163">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="58dce-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="58dce-164">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="58dce-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="58dce-165">Évaluer les frais d’utilisation lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="58dce-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="58dce-166">Frais d’utilisation de l’accès en cas d’annulation pour utilisation impayée au cours de la période de facturation actuelle.</span><span class="sxs-lookup"><span data-stu-id="58dce-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="58dce-167">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="58dce-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="58dce-168">Frais d’utilisation de l’accès pour la période de facturation en cours.</span><span class="sxs-lookup"><span data-stu-id="58dce-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="58dce-169">Crédits</span><span class="sxs-lookup"><span data-stu-id="58dce-169">Credits</span></span>

<span data-ttu-id="58dce-170">Pour mapper ces crédits à votre facture :</span><span class="sxs-lookup"><span data-stu-id="58dce-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="58dce-171">Additionner le **TotalForCustomer** à partir du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="58dce-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="58dce-172">Totalisez la colonne **PostTaxTotal** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="58dce-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="58dce-173">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="58dce-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="58dce-174">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="58dce-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="58dce-175">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="58dce-175">Offset a line item</span></span> | <span data-ttu-id="58dce-176">Remboursement partiel ou entier sur un élément de ligne, y compris les taxes.</span><span class="sxs-lookup"><span data-stu-id="58dce-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="58dce-177">Remises basées sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="58dce-177">Usage-based discounts</span></span>

<span data-ttu-id="58dce-178">Pour mapper ces remises basées sur l’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="58dce-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="58dce-179">Description des frais (colonne ChargeType dans le fichier de rapprochement)</span><span class="sxs-lookup"><span data-stu-id="58dce-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="58dce-180">Explication des frais</span><span class="sxs-lookup"><span data-stu-id="58dce-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="58dce-181">Remise d’activation</span><span class="sxs-lookup"><span data-stu-id="58dce-181">Activation discount</span></span> | <span data-ttu-id="58dce-182">Remise appliquée lorsque l’abonnement est activé.</span><span class="sxs-lookup"><span data-stu-id="58dce-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="58dce-183">Remise au cycle</span><span class="sxs-lookup"><span data-stu-id="58dce-183">Cycle discount</span></span> | <span data-ttu-id="58dce-184">Remise appliquée sur les frais périodiques.</span><span class="sxs-lookup"><span data-stu-id="58dce-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="58dce-185">Remise de renouvellement</span><span class="sxs-lookup"><span data-stu-id="58dce-185">Renew discount</span></span> | <span data-ttu-id="58dce-186">Remise appliquée lorsque l’abonnement est renouvelé.</span><span class="sxs-lookup"><span data-stu-id="58dce-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="58dce-187">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="58dce-187">Cancel discount</span></span> | <span data-ttu-id="58dce-188">Frais appliqués lorsque les remises sont annulées.</span><span class="sxs-lookup"><span data-stu-id="58dce-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="58dce-189">Remises basées sur une licence</span><span class="sxs-lookup"><span data-stu-id="58dce-189">License-based discounts</span></span>

<span data-ttu-id="58dce-190">Pour mapper les remises basées sur les licences à votre facture, faites la somme de la colonne **TotalOtherDiscount** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="58dce-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="58dce-191">*Les remises basées sur une licence peuvent être appliquées à plusieurs types de frais.*</span><span class="sxs-lookup"><span data-stu-id="58dce-191">*License-based discounts may be applied to multiple charge types.*</span></span>
