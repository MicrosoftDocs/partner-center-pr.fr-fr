---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 07/08/2019
description: Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 83be47cd9963d7e5f14b6c670cd57a8ab1d54011
ms.sourcegitcommit: 66afdaa662cfad217e29ba1f9e3a9ffd4349112f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/09/2019
ms.locfileid: "67694925"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="60c45-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="60c45-103">Use the reconciliation files</span></span>

<span data-ttu-id="60c45-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="60c45-104">**Applies to**</span></span>

-  <span data-ttu-id="60c45-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="60c45-105">Partner Center</span></span>
-  <span data-ttu-id="60c45-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="60c45-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="60c45-107">Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="60c45-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="60c45-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="60c45-109">Problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="60c45-109">Formatting issues</span></span>

<span data-ttu-id="60c45-110">Il peut arriver que votre fichier de rapprochement peut-être des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="60c45-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="60c45-111">(Cela peut se produire, par exemple, si les paramètres régionaux EN-US ne sont pas utilisé.) Suivez les étapes ci-dessous pour résoudre ces problèmes.</span><span class="sxs-lookup"><span data-stu-id="60c45-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="60c45-112">Ouvrez le fichier .csv dans Excel, puis sélectionnez la première colonne.</span><span class="sxs-lookup"><span data-stu-id="60c45-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="60c45-113">Dans le ruban, sélectionnez <strong>données</strong>, puis sélectionnez <strong>texte aux colonnes</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="60c45-114">Dans le texte de conversion Assistant, sélectionnez <strong>délimités de type de fichier</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="60c45-115">Dans le champ de séparateurs, sélectionnez <strong>virgules</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="60c45-116">Si <strong>onglet</strong> est déjà sélectionné, vous pouvez la laisser.</span><span class="sxs-lookup"><span data-stu-id="60c45-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="60c45-117">Sélectionnez <strong>Suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="60c45-118">Dans le champ de format de données de colonne, sélectionnez <strong>Date : MDY</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="60c45-119">Dans le champ de format de données de colonne, sélectionnez <strong>texte</strong> pour tout montant de colonnes, puis sélectionnez <strong>Terminer</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="60c45-120">Téléchargement d’un fichier de rapprochement volumineux</span><span class="sxs-lookup"><span data-stu-id="60c45-120">Downloading a large recon file</span></span>

<span data-ttu-id="60c45-121">Fichiers de rapprochement peuvent devenir très volumineux et sont parfois difficiles à télécharger.</span><span class="sxs-lookup"><span data-stu-id="60c45-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="60c45-122">Pour un script PowerShell aider à télécharger de gros fichiers de rapprochement, consultez [Get facturation](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="60c45-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="60c45-123">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="60c45-123">Itemize by partner</span></span>


<span data-ttu-id="60c45-124">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licence pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="60c45-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="60c45-125">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="60c45-125">MPN ID</span></span></th>
<th><span data-ttu-id="60c45-126">Description</span><span class="sxs-lookup"><span data-stu-id="60c45-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="60c45-127">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="60c45-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="60c45-128">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="60c45-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-129">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="60c45-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="60c45-130">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="60c45-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="60c45-131">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="60c45-132">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="60c45-133">vue d’eTo ou de mise à jour le revendeur, dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="60c45-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="60c45-134">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="60c45-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="60c45-135">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="60c45-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="60c45-136">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="60c45-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="60c45-137">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="60c45-138">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="60c45-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="60c45-139">Champs d’un fichier basé sur licence</span><span class="sxs-lookup"><span data-stu-id="60c45-139">License-based file fields</span></span>


