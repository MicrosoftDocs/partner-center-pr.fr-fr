---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 07/08/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pour obtenir une vue détaillée de chaque facture dans un cycle de facturation, téléchargez les fichiers de la conciliation à partir de l’espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 7b27e99e5c0dc55fad3b06cc22316e8282dbe35c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653973"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e9da2-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="e9da2-103">Use the reconciliation files</span></span>

<span data-ttu-id="e9da2-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="e9da2-104">**Applies to**</span></span>

-  <span data-ttu-id="e9da2-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e9da2-105">Partner Center</span></span>
-  <span data-ttu-id="e9da2-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e9da2-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="e9da2-107">Pour obtenir une vue détaillée de chaque facture dans un cycle de facturation, téléchargez les fichiers de la conciliation à partir de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="e9da2-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="e9da2-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="e9da2-109">Problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="e9da2-109">Formatting issues</span></span>

<span data-ttu-id="e9da2-110">Parfois, votre fichier de rapprochement peut présenter des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="e9da2-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="e9da2-111">(Cela peut se produire, par exemple, si les paramètres régionaux en-US ne sont pas utilisés.) Suivez les étapes ci-dessous pour résoudre ces problèmes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="e9da2-112">Ouvrez le fichier. csv dans Excel, puis sélectionnez la première colonne.</span><span class="sxs-lookup"><span data-stu-id="e9da2-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="e9da2-113">Dans le ruban, sélectionnez <strong>données</strong>, puis sélectionnez <strong>texte pour les colonnes</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="e9da2-114">Dans l’Assistant Conversion de texte en colonnes, sélectionnez <strong>type de fichier délimité</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="e9da2-115">Dans le champ séparateurs, sélectionnez <strong>virgule</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="e9da2-116">Si l’option <strong>onglet</strong> est déjà sélectionnée, vous pouvez la conserver.</span><span class="sxs-lookup"><span data-stu-id="e9da2-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="e9da2-117">Sélectionnez <strong>Suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="e9da2-118">Dans le champ format des données de la colonne, sélectionnez <strong>Date : mja</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="e9da2-119">Dans le champ format des données de la colonne, sélectionnez <strong>texte</strong> pour toutes les colonnes de montant, puis sélectionnez <strong>Terminer</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="e9da2-120">Téléchargement d’un fichier de rapprochement volumineux</span><span class="sxs-lookup"><span data-stu-id="e9da2-120">Downloading a large recon file</span></span>

<span data-ttu-id="e9da2-121">Les fichiers de rapprochement peuvent devenir très volumineux et parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="e9da2-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="e9da2-122">Pour obtenir un script PowerShell qui vous aide à télécharger des fichiers de rapprochement volumineux, consultez [obtenir des lignes de facturation](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="e9da2-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e9da2-123">Décomposant par partenaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-123">Itemize by partner</span></span>


<span data-ttu-id="e9da2-124">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="e9da2-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e9da2-125">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="e9da2-125">MPN ID</span></span></th>
<th><span data-ttu-id="e9da2-126">Description</span><span class="sxs-lookup"><span data-stu-id="e9da2-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e9da2-127">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="e9da2-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="e9da2-128">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="e9da2-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-129">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="e9da2-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e9da2-130">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="e9da2-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e9da2-131">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e9da2-132">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e9da2-133">affichage eTo ou mettez à jour le revendeur. dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="e9da2-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e9da2-134">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="e9da2-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e9da2-135">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e9da2-136">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="e9da2-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e9da2-137">Si un partenaire CSP a un revendeur sans ID MPN, cette valeur est définie sur l’ID MPN du partenaire à la place.</span><span class="sxs-lookup"><span data-stu-id="e9da2-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="e9da2-138">Si le partenaire fournisseur de solutions Cloud supprime un ID revendeur, cette valeur est définie sur-1.</span><span class="sxs-lookup"><span data-stu-id="e9da2-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="e9da2-139">Champs de fichier basés sur une licence</span><span class="sxs-lookup"><span data-stu-id="e9da2-139">License-based file fields</span></span>


