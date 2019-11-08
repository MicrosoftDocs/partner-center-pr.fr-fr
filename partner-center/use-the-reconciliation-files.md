---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pour obtenir une vue détaillée de chaque facture dans un cycle de facturation, téléchargez les fichiers de la conciliation à partir de l’espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753854"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="8c548-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="8c548-103">Use the reconciliation files</span></span>

<span data-ttu-id="8c548-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="8c548-104">**Applies to**</span></span>

-  <span data-ttu-id="8c548-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8c548-105">Partner Center</span></span>
-  <span data-ttu-id="8c548-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8c548-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8c548-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8c548-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8c548-108">Administration de facturation</span><span class="sxs-lookup"><span data-stu-id="8c548-108">Billing admin</span></span>
- <span data-ttu-id="8c548-109">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="8c548-109">Global admin</span></span>

<span data-ttu-id="8c548-110">Pour obtenir une vue détaillée de chaque facture dans un cycle de facturation, téléchargez les fichiers de la conciliation à partir de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="8c548-111">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="8c548-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="8c548-112">Problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="8c548-112">Formatting issues</span></span>

<span data-ttu-id="8c548-113">Parfois, votre fichier de rapprochement peut présenter des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="8c548-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="8c548-114">(Cela peut se produire, par exemple, si les paramètres régionaux en-US ne sont pas utilisés.) Suivez les étapes ci-dessous pour résoudre ces problèmes.</span><span class="sxs-lookup"><span data-stu-id="8c548-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="8c548-115">Ouvrez le fichier. csv dans Excel, puis sélectionnez la première colonne.</span><span class="sxs-lookup"><span data-stu-id="8c548-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="8c548-116">Dans le ruban, sélectionnez <strong>données</strong>, puis sélectionnez <strong>texte pour les colonnes</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="8c548-117">Dans l’Assistant Conversion de texte en colonnes, sélectionnez <strong>type de fichier délimité</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="8c548-118">Dans le champ séparateurs, sélectionnez <strong>virgule</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="8c548-119">Si l’option <strong>onglet</strong> est déjà sélectionnée, vous pouvez la conserver.</span><span class="sxs-lookup"><span data-stu-id="8c548-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="8c548-120">Sélectionnez <strong>Suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="8c548-121">Dans le champ format des données de la colonne, sélectionnez <strong>Date : mja</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="8c548-122">Dans le champ format des données de la colonne, sélectionnez <strong>texte</strong> pour toutes les colonnes de montant, puis sélectionnez <strong>Terminer</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="8c548-123">Téléchargement d’un fichier de rapprochement volumineux</span><span class="sxs-lookup"><span data-stu-id="8c548-123">Downloading a large recon file</span></span>

<span data-ttu-id="8c548-124">Les fichiers de rapprochement peuvent devenir très volumineux et parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="8c548-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="8c548-125">Pour obtenir un script PowerShell qui vous aide à télécharger des fichiers de rapprochement volumineux, consultez [obtenir des lignes de facturation](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="8c548-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="8c548-126">Décomposant par partenaire</span><span class="sxs-lookup"><span data-stu-id="8c548-126">Itemize by partner</span></span>


<span data-ttu-id="8c548-127">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="8c548-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="8c548-128">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="8c548-128">MPN ID</span></span></th>
<th><span data-ttu-id="8c548-129">Description</span><span class="sxs-lookup"><span data-stu-id="8c548-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="8c548-130">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="8c548-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="8c548-131">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="8c548-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-132">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="8c548-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="8c548-133">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="8c548-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="8c548-134">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="8c548-135">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="8c548-136">affichage eTo ou mettez à jour le revendeur. dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8c548-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="8c548-137">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8c548-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="8c548-138">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="8c548-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="8c548-139">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="8c548-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="8c548-140">Si un partenaire CSP a un revendeur sans ID MPN, cette valeur est définie sur l’ID MPN du partenaire à la place.</span><span class="sxs-lookup"><span data-stu-id="8c548-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="8c548-141">Si le partenaire fournisseur de solutions Cloud supprime un ID revendeur, cette valeur est définie sur-1.</span><span class="sxs-lookup"><span data-stu-id="8c548-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="8c548-142">Champs de fichier basés sur une licence</span><span class="sxs-lookup"><span data-stu-id="8c548-142">License-based file fields</span></span>


