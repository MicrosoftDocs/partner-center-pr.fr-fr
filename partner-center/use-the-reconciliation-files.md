---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 9997b01c76dacb736baa33f458def0b820753f1d
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682507"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="2c63c-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="2c63c-103">Use the reconciliation files</span></span>

<span data-ttu-id="2c63c-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="2c63c-104">**Applies to**</span></span>

-  <span data-ttu-id="2c63c-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="2c63c-105">Partner Center</span></span>
-  <span data-ttu-id="2c63c-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="2c63c-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="2c63c-107">Pour une vue détaillée de la ligne de chaque charge dans un cycle de facturation, téléchargez les fichiers de réconciliation de partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="2c63c-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="2c63c-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="2c63c-109">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-109">Itemize by partner</span></span>


<span data-ttu-id="2c63c-110">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licence pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="2c63c-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2c63c-111">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="2c63c-111">MPN ID</span></span></th>
<th><span data-ttu-id="2c63c-112">Description</span><span class="sxs-lookup"><span data-stu-id="2c63c-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2c63c-113">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="2c63c-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="2c63c-114">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="2c63c-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-115">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="2c63c-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="2c63c-116">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="2c63c-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="2c63c-117">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2c63c-118">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="2c63c-119">vue d’eTo ou de mise à jour le revendeur, dans le menu espace partenaires, sélectionnez <strong>clients</strong>, puis sélectionnez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="2c63c-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="2c63c-120">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="2c63c-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="2c63c-121">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="2c63c-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="2c63c-122">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="2c63c-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="2c63c-123">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="2c63c-124">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="2c63c-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="2c63c-125">Champs d’un fichier basé sur licence</span><span class="sxs-lookup"><span data-stu-id="2c63c-125">License-based file fields</span></span>


