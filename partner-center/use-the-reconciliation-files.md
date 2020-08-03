---
title: Utiliser vos fichiers de rapprochement
ms.topic: article
ms.date: 06/08/2020
description: En savoir plus sur les fichiers de rapprochement dans l’espace partenaires et sur l’interprétation des affichages détaillés des lignes de facturation pour un cycle de facturation donné.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05939dc5edaddeb2f74b3b75017e2062dff25e31
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468330"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="31f00-103">Découvrez comment lire les éléments de ligne dans vos fichiers de rapprochement de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="31f00-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="31f00-104">S’applique à :</span><span class="sxs-lookup"><span data-stu-id="31f00-104">Applies to:</span></span>

- <span data-ttu-id="31f00-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="31f00-105">Partner Center</span></span>
- <span data-ttu-id="31f00-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="31f00-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="31f00-107">Vous pouvez télécharger vos fichiers de conciliation à partir de l’espace partenaires pour obtenir une vue détaillée de chaque facture dans un cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="31f00-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="31f00-108">Les détails des éléments de ligne incluent les frais associés aux abonnements de chaque client et les événements détaillés (par exemple, ajout de licences à mi-parcours à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="31f00-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="31f00-109">Rôles appropriés :</span><span class="sxs-lookup"><span data-stu-id="31f00-109">Appropriate roles:</span></span>

- <span data-ttu-id="31f00-110">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="31f00-110">Billing admin</span></span>
- <span data-ttu-id="31f00-111">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="31f00-111">Global admin</span></span>