<span data-ttu-id="60c45-140">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="60c45-141"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="60c45-142"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="60c45-143"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="60c45-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="60c45-145">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="60c45-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="60c45-146">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="60c45-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="60c45-147">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="60c45-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="60c45-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="60c45-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="60c45-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="60c45-150">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="60c45-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="60c45-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="60c45-152">OrderID</span></span></td>
<td><p><span data-ttu-id="60c45-153">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="60c45-154">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="60c45-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="60c45-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="60c45-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="60c45-157">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="60c45-158">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="60c45-159">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="60c45-160">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="60c45-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="60c45-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="60c45-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-162">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="60c45-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="60c45-163">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="60c45-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="60c45-164">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="60c45-165">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="60c45-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="60c45-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="60c45-167">OfferID</span></span></td>
<td><p><span data-ttu-id="60c45-168">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="60c45-168">Unique offer ID.</span></span> <span data-ttu-id="60c45-169">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="60c45-170"><b>Remarque</b>: Cette valeur ne correspond pas d’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="60c45-171">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="60c45-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="60c45-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="60c45-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="60c45-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="60c45-174">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="60c45-175"><b>Remarque</b>: Cette valeur correspond à l’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="60c45-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="60c45-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="60c45-177">OfferName</span></span></td>
<td><p><span data-ttu-id="60c45-178">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="60c45-179">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="60c45-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="60c45-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="60c45-181">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="60c45-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="60c45-182">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="60c45-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="60c45-183">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="60c45-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="60c45-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="60c45-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="60c45-186">La date de fin d’abonnement : 12 mois + x jours après la date de début (pour les aligner avec date de facturation du partenaire) ou 12 mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="60c45-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="60c45-187">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="60c45-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="60c45-188">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="60c45-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="60c45-189">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="60c45-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="60c45-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="60c45-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="60c45-192">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="60c45-193">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="60c45-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="60c45-194">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="60c45-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="60c45-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="60c45-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="60c45-197">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="60c45-198">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="60c45-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="60c45-199">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="60c45-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="60c45-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="60c45-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="60c45-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="60c45-202">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="60c45-202">The type of charge or adjustment.</span></span> <span data-ttu-id="60c45-203">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="60c45-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="60c45-204">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="60c45-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="60c45-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="60c45-206">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="60c45-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="60c45-207">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="60c45-208">6.82</span><span class="sxs-lookup"><span data-stu-id="60c45-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-209">Quantité</span><span class="sxs-lookup"><span data-stu-id="60c45-209">Quantity</span></span></td>
<td><p><span data-ttu-id="60c45-210">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="60c45-210">Number of seats.</span></span> <span data-ttu-id="60c45-211">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="60c45-212">2</span><span class="sxs-lookup"><span data-stu-id="60c45-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-213">Montant</span><span class="sxs-lookup"><span data-stu-id="60c45-213">Amount</span></span></td>
<td><p><span data-ttu-id="60c45-214">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="60c45-214">Total of price for quantity.</span></span> <span data-ttu-id="60c45-215">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="60c45-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="60c45-216">13.32</span><span class="sxs-lookup"><span data-stu-id="60c45-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="60c45-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="60c45-218">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="60c45-219">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="60c45-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="60c45-220">2.32</span><span class="sxs-lookup"><span data-stu-id="60c45-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-221">Sous-total</span><span class="sxs-lookup"><span data-stu-id="60c45-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="60c45-222">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="60c45-222">Total before tax.</span></span> <span data-ttu-id="60c45-223">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="60c45-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="60c45-224">11</span><span class="sxs-lookup"><span data-stu-id="60c45-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-225">Taxe</span><span class="sxs-lookup"><span data-stu-id="60c45-225">Tax</span></span></td>
<td><p><span data-ttu-id="60c45-226">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="60c45-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="60c45-227">0</span><span class="sxs-lookup"><span data-stu-id="60c45-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="60c45-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="60c45-229">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="60c45-229">Total after tax.</span></span> <span data-ttu-id="60c45-230">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="60c45-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="60c45-231">11</span><span class="sxs-lookup"><span data-stu-id="60c45-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-232">Currency</span><span class="sxs-lookup"><span data-stu-id="60c45-232">Currency</span></span></td>
<td><p><span data-ttu-id="60c45-233">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-233">Currency type.</span></span> <span data-ttu-id="60c45-234">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="60c45-235">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="60c45-236">EUR</span><span class="sxs-lookup"><span data-stu-id="60c45-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="60c45-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="60c45-238">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="60c45-239">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="60c45-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="60c45-240">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="60c45-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-241">MPNID</span></span></td>
<td><p><span data-ttu-id="60c45-242">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="60c45-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="60c45-243">4390934</span><span class="sxs-lookup"><span data-stu-id="60c45-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="60c45-245">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="60c45-246">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="60c45-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="60c45-247">4390934</span><span class="sxs-lookup"><span data-stu-id="60c45-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="60c45-248">DomainName</span></span></td>
<td><p><span data-ttu-id="60c45-249">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="60c45-250">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="60c45-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="60c45-251">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="60c45-252">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="60c45-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="60c45-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="60c45-254">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-254">Subscription nickname.</span></span> <span data-ttu-id="60c45-255">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="60c45-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="60c45-256">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="60c45-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="60c45-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="60c45-258">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="60c45-259">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="60c45-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="60c45-260">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="60c45-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="60c45-261">Champs de fichier basée sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="60c45-261">Usage-based file fields</span></span>