<span data-ttu-id="8c548-143">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="8c548-144"><strong>Chronique</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="8c548-145"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="8c548-146"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="8c548-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="8c548-148">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="8c548-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="8c548-149">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="8c548-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="8c548-150">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="8c548-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="8c548-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="8c548-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="8c548-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="8c548-153">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="8c548-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="8c548-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-155">OrderId</span><span class="sxs-lookup"><span data-stu-id="8c548-155">OrderID</span></span></td>
<td><p><span data-ttu-id="8c548-156">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c548-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="8c548-157">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="8c548-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="8c548-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="8c548-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="8c548-160">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c548-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="8c548-161">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="8c548-162">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="8c548-163">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="8c548-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="8c548-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="8c548-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="8c548-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="8c548-166">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="8c548-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="8c548-167">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="8c548-168">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="8c548-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="8c548-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="8c548-170">OfferID</span></span></td>
<td><p><span data-ttu-id="8c548-171">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="8c548-171">Unique offer ID.</span></span> <span data-ttu-id="8c548-172">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="8c548-173"><b>Remarque</b> : cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="8c548-174">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8c548-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="8c548-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="8c548-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="8c548-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="8c548-177">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="8c548-178"><b>Remarque</b> : cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="8c548-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="8c548-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="8c548-180">OfferName</span></span></td>
<td><p><span data-ttu-id="8c548-181">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="8c548-182">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="8c548-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="8c548-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="8c548-184">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="8c548-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="8c548-185">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="8c548-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="8c548-186">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="8c548-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="8c548-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="8c548-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="8c548-189">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="8c548-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="8c548-190">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="8c548-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="8c548-191">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="8c548-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="8c548-192">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="8c548-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="8c548-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="8c548-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="8c548-195">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="8c548-196">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="8c548-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="8c548-197">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="8c548-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="8c548-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="8c548-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="8c548-200">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="8c548-201">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="8c548-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="8c548-202">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="8c548-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="8c548-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="8c548-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="8c548-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="8c548-205">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="8c548-205">The type of charge or adjustment.</span></span> <span data-ttu-id="8c548-206">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="8c548-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="8c548-207">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="8c548-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="8c548-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="8c548-209">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="8c548-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="8c548-210">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="8c548-211">6.82</span><span class="sxs-lookup"><span data-stu-id="8c548-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-212">Quantité</span><span class="sxs-lookup"><span data-stu-id="8c548-212">Quantity</span></span></td>
<td><p><span data-ttu-id="8c548-213">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="8c548-213">Number of seats.</span></span> <span data-ttu-id="8c548-214">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="8c548-215">2</span><span class="sxs-lookup"><span data-stu-id="8c548-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-216">Montant</span><span class="sxs-lookup"><span data-stu-id="8c548-216">Amount</span></span></td>
<td><p><span data-ttu-id="8c548-217">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="8c548-217">Total of price for quantity.</span></span> <span data-ttu-id="8c548-218">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="8c548-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="8c548-219">13.32</span><span class="sxs-lookup"><span data-stu-id="8c548-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="8c548-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="8c548-221">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="8c548-222">Les licences de produit comprises dans une compétence ou des cartes ou les nouveaux abonnements éligibles à un Incentive contiennent également un montant de remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="8c548-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="8c548-223">2.32</span><span class="sxs-lookup"><span data-stu-id="8c548-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-224">Sous-total</span><span class="sxs-lookup"><span data-stu-id="8c548-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="8c548-225">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="8c548-225">Total before tax.</span></span> <span data-ttu-id="8c548-226">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="8c548-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="8c548-227">11</span><span class="sxs-lookup"><span data-stu-id="8c548-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-228">Taxe</span><span class="sxs-lookup"><span data-stu-id="8c548-228">Tax</span></span></td>
<td><p><span data-ttu-id="8c548-229">Frais liés au montant des taxes, en&#39;fonction de vos règles fiscales et de certaines circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="8c548-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="8c548-230">0</span><span class="sxs-lookup"><span data-stu-id="8c548-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="8c548-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="8c548-232">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="8c548-232">Total after tax.</span></span> <span data-ttu-id="8c548-233">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="8c548-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="8c548-234">11</span><span class="sxs-lookup"><span data-stu-id="8c548-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-235">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="8c548-235">Currency</span></span></td>
<td><p><span data-ttu-id="8c548-236">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-236">Currency type.</span></span> <span data-ttu-id="8c548-237">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="8c548-238">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="8c548-239">EUR</span><span class="sxs-lookup"><span data-stu-id="8c548-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="8c548-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="8c548-241">Nom&#39;de l’organisation du client comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="8c548-242">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="8c548-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="8c548-243">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="8c548-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-244">MPNID</span></span></td>
<td><p><span data-ttu-id="8c548-245">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="8c548-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="8c548-246">4390934</span><span class="sxs-lookup"><span data-stu-id="8c548-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="8c548-248">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="8c548-249">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="8c548-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="8c548-250">4390934</span><span class="sxs-lookup"><span data-stu-id="8c548-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="8c548-251">DomainName</span></span></td>
<td><p><span data-ttu-id="8c548-252">Nom&#39;de domaine du client, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="8c548-253">Cela ne doit pas être utilisé pour identifier de manière unique le client, car le client ou le partenaire peut mettre à jour le domaine personnel/default via le portail O365.</span><span class="sxs-lookup"><span data-stu-id="8c548-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="8c548-254">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="8c548-255">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="8c548-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="8c548-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="8c548-257">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-257">Subscription nickname.</span></span> <span data-ttu-id="8c548-258">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="8c548-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="8c548-259">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="8c548-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="8c548-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="8c548-261">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="8c548-262">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="8c548-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="8c548-263">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="8c548-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="8c548-264">Champs de fichier basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="8c548-264">Usage-based file fields</span></span>