<span data-ttu-id="31f00-112">Pour plus d’informations sur la lecture de votre facture, consultez [lire votre](read-your-bill.md) **facture**.</span><span class="sxs-lookup"><span data-stu-id="31f00-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="31f00-113">Comprendre les champs de fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="31f00-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="31f00-114">Champs du fichier de réconciliation basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="31f00-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="31f00-115">Champs du fichier de réconciliation basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="31f00-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="31f00-116">Champs du fichier de réconciliation de l’utilisation évalué quotidiennement</span><span class="sxs-lookup"><span data-stu-id="31f00-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="31f00-117">Comprendre les types de frais dans les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="31f00-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="31f00-118">Pour comprendre les types de frais dans les fichiers de rapprochement (colonne **ChargeType** ), consultez la rubrique [types de frais de fichier de rapprochement](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="31f00-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="31f00-119">Résoudre les problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="31f00-119">Fix formatting issues</span></span>

<span data-ttu-id="31f00-120">Parfois, un fichier de réconciliation peut contenir des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="31f00-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="31f00-121">Par exemple, ce problème peut se produire si les paramètres régionaux en-US ne sont pas utilisés.</span><span class="sxs-lookup"><span data-stu-id="31f00-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="31f00-122">Pour résoudre les problèmes de mise en forme dans vos fichiers de rapprochement, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="31f00-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="31f00-123">Ouvrez le fichier de réconciliation (au format. csv) dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="31f00-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="31f00-124">Sélectionnez la première colonne du fichier.</span><span class="sxs-lookup"><span data-stu-id="31f00-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="31f00-125">Ouvrez l' **Assistant Conversion de texte en colonnes**.</span><span class="sxs-lookup"><span data-stu-id="31f00-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="31f00-126">Dans le ruban, sélectionnez **données**, puis sélectionnez **texte pour les colonnes**.</span><span class="sxs-lookup"><span data-stu-id="31f00-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="31f00-127">Dans l’Assistant, sélectionnez **type de fichier délimité**.</span><span class="sxs-lookup"><span data-stu-id="31f00-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="31f00-128">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="31f00-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="31f00-129">Dans le champ **séparateurs** , sélectionnez **virgule**.</span><span class="sxs-lookup"><span data-stu-id="31f00-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="31f00-130">(Si l' **onglet** est déjà sélectionné, vous pouvez conserver cette option sélectionnée.) Sélectionnez ensuite **suivant**.</span><span class="sxs-lookup"><span data-stu-id="31f00-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="31f00-131">Dans le champ **format des données** de la colonne, sélectionnez **Date : mja**.</span><span class="sxs-lookup"><span data-stu-id="31f00-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="31f00-132">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="31f00-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="31f00-133">Dans le champ **format des données** de la colonne, sélectionnez **texte** pour toutes les colonnes de montant.</span><span class="sxs-lookup"><span data-stu-id="31f00-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="31f00-134">Ensuite, sélectionnez **Terminer**.</span><span class="sxs-lookup"><span data-stu-id="31f00-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="31f00-135">Télécharger les fichiers de rapprochement par programmation</span><span class="sxs-lookup"><span data-stu-id="31f00-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="31f00-136">Les fichiers de réconciliation peuvent être très volumineux et parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="31f00-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="31f00-137">Pour télécharger des fichiers de conciliation par programme, consultez [obtenir des lignes de facturation](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="31f00-137">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="31f00-138">Taxes de carte ou TVA</span><span class="sxs-lookup"><span data-stu-id="31f00-138">Map taxes or VAT</span></span>

<span data-ttu-id="31f00-139">Pour mapper les taxes ou la T.V.A. sur votre facture :</span><span class="sxs-lookup"><span data-stu-id="31f00-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="31f00-140">Totalisez la colonne **Tax** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="31f00-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="31f00-141">Totalisez la colonne **TaxAmount** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="31f00-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="31f00-142">Décomposant les fichiers de rapprochement par partenaire</span><span class="sxs-lookup"><span data-stu-id="31f00-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="31f00-143">Les partenaires dans le **modèle indirect** peuvent utiliser ces champs supplémentaires dans des fichiers de réconciliation basés sur les licences et sur l’utilisation pour détailler les fichiers par le revendeur.</span><span class="sxs-lookup"><span data-stu-id="31f00-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="31f00-144">ID MPN</span><span class="sxs-lookup"><span data-stu-id="31f00-144">MPN ID</span></span> | <span data-ttu-id="31f00-145">Description</span><span class="sxs-lookup"><span data-stu-id="31f00-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="31f00-146">ID MPN</span><span class="sxs-lookup"><span data-stu-id="31f00-146">MPN ID</span></span> | <span data-ttu-id="31f00-147">Identificateur Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (CSP) (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="31f00-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="31f00-148">ID&amp;nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="31f00-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="31f00-149">[Identificateur MPN du revendeur de l’enregistrement pour l’abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="31f00-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="31f00-150">Ce champ correspond à l’ID du revendeur indiqué pour l’abonnement spécifique dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="31f00-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="31f00-151">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="31f00-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="31f00-152">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="31f00-152">Reseller MPN ID</span></span>

<span data-ttu-id="31f00-153">Si un partenaire CSP a vendu l’abonnement directement au client, son **ID MPN** est listé deux fois, à la fois avec l' **ID MPN** et l' **ID MPN du revendeur**.</span><span class="sxs-lookup"><span data-stu-id="31f00-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="31f00-154">Si un partenaire CSP a un revendeur sans **ID MPN**, cette valeur est définie sur l' **ID MPN** du partenaire à la place.</span><span class="sxs-lookup"><span data-stu-id="31f00-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="31f00-155">Si le partenaire CSP supprime un **ID MPN du revendeur**, cette valeur sera définie sur *-1*.</span><span class="sxs-lookup"><span data-stu-id="31f00-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="31f00-156">Pour afficher ou mettre à jour l' **ID MPN du revendeur**:</span><span class="sxs-lookup"><span data-stu-id="31f00-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="31f00-157">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="31f00-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="31f00-158">Dans le menu de l’Espace partenaires, sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="31f00-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="31f00-159">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="31f00-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="31f00-160">Dans le menu client, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="31f00-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="31f00-161">Choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="31f00-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="31f00-162">Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)**.</span><span class="sxs-lookup"><span data-stu-id="31f00-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>
