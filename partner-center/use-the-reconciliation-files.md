---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
description: Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8e7b17cb39f266c404d7873dc17e471741d52b32
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132779"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ca32e-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="ca32e-103">Use the reconciliation files</span></span>

<span data-ttu-id="ca32e-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="ca32e-104">**Applies to**</span></span>

-  <span data-ttu-id="ca32e-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ca32e-105">Partner Center</span></span>
-  <span data-ttu-id="ca32e-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ca32e-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ca32e-107">Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="ca32e-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="ca32e-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="ca32e-109">Problèmes de mise en forme</span><span class="sxs-lookup"><span data-stu-id="ca32e-109">Formatting issues</span></span>

<span data-ttu-id="ca32e-110">Il peut arriver que votre fichier de rapprochement peut-être des problèmes de mise en forme.</span><span class="sxs-lookup"><span data-stu-id="ca32e-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="ca32e-111">(Cela peut se produire, par exemple, si les paramètres régionaux EN-US ne sont pas utilisé.) Suivez les étapes ci-dessous pour résoudre ces problèmes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="ca32e-112">Ouvrez le fichier .csv dans Excel, puis sélectionnez la première colonne.</span><span class="sxs-lookup"><span data-stu-id="ca32e-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="ca32e-113">Dans le ruban, sélectionnez <strong>données</strong>, puis sélectionnez <strong>texte aux colonnes</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="ca32e-114">Dans le texte de conversion Assistant, sélectionnez <strong>délimités de type de fichier</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ca32e-115">Dans le champ de séparateurs, sélectionnez <strong>virgules</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="ca32e-116">Si <strong>onglet</strong> est déjà sélectionné, vous pouvez la laisser.</span><span class="sxs-lookup"><span data-stu-id="ca32e-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="ca32e-117">Sélectionnez <strong>Suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="ca32e-118">Dans le champ de format de données de colonne, sélectionnez <strong>Date : MDY</strong>, puis sélectionnez <strong>suivant</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ca32e-119">Dans le champ de format de données de colonne, sélectionnez <strong>texte</strong> pour tout montant de colonnes, puis sélectionnez <strong>Terminer</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="ca32e-120">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-120">Itemize by partner</span></span>


<span data-ttu-id="ca32e-121">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licence pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="ca32e-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ca32e-122">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="ca32e-122">MPN ID</span></span></th>
<th><span data-ttu-id="ca32e-123">Description</span><span class="sxs-lookup"><span data-stu-id="ca32e-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ca32e-124">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="ca32e-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="ca32e-125">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="ca32e-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-126">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="ca32e-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ca32e-127">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="ca32e-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ca32e-128">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ca32e-129">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ca32e-130">vue d’eTo ou de mise à jour le revendeur, dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="ca32e-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ca32e-131">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="ca32e-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ca32e-132">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ca32e-133">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="ca32e-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ca32e-134">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="ca32e-135">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="ca32e-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="ca32e-136">Champs d’un fichier basé sur licence</span><span class="sxs-lookup"><span data-stu-id="ca32e-136">License-based file fields</span></span>