<span data-ttu-id="2c63c-126">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2c63c-127"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="2c63c-128"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="2c63c-129"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2c63c-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="2c63c-131">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="2c63c-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="2c63c-132">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="2c63c-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="2c63c-133">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="2c63c-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="2c63c-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="2c63c-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2c63c-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="2c63c-136">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2c63c-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="2c63c-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="2c63c-138">OrderID</span></span></td>
<td><p><span data-ttu-id="2c63c-139">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2c63c-140">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2c63c-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2c63c-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2c63c-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2c63c-143">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2c63c-144">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2c63c-145">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="2c63c-146">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="2c63c-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="2c63c-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2c63c-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-148">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="2c63c-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="2c63c-149">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="2c63c-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="2c63c-150">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="2c63c-151">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2c63c-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="2c63c-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="2c63c-153">OfferID</span></span></td>
<td><p><span data-ttu-id="2c63c-154">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-154">Unique offer ID.</span></span> <span data-ttu-id="2c63c-155">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="2c63c-156"><b>Remarque</b>: Cette valeur ne correspond pas d’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="2c63c-157">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="2c63c-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="2c63c-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="2c63c-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="2c63c-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="2c63c-160">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="2c63c-161"><b>Remarque</b>: Cette valeur correspond à l’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="2c63c-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="2c63c-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="2c63c-163">OfferName</span></span></td>
<td><p><span data-ttu-id="2c63c-164">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="2c63c-165">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="2c63c-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="2c63c-167">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="2c63c-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="2c63c-168">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="2c63c-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="2c63c-169">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2c63c-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2c63c-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="2c63c-172">La date de fin d’abonnement : 12 mois + x jours après la date de début (pour les aligner avec date de facturation du partenaire) ou 12 mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="2c63c-173">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="2c63c-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="2c63c-174">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="2c63c-175">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2c63c-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2c63c-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2c63c-178">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="2c63c-179">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="2c63c-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2c63c-180">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2c63c-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2c63c-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2c63c-183">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="2c63c-184">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="2c63c-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2c63c-185">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="2c63c-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2c63c-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="2c63c-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2c63c-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="2c63c-188">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-188">The type of charge or adjustment.</span></span> <span data-ttu-id="2c63c-189">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="2c63c-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2c63c-190">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="2c63c-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="2c63c-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="2c63c-192">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="2c63c-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2c63c-193">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2c63c-194">6.82</span><span class="sxs-lookup"><span data-stu-id="2c63c-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-195">Quantité</span><span class="sxs-lookup"><span data-stu-id="2c63c-195">Quantity</span></span></td>
<td><p><span data-ttu-id="2c63c-196">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="2c63c-196">Number of seats.</span></span> <span data-ttu-id="2c63c-197">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2c63c-198">2</span><span class="sxs-lookup"><span data-stu-id="2c63c-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-199">Montant</span><span class="sxs-lookup"><span data-stu-id="2c63c-199">Amount</span></span></td>
<td><p><span data-ttu-id="2c63c-200">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="2c63c-200">Total of price for quantity.</span></span> <span data-ttu-id="2c63c-201">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="2c63c-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="2c63c-202">13.32</span><span class="sxs-lookup"><span data-stu-id="2c63c-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="2c63c-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="2c63c-204">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="2c63c-205">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="2c63c-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="2c63c-206">2.32</span><span class="sxs-lookup"><span data-stu-id="2c63c-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-207">Sous-total</span><span class="sxs-lookup"><span data-stu-id="2c63c-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="2c63c-208">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="2c63c-208">Total before tax.</span></span> <span data-ttu-id="2c63c-209">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="2c63c-210">11</span><span class="sxs-lookup"><span data-stu-id="2c63c-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-211">Taxe</span><span class="sxs-lookup"><span data-stu-id="2c63c-211">Tax</span></span></td>
<td><p><span data-ttu-id="2c63c-212">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="2c63c-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2c63c-213">0</span><span class="sxs-lookup"><span data-stu-id="2c63c-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="2c63c-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="2c63c-215">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="2c63c-215">Total after tax.</span></span> <span data-ttu-id="2c63c-216">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="2c63c-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="2c63c-217">11</span><span class="sxs-lookup"><span data-stu-id="2c63c-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-218">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-218">Currency</span></span></td>
<td><p><span data-ttu-id="2c63c-219">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-219">Currency type.</span></span> <span data-ttu-id="2c63c-220">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="2c63c-221">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2c63c-222">EUR</span><span class="sxs-lookup"><span data-stu-id="2c63c-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2c63c-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="2c63c-224">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="2c63c-225">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="2c63c-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2c63c-226">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="2c63c-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-227">MPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-228">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="2c63c-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="2c63c-229">4390934</span><span class="sxs-lookup"><span data-stu-id="2c63c-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-231">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2c63c-232">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="2c63c-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="2c63c-233">4390934</span><span class="sxs-lookup"><span data-stu-id="2c63c-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="2c63c-234">DomainName</span></span></td>
<td><p><span data-ttu-id="2c63c-235">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="2c63c-236">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c63c-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="2c63c-237">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="2c63c-238">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2c63c-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2c63c-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2c63c-240">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-240">Subscription nickname.</span></span> <span data-ttu-id="2c63c-241">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="2c63c-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="2c63c-242">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="2c63c-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2c63c-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2c63c-244">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="2c63c-245">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="2c63c-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="2c63c-246">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="2c63c-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="2c63c-247">Champs de fichier basée sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="2c63c-247">Usage-based file fields</span></span>