<span data-ttu-id="8c548-265">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="8c548-266">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="8c548-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="8c548-267"><strong>Chronique</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="8c548-268"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="8c548-269"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="8c548-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="8c548-271">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="8c548-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="8c548-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="8c548-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="8c548-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="8c548-274">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="8c548-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="8c548-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="8c548-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="8c548-277">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="8c548-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="8c548-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="8c548-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="8c548-280">Nom&#39;de l’organisation du client comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="8c548-281">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="8c548-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="8c548-282">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="8c548-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-283">MPNID</span></span></td>
<td><p><span data-ttu-id="8c548-284">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="8c548-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="8c548-285">4390934</span><span class="sxs-lookup"><span data-stu-id="8c548-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="8c548-287">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="8c548-288">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="8c548-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="8c548-289">4390934</span><span class="sxs-lookup"><span data-stu-id="8c548-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="8c548-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="8c548-291">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="8c548-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="8c548-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="8c548-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="8c548-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="8c548-294">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="8c548-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="8c548-295">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="8c548-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="8c548-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="8c548-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="8c548-298">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="8c548-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="8c548-299">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="8c548-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="8c548-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="8c548-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="8c548-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="8c548-302">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c548-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="8c548-303">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="8c548-304">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="8c548-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="8c548-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="8c548-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="8c548-307">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="8c548-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="8c548-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="8c548-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="8c548-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="8c548-310">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="8c548-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="8c548-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="8c548-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-312">OrderId</span><span class="sxs-lookup"><span data-stu-id="8c548-312">OrderID</span></span></td>
<td><p><span data-ttu-id="8c548-313">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c548-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="8c548-314">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="8c548-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="8c548-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="8c548-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="8c548-317">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="8c548-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="8c548-318">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="8c548-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="8c548-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="8c548-320">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="8c548-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="8c548-321">Service Bus-individu ou Pack</span><span class="sxs-lookup"><span data-stu-id="8c548-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="8c548-322">SQL Azure Database-Business ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="8c548-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="8c548-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="8c548-324">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="8c548-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="8c548-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="8c548-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-326">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="8c548-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="8c548-327">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="8c548-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="8c548-328">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="8c548-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="8c548-329">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="8c548-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-330">Région</span><span class="sxs-lookup"><span data-stu-id="8c548-330">Region</span></span></td>
<td><p><span data-ttu-id="8c548-331">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="8c548-331">The region the usage applies to.</span></span> <span data-ttu-id="8c548-332">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="8c548-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="8c548-333">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="8c548-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-334">SKU</span><span class="sxs-lookup"><span data-stu-id="8c548-334">SKU</span></span></td>
<td><p><span data-ttu-id="8c548-335">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="8c548-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="8c548-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="8c548-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="8c548-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="8c548-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="8c548-338">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="8c548-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="8c548-339">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="8c548-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="8c548-340">1</span><span class="sxs-lookup"><span data-stu-id="8c548-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="8c548-342">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="8c548-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="8c548-343">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="8c548-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="8c548-344">11</span><span class="sxs-lookup"><span data-stu-id="8c548-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="8c548-346">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="8c548-346">Units included as part of the offer.</span></span> <span data-ttu-id="8c548-347">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="8c548-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="8c548-348">0</span><span class="sxs-lookup"><span data-stu-id="8c548-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="8c548-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="8c548-350">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="8c548-351">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="8c548-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="8c548-352">11</span><span class="sxs-lookup"><span data-stu-id="8c548-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="8c548-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="8c548-354">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="8c548-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="8c548-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="8c548-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="8c548-357">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="8c548-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="8c548-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="8c548-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="8c548-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="8c548-360">Frais liés au montant des taxes, en&#39;fonction de vos règles fiscales et de certaines circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="8c548-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="8c548-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="8c548-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="8c548-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="8c548-363">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="8c548-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="8c548-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="8c548-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-365">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="8c548-365">Currency</span></span></td>
<td><p><span data-ttu-id="8c548-366">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-366">Currency type.</span></span> <span data-ttu-id="8c548-367">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="8c548-368">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="8c548-369">EUR</span><span class="sxs-lookup"><span data-stu-id="8c548-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="8c548-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="8c548-371">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="8c548-371">Pretax price per unit.</span></span> <span data-ttu-id="8c548-372">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="8c548-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="8c548-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="8c548-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="8c548-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="8c548-375">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="8c548-375">Post tax price per unit.</span></span> <span data-ttu-id="8c548-376">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="8c548-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="8c548-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="8c548-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="8c548-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="8c548-379">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="8c548-379">The type of charge or adjustment.</span></span> <span data-ttu-id="8c548-380">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="8c548-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="8c548-381">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="8c548-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="8c548-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="8c548-383">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="8c548-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="8c548-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="8c548-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="8c548-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="8c548-386">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="8c548-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="8c548-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="8c548-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="8c548-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="8c548-389">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="8c548-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="8c548-390">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="8c548-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="8c548-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="8c548-392">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="8c548-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="8c548-393">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="8c548-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="8c548-394">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="8c548-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="8c548-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="8c548-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="8c548-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="8c548-397">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="8c548-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="8c548-398">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="8c548-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-399">Project</span><span class="sxs-lookup"><span data-stu-id="8c548-399">Project</span></span></td>
<td><p><span data-ttu-id="8c548-400">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="8c548-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="8c548-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="8c548-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="8c548-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="8c548-403">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="8c548-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="8c548-404">Par exemple : Si vous avez une connexion configurée individuellement pendant une période de 30 jours, les informations de service 1 lisent « 1,000000 connexions/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="8c548-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="8c548-405">Si vous avez configuré un 25 Pack de connexions ServiceBus et que vous avez utilisé 1 pendant cette journée, votre instruction d’utilisation quotidienne pour ce jour indique « 25 connexions/30 jours-utilisé : 1,000000 ».</span><span class="sxs-lookup"><span data-stu-id="8c548-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="8c548-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="8c548-407">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="8c548-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="8c548-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="8c548-409">DomainName</span></span></td>
<td><p><span data-ttu-id="8c548-410">Nom&#39;de domaine du client, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="8c548-411">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="8c548-412">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="8c548-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-413">Unit</span><span class="sxs-lookup"><span data-stu-id="8c548-413">Unit</span></span></td>
<td><p><span data-ttu-id="8c548-414">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="8c548-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="8c548-415">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="8c548-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="8c548-416">Champs de fichier ponctuels et périodiques</span><span class="sxs-lookup"><span data-stu-id="8c548-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="8c548-417">Colonne</span><span class="sxs-lookup"><span data-stu-id="8c548-417">Column</span></span></th>
<th><span data-ttu-id="8c548-418">Description</span><span class="sxs-lookup"><span data-stu-id="8c548-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="8c548-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="8c548-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="8c548-420">Identificateur de locataire unique Microsoft Azure Active Directory pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="8c548-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="8c548-421">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="8c548-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="8c548-422">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="8c548-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-423">ID client</span><span class="sxs-lookup"><span data-stu-id="8c548-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="8c548-424">ID de locataire unique Microsoft Azure Active Directory, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-425">Nom du client</span><span class="sxs-lookup"><span data-stu-id="8c548-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="8c548-426">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="8c548-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="8c548-428">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="8c548-429">Cela ne doit pas être utilisé pour identifier de manière unique le client, car le client ou le partenaire peut mettre à jour le domaine personnel/default via le portail O365.</span><span class="sxs-lookup"><span data-stu-id="8c548-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="8c548-430">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-431">Pays du client</span><span class="sxs-lookup"><span data-stu-id="8c548-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="8c548-432">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-433">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="8c548-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="8c548-434">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="8c548-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="8c548-435">MpnId</span></span></td>
<td><p><span data-ttu-id="8c548-436">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="8c548-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-437">Revendeur MpnId</span><span class="sxs-lookup"><span data-stu-id="8c548-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="8c548-438">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-439">ID de commande</span><span class="sxs-lookup"><span data-stu-id="8c548-439">Order ID</span></span></td>
<td><p><span data-ttu-id="8c548-440">Identificateur unique d’une commande dans la plateforme Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="8c548-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="8c548-441">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-442">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="8c548-442">Order date</span></span></td>
<td><p><span data-ttu-id="8c548-443">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="8c548-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="8c548-444">ProductId</span></span></td>
<td><p><span data-ttu-id="8c548-445">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="8c548-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="8c548-446">SkuId</span></span></td>
<td><p><span data-ttu-id="8c548-447">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="8c548-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="8c548-449">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-449">The ID for a particular Availability.</span></span> <span data-ttu-id="8c548-450">La « disponibilité » indique si une référence (SKU) est disponible à l’achat pour le pays donné, la devise, le secteur d’activité, etc.</span><span class="sxs-lookup"><span data-stu-id="8c548-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-451">Nom de la référence</span><span class="sxs-lookup"><span data-stu-id="8c548-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="8c548-452">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-453">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="8c548-453">Product name</span></span></td>
<td><p><span data-ttu-id="8c548-454">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="8c548-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="8c548-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="8c548-456">Nom de l’éditeur du produit.</span><span class="sxs-lookup"><span data-stu-id="8c548-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="8c548-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="8c548-458">ID unique de ce serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="8c548-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-459">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="8c548-460">Nom convivial d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-461">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="8c548-462">Identificateur unique d’un abonnement dans la plateforme Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="8c548-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="8c548-463">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="8c548-464">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="8c548-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="8c548-466">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-466">Start day of the charges.</span></span> <span data-ttu-id="8c548-467">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="8c548-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="8c548-469">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-469">End day of the charges.</span></span> <span data-ttu-id="8c548-470">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="8c548-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-471">Term et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="8c548-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="8c548-472">La durée et le cycle de facturation de l’achat.</span><span class="sxs-lookup"><span data-stu-id="8c548-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="8c548-473">Par exemple, « 1 an, mensuelle. »</span><span class="sxs-lookup"><span data-stu-id="8c548-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-474">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="8c548-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="8c548-475">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="8c548-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-476">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="8c548-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="8c548-477">Prix tel qu’il a été publié dans le pricelist au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="8c548-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="8c548-478">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-479">Prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="8c548-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="8c548-480">Le prix unitaire après ajustements a été effectué.</span><span class="sxs-lookup"><span data-stu-id="8c548-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-481">Quantité</span><span class="sxs-lookup"><span data-stu-id="8c548-481">Quantity</span></span></td>
<td><p><span data-ttu-id="8c548-482">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="8c548-482">Number of units.</span></span> <span data-ttu-id="8c548-483">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-484">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="8c548-484">Unit type</span></span></td>
<td><p><span data-ttu-id="8c548-485">Type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="8c548-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="8c548-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="8c548-487">Une explication de toute remise applicable.</span><span class="sxs-lookup"><span data-stu-id="8c548-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-488">Sous-total</span><span class="sxs-lookup"><span data-stu-id="8c548-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="8c548-489">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="8c548-489">Total before tax.</span></span> <span data-ttu-id="8c548-490">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="8c548-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-491">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="8c548-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="8c548-492">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="8c548-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-493">Total</span><span class="sxs-lookup"><span data-stu-id="8c548-493">Total</span></span></td>
<td><p><span data-ttu-id="8c548-494">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="8c548-494">Total after tax.</span></span> <span data-ttu-id="8c548-495">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="8c548-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-496">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="8c548-496">Currency</span></span></td>
<td><p><span data-ttu-id="8c548-497">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-497">Currency type.</span></span> <span data-ttu-id="8c548-498">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="8c548-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="8c548-499">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="8c548-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="8c548-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="8c548-501">Autre identificateur à un ID de commande.</span><span class="sxs-lookup"><span data-stu-id="8c548-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="8c548-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="8c548-503">Affiche tous les mois lorsque la facturation mensuelle est activée.</span><span class="sxs-lookup"><span data-stu-id="8c548-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="8c548-504">Sinon, vide.</span><span class="sxs-lookup"><span data-stu-id="8c548-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="8c548-506">Représente le nombre total d’unités achetées ou consommées.</span><span class="sxs-lookup"><span data-stu-id="8c548-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-507">PricingCurrency</span><span class="sxs-lookup"><span data-stu-id="8c548-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="8c548-508">Répertorie le prix de la ressource ou de l’offre</span><span class="sxs-lookup"><span data-stu-id="8c548-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="8c548-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="8c548-510">Taux de change appliqué pour la devise de tarification à (clients) devise de facturation</span><span class="sxs-lookup"><span data-stu-id="8c548-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="8c548-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="8c548-512">Date à laquelle la devise de tarification du taux de change de la devise de facturation est déterminée.</span><span class="sxs-lookup"><span data-stu-id="8c548-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="8c548-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="8c548-514">Description du compteur pour l’élément de ligne consommation</span><span class="sxs-lookup"><span data-stu-id="8c548-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="8c548-515">Champs du fichier d’utilisation avec évaluation quotidienne</span><span class="sxs-lookup"><span data-stu-id="8c548-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="8c548-516">Colonne</span><span class="sxs-lookup"><span data-stu-id="8c548-516">Column</span></span></th>
<th><span data-ttu-id="8c548-517">Description</span><span class="sxs-lookup"><span data-stu-id="8c548-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="8c548-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="8c548-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="8c548-519">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="8c548-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="8c548-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="8c548-521">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="8c548-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="8c548-523">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="8c548-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="8c548-525">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8c548-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="8c548-526">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="8c548-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="8c548-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="8c548-528">Nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="8c548-528">The customer's domain name.</span></span> <span data-ttu-id="8c548-529">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-530">Pays du client</span><span class="sxs-lookup"><span data-stu-id="8c548-530">Customer country</span></span></td>
<td><p><span data-ttu-id="8c548-531">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="8c548-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-532">MPNID</span></span></td>
<td><p><span data-ttu-id="8c548-533">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="8c548-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-534">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="8c548-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="8c548-535">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="8c548-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="8c548-536">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="8c548-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="8c548-538">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="8c548-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="8c548-539">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="8c548-540">ProductId</span></span></td>
<td><p><span data-ttu-id="8c548-541">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="8c548-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="8c548-542">SkuId</span></span></td>
<td><p><span data-ttu-id="8c548-543">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="8c548-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="8c548-545">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-545">The ID for a particular Availability.</span></span> <span data-ttu-id="8c548-546">La « disponibilité » indique si une référence (SKU) est disponible à l’achat pour le pays donné, la devise, le secteur d’activité, etc.</span><span class="sxs-lookup"><span data-stu-id="8c548-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-547">Nom de la référence</span><span class="sxs-lookup"><span data-stu-id="8c548-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="8c548-548">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="8c548-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="8c548-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="8c548-550">Nom du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="8c548-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="8c548-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="8c548-552">ID du serveur de publication, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="8c548-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="8c548-553">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-554">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="8c548-555">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="8c548-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="8c548-556">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="8c548-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-557">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="8c548-558">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c548-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="8c548-559">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="8c548-560">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8c548-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="8c548-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="8c548-562">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="8c548-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="8c548-563">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="8c548-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="8c548-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="8c548-565">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="8c548-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="8c548-566">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="8c548-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-567">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="8c548-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="8c548-568">Date d’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="8c548-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-569">Type de compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="8c548-570">Type de compteur.</span><span class="sxs-lookup"><span data-stu-id="8c548-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-571">Catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="8c548-572">Service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="8c548-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-573">ID du compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="8c548-574">ID du compteur utilisé.</span><span class="sxs-lookup"><span data-stu-id="8c548-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-575">Sous-catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="8c548-576">Type de service Azure pouvant affecter le tarif.</span><span class="sxs-lookup"><span data-stu-id="8c548-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-577">Nom du compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="8c548-578">Unité de mesure du compteur consommé.</span><span class="sxs-lookup"><span data-stu-id="8c548-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-579">Région du compteur</span><span class="sxs-lookup"><span data-stu-id="8c548-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="8c548-580">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="8c548-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-581">Unit</span><span class="sxs-lookup"><span data-stu-id="8c548-581">Unit</span></span></td>
<td><p><span data-ttu-id="8c548-582">Unité du nom de la ressource.</span><span class="sxs-lookup"><span data-stu-id="8c548-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-583">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="8c548-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="8c548-584">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="8c548-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="8c548-585">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="8c548-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-586">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="8c548-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="8c548-587">Centre de stockage dans lequel le compteur est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="8c548-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-588">Service consommé</span><span class="sxs-lookup"><span data-stu-id="8c548-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="8c548-589">Service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="8c548-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="8c548-590">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="8c548-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="8c548-591">URI de la ressource en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="8c548-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-592">Type de frais</span><span class="sxs-lookup"><span data-stu-id="8c548-592">Charge type</span></span></td>
<td><p><span data-ttu-id="8c548-593">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="8c548-593">The type of charge or adjustment.</span></span> <span data-ttu-id="8c548-594">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-595">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="8c548-595">Unit price</span></span></td>
<td><p><span data-ttu-id="8c548-596">Prix par licence, tel que publié dans le pricelist au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="8c548-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="8c548-597">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-598">Quantité</span><span class="sxs-lookup"><span data-stu-id="8c548-598">Quantity</span></span></td>
<td><p><span data-ttu-id="8c548-599">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="8c548-599">Number of licenses.</span></span> <span data-ttu-id="8c548-600">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-601">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="8c548-601">Unit type</span></span></td>
<td><p><span data-ttu-id="8c548-602">Type d’unité dans lequel le compteur est facturé.</span><span class="sxs-lookup"><span data-stu-id="8c548-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="8c548-603">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="8c548-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-604">Facturation préalable</span><span class="sxs-lookup"><span data-stu-id="8c548-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="8c548-605">Montant total avant taxes.</span><span class="sxs-lookup"><span data-stu-id="8c548-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-606">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="8c548-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="8c548-607">Devise dans la région géographique du client</span><span class="sxs-lookup"><span data-stu-id="8c548-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-608">Total de la tarification Tarif</span><span class="sxs-lookup"><span data-stu-id="8c548-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="8c548-609">La tarification avant les taxes est ajoutée.</span><span class="sxs-lookup"><span data-stu-id="8c548-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-610">Devise de tarification</span><span class="sxs-lookup"><span data-stu-id="8c548-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="8c548-611">Devise dans le pricelist.</span><span class="sxs-lookup"><span data-stu-id="8c548-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-612">Informations sur le service 1</span><span class="sxs-lookup"><span data-stu-id="8c548-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="8c548-613">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="8c548-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="8c548-614">Informations sur le service 2</span><span class="sxs-lookup"><span data-stu-id="8c548-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="8c548-615">Champ hérité qui capture les métadonnées facultatives propres au service.</span><span class="sxs-lookup"><span data-stu-id="8c548-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="8c548-616">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="8c548-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="8c548-617">Toutes les informations supplémentaires non couvertes dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="8c548-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="8c548-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="8c548-619">Valeur réelle facturée par unité (cela comprend les remises, les crédits acquis, etc.).</span><span class="sxs-lookup"><span data-stu-id="8c548-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="8c548-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="8c548-621">Taux de change appliqué pour la devise de tarification à la devise de facturation (clients).</span><span class="sxs-lookup"><span data-stu-id="8c548-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="8c548-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="8c548-623">Date à laquelle la devise de tarification du taux de change de la devise de facturation est déterminée.</span><span class="sxs-lookup"><span data-stu-id="8c548-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="8c548-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="8c548-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="8c548-625">Représente Azure subscriptionID.</span><span class="sxs-lookup"><span data-stu-id="8c548-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="8c548-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="8c548-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="8c548-627">Représente le nom de l’abonnement Azure.</span><span class="sxs-lookup"><span data-stu-id="8c548-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="8c548-628">Mappage des frais entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="8c548-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="8c548-629">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="8c548-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="8c548-630">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="8c548-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="8c548-631">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="8c548-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="8c548-632">Un congé, des remises ou des remboursements qui apparaissent sur la facture comme « ajustements » ne s’affichent pas dans le fichier de réconciliation.</span><span class="sxs-lookup"><span data-stu-id="8c548-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="8c548-633">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="8c548-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="8c548-634"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-635"><strong>Description des frais de fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-636"><strong>Quels sont les frais ?</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-637"><strong>Comment faire mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="8c548-638"><strong>Frais basés sur les licences</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-639">Frais d’activation</span><span class="sxs-lookup"><span data-stu-id="8c548-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-640">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="8c548-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="8c548-641">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-642">Frais d’annulation</span><span class="sxs-lookup"><span data-stu-id="8c548-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-643">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="8c548-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-644">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="8c548-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-645">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-646">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="8c548-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-647">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="8c548-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-648">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="8c548-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-649">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="8c548-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-650">Frais au prorata à l’achat</span><span class="sxs-lookup"><span data-stu-id="8c548-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-651">Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="8c548-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-652">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-653">Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="8c548-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-654">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="8c548-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-655">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="8c548-656">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="8c548-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-657">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-658">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="8c548-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-659">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="8c548-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="8c548-660"><strong>Frais à usage unique</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="8c548-661">Nouveau</span><span class="sxs-lookup"><span data-stu-id="8c548-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-662">Utilisé lors de la création d’un nouvel achat</span><span class="sxs-lookup"><span data-stu-id="8c548-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-664">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après l’augmentation</span><span class="sxs-lookup"><span data-stu-id="8c548-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="8c548-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-666">Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après réduction</span><span class="sxs-lookup"><span data-stu-id="8c548-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-667">Annuler</span><span class="sxs-lookup"><span data-stu-id="8c548-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-668">Utilisé lors de l’annulation d’un abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-669">Convertir</span><span class="sxs-lookup"><span data-stu-id="8c548-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-670">Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé</span><span class="sxs-lookup"><span data-stu-id="8c548-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="8c548-671"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-672">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="8c548-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-673">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="8c548-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="8c548-674">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-675">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="8c548-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-676">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="8c548-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="8c548-677"><strong>Réserve</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-678">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="8c548-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-679">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="8c548-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-680">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="8c548-681">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="8c548-682"><strong>Remises basées sur l’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-683">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="8c548-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-684">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="8c548-685">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-686">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="8c548-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-687">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="8c548-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-688">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="8c548-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-689">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="8c548-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-690">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="8c548-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-691">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="8c548-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="8c548-692"><strong>Remises basées sur une licence</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-693"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="8c548-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="8c548-694">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="8c548-695">&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-696"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="8c548-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="8c548-697"><em>Exception : &quot;Offset un élément de ligne &quot; contient déjà des taxes. Consultez crédits, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="8c548-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-698">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="8c548-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="8c548-699">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="8c548-700">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="8c548-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