<span data-ttu-id="e9da2-140">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e9da2-141"><strong>Chronique</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e9da2-142"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e9da2-143"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e9da2-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="e9da2-145">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e9da2-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e9da2-146">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="e9da2-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e9da2-147">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e9da2-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e9da2-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e9da2-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="e9da2-150">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e9da2-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e9da2-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-152">OrderId</span><span class="sxs-lookup"><span data-stu-id="e9da2-152">OrderID</span></span></td>
<td><p><span data-ttu-id="e9da2-153">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9da2-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e9da2-154">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e9da2-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e9da2-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e9da2-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e9da2-157">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9da2-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e9da2-158">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e9da2-159">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e9da2-160">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="e9da2-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e9da2-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e9da2-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="e9da2-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e9da2-163">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="e9da2-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e9da2-164">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e9da2-165">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e9da2-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e9da2-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="e9da2-167">OfferID</span></span></td>
<td><p><span data-ttu-id="e9da2-168">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-168">Unique offer ID.</span></span> <span data-ttu-id="e9da2-169">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e9da2-170"><b>Remarque</b> : cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e9da2-171">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e9da2-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e9da2-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e9da2-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e9da2-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e9da2-174">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e9da2-175"><b>Remarque</b> : cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e9da2-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e9da2-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="e9da2-177">OfferName</span></span></td>
<td><p><span data-ttu-id="e9da2-178">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e9da2-179">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="e9da2-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e9da2-181">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="e9da2-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e9da2-182">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="e9da2-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e9da2-183">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e9da2-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e9da2-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e9da2-186">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e9da2-187">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="e9da2-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e9da2-188">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e9da2-189">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e9da2-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e9da2-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e9da2-192">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e9da2-193">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="e9da2-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e9da2-194">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e9da2-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e9da2-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e9da2-197">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="e9da2-198">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="e9da2-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e9da2-199">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e9da2-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e9da2-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e9da2-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e9da2-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="e9da2-202">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-202">The type of charge or adjustment.</span></span> <span data-ttu-id="e9da2-203">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e9da2-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e9da2-204">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e9da2-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e9da2-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e9da2-206">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="e9da2-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e9da2-207">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e9da2-208">6.82</span><span class="sxs-lookup"><span data-stu-id="e9da2-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-209">Quantité</span><span class="sxs-lookup"><span data-stu-id="e9da2-209">Quantity</span></span></td>
<td><p><span data-ttu-id="e9da2-210">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="e9da2-210">Number of seats.</span></span> <span data-ttu-id="e9da2-211">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e9da2-212">2</span><span class="sxs-lookup"><span data-stu-id="e9da2-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-213">Montant</span><span class="sxs-lookup"><span data-stu-id="e9da2-213">Amount</span></span></td>
<td><p><span data-ttu-id="e9da2-214">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="e9da2-214">Total of price for quantity.</span></span> <span data-ttu-id="e9da2-215">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="e9da2-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e9da2-216">13.32</span><span class="sxs-lookup"><span data-stu-id="e9da2-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e9da2-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e9da2-218">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e9da2-219">Les licences de produit comprises dans une compétence ou des cartes ou les nouveaux abonnements éligibles à un Incentive contiennent également un montant de remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="e9da2-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e9da2-220">2.32</span><span class="sxs-lookup"><span data-stu-id="e9da2-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-221">Sous-total</span><span class="sxs-lookup"><span data-stu-id="e9da2-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="e9da2-222">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="e9da2-222">Total before tax.</span></span> <span data-ttu-id="e9da2-223">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e9da2-224">11</span><span class="sxs-lookup"><span data-stu-id="e9da2-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-225">Taxe</span><span class="sxs-lookup"><span data-stu-id="e9da2-225">Tax</span></span></td>
<td><p><span data-ttu-id="e9da2-226">Frais liés au montant des taxes, en&#39;fonction de vos règles fiscales et de certaines circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e9da2-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e9da2-227">0</span><span class="sxs-lookup"><span data-stu-id="e9da2-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e9da2-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e9da2-229">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="e9da2-229">Total after tax.</span></span> <span data-ttu-id="e9da2-230">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="e9da2-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e9da2-231">11</span><span class="sxs-lookup"><span data-stu-id="e9da2-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-232">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-232">Currency</span></span></td>
<td><p><span data-ttu-id="e9da2-233">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-233">Currency type.</span></span> <span data-ttu-id="e9da2-234">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="e9da2-235">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e9da2-236">EUR</span><span class="sxs-lookup"><span data-stu-id="e9da2-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e9da2-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="e9da2-238">Nom&#39;de l’organisation du client comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e9da2-239">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e9da2-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e9da2-240">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="e9da2-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-241">MPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-242">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="e9da2-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e9da2-243">4390934</span><span class="sxs-lookup"><span data-stu-id="e9da2-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-245">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e9da2-246">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e9da2-247">4390934</span><span class="sxs-lookup"><span data-stu-id="e9da2-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="e9da2-248">DomainName</span></span></td>
<td><p><span data-ttu-id="e9da2-249">Nom&#39;de domaine du client, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e9da2-250">Cela ne doit pas être utilisé pour identifier de manière unique le client, car le client ou le partenaire peut mettre à jour le domaine personnel/default via le portail O365.</span><span class="sxs-lookup"><span data-stu-id="e9da2-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="e9da2-251">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e9da2-252">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e9da2-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e9da2-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e9da2-254">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-254">Subscription nickname.</span></span> <span data-ttu-id="e9da2-255">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="e9da2-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e9da2-256">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="e9da2-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e9da2-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e9da2-258">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e9da2-259">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="e9da2-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e9da2-260">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="e9da2-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e9da2-261">Champs de fichier basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="e9da2-261">Usage-based file fields</span></span>


