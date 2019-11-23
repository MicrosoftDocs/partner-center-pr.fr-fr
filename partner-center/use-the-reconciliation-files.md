---
title: Use your reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Use your reconciliation files to understand detailed line-item views of Partner Center charges.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384804"
---
# <a name="use-your-reconciliation-files"></a><span data-ttu-id="6ab90-103">Use your reconciliation files</span><span class="sxs-lookup"><span data-stu-id="6ab90-103">Use your reconciliation files</span></span>

<span data-ttu-id="6ab90-104">S'applique à :</span><span class="sxs-lookup"><span data-stu-id="6ab90-104">Applies to:</span></span>

- <span data-ttu-id="6ab90-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ab90-105">Partner Center</span></span>
- <span data-ttu-id="6ab90-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="6ab90-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6ab90-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span><span class="sxs-lookup"><span data-stu-id="6ab90-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="6ab90-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span><span class="sxs-lookup"><span data-stu-id="6ab90-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="6ab90-109">Appropriate roles:</span><span class="sxs-lookup"><span data-stu-id="6ab90-109">Appropriate roles:</span></span>

- <span data-ttu-id="6ab90-110">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="6ab90-110">Billing admin</span></span>
- <span data-ttu-id="6ab90-111">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="6ab90-111">Global admin</span></span>

<span data-ttu-id="6ab90-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="6ab90-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="6ab90-113">Understand reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="6ab90-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="6ab90-114">License-based reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="6ab90-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="6ab90-115">Usage-based reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="6ab90-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="6ab90-116">One-time and recurring reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="6ab90-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="6ab90-117">Daily-rated usage reconciliation file fields</span><span class="sxs-lookup"><span data-stu-id="6ab90-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="6ab90-118">Understand charge types in reconciliation files</span><span class="sxs-lookup"><span data-stu-id="6ab90-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="6ab90-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="6ab90-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="6ab90-120">Fix formatting issues</span><span class="sxs-lookup"><span data-stu-id="6ab90-120">Fix formatting issues</span></span>

<span data-ttu-id="6ab90-121">Occasionally, a reconciliation file might contain formatting issues.</span><span class="sxs-lookup"><span data-stu-id="6ab90-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="6ab90-122">For example, this issue might occur if the en-US locale is not used.</span><span class="sxs-lookup"><span data-stu-id="6ab90-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="6ab90-123">Follow these steps for fix any formatting issues in your reconciliation files:</span><span class="sxs-lookup"><span data-stu-id="6ab90-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="6ab90-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6ab90-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="6ab90-125">Select the first column in the file.</span><span class="sxs-lookup"><span data-stu-id="6ab90-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="6ab90-126">Open the **Convert Text to Columns Wizard**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="6ab90-127">On the ribbon, select **Data**, then select **Text to Columns**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="6ab90-128">In the wizard, select **Delimited file type**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="6ab90-129">Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="6ab90-130">In the **Delimiters** field, select **Comma**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="6ab90-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="6ab90-132">In the **Column data format** field, select **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="6ab90-133">Then, select **Next**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="6ab90-134">In the **Column data format** field, select **Text** for all amount columns.</span><span class="sxs-lookup"><span data-stu-id="6ab90-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="6ab90-135">Then, select **Finish**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="6ab90-136">Download reconciliation files programmatically</span><span class="sxs-lookup"><span data-stu-id="6ab90-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="6ab90-137">Reconciliation files can be very large and are sometimes difficult to download.</span><span class="sxs-lookup"><span data-stu-id="6ab90-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="6ab90-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="6ab90-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="6ab90-139">Map taxes or VAT</span><span class="sxs-lookup"><span data-stu-id="6ab90-139">Map taxes or VAT</span></span>

<span data-ttu-id="6ab90-140">To map Taxes or value-added tax (VAT) to your invoice:</span><span class="sxs-lookup"><span data-stu-id="6ab90-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="6ab90-141">Sum the **Tax** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="6ab90-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="6ab90-142">Sum the **TaxAmount** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="6ab90-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="6ab90-143">Itemize reconciliation files by partner</span><span class="sxs-lookup"><span data-stu-id="6ab90-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="6ab90-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span><span class="sxs-lookup"><span data-stu-id="6ab90-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="6ab90-145">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="6ab90-145">MPN ID</span></span> | <span data-ttu-id="6ab90-146">Description</span><span class="sxs-lookup"><span data-stu-id="6ab90-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6ab90-147">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="6ab90-147">MPN ID</span></span> | <span data-ttu-id="6ab90-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span><span class="sxs-lookup"><span data-stu-id="6ab90-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="6ab90-149">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="6ab90-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="6ab90-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="6ab90-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="6ab90-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="6ab90-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="6ab90-152">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="6ab90-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="6ab90-153">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="6ab90-153">Reseller MPN ID</span></span>

<span data-ttu-id="6ab90-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="6ab90-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span><span class="sxs-lookup"><span data-stu-id="6ab90-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="6ab90-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span><span class="sxs-lookup"><span data-stu-id="6ab90-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="6ab90-157">To view or update the **Reseller MPN ID**:</span><span class="sxs-lookup"><span data-stu-id="6ab90-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="6ab90-158">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ab90-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="6ab90-159">Dans le menu de l'Espace partenaires, sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="6ab90-160">Dans la liste, choisissez le client.</span><span class="sxs-lookup"><span data-stu-id="6ab90-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="6ab90-161">In the customer menu, select **Subscriptions**.</span><span class="sxs-lookup"><span data-stu-id="6ab90-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="6ab90-162">Choose the subscription from the list.</span><span class="sxs-lookup"><span data-stu-id="6ab90-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="6ab90-163">Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)** .</span><span class="sxs-lookup"><span data-stu-id="6ab90-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