<span data-ttu-id="ca32e-137">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ca32e-138"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ca32e-139"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ca32e-140"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ca32e-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="ca32e-142">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="ca32e-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ca32e-143">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="ca32e-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ca32e-144">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ca32e-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ca32e-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ca32e-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="ca32e-147">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ca32e-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ca32e-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="ca32e-149">OrderID</span></span></td>
<td><p><span data-ttu-id="ca32e-150">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ca32e-151">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ca32e-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ca32e-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ca32e-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ca32e-154">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ca32e-155">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ca32e-156">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ca32e-157">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="ca32e-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ca32e-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ca32e-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-159">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="ca32e-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ca32e-160">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="ca32e-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ca32e-161">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ca32e-162">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ca32e-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ca32e-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="ca32e-164">OfferID</span></span></td>
<td><p><span data-ttu-id="ca32e-165">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-165">Unique offer ID.</span></span> <span data-ttu-id="ca32e-166">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ca32e-167"><b>Remarque</b>: Cette valeur ne correspond pas d’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ca32e-168">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="ca32e-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ca32e-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ca32e-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ca32e-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ca32e-171">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ca32e-172"><b>Remarque</b>: Cette valeur correspond à l’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ca32e-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ca32e-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="ca32e-174">OfferName</span></span></td>
<td><p><span data-ttu-id="ca32e-175">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ca32e-176">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="ca32e-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ca32e-178">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="ca32e-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ca32e-179">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="ca32e-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ca32e-180">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ca32e-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ca32e-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ca32e-183">La date de fin d’abonnement : 12 mois + x jours après la date de début (pour les aligner avec date de facturation du partenaire) ou 12 mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ca32e-184">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="ca32e-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ca32e-185">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ca32e-186">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ca32e-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ca32e-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ca32e-189">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ca32e-190">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="ca32e-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ca32e-191">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ca32e-192">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ca32e-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ca32e-194">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="ca32e-195">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="ca32e-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ca32e-196">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ca32e-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ca32e-197">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ca32e-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ca32e-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="ca32e-199">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-199">The type of charge or adjustment.</span></span> <span data-ttu-id="ca32e-200">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="ca32e-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ca32e-201">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="ca32e-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ca32e-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ca32e-203">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="ca32e-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ca32e-204">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ca32e-205">6.82</span><span class="sxs-lookup"><span data-stu-id="ca32e-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-206">Quantité</span><span class="sxs-lookup"><span data-stu-id="ca32e-206">Quantity</span></span></td>
<td><p><span data-ttu-id="ca32e-207">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="ca32e-207">Number of seats.</span></span> <span data-ttu-id="ca32e-208">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ca32e-209">2</span><span class="sxs-lookup"><span data-stu-id="ca32e-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-210">Montant</span><span class="sxs-lookup"><span data-stu-id="ca32e-210">Amount</span></span></td>
<td><p><span data-ttu-id="ca32e-211">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="ca32e-211">Total of price for quantity.</span></span> <span data-ttu-id="ca32e-212">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="ca32e-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ca32e-213">13.32</span><span class="sxs-lookup"><span data-stu-id="ca32e-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ca32e-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ca32e-215">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ca32e-216">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="ca32e-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ca32e-217">2.32</span><span class="sxs-lookup"><span data-stu-id="ca32e-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-218">Sous-total</span><span class="sxs-lookup"><span data-stu-id="ca32e-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="ca32e-219">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="ca32e-219">Total before tax.</span></span> <span data-ttu-id="ca32e-220">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ca32e-221">11</span><span class="sxs-lookup"><span data-stu-id="ca32e-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-222">Taxe</span><span class="sxs-lookup"><span data-stu-id="ca32e-222">Tax</span></span></td>
<td><p><span data-ttu-id="ca32e-223">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="ca32e-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ca32e-224">0</span><span class="sxs-lookup"><span data-stu-id="ca32e-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ca32e-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ca32e-226">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="ca32e-226">Total after tax.</span></span> <span data-ttu-id="ca32e-227">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="ca32e-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ca32e-228">11</span><span class="sxs-lookup"><span data-stu-id="ca32e-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-229">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-229">Currency</span></span></td>
<td><p><span data-ttu-id="ca32e-230">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-230">Currency type.</span></span> <span data-ttu-id="ca32e-231">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="ca32e-232">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ca32e-233">EUR</span><span class="sxs-lookup"><span data-stu-id="ca32e-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ca32e-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="ca32e-235">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ca32e-236">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="ca32e-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ca32e-237">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="ca32e-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-238">MPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-239">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="ca32e-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ca32e-240">4390934</span><span class="sxs-lookup"><span data-stu-id="ca32e-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-242">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ca32e-243">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ca32e-244">4390934</span><span class="sxs-lookup"><span data-stu-id="ca32e-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="ca32e-245">DomainName</span></span></td>
<td><p><span data-ttu-id="ca32e-246">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ca32e-247">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="ca32e-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ca32e-248">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ca32e-249">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ca32e-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ca32e-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ca32e-251">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-251">Subscription nickname.</span></span> <span data-ttu-id="ca32e-252">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="ca32e-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ca32e-253">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="ca32e-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ca32e-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ca32e-255">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ca32e-256">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="ca32e-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ca32e-257">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="ca32e-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="ca32e-258">Champs de fichier basée sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="ca32e-258">Usage-based file fields</span></span>