<span data-ttu-id="e9da2-262">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e9da2-263">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="e9da2-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e9da2-264"><strong>Chronique</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="e9da2-265"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="e9da2-266"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e9da2-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="e9da2-268">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e9da2-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e9da2-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e9da2-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e9da2-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="e9da2-271">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e9da2-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="e9da2-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e9da2-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e9da2-274">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e9da2-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="e9da2-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e9da2-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="e9da2-277">Nom&#39;de l’organisation du client comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="e9da2-278">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e9da2-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e9da2-279">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="e9da2-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-280">MPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-281">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="e9da2-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e9da2-282">4390934</span><span class="sxs-lookup"><span data-stu-id="e9da2-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-284">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e9da2-285">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="e9da2-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="e9da2-286">4390934</span><span class="sxs-lookup"><span data-stu-id="e9da2-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e9da2-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e9da2-288">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="e9da2-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e9da2-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e9da2-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e9da2-291">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e9da2-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e9da2-292">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e9da2-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e9da2-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e9da2-295">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e9da2-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e9da2-296">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e9da2-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e9da2-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e9da2-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e9da2-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e9da2-299">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9da2-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e9da2-300">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e9da2-301">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e9da2-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e9da2-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e9da2-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e9da2-304">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="e9da2-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e9da2-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e9da2-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e9da2-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e9da2-307">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="e9da2-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e9da2-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e9da2-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-309">OrderId</span><span class="sxs-lookup"><span data-stu-id="e9da2-309">OrderID</span></span></td>
<td><p><span data-ttu-id="e9da2-310">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9da2-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e9da2-311">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e9da2-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e9da2-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e9da2-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="e9da2-314">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="e9da2-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e9da2-315">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="e9da2-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e9da2-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="e9da2-317">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="e9da2-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e9da2-318">Service Bus-individu ou Pack</span><span class="sxs-lookup"><span data-stu-id="e9da2-318">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="e9da2-319">SQL Azure Database-Business ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="e9da2-319">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e9da2-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e9da2-321">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="e9da2-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e9da2-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e9da2-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-323">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="e9da2-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="e9da2-324">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="e9da2-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e9da2-325">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="e9da2-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e9da2-326">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="e9da2-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-327">Région</span><span class="sxs-lookup"><span data-stu-id="e9da2-327">Region</span></span></td>
<td><p><span data-ttu-id="e9da2-328">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-328">The region the usage applies to.</span></span> <span data-ttu-id="e9da2-329">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="e9da2-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e9da2-330">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="e9da2-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-331">SKU</span><span class="sxs-lookup"><span data-stu-id="e9da2-331">SKU</span></span></td>
<td><p><span data-ttu-id="e9da2-332">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="e9da2-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e9da2-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e9da2-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e9da2-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e9da2-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e9da2-335">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="e9da2-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e9da2-336">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="e9da2-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e9da2-337">1</span><span class="sxs-lookup"><span data-stu-id="e9da2-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e9da2-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e9da2-339">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="e9da2-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e9da2-340">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e9da2-341">11</span><span class="sxs-lookup"><span data-stu-id="e9da2-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e9da2-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e9da2-343">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="e9da2-343">Units included as part of the offer.</span></span> <span data-ttu-id="e9da2-344">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="e9da2-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e9da2-345">0</span><span class="sxs-lookup"><span data-stu-id="e9da2-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e9da2-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e9da2-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e9da2-347">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e9da2-348">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="e9da2-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e9da2-349">11</span><span class="sxs-lookup"><span data-stu-id="e9da2-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e9da2-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="e9da2-351">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e9da2-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="e9da2-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e9da2-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e9da2-354">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e9da2-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e9da2-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="e9da2-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e9da2-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e9da2-357">Frais liés au montant des taxes, en&#39;fonction de vos règles fiscales et de certaines circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="e9da2-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e9da2-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="e9da2-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e9da2-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e9da2-360">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="e9da2-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e9da2-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="e9da2-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-362">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-362">Currency</span></span></td>
<td><p><span data-ttu-id="e9da2-363">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-363">Currency type.</span></span> <span data-ttu-id="e9da2-364">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="e9da2-365">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e9da2-366">EUR</span><span class="sxs-lookup"><span data-stu-id="e9da2-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e9da2-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e9da2-368">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="e9da2-368">Pretax price per unit.</span></span> <span data-ttu-id="e9da2-369">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e9da2-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e9da2-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="e9da2-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e9da2-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e9da2-372">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="e9da2-372">Post tax price per unit.</span></span> <span data-ttu-id="e9da2-373">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e9da2-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e9da2-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="e9da2-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e9da2-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="e9da2-376">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-376">The type of charge or adjustment.</span></span> <span data-ttu-id="e9da2-377">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e9da2-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e9da2-378">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e9da2-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e9da2-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e9da2-380">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="e9da2-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e9da2-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="e9da2-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="e9da2-383">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="e9da2-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e9da2-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e9da2-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e9da2-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e9da2-386">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="e9da2-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e9da2-387">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="e9da2-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e9da2-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="e9da2-389">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="e9da2-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e9da2-390">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="e9da2-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e9da2-391">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="e9da2-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e9da2-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="e9da2-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e9da2-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e9da2-394">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="e9da2-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e9da2-395">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="e9da2-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-396">Project</span><span class="sxs-lookup"><span data-stu-id="e9da2-396">Project</span></span></td>
<td><p><span data-ttu-id="e9da2-397">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="e9da2-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e9da2-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e9da2-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e9da2-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e9da2-400">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="e9da2-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e9da2-401">Par exemple : Si vous avez une connexion configurée individuellement pendant une période de 30 jours, les informations de service 1 lisent « 1,000000 connexions/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="e9da2-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="e9da2-402">Si vous avez configuré un 25 Pack de connexions ServiceBus et que vous avez utilisé 1 pendant cette journée, votre instruction d’utilisation quotidienne pour ce jour indique « 25 connexions/30 jours-utilisé : 1,000000 ».</span><span class="sxs-lookup"><span data-stu-id="e9da2-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e9da2-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="e9da2-404">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e9da2-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e9da2-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e9da2-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="e9da2-406">DomainName</span></span></td>
<td><p><span data-ttu-id="e9da2-407">Nom&#39;de domaine du client, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="e9da2-408">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e9da2-409">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e9da2-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="e9da2-410">Unit</span><span class="sxs-lookup"><span data-stu-id="e9da2-410">Unit</span></span></td>
<td><p><span data-ttu-id="e9da2-411">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="e9da2-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="e9da2-412">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="e9da2-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="e9da2-413">Champs de fichier ponctuels et périodiques</span><span class="sxs-lookup"><span data-stu-id="e9da2-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e9da2-414">Colonne</span><span class="sxs-lookup"><span data-stu-id="e9da2-414">Column</span></span></th>
<th><span data-ttu-id="e9da2-415">Description</span><span class="sxs-lookup"><span data-stu-id="e9da2-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="e9da2-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e9da2-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="e9da2-417">Identificateur de locataire unique Microsoft Azure Active Directory pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e9da2-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e9da2-418">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="e9da2-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e9da2-419">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-420">ID client</span><span class="sxs-lookup"><span data-stu-id="e9da2-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="e9da2-421">ID de locataire unique Microsoft Azure Active Directory, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-422">Nom du client</span><span class="sxs-lookup"><span data-stu-id="e9da2-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="e9da2-423">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e9da2-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="e9da2-425">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="e9da2-426">Cela ne doit pas être utilisé pour identifier de manière unique le client, car le client ou le partenaire peut mettre à jour le domaine personnel/default via le portail O365.</span><span class="sxs-lookup"><span data-stu-id="e9da2-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="e9da2-427">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-428">Pays du client</span><span class="sxs-lookup"><span data-stu-id="e9da2-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="e9da2-429">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-430">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="e9da2-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="e9da2-431">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="e9da2-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="e9da2-432">MpnId</span></span></td>
<td><p><span data-ttu-id="e9da2-433">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="e9da2-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-434">Revendeur MpnId</span><span class="sxs-lookup"><span data-stu-id="e9da2-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="e9da2-435">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-436">ID de commande</span><span class="sxs-lookup"><span data-stu-id="e9da2-436">Order ID</span></span></td>
<td><p><span data-ttu-id="e9da2-437">Identificateur unique d’une commande dans la plateforme Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="e9da2-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="e9da2-438">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-439">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="e9da2-439">Order date</span></span></td>
<td><p><span data-ttu-id="e9da2-440">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="e9da2-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="e9da2-441">ProductId</span></span></td>
<td><p><span data-ttu-id="e9da2-442">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="e9da2-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="e9da2-443">SkuId</span></span></td>
<td><p><span data-ttu-id="e9da2-444">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e9da2-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="e9da2-446">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-446">The ID for a particular Availability.</span></span> <span data-ttu-id="e9da2-447">La « disponibilité » indique si une référence (SKU) est disponible à l’achat pour le pays donné, la devise, le secteur d’activité, etc.</span><span class="sxs-lookup"><span data-stu-id="e9da2-447">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-448">Nom de la référence</span><span class="sxs-lookup"><span data-stu-id="e9da2-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="e9da2-449">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-450">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="e9da2-450">Product name</span></span></td>
<td><p><span data-ttu-id="e9da2-451">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="e9da2-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="e9da2-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="e9da2-453">Nom de l’éditeur du produit.</span><span class="sxs-lookup"><span data-stu-id="e9da2-453">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="e9da2-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="e9da2-455">ID unique de ce serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="e9da2-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-456">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="e9da2-457">Nom convivial d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-458">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="e9da2-459">Identificateur unique d’un abonnement dans la plateforme Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="e9da2-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="e9da2-460">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="e9da2-461">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e9da2-463">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-463">Start day of the charges.</span></span> <span data-ttu-id="e9da2-464">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e9da2-466">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-466">End day of the charges.</span></span> <span data-ttu-id="e9da2-467">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e9da2-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-468">Term et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="e9da2-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="e9da2-469">La durée et le cycle de facturation de l’achat.</span><span class="sxs-lookup"><span data-stu-id="e9da2-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="e9da2-470">Par exemple, « 1 an, mensuelle. »</span><span class="sxs-lookup"><span data-stu-id="e9da2-470">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-471">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="e9da2-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="e9da2-472">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-473">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="e9da2-474">Prix tel qu’il a été publié dans le pricelist au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="e9da2-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e9da2-475">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-476">Prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="e9da2-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="e9da2-477">Le prix unitaire après ajustements a été effectué.</span><span class="sxs-lookup"><span data-stu-id="e9da2-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-478">Quantité</span><span class="sxs-lookup"><span data-stu-id="e9da2-478">Quantity</span></span></td>
<td><p><span data-ttu-id="e9da2-479">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="e9da2-479">Number of units.</span></span> <span data-ttu-id="e9da2-480">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-481">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="e9da2-481">Unit type</span></span></td>
<td><p><span data-ttu-id="e9da2-482">Type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="e9da2-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="e9da2-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="e9da2-484">Une explication de toute remise applicable.</span><span class="sxs-lookup"><span data-stu-id="e9da2-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-485">Sous-total</span><span class="sxs-lookup"><span data-stu-id="e9da2-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="e9da2-486">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="e9da2-486">Total before tax.</span></span> <span data-ttu-id="e9da2-487">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-488">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="e9da2-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="e9da2-489">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="e9da2-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-490">Total</span><span class="sxs-lookup"><span data-stu-id="e9da2-490">Total</span></span></td>
<td><p><span data-ttu-id="e9da2-491">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="e9da2-491">Total after tax.</span></span> <span data-ttu-id="e9da2-492">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="e9da2-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-493">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-493">Currency</span></span></td>
<td><p><span data-ttu-id="e9da2-494">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-494">Currency type.</span></span> <span data-ttu-id="e9da2-495">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e9da2-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="e9da2-496">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="e9da2-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="e9da2-498">Autre identificateur à un ID de commande.</span><span class="sxs-lookup"><span data-stu-id="e9da2-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-499">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="e9da2-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="e9da2-500">Affiche tous les mois lorsque la facturation mensuelle est activée.</span><span class="sxs-lookup"><span data-stu-id="e9da2-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="e9da2-501">Sinon, vide.</span><span class="sxs-lookup"><span data-stu-id="e9da2-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="e9da2-502">Champs du fichier d’utilisation avec évaluation quotidienne</span><span class="sxs-lookup"><span data-stu-id="e9da2-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e9da2-503">Colonne</span><span class="sxs-lookup"><span data-stu-id="e9da2-503">Column</span></span></th>
<th><span data-ttu-id="e9da2-504">Description</span><span class="sxs-lookup"><span data-stu-id="e9da2-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="e9da2-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e9da2-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="e9da2-506">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e9da2-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e9da2-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="e9da2-508">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="e9da2-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="e9da2-510">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-511">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="e9da2-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="e9da2-512">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e9da2-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e9da2-513">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e9da2-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e9da2-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="e9da2-515">Nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-515">The customer's domain name.</span></span> <span data-ttu-id="e9da2-516">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-517">Pays du client</span><span class="sxs-lookup"><span data-stu-id="e9da2-517">Customer country</span></span></td>
<td><p><span data-ttu-id="e9da2-518">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="e9da2-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-519">MPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-520">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="e9da2-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-521">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="e9da2-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="e9da2-522">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e9da2-523">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e9da2-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e9da2-525">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="e9da2-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="e9da2-526">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-527">ProductId</span><span class="sxs-lookup"><span data-stu-id="e9da2-527">ProductId</span></span></td>
<td><p><span data-ttu-id="e9da2-528">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="e9da2-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="e9da2-529">SkuId</span></span></td>
<td><p><span data-ttu-id="e9da2-530">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e9da2-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="e9da2-532">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-532">The ID for a particular Availability.</span></span> <span data-ttu-id="e9da2-533">La « disponibilité » indique si une référence (SKU) est disponible à l’achat pour le pays donné, la devise, le secteur d’activité, etc.</span><span class="sxs-lookup"><span data-stu-id="e9da2-533">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-534">Nom de la référence</span><span class="sxs-lookup"><span data-stu-id="e9da2-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="e9da2-535">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="e9da2-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="e9da2-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="e9da2-537">Nom du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="e9da2-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="e9da2-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="e9da2-539">ID du serveur de publication, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e9da2-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="e9da2-540">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-541">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="e9da2-542">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e9da2-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e9da2-543">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="e9da2-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-544">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="e9da2-545">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9da2-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e9da2-546">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="e9da2-547">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e9da2-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e9da2-549">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e9da2-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="e9da2-550">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e9da2-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e9da2-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e9da2-552">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e9da2-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="e9da2-553">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e9da2-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-554">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="e9da2-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="e9da2-555">Date d’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="e9da2-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-556">Type de compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="e9da2-557">Type de compteur.</span><span class="sxs-lookup"><span data-stu-id="e9da2-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-558">Catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="e9da2-559">Service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-560">ID du compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="e9da2-561">ID du compteur utilisé.</span><span class="sxs-lookup"><span data-stu-id="e9da2-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-562">Sous-catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="e9da2-563">Type de service Azure pouvant affecter le tarif.</span><span class="sxs-lookup"><span data-stu-id="e9da2-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-564">Nom du compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="e9da2-565">Unité de mesure du compteur consommé.</span><span class="sxs-lookup"><span data-stu-id="e9da2-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-566">Région du compteur</span><span class="sxs-lookup"><span data-stu-id="e9da2-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="e9da2-567">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="e9da2-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-568">Unit</span><span class="sxs-lookup"><span data-stu-id="e9da2-568">Unit</span></span></td>
<td><p><span data-ttu-id="e9da2-569">Unité du nom de la ressource.</span><span class="sxs-lookup"><span data-stu-id="e9da2-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-570">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="e9da2-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="e9da2-571">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="e9da2-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="e9da2-572">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-573">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="e9da2-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="e9da2-574">Centre de stockage dans lequel le compteur est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="e9da2-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-575">Service consommé</span><span class="sxs-lookup"><span data-stu-id="e9da2-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="e9da2-576">Service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="e9da2-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="e9da2-577">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="e9da2-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="e9da2-578">URI de la ressource en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-579">Type de frais</span><span class="sxs-lookup"><span data-stu-id="e9da2-579">Charge type</span></span></td>
<td><p><span data-ttu-id="e9da2-580">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-580">The type of charge or adjustment.</span></span> <span data-ttu-id="e9da2-581">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-582">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="e9da2-582">Unit price</span></span></td>
<td><p><span data-ttu-id="e9da2-583">Prix par licence, tel que publié dans le pricelist au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="e9da2-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e9da2-584">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-585">Quantité</span><span class="sxs-lookup"><span data-stu-id="e9da2-585">Quantity</span></span></td>
<td><p><span data-ttu-id="e9da2-586">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="e9da2-586">Number of licenses.</span></span> <span data-ttu-id="e9da2-587">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-588">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="e9da2-588">Unit type</span></span></td>
<td><p><span data-ttu-id="e9da2-589">Type d’unité dans lequel le compteur est facturé.</span><span class="sxs-lookup"><span data-stu-id="e9da2-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="e9da2-590">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="e9da2-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-591">Facturation préalable</span><span class="sxs-lookup"><span data-stu-id="e9da2-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="e9da2-592">Montant total avant taxes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-593">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="e9da2-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="e9da2-594">Devise dans la région géographique du client</span><span class="sxs-lookup"><span data-stu-id="e9da2-594">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-595">Total de la tarification Tarif</span><span class="sxs-lookup"><span data-stu-id="e9da2-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="e9da2-596">La tarification avant les taxes est ajoutée.</span><span class="sxs-lookup"><span data-stu-id="e9da2-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-597">Devise de tarification</span><span class="sxs-lookup"><span data-stu-id="e9da2-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="e9da2-598">Devise dans le pricelist.</span><span class="sxs-lookup"><span data-stu-id="e9da2-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="e9da2-599">Informations sur le service 1</span><span class="sxs-lookup"><span data-stu-id="e9da2-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="e9da2-600">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="e9da2-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-601">Informations sur le service 2</span><span class="sxs-lookup"><span data-stu-id="e9da2-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="e9da2-602">Champ hérité qui capture les métadonnées facultatives propres au service.</span><span class="sxs-lookup"><span data-stu-id="e9da2-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="e9da2-603">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="e9da2-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="e9da2-604">Toutes les informations supplémentaires non couvertes dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="e9da2-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="e9da2-605">Mappage des frais entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="e9da2-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e9da2-606">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="e9da2-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e9da2-607">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="e9da2-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e9da2-608">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="e9da2-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="e9da2-609">Un congé, des remises ou des remboursements qui apparaissent sur la facture comme « ajustements » ne s’affichent pas dans le fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="e9da2-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="e9da2-610">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e9da2-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="e9da2-611"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-612"><strong>Description des frais de fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-613"><strong>Quels sont les frais ?</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-614"><strong>Comment faire mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="e9da2-615"><strong>Frais basés sur les licences</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-616">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="e9da2-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-617">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="e9da2-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="e9da2-618">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-619">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="e9da2-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-620">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="e9da2-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-621">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="e9da2-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-622">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-623">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="e9da2-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-624">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="e9da2-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-625">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="e9da2-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-626">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="e9da2-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-627">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="e9da2-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-628">Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="e9da2-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-629">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-630">Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="e9da2-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-631">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="e9da2-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-632">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="e9da2-633">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="e9da2-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-634">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-635">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="e9da2-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-636">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="e9da2-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="e9da2-637"><strong>Frais à usage unique</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="e9da2-638">Nouveau</span><span class="sxs-lookup"><span data-stu-id="e9da2-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-639">Utilisé lors de la création d’un nouvel achat</span><span class="sxs-lookup"><span data-stu-id="e9da2-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e9da2-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-641">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après l’augmentation</span><span class="sxs-lookup"><span data-stu-id="e9da2-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e9da2-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-643">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après réduction</span><span class="sxs-lookup"><span data-stu-id="e9da2-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-644">Annuler</span><span class="sxs-lookup"><span data-stu-id="e9da2-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-645">Utilisé lors de l’annulation d’un abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-646">Convertir</span><span class="sxs-lookup"><span data-stu-id="e9da2-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-647">Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé</span><span class="sxs-lookup"><span data-stu-id="e9da2-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="e9da2-648"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-649">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="e9da2-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-650">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="e9da2-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e9da2-651">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-652">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="e9da2-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-653">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="e9da2-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="e9da2-654"><strong>Réserve</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-655">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="e9da2-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-656">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="e9da2-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-657">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e9da2-658">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="e9da2-659"><strong>Remises basées sur l’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-660">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="e9da2-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-661">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="e9da2-662">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-663">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="e9da2-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-664">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="e9da2-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-665">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="e9da2-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-666">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e9da2-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-667">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="e9da2-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-668">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="e9da2-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="e9da2-669"><strong>Remises basées sur une licence</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-670"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="e9da2-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="e9da2-671">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e9da2-672">&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-673"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="e9da2-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="e9da2-674"><em>Exception : &quot;Offset un élément de ligne &quot; contient déjà des taxes. Consultez crédits, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="e9da2-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-675">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="e9da2-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e9da2-676">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e9da2-677">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="e9da2-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
