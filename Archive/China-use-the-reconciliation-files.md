---
title: Utilisez les fichiers de réconciliation (Partner Center géré par 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132079"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="6496d-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="6496d-103">Use the reconciliation files</span></span>

<span data-ttu-id="6496d-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="6496d-104">**Applies to**</span></span>

-   <span data-ttu-id="6496d-105">Espace partenaires géré par 21Vianet</span><span class="sxs-lookup"><span data-stu-id="6496d-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="6496d-106">Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="6496d-107">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="6496d-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="6496d-108">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="6496d-108">Itemize by partner</span></span>


<span data-ttu-id="6496d-109">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licence pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="6496d-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="6496d-110">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="6496d-110">MPN ID</span></span></th>
<th><span data-ttu-id="6496d-111">Description</span><span class="sxs-lookup"><span data-stu-id="6496d-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="6496d-112">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="6496d-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="6496d-113">L’ID Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="6496d-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-114">ID&nbsp;MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="6496d-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="6496d-115">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="6496d-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="6496d-116">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6496d-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6496d-117">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="6496d-118">Pour afficher ou mettre à jour le revendeur, dans le menu Espace partenaires, sélectionnez <strong>Clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6496d-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="6496d-119">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6496d-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="6496d-120">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="6496d-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="6496d-121">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="6496d-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="6496d-122">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="6496d-123">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="6496d-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="6496d-124">Champs d’un fichier basé sur licence</span><span class="sxs-lookup"><span data-stu-id="6496d-124">License-based file fields</span></span>


<span data-ttu-id="6496d-125">Pour rapprocher vos frais des commandes des clients, comparez le Syndication\_Partenaire\_Abonnement\_Numéro dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="6496d-126"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="6496d-127"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="6496d-128"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="6496d-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="6496d-130">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6496d-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="6496d-131">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="6496d-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="6496d-132">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="6496d-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="6496d-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="6496d-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="6496d-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="6496d-135">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6496d-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="6496d-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="6496d-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="6496d-137">OrderID</span></span></td>
<td><p><span data-ttu-id="6496d-138">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6496d-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="6496d-139">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="6496d-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="6496d-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="6496d-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="6496d-142">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6496d-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="6496d-143">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="6496d-144">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="6496d-145">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="6496d-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="6496d-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="6496d-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-147">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="6496d-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="6496d-148">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="6496d-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="6496d-149">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="6496d-150">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="6496d-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="6496d-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="6496d-152">OfferID</span></span></td>
<td><p><span data-ttu-id="6496d-153">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="6496d-153">Unique offer ID.</span></span> <span data-ttu-id="6496d-154">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="6496d-155"><b>Remarque</b>: Cette valeur ne correspond pas d’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="6496d-156">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="6496d-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="6496d-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="6496d-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="6496d-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="6496d-159">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="6496d-160"><b>Remarque</b>: Cette valeur correspond à l’ID de l’offre à partir de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="6496d-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="6496d-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="6496d-162">OfferName</span></span></td>
<td><p><span data-ttu-id="6496d-163">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="6496d-164">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="6496d-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="6496d-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="6496d-166">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="6496d-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="6496d-167">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="6496d-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="6496d-168">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6496d-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6496d-169">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6496d-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="6496d-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="6496d-171">La date de fin d’abonnement : 12 mois + x jours après la date de début (pour les aligner avec date de facturation du partenaire) ou 12 mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="6496d-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="6496d-172">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="6496d-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="6496d-173">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="6496d-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="6496d-174">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6496d-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6496d-175">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6496d-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6496d-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6496d-177">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="6496d-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="6496d-178">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="6496d-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="6496d-179">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6496d-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6496d-180">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6496d-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6496d-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6496d-182">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="6496d-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="6496d-183">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="6496d-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="6496d-184">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6496d-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="6496d-185">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="6496d-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="6496d-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="6496d-187">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6496d-187">The type of charge or adjustment.</span></span> <span data-ttu-id="6496d-188">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6496d-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="6496d-189">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6496d-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="6496d-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="6496d-191">Prix par siège.</span><span class="sxs-lookup"><span data-stu-id="6496d-191">Price per seat.</span></span> <span data-ttu-id="6496d-192">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="6496d-193">6.82</span><span class="sxs-lookup"><span data-stu-id="6496d-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-194">Quantité</span><span class="sxs-lookup"><span data-stu-id="6496d-194">Quantity</span></span></td>
<td><p><span data-ttu-id="6496d-195">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="6496d-195">Number of seats.</span></span> <span data-ttu-id="6496d-196">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="6496d-197">2</span><span class="sxs-lookup"><span data-stu-id="6496d-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-198">Montant</span><span class="sxs-lookup"><span data-stu-id="6496d-198">Amount</span></span></td>
<td><p><span data-ttu-id="6496d-199">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="6496d-199">Total of price for quantity.</span></span> <span data-ttu-id="6496d-200">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="6496d-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="6496d-201">13.32</span><span class="sxs-lookup"><span data-stu-id="6496d-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="6496d-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="6496d-203">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="6496d-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="6496d-204">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="6496d-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="6496d-205">2.32</span><span class="sxs-lookup"><span data-stu-id="6496d-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-206">Sous-total</span><span class="sxs-lookup"><span data-stu-id="6496d-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="6496d-207">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="6496d-207">Total before tax.</span></span> <span data-ttu-id="6496d-208">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="6496d-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="6496d-209">11</span><span class="sxs-lookup"><span data-stu-id="6496d-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-210">Taxe</span><span class="sxs-lookup"><span data-stu-id="6496d-210">Tax</span></span></td>
<td><p><span data-ttu-id="6496d-211">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="6496d-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="6496d-212">0</span><span class="sxs-lookup"><span data-stu-id="6496d-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="6496d-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="6496d-214">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="6496d-214">Total after tax.</span></span> <span data-ttu-id="6496d-215">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="6496d-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="6496d-216">11</span><span class="sxs-lookup"><span data-stu-id="6496d-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-217">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="6496d-217">Currency</span></span></td>
<td><p><span data-ttu-id="6496d-218">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="6496d-218">Currency type.</span></span> <span data-ttu-id="6496d-219">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="6496d-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="6496d-220">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="6496d-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="6496d-221">CNY</span><span class="sxs-lookup"><span data-stu-id="6496d-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="6496d-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="6496d-223">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="6496d-224">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="6496d-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="6496d-225">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="6496d-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="6496d-226">MPNID</span></span></td>
<td><p><span data-ttu-id="6496d-227">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="6496d-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="6496d-228">4390934</span><span class="sxs-lookup"><span data-stu-id="6496d-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="6496d-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="6496d-230">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6496d-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6496d-231">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="6496d-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="6496d-232">4390934</span><span class="sxs-lookup"><span data-stu-id="6496d-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="6496d-233">DomainName</span></span></td>
<td><p><span data-ttu-id="6496d-234">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6496d-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="6496d-235">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6496d-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="6496d-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="6496d-237">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="6496d-237">Subscription nickname.</span></span> <span data-ttu-id="6496d-238">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="6496d-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="6496d-239">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="6496d-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="6496d-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="6496d-241">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6496d-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="6496d-242">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="6496d-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="6496d-243">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="6496d-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="6496d-244">Champs de fichier basée sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="6496d-244">Usage-based file fields</span></span>


<span data-ttu-id="6496d-245">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="6496d-246">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="6496d-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="6496d-247"><strong>Colonne</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="6496d-248"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="6496d-249"><strong>Exemple de valeur</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="6496d-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="6496d-251">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6496d-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="6496d-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="6496d-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="6496d-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="6496d-254">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="6496d-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="6496d-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="6496d-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="6496d-257">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="6496d-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="6496d-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="6496d-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="6496d-260">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6496d-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="6496d-261">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="6496d-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="6496d-262">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="6496d-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="6496d-263">MPNID</span></span></td>
<td><p><span data-ttu-id="6496d-264">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="6496d-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="6496d-265">4390934</span><span class="sxs-lookup"><span data-stu-id="6496d-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="6496d-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="6496d-267">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6496d-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6496d-268">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="6496d-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="6496d-269">4390934</span><span class="sxs-lookup"><span data-stu-id="6496d-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="6496d-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="6496d-271">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="6496d-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="6496d-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="6496d-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6496d-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6496d-274">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6496d-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="6496d-275">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6496d-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6496d-276">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="6496d-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6496d-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6496d-278">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6496d-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="6496d-279">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6496d-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="6496d-280">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="6496d-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="6496d-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="6496d-282">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6496d-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="6496d-283">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="6496d-284">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="6496d-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="6496d-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="6496d-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="6496d-287">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="6496d-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="6496d-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="6496d-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="6496d-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="6496d-290">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="6496d-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="6496d-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="6496d-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="6496d-292">OrderID</span></span></td>
<td><p><span data-ttu-id="6496d-293">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6496d-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="6496d-294">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="6496d-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="6496d-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="6496d-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="6496d-297">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="6496d-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="6496d-298">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="6496d-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="6496d-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="6496d-300">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="6496d-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="6496d-301">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="6496d-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="6496d-302">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="6496d-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="6496d-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="6496d-304">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="6496d-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="6496d-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="6496d-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-306">Nom de ressource</span><span class="sxs-lookup"><span data-stu-id="6496d-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="6496d-307">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="6496d-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="6496d-308">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="6496d-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="6496d-309">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="6496d-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-310">Région</span><span class="sxs-lookup"><span data-stu-id="6496d-310">Region</span></span></td>
<td><p><span data-ttu-id="6496d-311">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="6496d-311">The region the usage applies to.</span></span> <span data-ttu-id="6496d-312">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="6496d-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="6496d-313">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="6496d-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-314">référence SKU</span><span class="sxs-lookup"><span data-stu-id="6496d-314">SKU</span></span></td>
<td><p><span data-ttu-id="6496d-315">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="6496d-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="6496d-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="6496d-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="6496d-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="6496d-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="6496d-318">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="6496d-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="6496d-319">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="6496d-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="6496d-320">1</span><span class="sxs-lookup"><span data-stu-id="6496d-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="6496d-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="6496d-322">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="6496d-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="6496d-323">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="6496d-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="6496d-324">11</span><span class="sxs-lookup"><span data-stu-id="6496d-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="6496d-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="6496d-326">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="6496d-326">Units included as part of the offer.</span></span> <span data-ttu-id="6496d-327">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="6496d-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="6496d-328">0</span><span class="sxs-lookup"><span data-stu-id="6496d-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="6496d-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="6496d-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="6496d-330">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="6496d-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="6496d-331">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="6496d-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="6496d-332">11</span><span class="sxs-lookup"><span data-stu-id="6496d-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="6496d-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="6496d-334">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6496d-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="6496d-335">$0.0808</span><span class="sxs-lookup"><span data-stu-id="6496d-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="6496d-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="6496d-337">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6496d-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6496d-338">$0.085</span><span class="sxs-lookup"><span data-stu-id="6496d-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="6496d-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="6496d-340">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="6496d-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="6496d-341">$0.08</span><span class="sxs-lookup"><span data-stu-id="6496d-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="6496d-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="6496d-343">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="6496d-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="6496d-344">$0.93</span><span class="sxs-lookup"><span data-stu-id="6496d-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-345">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="6496d-345">Currency</span></span></td>
<td><p><span data-ttu-id="6496d-346">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="6496d-346">Currency type.</span></span> <span data-ttu-id="6496d-347">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="6496d-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="6496d-348">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="6496d-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="6496d-349">CNY</span><span class="sxs-lookup"><span data-stu-id="6496d-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="6496d-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="6496d-351">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="6496d-351">Pretax price per unit.</span></span> <span data-ttu-id="6496d-352">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6496d-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6496d-353">$0.08</span><span class="sxs-lookup"><span data-stu-id="6496d-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="6496d-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="6496d-355">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="6496d-355">Post tax price per unit.</span></span> <span data-ttu-id="6496d-356">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6496d-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6496d-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="6496d-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="6496d-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="6496d-359">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6496d-359">The type of charge or adjustment.</span></span> <span data-ttu-id="6496d-360">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6496d-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="6496d-361">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6496d-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="6496d-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="6496d-363">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="6496d-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="6496d-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="6496d-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="6496d-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="6496d-366">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="6496d-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="6496d-367">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="6496d-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="6496d-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="6496d-369">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="6496d-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="6496d-370">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="6496d-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="6496d-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="6496d-372">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="6496d-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="6496d-373">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="6496d-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="6496d-374">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="6496d-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="6496d-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="6496d-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="6496d-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="6496d-377">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="6496d-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="6496d-378">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="6496d-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-379">Projet</span><span class="sxs-lookup"><span data-stu-id="6496d-379">Project</span></span></td>
<td><p><span data-ttu-id="6496d-380">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="6496d-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="6496d-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="6496d-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="6496d-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="6496d-383">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="6496d-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="6496d-384">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="6496d-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="6496d-385">Si vous aviez un pack de 25 connexions ServiceBus mis en service et vous aviez utilisé 1 pendant cette journée, votre relevé d’utilisation quotidienne pour ce jour indiquerait « 25 connexions / 30 jours – utilisé : 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="6496d-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6496d-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="6496d-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="6496d-387">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6496d-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="6496d-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="6496d-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6496d-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="6496d-389">DomainName</span></span></td>
<td><p><span data-ttu-id="6496d-390">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6496d-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="6496d-391">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6496d-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="6496d-392">Frais de mappage entre une facture et le fichier de réconciliation</span><span class="sxs-lookup"><span data-stu-id="6496d-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="6496d-393">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="6496d-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="6496d-394">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de Microsoft Excel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="6496d-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="6496d-395">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6496d-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="6496d-396"><strong>Description des frais de facture</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-397"><strong>Description des frais fichier de réconciliation (colonne ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-398"><strong>Qu’est ce coût ?</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-399"><strong>Comment pour mapper ces ChargeTypes à la facture ?</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="6496d-400"><strong>Frais récurrents</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-401">Instance d'annulation au prorata</span><span class="sxs-lookup"><span data-stu-id="6496d-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-402">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="6496d-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="6496d-403">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-404">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="6496d-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-405">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-406">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="6496d-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-407">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="6496d-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-408">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="6496d-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-409">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="6496d-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-410">Frais au prorata à l'achat</span><span class="sxs-lookup"><span data-stu-id="6496d-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-411">Frais au prorata lors de l’achat</span><span class="sxs-lookup"><span data-stu-id="6496d-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-412">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-413">Frais initiaux de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-414">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="6496d-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-415">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-416">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="6496d-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-417">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-418"><strong>Autres produits et Services</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-419">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="6496d-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-420">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="6496d-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-421">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="6496d-422"><strong>Frais d’utilisation</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-423">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="6496d-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-424">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="6496d-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="6496d-425">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-426">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="6496d-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-427">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="6496d-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-428"><strong>Crédits &amp; ajustements</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-429">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="6496d-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-430">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="6496d-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-431">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="6496d-432">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="6496d-433"><strong>Autres remises</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="6496d-434">
<em>(basée sur l’utilisation)</em></span><span class="sxs-lookup"><span data-stu-id="6496d-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-435">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="6496d-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-436">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="6496d-437">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-438">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="6496d-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-439">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="6496d-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="6496d-440">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="6496d-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-441">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6496d-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="6496d-442">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="6496d-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-443">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="6496d-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-444"><strong>Autres remises</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="6496d-445">
<em>(license-based)</em></span><span class="sxs-lookup"><span data-stu-id="6496d-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-446"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="6496d-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="6496d-447">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6496d-448"><strong>Taxes</strong>  &nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-449"><em>Peut être appliqué à plusieurs types de frais</em></span><span class="sxs-lookup"><span data-stu-id="6496d-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="6496d-450"><em>Exception : « Compense un élément de ligne » inclut déjà des taxes. Afficher les crédits &amp; ajustements, ci-dessus.</em></span><span class="sxs-lookup"><span data-stu-id="6496d-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-451">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="6496d-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="6496d-452">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="6496d-453">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="6496d-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
