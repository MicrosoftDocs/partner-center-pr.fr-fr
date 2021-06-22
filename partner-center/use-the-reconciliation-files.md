---
title: Utiliser vos fichiers de rapprochement
ms.topic: article
ms.date: 03/26/2021
description: En savoir plus sur les fichiers de rapprochement dans l’espace partenaires et sur l’interprétation des affichages détaillés des lignes de facturation pour un cycle de facturation donné.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431573"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="20cac-103">Découvrez comment lire les éléments de ligne dans vos fichiers de rapprochement de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="20cac-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="20cac-104">**Rôles appropriés**: administrateur de facturation | Administrateur général</span><span class="sxs-lookup"><span data-stu-id="20cac-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="20cac-105">Vous pouvez télécharger vos fichiers de conciliation à partir de l’espace partenaires pour obtenir une vue détaillée de chaque facture dans un cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="20cac-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="20cac-106">Les détails des éléments de ligne incluent les frais associés aux abonnements de chaque client et les événements détaillés (par exemple, ajout de licences à mi-parcours à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="20cac-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="20cac-107">Pour plus d’informations sur la lecture de votre facture, consultez [lire votre](read-your-bill.md) **facture**.</span><span class="sxs-lookup"><span data-stu-id="20cac-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="20cac-108">Comprendre les champs de fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="20cac-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="20cac-109">Champs du fichier de rapprochement basé sur les licences</span><span class="sxs-lookup"><span data-stu-id="20cac-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="20cac-110">Champs du fichier de rapprochement basé sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="20cac-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="20cac-111">Champs du fichier de rapprochement basé sur l’utilisation quotidienne estimée</span><span class="sxs-lookup"><span data-stu-id="20cac-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="20cac-112">Champs du fichier de rapprochement des fournisseurs CSP à usage unique</span><span class="sxs-lookup"><span data-stu-id="20cac-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="20cac-113">Comprendre les types de frais dans les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="20cac-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="20cac-114">Pour comprendre les types de frais dans les fichiers de rapprochement (colonne **ChargeType** ), consultez la rubrique [types de frais de fichier de rapprochement](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="20cac-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="20cac-115">Résoudre les problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="20cac-115">Fix formatting issues</span></span>

<span data-ttu-id="20cac-116">Parfois, un fichier de réconciliation peut contenir des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="20cac-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="20cac-117">Par exemple, ce problème peut se produire si les paramètres régionaux en-US ne sont pas utilisés.</span><span class="sxs-lookup"><span data-stu-id="20cac-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="20cac-118">Pour résoudre les problèmes de mise en forme dans vos fichiers de rapprochement, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="20cac-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="20cac-119">Ouvrez le fichier de réconciliation (au format .csv) dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="20cac-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="20cac-120">Sélectionnez la première colonne du fichier.</span><span class="sxs-lookup"><span data-stu-id="20cac-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="20cac-121">Ouvrez l' **Assistant Conversion de texte en colonnes**.</span><span class="sxs-lookup"><span data-stu-id="20cac-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="20cac-122">Dans le ruban, sélectionnez **données**, puis sélectionnez **texte pour les colonnes**.</span><span class="sxs-lookup"><span data-stu-id="20cac-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="20cac-123">Dans l’Assistant, sélectionnez **type de fichier délimité**.</span><span class="sxs-lookup"><span data-stu-id="20cac-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="20cac-124">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="20cac-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="20cac-125">Dans le champ **séparateurs** , sélectionnez **virgule**.</span><span class="sxs-lookup"><span data-stu-id="20cac-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="20cac-126">(Si l' **onglet** est déjà sélectionné, vous pouvez conserver cette option sélectionnée.) Sélectionnez ensuite **suivant**.</span><span class="sxs-lookup"><span data-stu-id="20cac-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="20cac-127">Dans le champ **format des données** de la colonne, sélectionnez **Date : mja**.</span><span class="sxs-lookup"><span data-stu-id="20cac-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="20cac-128">Ensuite, sélectionnez **Suivant**.</span><span class="sxs-lookup"><span data-stu-id="20cac-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="20cac-129">Dans le champ **format des données** de la colonne, sélectionnez **texte** pour toutes les colonnes de montant.</span><span class="sxs-lookup"><span data-stu-id="20cac-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="20cac-130">Ensuite, sélectionnez **Finish**.</span><span class="sxs-lookup"><span data-stu-id="20cac-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="20cac-131">Télécharger les fichiers de rapprochement par programmation</span><span class="sxs-lookup"><span data-stu-id="20cac-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="20cac-132">Les fichiers de réconciliation peuvent être très volumineux et parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="20cac-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="20cac-133">Pour télécharger des fichiers de conciliation par programme, consultez [obtenir des lignes de facturation](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="20cac-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="20cac-134">Si votre fichier dépasse la limite de lignes dans Excel</span><span class="sxs-lookup"><span data-stu-id="20cac-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="20cac-135">Si vous êtes en mesure de télécharger un fichier de réconciliation sans l’ouvrir dans Microsoft Excel, cela signifie probablement que le fichier contient plus de lignes qu’Excel ne l’autorise.</span><span class="sxs-lookup"><span data-stu-id="20cac-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="20cac-136">Dans ce cas, vous pouvez utiliser l’une des procédures ci-dessous pour ouvrir le fichier.</span><span class="sxs-lookup"><span data-stu-id="20cac-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="20cac-137">Ouvrir un fichier de rapprochement dans Power BI</span><span class="sxs-lookup"><span data-stu-id="20cac-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="20cac-138">Téléchargez le fichier de réconciliation comme vous le feriez normalement.</span><span class="sxs-lookup"><span data-stu-id="20cac-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="20cac-139">Téléchargez, installez et ouvrez une instance de Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="20cac-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="20cac-140">Sous **l’onglet Power bi** , sélectionnez récupérer des **données**.</span><span class="sxs-lookup"><span data-stu-id="20cac-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="20cac-141">Dans la liste des **sources de données courantes**, sélectionnez **texte/CSV**.</span><span class="sxs-lookup"><span data-stu-id="20cac-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="20cac-142">Lorsque vous y êtes invité, ouvrez votre fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="20cac-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="20cac-143">Ouvrir un fichier de rapprochement dans un tableau croisé dynamique Excel</span><span class="sxs-lookup"><span data-stu-id="20cac-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="20cac-144">Téléchargez le fichier de réconciliation comme vous le feriez normalement.</span><span class="sxs-lookup"><span data-stu-id="20cac-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="20cac-145">Ouvrez un nouveau fichier dans Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="20cac-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="20cac-146">Sous l’onglet **données** , sélectionnez **récupérer des données**, sélectionnez **à partir d’un fichier**, puis sélectionnez **texte/CSV**.</span><span class="sxs-lookup"><span data-stu-id="20cac-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="20cac-147">Lorsque vous y êtes invité, ouvrez votre fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="20cac-147">When prompted, open your recon file.</span></span> <span data-ttu-id="20cac-148">Vos données s’affichent.</span><span class="sxs-lookup"><span data-stu-id="20cac-148">Your data will appear.</span></span>
5. <span data-ttu-id="20cac-149">Dans le menu déroulant **charger** , sélectionnez **charger sur**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="20cac-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="20cac-150">Dans la boîte de dialogue **importer des données** , sélectionnez **rapport de tableau croisé dynamique** pour ouvrir votre fichier.</span><span class="sxs-lookup"><span data-stu-id="20cac-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="20cac-151">Montant négatif affiché</span><span class="sxs-lookup"><span data-stu-id="20cac-151">Negative amount displayed</span></span>

<span data-ttu-id="20cac-152">Vous pouvez voir un montant négatif dans votre fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="20cac-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="20cac-153">Ce problème est probablement dû à l’une des causes suivantes :</span><span class="sxs-lookup"><span data-stu-id="20cac-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="20cac-154">Vous avez récemment annulé ou réduit votre nombre de licences</span><span class="sxs-lookup"><span data-stu-id="20cac-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="20cac-155">Vous avez reçu un crédit pour un contrat de licence de service (SLA) ou pour la consommation Azure</span><span class="sxs-lookup"><span data-stu-id="20cac-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="20cac-156">Pour obtenir plus d’informations sur cette transaction, examinez son attribut de type de frais dans votre fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="20cac-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="20cac-157">Taxes de carte ou TVA</span><span class="sxs-lookup"><span data-stu-id="20cac-157">Map taxes or VAT</span></span>

<span data-ttu-id="20cac-158">Pour mapper les taxes ou la T.V.A. sur votre facture :</span><span class="sxs-lookup"><span data-stu-id="20cac-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="20cac-159">Totalisez la colonne **Tax** du fichier basé sur une licence.</span><span class="sxs-lookup"><span data-stu-id="20cac-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="20cac-160">Totalisez la colonne **TaxAmount** à partir du fichier d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="20cac-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="20cac-161">Décomposant les fichiers de rapprochement par partenaire</span><span class="sxs-lookup"><span data-stu-id="20cac-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="20cac-162">Les partenaires dans le **modèle indirect** peuvent utiliser ces champs supplémentaires dans des fichiers de réconciliation basés sur les licences et sur l’utilisation pour détailler les fichiers par le revendeur.</span><span class="sxs-lookup"><span data-stu-id="20cac-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="20cac-163">ID MPN</span><span class="sxs-lookup"><span data-stu-id="20cac-163">MPN ID</span></span> | <span data-ttu-id="20cac-164">Description</span><span class="sxs-lookup"><span data-stu-id="20cac-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="20cac-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="20cac-165">MPN ID</span></span> | <span data-ttu-id="20cac-166">Identificateur Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (CSP) (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="20cac-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="20cac-167">ID&amp;nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="20cac-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="20cac-168">[Identificateur MPN du revendeur de l’enregistrement pour l’abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="20cac-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="20cac-169">Ce champ correspond à l’ID du revendeur indiqué pour l’abonnement spécifique dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="20cac-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="20cac-170">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="20cac-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="20cac-171">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="20cac-171">Reseller MPN ID</span></span>

<span data-ttu-id="20cac-172">Si un partenaire CSP a vendu l’abonnement directement au client, son **ID MPN** est listé deux fois, à la fois avec l' **ID MPN** et l' **ID MPN du revendeur**.</span><span class="sxs-lookup"><span data-stu-id="20cac-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="20cac-173">Si un partenaire CSP a un revendeur sans **ID MPN**, cette valeur est définie sur l' **ID MPN** du partenaire à la place.</span><span class="sxs-lookup"><span data-stu-id="20cac-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="20cac-174">Si le partenaire CSP supprime un **ID MPN du revendeur**, cette valeur sera définie sur *-1*.</span><span class="sxs-lookup"><span data-stu-id="20cac-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="20cac-175">Pour afficher ou mettre à jour l' **ID MPN du revendeur**:</span><span class="sxs-lookup"><span data-stu-id="20cac-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="20cac-176">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="20cac-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="20cac-177">Dans le menu de l’Espace partenaires, sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="20cac-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="20cac-178">Sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="20cac-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="20cac-179">Dans le menu client, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="20cac-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="20cac-180">Choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="20cac-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="20cac-181">Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)**.</span><span class="sxs-lookup"><span data-stu-id="20cac-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20cac-182">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="20cac-182">Next steps</span></span>

- [<span data-ttu-id="20cac-183">Comment lire votre fichier de conciliation de factures &</span><span class="sxs-lookup"><span data-stu-id="20cac-183">How to read your bill & recon file</span></span>](read-your-bill.md) 