<span data-ttu-id="2c63c-248">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="2c63c-249">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="2c63c-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2c63c-250"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="2c63c-251"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="2c63c-252"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="2c63c-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="2c63c-254">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="2c63c-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="2c63c-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2c63c-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="2c63c-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="2c63c-257">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="2c63c-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="2c63c-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="2c63c-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="2c63c-260">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="2c63c-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="2c63c-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2c63c-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="2c63c-263">Client&#39;nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="2c63c-264">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="2c63c-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2c63c-265">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="2c63c-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-266">MPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-267">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="2c63c-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="2c63c-268">4390934</span><span class="sxs-lookup"><span data-stu-id="2c63c-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-270">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2c63c-271">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="2c63c-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="2c63c-272">4390934</span><span class="sxs-lookup"><span data-stu-id="2c63c-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2c63c-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="2c63c-274">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="2c63c-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="2c63c-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="2c63c-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2c63c-277">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="2c63c-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2c63c-278">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2c63c-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2c63c-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2c63c-281">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="2c63c-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2c63c-282">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="2c63c-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2c63c-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="2c63c-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2c63c-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2c63c-285">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2c63c-286">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2c63c-287">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2c63c-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2c63c-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2c63c-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2c63c-290">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="2c63c-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="2c63c-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2c63c-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2c63c-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2c63c-293">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="2c63c-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="2c63c-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2c63c-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="2c63c-295">OrderID</span></span></td>
<td><p><span data-ttu-id="2c63c-296">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2c63c-297">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2c63c-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2c63c-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="2c63c-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="2c63c-300">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="2c63c-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="2c63c-301">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="2c63c-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="2c63c-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="2c63c-303">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="2c63c-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2c63c-304">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="2c63c-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="2c63c-305">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="2c63c-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="2c63c-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="2c63c-307">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="2c63c-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="2c63c-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2c63c-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-309">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="2c63c-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="2c63c-310">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="2c63c-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2c63c-311">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="2c63c-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="2c63c-312">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="2c63c-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-313">Région</span><span class="sxs-lookup"><span data-stu-id="2c63c-313">Region</span></span></td>
<td><p><span data-ttu-id="2c63c-314">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-314">The region the usage applies to.</span></span> <span data-ttu-id="2c63c-315">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="2c63c-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="2c63c-316">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="2c63c-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-317">référence SKU</span><span class="sxs-lookup"><span data-stu-id="2c63c-317">SKU</span></span></td>
<td><p><span data-ttu-id="2c63c-318">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="2c63c-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="2c63c-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="2c63c-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="2c63c-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="2c63c-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="2c63c-321">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="2c63c-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="2c63c-322">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="2c63c-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="2c63c-323">1</span><span class="sxs-lookup"><span data-stu-id="2c63c-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="2c63c-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="2c63c-325">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="2c63c-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="2c63c-326">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="2c63c-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="2c63c-327">11</span><span class="sxs-lookup"><span data-stu-id="2c63c-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="2c63c-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="2c63c-329">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="2c63c-329">Units included as part of the offer.</span></span> <span data-ttu-id="2c63c-330">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="2c63c-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="2c63c-331">0</span><span class="sxs-lookup"><span data-stu-id="2c63c-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2c63c-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="2c63c-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="2c63c-333">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="2c63c-334">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="2c63c-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="2c63c-335">11</span><span class="sxs-lookup"><span data-stu-id="2c63c-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="2c63c-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="2c63c-337">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="2c63c-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="2c63c-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="2c63c-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="2c63c-340">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="2c63c-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2c63c-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="2c63c-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="2c63c-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="2c63c-343">Frais de quantité, en fonction de votre marché de taxe&#39;les règles de taxe s et des circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="2c63c-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2c63c-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="2c63c-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="2c63c-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="2c63c-346">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="2c63c-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="2c63c-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="2c63c-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-348">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-348">Currency</span></span></td>
<td><p><span data-ttu-id="2c63c-349">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-349">Currency type.</span></span> <span data-ttu-id="2c63c-350">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="2c63c-351">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2c63c-352">EUR</span><span class="sxs-lookup"><span data-stu-id="2c63c-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2c63c-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2c63c-354">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="2c63c-354">Pretax price per unit.</span></span> <span data-ttu-id="2c63c-355">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="2c63c-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2c63c-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="2c63c-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2c63c-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2c63c-358">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="2c63c-358">Post tax price per unit.</span></span> <span data-ttu-id="2c63c-359">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="2c63c-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2c63c-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="2c63c-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2c63c-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="2c63c-362">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-362">The type of charge or adjustment.</span></span> <span data-ttu-id="2c63c-363">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="2c63c-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2c63c-364">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="2c63c-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="2c63c-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="2c63c-366">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="2c63c-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="2c63c-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="2c63c-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="2c63c-369">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="2c63c-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="2c63c-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2c63c-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="2c63c-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="2c63c-372">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="2c63c-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="2c63c-373">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="2c63c-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="2c63c-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="2c63c-375">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="2c63c-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="2c63c-376">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="2c63c-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="2c63c-377">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="2c63c-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="2c63c-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="2c63c-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="2c63c-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="2c63c-380">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="2c63c-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="2c63c-381">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="2c63c-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-382">Projet</span><span class="sxs-lookup"><span data-stu-id="2c63c-382">Project</span></span></td>
<td><p><span data-ttu-id="2c63c-383">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="2c63c-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="2c63c-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2c63c-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="2c63c-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="2c63c-386">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="2c63c-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="2c63c-387">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="2c63c-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="2c63c-388">Si vous aviez un pack de 25 connexions ServiceBus mis en service et vous aviez utilisé 1 pendant cette journée, votre relevé d’utilisation quotidienne pour ce jour indiquerait « 25 connexions / 30 jours – utilisé : 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="2c63c-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2c63c-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="2c63c-390">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2c63c-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2c63c-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2c63c-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="2c63c-392">DomainName</span></span></td>
<td><p><span data-ttu-id="2c63c-393">Client&#39;-s nom de domaine, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="2c63c-394">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="2c63c-395">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2c63c-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="2c63c-396">Unit</span><span class="sxs-lookup"><span data-stu-id="2c63c-396">Unit</span></span></td>
<td><p><span data-ttu-id="2c63c-397">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="2c63c-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="2c63c-398">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="2c63c-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="2c63c-399">Champs de fichier uniques et récurrentes</span><span class="sxs-lookup"><span data-stu-id="2c63c-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2c63c-400">colonne</span><span class="sxs-lookup"><span data-stu-id="2c63c-400">Column</span></span></th>
<th><span data-ttu-id="2c63c-401">Description</span><span class="sxs-lookup"><span data-stu-id="2c63c-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="2c63c-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2c63c-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="2c63c-403">Identificateur de locataire Microsoft Azure Active Directory unique pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="2c63c-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="2c63c-404">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="2c63c-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="2c63c-405">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="2c63c-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-406">Id du client</span><span class="sxs-lookup"><span data-stu-id="2c63c-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="2c63c-407">Microsoft Azure Active Directory ID de locataire unique, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-408">Nom du client</span><span class="sxs-lookup"><span data-stu-id="2c63c-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="2c63c-409">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="2c63c-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="2c63c-411">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="2c63c-412">Cela ne doit pas être utilisé pour identifier le client, comme le client/partenaire peut mettre à jour le domaine personnel/par défaut par le biais du portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c63c-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="2c63c-413">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-414">Pays du client</span><span class="sxs-lookup"><span data-stu-id="2c63c-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="2c63c-415">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-416">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="2c63c-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="2c63c-417">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="2c63c-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="2c63c-418">MpnId</span></span></td>
<td><p><span data-ttu-id="2c63c-419">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="2c63c-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-420">MpnId du revendeur</span><span class="sxs-lookup"><span data-stu-id="2c63c-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="2c63c-421">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-422">ID de commande</span><span class="sxs-lookup"><span data-stu-id="2c63c-422">Order ID</span></span></td>
<td><p><span data-ttu-id="2c63c-423">Identificateur unique d’une commande dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="2c63c-424">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-425">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="2c63c-425">Order date</span></span></td>
<td><p><span data-ttu-id="2c63c-426">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="2c63c-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="2c63c-427">ProductId</span></span></td>
<td><p><span data-ttu-id="2c63c-428">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="2c63c-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="2c63c-429">SkuId</span></span></td>
<td><p><span data-ttu-id="2c63c-430">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="2c63c-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="2c63c-432">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-432">The ID for a particular Availability.</span></span> <span data-ttu-id="2c63c-433">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="2c63c-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-434">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="2c63c-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="2c63c-435">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-436">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="2c63c-436">Product name</span></span></td>
<td><p><span data-ttu-id="2c63c-437">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="2c63c-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="2c63c-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="2c63c-439">Nom du serveur de publication du produit.</span><span class="sxs-lookup"><span data-stu-id="2c63c-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="2c63c-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="2c63c-441">ID unique pour ce serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="2c63c-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-442">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="2c63c-443">Nom convivial d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-444">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="2c63c-445">Identificateur unique pour un abonnement dans la plateforme de commerce de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="2c63c-446">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="2c63c-447">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2c63c-449">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-449">Start day of the charges.</span></span> <span data-ttu-id="2c63c-450">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2c63c-452">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-452">End day of the charges.</span></span> <span data-ttu-id="2c63c-453">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="2c63c-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-454">Terme et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="2c63c-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="2c63c-455">La longueur de terme et d’un cycle de facturation pour l’achat.</span><span class="sxs-lookup"><span data-stu-id="2c63c-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="2c63c-456">Par exemple, « 1 an, tous les mois. »</span><span class="sxs-lookup"><span data-stu-id="2c63c-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-457">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="2c63c-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="2c63c-458">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-459">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="2c63c-460">Le prix publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="2c63c-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2c63c-461">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-462">Prix unitaire efficace</span><span class="sxs-lookup"><span data-stu-id="2c63c-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="2c63c-463">Le prix unitaire après ont apporté des ajustements.</span><span class="sxs-lookup"><span data-stu-id="2c63c-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-464">Quantité</span><span class="sxs-lookup"><span data-stu-id="2c63c-464">Quantity</span></span></td>
<td><p><span data-ttu-id="2c63c-465">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="2c63c-465">Number of units.</span></span> <span data-ttu-id="2c63c-466">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-467">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="2c63c-467">Unit type</span></span></td>
<td><p><span data-ttu-id="2c63c-468">Le type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="2c63c-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="2c63c-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="2c63c-470">Explication sur les remises applicables.</span><span class="sxs-lookup"><span data-stu-id="2c63c-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-471">Sous-total</span><span class="sxs-lookup"><span data-stu-id="2c63c-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="2c63c-472">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="2c63c-472">Total before tax.</span></span> <span data-ttu-id="2c63c-473">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-474">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="2c63c-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="2c63c-475">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="2c63c-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-476">Total</span><span class="sxs-lookup"><span data-stu-id="2c63c-476">Total</span></span></td>
<td><p><span data-ttu-id="2c63c-477">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="2c63c-477">Total after tax.</span></span> <span data-ttu-id="2c63c-478">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="2c63c-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-479">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-479">Currency</span></span></td>
<td><p><span data-ttu-id="2c63c-480">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-480">Currency type.</span></span> <span data-ttu-id="2c63c-481">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="2c63c-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="2c63c-482">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="2c63c-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="2c63c-484">Un autre identificateur pour un ID de commande.</span><span class="sxs-lookup"><span data-stu-id="2c63c-484">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="2c63c-485">Champs de fichier d’utilisation quotidienne-évalués</span><span class="sxs-lookup"><span data-stu-id="2c63c-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2c63c-486">colonne</span><span class="sxs-lookup"><span data-stu-id="2c63c-486">Column</span></span></th>
<th><span data-ttu-id="2c63c-487">Description</span><span class="sxs-lookup"><span data-stu-id="2c63c-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="2c63c-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2c63c-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="2c63c-489">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="2c63c-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="2c63c-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="2c63c-491">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="2c63c-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="2c63c-493">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="2c63c-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="2c63c-495">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c63c-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="2c63c-496">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="2c63c-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="2c63c-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="2c63c-498">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-498">The customer’s domain name.</span></span> <span data-ttu-id="2c63c-499">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-500">Pays du client</span><span class="sxs-lookup"><span data-stu-id="2c63c-500">Customer country</span></span></td>
<td><p><span data-ttu-id="2c63c-501">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="2c63c-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-502">MPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-503">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="2c63c-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-504">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="2c63c-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="2c63c-505">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2c63c-506">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2c63c-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="2c63c-508">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="2c63c-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="2c63c-509">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="2c63c-510">ProductId</span></span></td>
<td><p><span data-ttu-id="2c63c-511">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="2c63c-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="2c63c-512">SkuId</span></span></td>
<td><p><span data-ttu-id="2c63c-513">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="2c63c-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="2c63c-515">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-515">The ID for a particular Availability.</span></span> <span data-ttu-id="2c63c-516">La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="2c63c-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-517">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="2c63c-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="2c63c-518">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="2c63c-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="2c63c-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="2c63c-520">Le nom du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="2c63c-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="2c63c-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="2c63c-522">L’ID du serveur de publication, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="2c63c-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="2c63c-523">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="2c63c-524">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="2c63c-525">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="2c63c-526">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="2c63c-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-527">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="2c63c-528">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2c63c-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2c63c-529">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="2c63c-530">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="2c63c-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2c63c-532">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="2c63c-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="2c63c-533">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="2c63c-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2c63c-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2c63c-535">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="2c63c-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="2c63c-536">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="2c63c-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-537">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="2c63c-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="2c63c-538">Date de l’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="2c63c-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-539">Type de compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="2c63c-540">Le type de compteur.</span><span class="sxs-lookup"><span data-stu-id="2c63c-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-541">Catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="2c63c-542">Le service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-543">Id de compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="2c63c-544">L’ID du compteur utilisé.</span><span class="sxs-lookup"><span data-stu-id="2c63c-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-545">Sous-catégorie du compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="2c63c-546">Le type de service Azure qui peut affecter le tarif.</span><span class="sxs-lookup"><span data-stu-id="2c63c-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-547">Nom du compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="2c63c-548">L’unité de mesure du compteur consommé.</span><span class="sxs-lookup"><span data-stu-id="2c63c-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-549">Région du compteur</span><span class="sxs-lookup"><span data-stu-id="2c63c-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="2c63c-550">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="2c63c-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-551">Unit</span><span class="sxs-lookup"><span data-stu-id="2c63c-551">Unit</span></span></td>
<td><p><span data-ttu-id="2c63c-552">L’unité de la ressource de nom.</span><span class="sxs-lookup"><span data-stu-id="2c63c-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-553">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="2c63c-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="2c63c-554">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="2c63c-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="2c63c-555">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="2c63c-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-556">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="2c63c-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="2c63c-557">Le centre de données où le compteur est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="2c63c-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-558">Service consommé</span><span class="sxs-lookup"><span data-stu-id="2c63c-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="2c63c-559">Le service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="2c63c-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-560">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="2c63c-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="2c63c-561">Le groupe de ressources dans lequel le compteur déployé s’exécute.</span><span class="sxs-lookup"><span data-stu-id="2c63c-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-562">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="2c63c-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="2c63c-563">L’URI de la ressource qui est utilisée.</span><span class="sxs-lookup"><span data-stu-id="2c63c-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-564">Type de frais</span><span class="sxs-lookup"><span data-stu-id="2c63c-564">Charge type</span></span></td>
<td><p><span data-ttu-id="2c63c-565">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-565">The type of charge or adjustment.</span></span> <span data-ttu-id="2c63c-566">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-567">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="2c63c-567">Unit price</span></span></td>
<td><p><span data-ttu-id="2c63c-568">Prix par licence, telles que publiées dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="2c63c-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2c63c-569">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-570">Quantité</span><span class="sxs-lookup"><span data-stu-id="2c63c-570">Quantity</span></span></td>
<td><p><span data-ttu-id="2c63c-571">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="2c63c-571">Number of licenses.</span></span> <span data-ttu-id="2c63c-572">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-573">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="2c63c-573">Unit type</span></span></td>
<td><p><span data-ttu-id="2c63c-574">Le type d’unité dans que le compteur est facturé.</span><span class="sxs-lookup"><span data-stu-id="2c63c-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="2c63c-575">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="2c63c-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-576">Facturation avant impôts</span><span class="sxs-lookup"><span data-stu-id="2c63c-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="2c63c-577">Quantité totale avant impôts.</span><span class="sxs-lookup"><span data-stu-id="2c63c-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-578">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="2c63c-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="2c63c-579">La devise dans la région géographique du client</span><span class="sxs-lookup"><span data-stu-id="2c63c-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-580">Prix total avant impôt</span><span class="sxs-lookup"><span data-stu-id="2c63c-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="2c63c-581">La tarification avant les taxes sont ajoutées.</span><span class="sxs-lookup"><span data-stu-id="2c63c-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-582">Tarification de devise</span><span class="sxs-lookup"><span data-stu-id="2c63c-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="2c63c-583">La devise dans la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="2c63c-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-584">Informations sur le service 1</span><span class="sxs-lookup"><span data-stu-id="2c63c-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="2c63c-585">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="2c63c-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-586">Informations sur le service 2</span><span class="sxs-lookup"><span data-stu-id="2c63c-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="2c63c-587">Champ hérité capturant les métadonnées facultatives propres au service.</span><span class="sxs-lookup"><span data-stu-id="2c63c-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="2c63c-588">Balises</span><span class="sxs-lookup"><span data-stu-id="2c63c-588">Tags</span></span></td>
<td><p><span data-ttu-id="2c63c-589">Balises que vous affectez au compteur dans l’ordre pour regrouper les enregistrements de facturation.</span><span class="sxs-lookup"><span data-stu-id="2c63c-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="2c63c-590">Par exemple, vous pouvez utiliser des balises pour répartir les coûts par département qui utilise le compteur.</span><span class="sxs-lookup"><span data-stu-id="2c63c-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="2c63c-591">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="2c63c-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="2c63c-592">Toute information supplémentaire non couverte dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="2c63c-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="2c63c-593">Frais de mappage entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="2c63c-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="2c63c-594">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="2c63c-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="2c63c-595">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="2c63c-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="2c63c-596">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="2c63c-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="2c63c-597">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’« ajustements » ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="2c63c-598">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="2c63c-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="2c63c-599"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-600"><strong>Description des frais fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-601"><strong>Qu’est ce coût ?</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-602"><strong>Comment pour mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="2c63c-603"><strong>Frais sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-604">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="2c63c-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-605">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="2c63c-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="2c63c-606">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-607">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="2c63c-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-608">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="2c63c-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-609">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="2c63c-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-610">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-611">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="2c63c-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-612">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="2c63c-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-613">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="2c63c-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-614">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="2c63c-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-615">Frais au prorata à l'achat</span><span class="sxs-lookup"><span data-stu-id="2c63c-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-616">Le type de frais pour un abonnement lors de l’utilisation de facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="2c63c-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-617">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-618">Le type de frais pour un abonnement lors de l’utilisation de la facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="2c63c-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-619">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="2c63c-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-620">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="2c63c-621">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="2c63c-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-622">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-623">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="2c63c-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-624">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="2c63c-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="2c63c-625"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-626">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="2c63c-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-627">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="2c63c-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="2c63c-628">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-629">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="2c63c-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-630">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="2c63c-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-631"><strong>Crédits</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-632">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="2c63c-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-633">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="2c63c-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-634">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="2c63c-635">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="2c63c-636"><strong>Basée sur l’utilisation des remises</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-637">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="2c63c-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-638">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="2c63c-639">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-640">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="2c63c-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-641">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="2c63c-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-642">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="2c63c-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-643">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="2c63c-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-644">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="2c63c-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-645">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="2c63c-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="2c63c-646"><strong>Remises sous licence</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-647"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="2c63c-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="2c63c-648">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2c63c-649"><strong>Taxes</strong>  &nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-650"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="2c63c-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="2c63c-651"><em>Exception : &quot;Compense un élément de ligne&quot; inclut déjà des taxes. Consultez des crédits, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="2c63c-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-652">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="2c63c-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="2c63c-653">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="2c63c-654">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="2c63c-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