<span data-ttu-id="60c45-262">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="60c45-263">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="60c45-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="60c45-264"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="60c45-265"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="60c45-266"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="60c45-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="60c45-268">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="60c45-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="60c45-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="60c45-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="60c45-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="60c45-271">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="60c45-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="60c45-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="60c45-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="60c45-274">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="60c45-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="60c45-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="60c45-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="60c45-277">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="60c45-278">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="60c45-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="60c45-279">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="60c45-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-280">MPNID</span></span></td>
<td><p><span data-ttu-id="60c45-281">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="60c45-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="60c45-282">4390934</span><span class="sxs-lookup"><span data-stu-id="60c45-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="60c45-284">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="60c45-285">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="60c45-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="60c45-286">4390934</span><span class="sxs-lookup"><span data-stu-id="60c45-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="60c45-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="60c45-288">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="60c45-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="60c45-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="60c45-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="60c45-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="60c45-291">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="60c45-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="60c45-292">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="60c45-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="60c45-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="60c45-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="60c45-295">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="60c45-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="60c45-296">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="60c45-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="60c45-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="60c45-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="60c45-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="60c45-299">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="60c45-300">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="60c45-301">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="60c45-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="60c45-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="60c45-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="60c45-304">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="60c45-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="60c45-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="60c45-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="60c45-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="60c45-307">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="60c45-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="60c45-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="60c45-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="60c45-309">OrderID</span></span></td>
<td><p><span data-ttu-id="60c45-310">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="60c45-311">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="60c45-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="60c45-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="60c45-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="60c45-314">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="60c45-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="60c45-315">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="60c45-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="60c45-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="60c45-317">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="60c45-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="60c45-318">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="60c45-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="60c45-319">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="60c45-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="60c45-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="60c45-321">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="60c45-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="60c45-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="60c45-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-323">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="60c45-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="60c45-324">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="60c45-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="60c45-325">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="60c45-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="60c45-326">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="60c45-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-327">Région</span><span class="sxs-lookup"><span data-stu-id="60c45-327">Region</span></span></td>
<td><p><span data-ttu-id="60c45-328">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="60c45-328">The region the usage applies to.</span></span> <span data-ttu-id="60c45-329">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="60c45-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="60c45-330">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="60c45-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-331">référence SKU</span><span class="sxs-lookup"><span data-stu-id="60c45-331">SKU</span></span></td>
<td><p><span data-ttu-id="60c45-332">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="60c45-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="60c45-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="60c45-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="60c45-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="60c45-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="60c45-335">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="60c45-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="60c45-336">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="60c45-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="60c45-337">1</span><span class="sxs-lookup"><span data-stu-id="60c45-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="60c45-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="60c45-339">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="60c45-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="60c45-340">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="60c45-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="60c45-341">11</span><span class="sxs-lookup"><span data-stu-id="60c45-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="60c45-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="60c45-343">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="60c45-343">Units included as part of the offer.</span></span> <span data-ttu-id="60c45-344">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="60c45-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="60c45-345">0</span><span class="sxs-lookup"><span data-stu-id="60c45-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="60c45-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="60c45-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="60c45-347">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="60c45-348">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="60c45-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="60c45-349">11</span><span class="sxs-lookup"><span data-stu-id="60c45-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="60c45-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="60c45-351">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="60c45-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="60c45-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="60c45-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="60c45-354">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="60c45-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="60c45-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="60c45-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="60c45-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="60c45-357">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="60c45-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="60c45-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="60c45-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="60c45-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="60c45-360">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="60c45-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="60c45-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="60c45-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-362">Currency</span><span class="sxs-lookup"><span data-stu-id="60c45-362">Currency</span></span></td>
<td><p><span data-ttu-id="60c45-363">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-363">Currency type.</span></span> <span data-ttu-id="60c45-364">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="60c45-365">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="60c45-366">EUR</span><span class="sxs-lookup"><span data-stu-id="60c45-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="60c45-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="60c45-368">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="60c45-368">Pretax price per unit.</span></span> <span data-ttu-id="60c45-369">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="60c45-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="60c45-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="60c45-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="60c45-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="60c45-372">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="60c45-372">Post tax price per unit.</span></span> <span data-ttu-id="60c45-373">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="60c45-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="60c45-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="60c45-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="60c45-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="60c45-376">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="60c45-376">The type of charge or adjustment.</span></span> <span data-ttu-id="60c45-377">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="60c45-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="60c45-378">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="60c45-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="60c45-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="60c45-380">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="60c45-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="60c45-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="60c45-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="60c45-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="60c45-383">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="60c45-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="60c45-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="60c45-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="60c45-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="60c45-386">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="60c45-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="60c45-387">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="60c45-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="60c45-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="60c45-389">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="60c45-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="60c45-390">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="60c45-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="60c45-391">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="60c45-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="60c45-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="60c45-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="60c45-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="60c45-394">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="60c45-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="60c45-395">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="60c45-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-396">Projet</span><span class="sxs-lookup"><span data-stu-id="60c45-396">Project</span></span></td>
<td><p><span data-ttu-id="60c45-397">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="60c45-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="60c45-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="60c45-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="60c45-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="60c45-400">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="60c45-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="60c45-401">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="60c45-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="60c45-402">Si vous aviez un pack de 25 connexions ServiceBus mis en service et vous aviez utilisé 1 pendant cette journée, votre relevé d’utilisation quotidienne pour ce jour indiquerait « 25 connexions / 30 jours – utilisé : 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="60c45-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="60c45-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="60c45-404">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="60c45-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="60c45-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="60c45-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="60c45-406">DomainName</span></span></td>
<td><p><span data-ttu-id="60c45-407">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="60c45-408">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="60c45-409">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="60c45-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="60c45-410">Unit</span><span class="sxs-lookup"><span data-stu-id="60c45-410">Unit</span></span></td>
<td><p><span data-ttu-id="60c45-411">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="60c45-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="60c45-412">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="60c45-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="60c45-413">Champs de fichier uniques et récurrentes</span><span class="sxs-lookup"><span data-stu-id="60c45-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="60c45-414">colonne</span><span class="sxs-lookup"><span data-stu-id="60c45-414">Column</span></span></th>
<th><span data-ttu-id="60c45-415">Description</span><span class="sxs-lookup"><span data-stu-id="60c45-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="60c45-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="60c45-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="60c45-417">Identificateur de locataire Microsoft Azure Active Directory unique pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="60c45-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="60c45-418">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="60c45-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="60c45-419">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="60c45-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-420">Id du client</span><span class="sxs-lookup"><span data-stu-id="60c45-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="60c45-421">Microsoft Azure Active Directory ID de locataire unique, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-422">Nom du client</span><span class="sxs-lookup"><span data-stu-id="60c45-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="60c45-423">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="60c45-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="60c45-425">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="60c45-426">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="60c45-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="60c45-427">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-428">Pays du client</span><span class="sxs-lookup"><span data-stu-id="60c45-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="60c45-429">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-430">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="60c45-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="60c45-431">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="60c45-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="60c45-432">MpnId</span></span></td>
<td><p><span data-ttu-id="60c45-433">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="60c45-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-434">MpnId du revendeur</span><span class="sxs-lookup"><span data-stu-id="60c45-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="60c45-435">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-436">ID de commande</span><span class="sxs-lookup"><span data-stu-id="60c45-436">Order ID</span></span></td>
<td><p><span data-ttu-id="60c45-437">Identificateur unique d’une commande dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="60c45-438">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-439">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="60c45-439">Order date</span></span></td>
<td><p><span data-ttu-id="60c45-440">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="60c45-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="60c45-441">ProductId</span></span></td>
<td><p><span data-ttu-id="60c45-442">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="60c45-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="60c45-443">SkuId</span></span></td>
<td><p><span data-ttu-id="60c45-444">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="60c45-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="60c45-446">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-446">The ID for a particular Availability.</span></span> <span data-ttu-id="60c45-447">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="60c45-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-448">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="60c45-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="60c45-449">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-450">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="60c45-450">Product name</span></span></td>
<td><p><span data-ttu-id="60c45-451">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="60c45-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="60c45-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="60c45-453">Nom du serveur de publication du produit.</span><span class="sxs-lookup"><span data-stu-id="60c45-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="60c45-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="60c45-455">ID unique pour ce serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="60c45-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-456">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="60c45-457">Nom convivial d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-458">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="60c45-459">Identificateur unique pour un abonnement dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="60c45-460">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="60c45-461">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="60c45-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="60c45-463">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-463">Start day of the charges.</span></span> <span data-ttu-id="60c45-464">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="60c45-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="60c45-466">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-466">End day of the charges.</span></span> <span data-ttu-id="60c45-467">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="60c45-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-468">Terme et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="60c45-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="60c45-469">La longueur de terme et d’un cycle de facturation pour l’achat.</span><span class="sxs-lookup"><span data-stu-id="60c45-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="60c45-470">Par exemple, « 1 an, tous les mois. »</span><span class="sxs-lookup"><span data-stu-id="60c45-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-471">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="60c45-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="60c45-472">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="60c45-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-473">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="60c45-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="60c45-474">Le prix publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="60c45-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="60c45-475">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-476">Prix unitaire efficace</span><span class="sxs-lookup"><span data-stu-id="60c45-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="60c45-477">Le prix unitaire après ont apporté des ajustements.</span><span class="sxs-lookup"><span data-stu-id="60c45-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-478">Quantité</span><span class="sxs-lookup"><span data-stu-id="60c45-478">Quantity</span></span></td>
<td><p><span data-ttu-id="60c45-479">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="60c45-479">Number of units.</span></span> <span data-ttu-id="60c45-480">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-481">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="60c45-481">Unit type</span></span></td>
<td><p><span data-ttu-id="60c45-482">Le type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="60c45-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="60c45-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="60c45-484">Explication sur les remises applicables.</span><span class="sxs-lookup"><span data-stu-id="60c45-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-485">Sous-total</span><span class="sxs-lookup"><span data-stu-id="60c45-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="60c45-486">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="60c45-486">Total before tax.</span></span> <span data-ttu-id="60c45-487">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="60c45-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-488">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="60c45-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="60c45-489">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="60c45-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-490">Total</span><span class="sxs-lookup"><span data-stu-id="60c45-490">Total</span></span></td>
<td><p><span data-ttu-id="60c45-491">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="60c45-491">Total after tax.</span></span> <span data-ttu-id="60c45-492">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="60c45-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-493">Currency</span><span class="sxs-lookup"><span data-stu-id="60c45-493">Currency</span></span></td>
<td><p><span data-ttu-id="60c45-494">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-494">Currency type.</span></span> <span data-ttu-id="60c45-495">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="60c45-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="60c45-496">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="60c45-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="60c45-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="60c45-498">Un autre identificateur pour un ID de commande.</span><span class="sxs-lookup"><span data-stu-id="60c45-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="60c45-499">Champs de fichier d’utilisation quotidienne-évalués</span><span class="sxs-lookup"><span data-stu-id="60c45-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="60c45-500">colonne</span><span class="sxs-lookup"><span data-stu-id="60c45-500">Column</span></span></th>
<th><span data-ttu-id="60c45-501">Description</span><span class="sxs-lookup"><span data-stu-id="60c45-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="60c45-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="60c45-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="60c45-503">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="60c45-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="60c45-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="60c45-505">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="60c45-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="60c45-507">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="60c45-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="60c45-509">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="60c45-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="60c45-510">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="60c45-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="60c45-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="60c45-512">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="60c45-512">The customer’s domain name.</span></span> <span data-ttu-id="60c45-513">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-514">Pays du client</span><span class="sxs-lookup"><span data-stu-id="60c45-514">Customer country</span></span></td>
<td><p><span data-ttu-id="60c45-515">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="60c45-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-516">MPNID</span></span></td>
<td><p><span data-ttu-id="60c45-517">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="60c45-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-518">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="60c45-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="60c45-519">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="60c45-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="60c45-520">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="60c45-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="60c45-522">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="60c45-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="60c45-523">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="60c45-524">ProductId</span></span></td>
<td><p><span data-ttu-id="60c45-525">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="60c45-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="60c45-526">SkuId</span></span></td>
<td><p><span data-ttu-id="60c45-527">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="60c45-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="60c45-529">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-529">The ID for a particular Availability.</span></span> <span data-ttu-id="60c45-530">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="60c45-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-531">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="60c45-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="60c45-532">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="60c45-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="60c45-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="60c45-534">Le nom du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="60c45-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="60c45-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="60c45-536">L’ID du serveur de publication, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="60c45-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="60c45-537">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="60c45-538">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="60c45-539">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="60c45-540">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="60c45-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-541">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="60c45-542">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="60c45-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="60c45-543">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="60c45-544">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="60c45-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="60c45-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="60c45-546">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="60c45-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="60c45-547">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="60c45-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="60c45-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="60c45-549">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="60c45-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="60c45-550">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="60c45-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-551">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="60c45-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="60c45-552">Date de l’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="60c45-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-553">Type de compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="60c45-554">Le type de compteur.</span><span class="sxs-lookup"><span data-stu-id="60c45-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-555">Catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="60c45-556">Le service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="60c45-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-557">Id de compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="60c45-558">L’ID du compteur utilisé.</span><span class="sxs-lookup"><span data-stu-id="60c45-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-559">Sous-catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="60c45-560">Le type de service Azure qui peut affecter le tarif.</span><span class="sxs-lookup"><span data-stu-id="60c45-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-561">Nom du compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="60c45-562">L’unité de mesure du compteur consommé.</span><span class="sxs-lookup"><span data-stu-id="60c45-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-563">Région du compteur</span><span class="sxs-lookup"><span data-stu-id="60c45-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="60c45-564">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="60c45-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-565">Unit</span><span class="sxs-lookup"><span data-stu-id="60c45-565">Unit</span></span></td>
<td><p><span data-ttu-id="60c45-566">L’unité de la ressource de nom.</span><span class="sxs-lookup"><span data-stu-id="60c45-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-567">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="60c45-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="60c45-568">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="60c45-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="60c45-569">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="60c45-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-570">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="60c45-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="60c45-571">Le centre de données où le compteur est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="60c45-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-572">Service consommé</span><span class="sxs-lookup"><span data-stu-id="60c45-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="60c45-573">Le service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="60c45-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="60c45-574">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="60c45-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="60c45-575">L’URI de la ressource qui est utilisée.</span><span class="sxs-lookup"><span data-stu-id="60c45-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-576">Type de frais</span><span class="sxs-lookup"><span data-stu-id="60c45-576">Charge type</span></span></td>
<td><p><span data-ttu-id="60c45-577">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="60c45-577">The type of charge or adjustment.</span></span> <span data-ttu-id="60c45-578">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-579">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="60c45-579">Unit price</span></span></td>
<td><p><span data-ttu-id="60c45-580">Prix par licence, telles que publiées dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="60c45-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="60c45-581">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-582">Quantité</span><span class="sxs-lookup"><span data-stu-id="60c45-582">Quantity</span></span></td>
<td><p><span data-ttu-id="60c45-583">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="60c45-583">Number of licenses.</span></span> <span data-ttu-id="60c45-584">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-585">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="60c45-585">Unit type</span></span></td>
<td><p><span data-ttu-id="60c45-586">Le type d’unité dans que le compteur est facturé.</span><span class="sxs-lookup"><span data-stu-id="60c45-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="60c45-587">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="60c45-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-588">Facturation avant impôts</span><span class="sxs-lookup"><span data-stu-id="60c45-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="60c45-589">Quantité totale avant impôts.</span><span class="sxs-lookup"><span data-stu-id="60c45-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-590">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="60c45-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="60c45-591">La devise dans la région géographique du client</span><span class="sxs-lookup"><span data-stu-id="60c45-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-592">Prix total avant impôt</span><span class="sxs-lookup"><span data-stu-id="60c45-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="60c45-593">La tarification avant les taxes sont ajoutées.</span><span class="sxs-lookup"><span data-stu-id="60c45-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-594">Tarification de devise</span><span class="sxs-lookup"><span data-stu-id="60c45-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="60c45-595">La devise dans la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="60c45-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="60c45-596">Informations sur le service 1</span><span class="sxs-lookup"><span data-stu-id="60c45-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="60c45-597">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="60c45-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-598">Informations sur le service 2</span><span class="sxs-lookup"><span data-stu-id="60c45-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="60c45-599">Champ hérité capturant les métadonnées facultatives propres au service.</span><span class="sxs-lookup"><span data-stu-id="60c45-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="60c45-600">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="60c45-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="60c45-601">Toute information supplémentaire non couverte dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="60c45-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="60c45-602">Frais de mappage entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="60c45-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="60c45-603">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="60c45-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="60c45-604">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="60c45-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="60c45-605">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="60c45-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="60c45-606">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’« ajustements » ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="60c45-607">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="60c45-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="60c45-608"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-609"><strong>Description des frais fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-610"><strong>Qu’est ce coût ?</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-611"><strong>Comment pour mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="60c45-612"><strong>Frais sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-613">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="60c45-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-614">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="60c45-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="60c45-615">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-616">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="60c45-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-617">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="60c45-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-618">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="60c45-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-619">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-620">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="60c45-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-621">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="60c45-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-622">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="60c45-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-623">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="60c45-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-624">Frais au prorata à l'achat</span><span class="sxs-lookup"><span data-stu-id="60c45-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-625">Le type de frais pour un abonnement lors de l’utilisation de facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="60c45-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-626">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-627">Le type de frais pour un abonnement lors de l’utilisation de la facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="60c45-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-628">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="60c45-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-629">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="60c45-630">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="60c45-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-631">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-632">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="60c45-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-633">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="60c45-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="60c45-634"><strong>Frais à usage unique</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="60c45-635">Nouveau</span><span class="sxs-lookup"><span data-stu-id="60c45-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-636">Utilisé lors de l’achat d’un nouveau est créé.</span><span class="sxs-lookup"><span data-stu-id="60c45-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="60c45-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-638">Utilisé dans les deux la restitution de l’achat d’origine et la quantité de nouveau après augmentation</span><span class="sxs-lookup"><span data-stu-id="60c45-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="60c45-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-640">Utilisé dans les deux la restitution de l’achat d’origine et la quantité de nouveau après réduction</span><span class="sxs-lookup"><span data-stu-id="60c45-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-641">Cancel</span><span class="sxs-lookup"><span data-stu-id="60c45-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-642">Utilisé quand un abonnement est annulé.</span><span class="sxs-lookup"><span data-stu-id="60c45-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-643">Convertir</span><span class="sxs-lookup"><span data-stu-id="60c45-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-644">Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé</span><span class="sxs-lookup"><span data-stu-id="60c45-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="60c45-645"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-646">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="60c45-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-647">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="60c45-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="60c45-648">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-649">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="60c45-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-650">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="60c45-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="60c45-651"><strong>Crédits</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-652">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="60c45-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-653">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="60c45-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-654">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="60c45-655">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="60c45-656"><strong>Basée sur l’utilisation des remises</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-657">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="60c45-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-658">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="60c45-659">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-660">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="60c45-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-661">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="60c45-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-662">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="60c45-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-663">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="60c45-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-664">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="60c45-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-665">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="60c45-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="60c45-666"><strong>Remises sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-667"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="60c45-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="60c45-668">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="60c45-669"><strong>Taxes</strong>  &nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-670"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="60c45-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="60c45-671"><em>Exception : &quot;Compense un élément de ligne&quot; inclut déjà des taxes. Consultez des crédits, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="60c45-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-672">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="60c45-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="60c45-673">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="60c45-674">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="60c45-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