<span data-ttu-id="ca32e-259">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ca32e-260">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="ca32e-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ca32e-261"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ca32e-262"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ca32e-263"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ca32e-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="ca32e-265">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="ca32e-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ca32e-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ca32e-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ca32e-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="ca32e-268">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ca32e-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ca32e-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ca32e-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ca32e-271">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ca32e-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="ca32e-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ca32e-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="ca32e-274">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ca32e-275">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="ca32e-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ca32e-276">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="ca32e-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-277">MPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-278">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="ca32e-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ca32e-279">4390934</span><span class="sxs-lookup"><span data-stu-id="ca32e-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-281">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ca32e-282">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="ca32e-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ca32e-283">4390934</span><span class="sxs-lookup"><span data-stu-id="ca32e-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ca32e-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ca32e-285">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="ca32e-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ca32e-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ca32e-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ca32e-288">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="ca32e-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ca32e-289">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ca32e-290">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ca32e-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ca32e-292">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="ca32e-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ca32e-293">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ca32e-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ca32e-294">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ca32e-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ca32e-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ca32e-296">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ca32e-297">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ca32e-298">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ca32e-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ca32e-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ca32e-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ca32e-301">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="ca32e-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ca32e-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ca32e-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ca32e-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ca32e-304">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="ca32e-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ca32e-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ca32e-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="ca32e-306">OrderID</span></span></td>
<td><p><span data-ttu-id="ca32e-307">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ca32e-308">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ca32e-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ca32e-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ca32e-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="ca32e-311">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="ca32e-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ca32e-312">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="ca32e-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ca32e-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="ca32e-314">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="ca32e-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ca32e-315">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="ca32e-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="ca32e-316">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="ca32e-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ca32e-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ca32e-318">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="ca32e-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ca32e-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ca32e-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-320">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="ca32e-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="ca32e-321">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="ca32e-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ca32e-322">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="ca32e-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ca32e-323">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="ca32e-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-324">Région</span><span class="sxs-lookup"><span data-stu-id="ca32e-324">Region</span></span></td>
<td><p><span data-ttu-id="ca32e-325">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-325">The region the usage applies to.</span></span> <span data-ttu-id="ca32e-326">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="ca32e-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ca32e-327">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="ca32e-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-328">référence SKU</span><span class="sxs-lookup"><span data-stu-id="ca32e-328">SKU</span></span></td>
<td><p><span data-ttu-id="ca32e-329">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="ca32e-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ca32e-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ca32e-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ca32e-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ca32e-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ca32e-332">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="ca32e-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ca32e-333">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="ca32e-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ca32e-334">1</span><span class="sxs-lookup"><span data-stu-id="ca32e-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ca32e-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ca32e-336">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="ca32e-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ca32e-337">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ca32e-338">11</span><span class="sxs-lookup"><span data-stu-id="ca32e-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ca32e-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ca32e-340">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="ca32e-340">Units included as part of the offer.</span></span> <span data-ttu-id="ca32e-341">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="ca32e-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ca32e-342">0</span><span class="sxs-lookup"><span data-stu-id="ca32e-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ca32e-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ca32e-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ca32e-344">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ca32e-345">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="ca32e-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ca32e-346">11</span><span class="sxs-lookup"><span data-stu-id="ca32e-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ca32e-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="ca32e-348">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ca32e-349">$0.0808</span><span class="sxs-lookup"><span data-stu-id="ca32e-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ca32e-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ca32e-351">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="ca32e-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ca32e-352">$0.085</span><span class="sxs-lookup"><span data-stu-id="ca32e-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ca32e-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ca32e-354">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="ca32e-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ca32e-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="ca32e-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ca32e-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ca32e-357">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="ca32e-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ca32e-358">$0.93</span><span class="sxs-lookup"><span data-stu-id="ca32e-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-359">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-359">Currency</span></span></td>
<td><p><span data-ttu-id="ca32e-360">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-360">Currency type.</span></span> <span data-ttu-id="ca32e-361">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="ca32e-362">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ca32e-363">EUR</span><span class="sxs-lookup"><span data-stu-id="ca32e-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ca32e-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ca32e-365">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="ca32e-365">Pretax price per unit.</span></span> <span data-ttu-id="ca32e-366">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="ca32e-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ca32e-367">$0.08</span><span class="sxs-lookup"><span data-stu-id="ca32e-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ca32e-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ca32e-369">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="ca32e-369">Post tax price per unit.</span></span> <span data-ttu-id="ca32e-370">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="ca32e-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ca32e-371">$0.08</span><span class="sxs-lookup"><span data-stu-id="ca32e-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ca32e-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="ca32e-373">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-373">The type of charge or adjustment.</span></span> <span data-ttu-id="ca32e-374">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="ca32e-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ca32e-375">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="ca32e-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ca32e-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ca32e-377">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="ca32e-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ca32e-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="ca32e-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="ca32e-380">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="ca32e-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ca32e-381">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ca32e-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ca32e-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ca32e-383">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="ca32e-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ca32e-384">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="ca32e-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="ca32e-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="ca32e-386">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="ca32e-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ca32e-387">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="ca32e-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ca32e-388">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="ca32e-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ca32e-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="ca32e-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ca32e-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ca32e-391">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="ca32e-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ca32e-392">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="ca32e-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-393">Projet</span><span class="sxs-lookup"><span data-stu-id="ca32e-393">Project</span></span></td>
<td><p><span data-ttu-id="ca32e-394">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="ca32e-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ca32e-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ca32e-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ca32e-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ca32e-397">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="ca32e-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ca32e-398">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="ca32e-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="ca32e-399">Si vous aviez un pack de 25 connexions ServiceBus mis en service et vous aviez utilisé 1 pendant cette journée, votre relevé d’utilisation quotidienne pour ce jour indiquerait « 25 connexions / 30 jours – utilisé : 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="ca32e-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ca32e-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="ca32e-401">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ca32e-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ca32e-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ca32e-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="ca32e-403">DomainName</span></span></td>
<td><p><span data-ttu-id="ca32e-404">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ca32e-405">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ca32e-406">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ca32e-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ca32e-407">Unit</span><span class="sxs-lookup"><span data-stu-id="ca32e-407">Unit</span></span></td>
<td><p><span data-ttu-id="ca32e-408">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="ca32e-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ca32e-409">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="ca32e-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="ca32e-410">Champs de fichier uniques et récurrentes</span><span class="sxs-lookup"><span data-stu-id="ca32e-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ca32e-411">colonne</span><span class="sxs-lookup"><span data-stu-id="ca32e-411">Column</span></span></th>
<th><span data-ttu-id="ca32e-412">Description</span><span class="sxs-lookup"><span data-stu-id="ca32e-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="ca32e-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ca32e-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="ca32e-414">Identificateur de locataire Microsoft Azure Active Directory unique pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="ca32e-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ca32e-415">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="ca32e-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ca32e-416">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-417">Id du client</span><span class="sxs-lookup"><span data-stu-id="ca32e-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="ca32e-418">Microsoft Azure Active Directory ID de locataire unique, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-419">Nom du client</span><span class="sxs-lookup"><span data-stu-id="ca32e-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="ca32e-420">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ca32e-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ca32e-422">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ca32e-423">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="ca32e-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ca32e-424">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-425">Pays du client</span><span class="sxs-lookup"><span data-stu-id="ca32e-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="ca32e-426">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-427">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="ca32e-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="ca32e-428">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="ca32e-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="ca32e-429">MpnId</span></span></td>
<td><p><span data-ttu-id="ca32e-430">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="ca32e-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-431">MpnId du revendeur</span><span class="sxs-lookup"><span data-stu-id="ca32e-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="ca32e-432">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-433">ID de commande</span><span class="sxs-lookup"><span data-stu-id="ca32e-433">Order ID</span></span></td>
<td><p><span data-ttu-id="ca32e-434">Identificateur unique d’une commande dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="ca32e-435">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-436">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="ca32e-436">Order date</span></span></td>
<td><p><span data-ttu-id="ca32e-437">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="ca32e-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="ca32e-438">ProductId</span></span></td>
<td><p><span data-ttu-id="ca32e-439">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="ca32e-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="ca32e-440">SkuId</span></span></td>
<td><p><span data-ttu-id="ca32e-441">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ca32e-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ca32e-443">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-443">The ID for a particular Availability.</span></span> <span data-ttu-id="ca32e-444">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="ca32e-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-445">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="ca32e-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="ca32e-446">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-447">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="ca32e-447">Product name</span></span></td>
<td><p><span data-ttu-id="ca32e-448">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="ca32e-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ca32e-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="ca32e-450">Nom du serveur de publication du produit.</span><span class="sxs-lookup"><span data-stu-id="ca32e-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ca32e-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="ca32e-452">ID unique pour ce serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="ca32e-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-453">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ca32e-454">Nom convivial d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-455">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ca32e-456">Identificateur unique pour un abonnement dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="ca32e-457">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ca32e-458">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ca32e-460">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-460">Start day of the charges.</span></span> <span data-ttu-id="ca32e-461">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ca32e-463">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-463">End day of the charges.</span></span> <span data-ttu-id="ca32e-464">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ca32e-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-465">Terme et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="ca32e-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="ca32e-466">La longueur de terme et d’un cycle de facturation pour l’achat.</span><span class="sxs-lookup"><span data-stu-id="ca32e-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="ca32e-467">Par exemple, « 1 an, tous les mois. »</span><span class="sxs-lookup"><span data-stu-id="ca32e-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-468">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="ca32e-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="ca32e-469">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-470">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="ca32e-471">Le prix publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="ca32e-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ca32e-472">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-473">Prix unitaire efficace</span><span class="sxs-lookup"><span data-stu-id="ca32e-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="ca32e-474">Le prix unitaire après ont apporté des ajustements.</span><span class="sxs-lookup"><span data-stu-id="ca32e-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-475">Quantité</span><span class="sxs-lookup"><span data-stu-id="ca32e-475">Quantity</span></span></td>
<td><p><span data-ttu-id="ca32e-476">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="ca32e-476">Number of units.</span></span> <span data-ttu-id="ca32e-477">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-478">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="ca32e-478">Unit type</span></span></td>
<td><p><span data-ttu-id="ca32e-479">Le type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="ca32e-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="ca32e-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="ca32e-481">Explication sur les remises applicables.</span><span class="sxs-lookup"><span data-stu-id="ca32e-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-482">Sous-total</span><span class="sxs-lookup"><span data-stu-id="ca32e-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="ca32e-483">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="ca32e-483">Total before tax.</span></span> <span data-ttu-id="ca32e-484">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-485">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="ca32e-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="ca32e-486">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="ca32e-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-487">Total</span><span class="sxs-lookup"><span data-stu-id="ca32e-487">Total</span></span></td>
<td><p><span data-ttu-id="ca32e-488">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="ca32e-488">Total after tax.</span></span> <span data-ttu-id="ca32e-489">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="ca32e-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-490">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-490">Currency</span></span></td>
<td><p><span data-ttu-id="ca32e-491">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-491">Currency type.</span></span> <span data-ttu-id="ca32e-492">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="ca32e-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="ca32e-493">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="ca32e-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="ca32e-495">Un autre identificateur pour un ID de commande.</span><span class="sxs-lookup"><span data-stu-id="ca32e-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="ca32e-496">Champs de fichier d’utilisation quotidienne-évalués</span><span class="sxs-lookup"><span data-stu-id="ca32e-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ca32e-497">colonne</span><span class="sxs-lookup"><span data-stu-id="ca32e-497">Column</span></span></th>
<th><span data-ttu-id="ca32e-498">Description</span><span class="sxs-lookup"><span data-stu-id="ca32e-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="ca32e-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ca32e-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="ca32e-500">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="ca32e-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ca32e-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="ca32e-502">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="ca32e-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="ca32e-504">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="ca32e-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="ca32e-506">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ca32e-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ca32e-507">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="ca32e-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ca32e-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ca32e-509">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-509">The customer’s domain name.</span></span> <span data-ttu-id="ca32e-510">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-511">Pays du client</span><span class="sxs-lookup"><span data-stu-id="ca32e-511">Customer country</span></span></td>
<td><p><span data-ttu-id="ca32e-512">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="ca32e-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-513">MPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-514">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="ca32e-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-515">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="ca32e-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="ca32e-516">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ca32e-517">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ca32e-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ca32e-519">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="ca32e-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="ca32e-520">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="ca32e-521">ProductId</span></span></td>
<td><p><span data-ttu-id="ca32e-522">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="ca32e-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="ca32e-523">SkuId</span></span></td>
<td><p><span data-ttu-id="ca32e-524">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ca32e-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ca32e-526">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-526">The ID for a particular Availability.</span></span> <span data-ttu-id="ca32e-527">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="ca32e-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-528">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="ca32e-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="ca32e-529">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="ca32e-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ca32e-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="ca32e-531">Le nom du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="ca32e-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ca32e-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="ca32e-533">L’ID du serveur de publication, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="ca32e-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="ca32e-534">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="ca32e-535">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ca32e-536">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ca32e-537">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="ca32e-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-538">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ca32e-539">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ca32e-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ca32e-540">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ca32e-541">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="ca32e-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ca32e-543">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="ca32e-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ca32e-544">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="ca32e-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ca32e-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ca32e-546">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="ca32e-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ca32e-547">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="ca32e-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-548">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="ca32e-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="ca32e-549">Date de l’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="ca32e-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-550">Type de compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="ca32e-551">Le type de compteur.</span><span class="sxs-lookup"><span data-stu-id="ca32e-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-552">Catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="ca32e-553">Le service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-554">Id de compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="ca32e-555">L’ID du compteur utilisé.</span><span class="sxs-lookup"><span data-stu-id="ca32e-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-556">Sous-catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="ca32e-557">Le type de service Azure qui peut affecter le tarif.</span><span class="sxs-lookup"><span data-stu-id="ca32e-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-558">Nom du compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="ca32e-559">L’unité de mesure du compteur consommé.</span><span class="sxs-lookup"><span data-stu-id="ca32e-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-560">Région du compteur</span><span class="sxs-lookup"><span data-stu-id="ca32e-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="ca32e-561">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="ca32e-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-562">Unit</span><span class="sxs-lookup"><span data-stu-id="ca32e-562">Unit</span></span></td>
<td><p><span data-ttu-id="ca32e-563">L’unité de la ressource de nom.</span><span class="sxs-lookup"><span data-stu-id="ca32e-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-564">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="ca32e-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="ca32e-565">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="ca32e-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="ca32e-566">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-567">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="ca32e-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="ca32e-568">Le centre de données où le compteur est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="ca32e-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-569">Service consommé</span><span class="sxs-lookup"><span data-stu-id="ca32e-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="ca32e-570">Le service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="ca32e-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-571">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="ca32e-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="ca32e-572">Le groupe de ressources dans lequel le compteur déployé s’exécute.</span><span class="sxs-lookup"><span data-stu-id="ca32e-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-573">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="ca32e-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="ca32e-574">L’URI de la ressource qui est utilisée.</span><span class="sxs-lookup"><span data-stu-id="ca32e-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-575">Type de frais</span><span class="sxs-lookup"><span data-stu-id="ca32e-575">Charge type</span></span></td>
<td><p><span data-ttu-id="ca32e-576">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-576">The type of charge or adjustment.</span></span> <span data-ttu-id="ca32e-577">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-578">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="ca32e-578">Unit price</span></span></td>
<td><p><span data-ttu-id="ca32e-579">Prix par licence, telles que publiées dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="ca32e-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ca32e-580">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-581">Quantité</span><span class="sxs-lookup"><span data-stu-id="ca32e-581">Quantity</span></span></td>
<td><p><span data-ttu-id="ca32e-582">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="ca32e-582">Number of licenses.</span></span> <span data-ttu-id="ca32e-583">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-584">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="ca32e-584">Unit type</span></span></td>
<td><p><span data-ttu-id="ca32e-585">Le type d’unité dans que le compteur est facturé.</span><span class="sxs-lookup"><span data-stu-id="ca32e-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="ca32e-586">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="ca32e-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-587">Facturation avant impôts</span><span class="sxs-lookup"><span data-stu-id="ca32e-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="ca32e-588">Quantité totale avant impôts.</span><span class="sxs-lookup"><span data-stu-id="ca32e-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-589">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="ca32e-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="ca32e-590">La devise dans la région géographique du client</span><span class="sxs-lookup"><span data-stu-id="ca32e-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-591">Prix total avant impôt</span><span class="sxs-lookup"><span data-stu-id="ca32e-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="ca32e-592">La tarification avant les taxes sont ajoutées.</span><span class="sxs-lookup"><span data-stu-id="ca32e-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-593">Tarification de devise</span><span class="sxs-lookup"><span data-stu-id="ca32e-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="ca32e-594">La devise dans la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="ca32e-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-595">Informations sur le service 1</span><span class="sxs-lookup"><span data-stu-id="ca32e-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="ca32e-596">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="ca32e-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-597">Informations sur le service 2</span><span class="sxs-lookup"><span data-stu-id="ca32e-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="ca32e-598">Champ hérité capturant les métadonnées facultatives propres au service.</span><span class="sxs-lookup"><span data-stu-id="ca32e-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ca32e-599">Balises</span><span class="sxs-lookup"><span data-stu-id="ca32e-599">Tags</span></span></td>
<td><p><span data-ttu-id="ca32e-600">Balises que vous affectez au compteur dans l’ordre pour regrouper les enregistrements de facturation.</span><span class="sxs-lookup"><span data-stu-id="ca32e-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="ca32e-601">Par exemple, vous pouvez utiliser des balises pour répartir les coûts par département qui utilise le compteur.</span><span class="sxs-lookup"><span data-stu-id="ca32e-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ca32e-602">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="ca32e-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="ca32e-603">Toute information supplémentaire non couverte dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="ca32e-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="ca32e-604">Frais de mappage entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="ca32e-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ca32e-605">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="ca32e-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ca32e-606">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="ca32e-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ca32e-607">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="ca32e-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="ca32e-608">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’« ajustements » ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="ca32e-609">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="ca32e-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="ca32e-610"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-611"><strong>Description des frais fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-612"><strong>Qu’est ce coût ?</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-613"><strong>Comment pour mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="ca32e-614"><strong>Frais sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-615">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="ca32e-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-616">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="ca32e-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="ca32e-617">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-618">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="ca32e-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-619">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="ca32e-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-620">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="ca32e-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-621">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-622">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="ca32e-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-623">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="ca32e-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-624">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="ca32e-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-625">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="ca32e-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-626">Frais au prorata à l'achat</span><span class="sxs-lookup"><span data-stu-id="ca32e-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-627">Le type de frais pour un abonnement lors de l’utilisation de facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="ca32e-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-628">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-629">Le type de frais pour un abonnement lors de l’utilisation de la facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="ca32e-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-630">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="ca32e-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-631">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="ca32e-632">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="ca32e-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-633">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-634">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="ca32e-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-635">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="ca32e-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="ca32e-636"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-637">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="ca32e-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-638">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="ca32e-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ca32e-639">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-640">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="ca32e-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-641">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="ca32e-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-642"><strong>Crédits</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-643">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="ca32e-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-644">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="ca32e-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-645">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ca32e-646">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="ca32e-647"><strong>Basée sur l’utilisation des remises</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-648">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="ca32e-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-649">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="ca32e-650">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-651">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="ca32e-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-652">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="ca32e-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-653">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="ca32e-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-654">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="ca32e-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-655">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="ca32e-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-656">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="ca32e-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="ca32e-657"><strong>Remises sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-658"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="ca32e-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="ca32e-659">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ca32e-660"><strong>Taxes</strong>  &nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-661"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="ca32e-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="ca32e-662"><em>Exception : &quot;Compense un élément de ligne&quot; inclut déjà des taxes. Consultez des crédits, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="ca32e-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-663">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="ca32e-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ca32e-664">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ca32e-665">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="ca32e-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
