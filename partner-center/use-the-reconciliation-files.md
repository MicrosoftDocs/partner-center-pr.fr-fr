---
title: Utiliser vos fichiers de rapprochement
ms.topic: article
ms.date: 03/10/2021
description: En savoir plus sur les fichiers de rapprochement dans l’espace partenaires et sur l’interprétation des affichages détaillés des lignes de facturation pour un cycle de facturation donné.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022772"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="8ee24-103">Découvrez comment lire les éléments de ligne dans vos fichiers de rapprochement de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8ee24-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="8ee24-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8ee24-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8ee24-105">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="8ee24-105">Billing admin</span></span>
- <span data-ttu-id="8ee24-106">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="8ee24-106">Global admin</span></span>

<span data-ttu-id="8ee24-107">Vous pouvez télécharger vos fichiers de conciliation à partir de l’espace partenaires pour obtenir une vue détaillée de chaque facture dans un cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="8ee24-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="8ee24-108">Les détails des éléments de ligne incluent les frais associés aux abonnements de chaque client et les événements détaillés (par exemple, ajout de licences à mi-parcours à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="8ee24-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="8ee24-109">Pour plus d’informations sur la lecture de votre facture, consultez [lire votre](read-your-bill.md) **facture**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="8ee24-110">Comprendre les champs de fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="8ee24-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="8ee24-111">Champs du fichier de rapprochement basé sur les licences</span><span class="sxs-lookup"><span data-stu-id="8ee24-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="8ee24-112">Champs du fichier de rapprochement basé sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="8ee24-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="8ee24-113">Champs du fichier de rapprochement basé sur l’utilisation quotidienne estimée</span><span class="sxs-lookup"><span data-stu-id="8ee24-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="8ee24-114">Champs du fichier de rapprochement des fournisseurs CSP à usage unique</span><span class="sxs-lookup"><span data-stu-id="8ee24-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="8ee24-115">Comprendre les types de frais dans les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="8ee24-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="8ee24-116">Pour comprendre les types de frais dans les fichiers de rapprochement (colonne **ChargeType** ), consultez la rubrique [types de frais de fichier de rapprochement](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="8ee24-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="8ee24-117">Résoudre les problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="8ee24-117">Fix formatting issues</span></span>

<span data-ttu-id="8ee24-118">Parfois, un fichier de réconciliation peut contenir des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="8ee24-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="8ee24-119">Par exemple, ce problème peut se produire si les paramètres régionaux en-US ne sont pas utilisés.</span><span class="sxs-lookup"><span data-stu-id="8ee24-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="8ee24-120">Pour résoudre les problèmes de mise en forme dans vos fichiers de rapprochement, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="8ee24-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="8ee24-121">Ouvrez le fichier de réconciliation (au format. csv) dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8ee24-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="8ee24-122">Sélectionnez la première colonne du fichier.</span><span class="sxs-lookup"><span data-stu-id="8ee24-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="8ee24-123">Ouvrez l' **Assistant Conversion de texte en colonnes**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="8ee24-124">Dans le ruban, sélectionnez **données**, puis sélectionnez **texte pour les colonnes**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="8ee24-125">Dans l’Assistant, sélectionnez **type de fichier délimité**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="8ee24-126">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="8ee24-127">Dans le champ **séparateurs** , sélectionnez **virgule**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="8ee24-128">(Si l' **onglet** est déjà sélectionné, vous pouvez conserver cette option sélectionnée.) Sélectionnez ensuite **suivant**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="8ee24-129">Dans le champ **format des données** de la colonne, sélectionnez **Date : mja**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="8ee24-130">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="8ee24-131">Dans le champ **format des données** de la colonne, sélectionnez **texte** pour toutes les colonnes de montant.</span><span class="sxs-lookup"><span data-stu-id="8ee24-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="8ee24-132">Ensuite, sélectionnez **Finish**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="8ee24-133">Télécharger les fichiers de rapprochement par programmation</span><span class="sxs-lookup"><span data-stu-id="8ee24-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="8ee24-134">Les fichiers de réconciliation peuvent être très volumineux et parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="8ee24-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="8ee24-135">Pour télécharger des fichiers de conciliation par programme, consultez [obtenir des lignes de facturation](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="8ee24-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="8ee24-136">Taxes de carte ou TVA</span><span class="sxs-lookup"><span data-stu-id="8ee24-136">Map taxes or VAT</span></span>

<span data-ttu-id="8ee24-137">Pour mapper les taxes ou la T.V.A. sur votre facture :</span><span class="sxs-lookup"><span data-stu-id="8ee24-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="8ee24-138">Totalisez la colonne **Tax** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="8ee24-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="8ee24-139">Totalisez la colonne **TaxAmount** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="8ee24-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="8ee24-140">Décomposant les fichiers de rapprochement par partenaire</span><span class="sxs-lookup"><span data-stu-id="8ee24-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="8ee24-141">Les partenaires dans le **modèle indirect** peuvent utiliser ces champs supplémentaires dans des fichiers de réconciliation basés sur les licences et sur l’utilisation pour détailler les fichiers par le revendeur.</span><span class="sxs-lookup"><span data-stu-id="8ee24-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="8ee24-142">ID MPN</span><span class="sxs-lookup"><span data-stu-id="8ee24-142">MPN ID</span></span> | <span data-ttu-id="8ee24-143">Description</span><span class="sxs-lookup"><span data-stu-id="8ee24-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="8ee24-144">ID MPN</span><span class="sxs-lookup"><span data-stu-id="8ee24-144">MPN ID</span></span> | <span data-ttu-id="8ee24-145">Identificateur Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (CSP) (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="8ee24-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="8ee24-146">ID&amp;nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="8ee24-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="8ee24-147">[Identificateur MPN du revendeur de l’enregistrement pour l’abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="8ee24-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="8ee24-148">Ce champ correspond à l’ID du revendeur indiqué pour l’abonnement spécifique dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8ee24-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="8ee24-149">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="8ee24-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="8ee24-150">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="8ee24-150">Reseller MPN ID</span></span>

<span data-ttu-id="8ee24-151">Si un partenaire CSP a vendu l’abonnement directement au client, son **ID MPN** est listé deux fois, à la fois avec l' **ID MPN** et l' **ID MPN du revendeur**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="8ee24-152">Si un partenaire CSP a un revendeur sans **ID MPN**, cette valeur est définie sur l' **ID MPN** du partenaire à la place.</span><span class="sxs-lookup"><span data-stu-id="8ee24-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="8ee24-153">Si le partenaire CSP supprime un **ID MPN du revendeur**, cette valeur sera définie sur *-1*.</span><span class="sxs-lookup"><span data-stu-id="8ee24-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="8ee24-154">Pour afficher ou mettre à jour l' **ID MPN du revendeur**:</span><span class="sxs-lookup"><span data-stu-id="8ee24-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="8ee24-155">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8ee24-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="8ee24-156">Dans le menu de l’Espace partenaires, sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="8ee24-157">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8ee24-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="8ee24-158">Dans le menu client, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="8ee24-159">Choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8ee24-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="8ee24-160">Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)**.</span><span class="sxs-lookup"><span data-stu-id="8ee24-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8ee24-161">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="8ee24-161">Next steps</span></span>

- [<span data-ttu-id="8ee24-162">Comment lire votre fichier de conciliation de factures &</span><span class="sxs-lookup"><span data-stu-id="8ee24-162">How to read your bill & recon file</span></span>](read-your-bill.md) 