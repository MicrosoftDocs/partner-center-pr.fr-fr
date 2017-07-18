---
title: Utiliser les fichiers de rapprochement | Espace partenaires
description: "Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 61e71d4207d9e8ac68ee4fcfc1f0d04282474032
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/19/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="a5c55-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="a5c55-103">Use the reconciliation files</span></span>

**<span data-ttu-id="a5c55-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="a5c55-104">Applies to</span></span>**

-  <span data-ttu-id="a5c55-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a5c55-105">Partner Center</span></span>
-  <span data-ttu-id="a5c55-106">Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis</span><span class="sxs-lookup"><span data-stu-id="a5c55-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="a5c55-107">Espace partenaires de Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="a5c55-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="a5c55-108">Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="a5c55-109">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="a5c55-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <span data-ttu-id="a5c55-110"><a href="" id="itemizebypartner"></a>Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="a5c55-110"><a href="" id="itemizebypartner"></a>Itemize by partner</span></span>


<span data-ttu-id="a5c55-111">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="a5c55-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a5c55-112">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="a5c55-112">MPN ID</span></span></th>
<th><span data-ttu-id="a5c55-113">Description</span><span class="sxs-lookup"><span data-stu-id="a5c55-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="a5c55-114">ID MPN</span><span class="sxs-lookup"><span data-stu-id="a5c55-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="a5c55-115">L’ID MicrosoftPartner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="a5c55-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-116">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="a5c55-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="a5c55-117">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="a5c55-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="a5c55-118">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a5c55-119">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="a5c55-120">Pour afficher ou mettre à jour le revendeur, dans le menu Espace partenaires, sélectionnez <strong>Clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a5c55-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="a5c55-121">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a5c55-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="a5c55-122">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="a5c55-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="a5c55-123">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="a5c55-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="a5c55-124">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="a5c55-125">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="a5c55-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <span data-ttu-id="a5c55-126"><a href="" id="licencebasedfiles"></a> Champs des fichiers basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="a5c55-126"><a href="" id="licencebasedfiles"></a> License-based file fields</span></span>


<span data-ttu-id="a5c55-127">Pour rapprocher vos frais des commandes des clients, comparez le numéro d’abonnement du partenaire de syndication dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a5c55-128">Colonne</span><span class="sxs-lookup"><span data-stu-id="a5c55-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a5c55-129">Description</span><span class="sxs-lookup"><span data-stu-id="a5c55-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a5c55-130">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="a5c55-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-131">OperatingUnit</span><span class="sxs-lookup"><span data-stu-id="a5c55-131">OperatingUnit</span></span></td>
<td><p><span data-ttu-id="a5c55-132">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="a5c55-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="a5c55-133">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="a5c55-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="a5c55-134">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="a5c55-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="a5c55-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="a5c55-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a5c55-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="a5c55-137">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="a5c55-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a5c55-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="a5c55-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="a5c55-139">OrderID</span></span></td>
<td><p><span data-ttu-id="a5c55-140">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5c55-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a5c55-141">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a5c55-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a5c55-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a5c55-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a5c55-144">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5c55-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a5c55-145">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a5c55-146">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="a5c55-147">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="a5c55-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="a5c55-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a5c55-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-149">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="a5c55-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="a5c55-150">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="a5c55-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="a5c55-151">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="a5c55-152">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a5c55-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="a5c55-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="a5c55-154">OfferID</span></span></td>
<td><p><span data-ttu-id="a5c55-155">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="a5c55-155">Unique offer ID.</span></span> <span data-ttu-id="a5c55-156">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="a5c55-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="a5c55-157"><b>Remarque</b>: cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="a5c55-158">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a5c55-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="a5c55-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="a5c55-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="a5c55-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="a5c55-161">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="a5c55-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="a5c55-162"><b>Remarque</b>: cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="a5c55-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="a5c55-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="a5c55-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="a5c55-164">OfferName</span></span></td>
<td><p><span data-ttu-id="a5c55-165">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="a5c55-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="a5c55-166">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="a5c55-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="a5c55-168">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="a5c55-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="a5c55-169">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="a5c55-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="a5c55-170">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a5c55-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a5c55-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a5c55-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="a5c55-173">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="a5c55-174">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="a5c55-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="a5c55-175">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="a5c55-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="a5c55-176">L’heure indique toujours le début de la journée (0:00).</span><span class="sxs-lookup"><span data-stu-id="a5c55-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a5c55-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a5c55-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a5c55-179">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="a5c55-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="a5c55-180">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="a5c55-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a5c55-181">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a5c55-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a5c55-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a5c55-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a5c55-184">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="a5c55-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="a5c55-185">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="a5c55-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a5c55-186">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="a5c55-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a5c55-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="a5c55-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a5c55-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="a5c55-189">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-189">The type of charge or adjustment.</span></span> <span data-ttu-id="a5c55-190">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="a5c55-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a5c55-191">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="a5c55-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="a5c55-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="a5c55-193">Prix par siège.</span><span class="sxs-lookup"><span data-stu-id="a5c55-193">Price per seat.</span></span> <span data-ttu-id="a5c55-194">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a5c55-195">6.82</span><span class="sxs-lookup"><span data-stu-id="a5c55-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-196">Quantité</span><span class="sxs-lookup"><span data-stu-id="a5c55-196">Quantity</span></span></td>
<td><p><span data-ttu-id="a5c55-197">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="a5c55-197">Number of seats.</span></span> <span data-ttu-id="a5c55-198">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a5c55-199">2</span><span class="sxs-lookup"><span data-stu-id="a5c55-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-200">Montant</span><span class="sxs-lookup"><span data-stu-id="a5c55-200">Amount</span></span></td>
<td><p><span data-ttu-id="a5c55-201">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="a5c55-201">Total of price for quantity.</span></span> <span data-ttu-id="a5c55-202">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="a5c55-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="a5c55-203">13.32</span><span class="sxs-lookup"><span data-stu-id="a5c55-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="a5c55-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="a5c55-205">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="a5c55-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="a5c55-206">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="a5c55-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="a5c55-207">2.32</span><span class="sxs-lookup"><span data-stu-id="a5c55-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-208">Sous-total</span><span class="sxs-lookup"><span data-stu-id="a5c55-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="a5c55-209">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="a5c55-209">Total before tax.</span></span> <span data-ttu-id="a5c55-210">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="a5c55-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="a5c55-211">11</span><span class="sxs-lookup"><span data-stu-id="a5c55-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-212">Taxe</span><span class="sxs-lookup"><span data-stu-id="a5c55-212">Tax</span></span></td>
<td><p><span data-ttu-id="a5c55-213">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="a5c55-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a5c55-214">0</span><span class="sxs-lookup"><span data-stu-id="a5c55-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="a5c55-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="a5c55-216">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="a5c55-216">Total after tax.</span></span> <span data-ttu-id="a5c55-217">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="a5c55-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="a5c55-218">11</span><span class="sxs-lookup"><span data-stu-id="a5c55-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-219">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="a5c55-219">Currency</span></span></td>
<td><p><span data-ttu-id="a5c55-220">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="a5c55-220">Currency type.</span></span> <span data-ttu-id="a5c55-221">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="a5c55-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="a5c55-222">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="a5c55-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a5c55-223">EUR</span><span class="sxs-lookup"><span data-stu-id="a5c55-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a5c55-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="a5c55-225">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="a5c55-226">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="a5c55-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a5c55-227">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="a5c55-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="a5c55-228">MPNID</span></span></td>
<td><p><span data-ttu-id="a5c55-229">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="a5c55-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="a5c55-230">4390934</span><span class="sxs-lookup"><span data-stu-id="a5c55-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a5c55-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a5c55-232">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a5c55-233">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="a5c55-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="a5c55-234">4390934</span><span class="sxs-lookup"><span data-stu-id="a5c55-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="a5c55-235">DomainName</span></span></td>
<td><p><span data-ttu-id="a5c55-236">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="a5c55-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="a5c55-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a5c55-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a5c55-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a5c55-239">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-239">Subscription nickname.</span></span> <span data-ttu-id="a5c55-240">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="a5c55-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="a5c55-241">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="a5c55-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a5c55-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a5c55-243">Le nom de l’offre de service achetée par le client, telle que définie dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="a5c55-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="a5c55-244">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="a5c55-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="a5c55-245">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="a5c55-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <span data-ttu-id="a5c55-246"><a href="" id="usagebasedfiles"></a>Champs des fichiers basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="a5c55-246"><a href="" id="usagebasedfiles"></a>Usage-based file fields</span></span>


<span data-ttu-id="a5c55-247">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="a5c55-248">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="a5c55-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a5c55-249">Colonne</span><span class="sxs-lookup"><span data-stu-id="a5c55-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a5c55-250">Description</span><span class="sxs-lookup"><span data-stu-id="a5c55-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a5c55-251">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="a5c55-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="a5c55-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="a5c55-253">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="a5c55-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="a5c55-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a5c55-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="a5c55-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="a5c55-256">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="a5c55-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="a5c55-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="a5c55-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="a5c55-259">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="a5c55-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="a5c55-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a5c55-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="a5c55-262">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a5c55-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="a5c55-263">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="a5c55-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a5c55-264">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="a5c55-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="a5c55-265">MPNID</span></span></td>
<td><p><span data-ttu-id="a5c55-266">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="a5c55-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="a5c55-267">4390934</span><span class="sxs-lookup"><span data-stu-id="a5c55-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a5c55-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a5c55-269">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a5c55-270">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="a5c55-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="a5c55-271">4390934</span><span class="sxs-lookup"><span data-stu-id="a5c55-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="a5c55-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="a5c55-273">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="a5c55-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="a5c55-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="a5c55-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a5c55-276">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="a5c55-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a5c55-277">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a5c55-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a5c55-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a5c55-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a5c55-280">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="a5c55-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a5c55-281">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="a5c55-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a5c55-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="a5c55-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a5c55-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a5c55-284">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5c55-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a5c55-285">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a5c55-286">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a5c55-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a5c55-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a5c55-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a5c55-289">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="a5c55-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="a5c55-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a5c55-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a5c55-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a5c55-292">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="a5c55-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="a5c55-293">Microsoft&nbsp;Azure</span><span class="sxs-lookup"><span data-stu-id="a5c55-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-294">OrderId</span><span class="sxs-lookup"><span data-stu-id="a5c55-294">OrderID</span></span></td>
<td><p><span data-ttu-id="a5c55-295">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5c55-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a5c55-296">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a5c55-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a5c55-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="a5c55-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="a5c55-299">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="a5c55-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="a5c55-300">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="a5c55-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="a5c55-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="a5c55-302">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="a5c55-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a5c55-303">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="a5c55-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="a5c55-304">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="a5c55-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="a5c55-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="a5c55-306">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="a5c55-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="a5c55-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a5c55-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-308">Nom de la ressource</span><span class="sxs-lookup"><span data-stu-id="a5c55-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="a5c55-309">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="a5c55-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a5c55-310">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="a5c55-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="a5c55-311">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="a5c55-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-312">Région</span><span class="sxs-lookup"><span data-stu-id="a5c55-312">Region</span></span></td>
<td><p><span data-ttu-id="a5c55-313">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="a5c55-313">The region the usage applies to.</span></span> <span data-ttu-id="a5c55-314">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="a5c55-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="a5c55-315">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="a5c55-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-316">SKU</span><span class="sxs-lookup"><span data-stu-id="a5c55-316">SKU</span></span></td>
<td><p><span data-ttu-id="a5c55-317">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="a5c55-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="a5c55-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="a5c55-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a5c55-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="a5c55-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="a5c55-320">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="a5c55-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="a5c55-321">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="a5c55-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="a5c55-322">1</span><span class="sxs-lookup"><span data-stu-id="a5c55-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="a5c55-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="a5c55-324">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="a5c55-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="a5c55-325">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="a5c55-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="a5c55-326">11</span><span class="sxs-lookup"><span data-stu-id="a5c55-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="a5c55-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="a5c55-328">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="a5c55-328">Units included as part of the offer.</span></span> <span data-ttu-id="a5c55-329">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="a5c55-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="a5c55-330">0</span><span class="sxs-lookup"><span data-stu-id="a5c55-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a5c55-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="a5c55-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="a5c55-332">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="a5c55-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="a5c55-333">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="a5c55-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="a5c55-334">11</span><span class="sxs-lookup"><span data-stu-id="a5c55-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="a5c55-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="a5c55-336">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="a5c55-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="a5c55-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="a5c55-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="a5c55-339">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="a5c55-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a5c55-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="a5c55-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="a5c55-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="a5c55-342">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="a5c55-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a5c55-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="a5c55-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="a5c55-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="a5c55-345">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="a5c55-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="a5c55-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="a5c55-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-347">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="a5c55-347">Currency</span></span></td>
<td><p><span data-ttu-id="a5c55-348">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="a5c55-348">Currency type.</span></span> <span data-ttu-id="a5c55-349">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="a5c55-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="a5c55-350">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="a5c55-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a5c55-351">EUR</span><span class="sxs-lookup"><span data-stu-id="a5c55-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a5c55-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a5c55-353">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="a5c55-353">Pretax price per unit.</span></span> <span data-ttu-id="a5c55-354">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="a5c55-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a5c55-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="a5c55-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a5c55-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a5c55-357">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="a5c55-357">Post tax price per unit.</span></span> <span data-ttu-id="a5c55-358">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="a5c55-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a5c55-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="a5c55-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a5c55-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="a5c55-361">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-361">The type of charge or adjustment.</span></span> <span data-ttu-id="a5c55-362">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="a5c55-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a5c55-363">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="a5c55-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="a5c55-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="a5c55-365">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="a5c55-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="a5c55-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="a5c55-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="a5c55-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="a5c55-368">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="a5c55-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="a5c55-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a5c55-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="a5c55-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="a5c55-371">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="a5c55-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="a5c55-372">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="a5c55-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="a5c55-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="a5c55-374">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="a5c55-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="a5c55-375">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="a5c55-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="a5c55-376">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="a5c55-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="a5c55-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="a5c55-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="a5c55-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="a5c55-379">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="a5c55-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="a5c55-380">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="a5c55-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-381">Projet</span><span class="sxs-lookup"><span data-stu-id="a5c55-381">Project</span></span></td>
<td><p><span data-ttu-id="a5c55-382">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="a5c55-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="a5c55-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a5c55-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="a5c55-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="a5c55-385">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="a5c55-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="a5c55-386">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="a5c55-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="a5c55-387">Si vous avez un pack de 25 connexions ServiceBus et que vous en avez utilisé 1 ce jour-là, votre relevé d’utilisation quotidienne indiquera « 25 connexions/30 jours - Utilisées : 1 ».</span><span class="sxs-lookup"><span data-stu-id="a5c55-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a5c55-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a5c55-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="a5c55-389">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="a5c55-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a5c55-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a5c55-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a5c55-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="a5c55-391">DomainName</span></span></td>
<td><p><span data-ttu-id="a5c55-392">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="a5c55-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="a5c55-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a5c55-393">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <span data-ttu-id="a5c55-394"><a href="" id="charge_types"></a>Frais de mappage entre une facture et le fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="a5c55-394"><a href="" id="charge_types"></a>Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="a5c55-395">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="a5c55-395">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="a5c55-396">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de MicrosoftExcel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="a5c55-396">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="a5c55-397">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="a5c55-397">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="a5c55-398">Description des frais indiqués sur les factures</span><span class="sxs-lookup"><span data-stu-id="a5c55-398">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a5c55-399">Description des frais figurant sur le fichier de rapprochement (colonne ChargeType)</span><span class="sxs-lookup"><span data-stu-id="a5c55-399">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a5c55-400">À quoi correspondent ces frais?</span><span class="sxs-lookup"><span data-stu-id="a5c55-400">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a5c55-401">Comment faire correspondre ces types de frais ChargeType sur la facture?</span><span class="sxs-lookup"><span data-stu-id="a5c55-401">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="a5c55-402">Frais récurrents</span><span class="sxs-lookup"><span data-stu-id="a5c55-402">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a5c55-403">Annuler l'instance au prorata</span><span class="sxs-lookup"><span data-stu-id="a5c55-403">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-404">Les frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="a5c55-404">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="a5c55-405">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-405">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-406">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="a5c55-406">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-407">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-407">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-408">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="a5c55-408">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-409">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="a5c55-409">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-410">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="a5c55-410">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-411">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="a5c55-411">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-412">Frais au prorata en cas d’achat</span><span class="sxs-lookup"><span data-stu-id="a5c55-412">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-413">Frais au prorata lors de l’achat</span><span class="sxs-lookup"><span data-stu-id="a5c55-413">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-414">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-414">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-415">Frais initiaux de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-415">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-416">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="a5c55-416">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-417">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-417">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-418">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="a5c55-418">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-419">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-419">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a5c55-420">Autres produits et services</span><span class="sxs-lookup"><span data-stu-id="a5c55-420">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a5c55-421">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="a5c55-421">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-422">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="a5c55-422">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-423">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-423">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="a5c55-424">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="a5c55-424">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a5c55-425">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="a5c55-425">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-426">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="a5c55-426">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="a5c55-427">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-427">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-428">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="a5c55-428">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-429">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="a5c55-429">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a5c55-430">Crédits &amp; ajustements</span><span class="sxs-lookup"><span data-stu-id="a5c55-430">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a5c55-431">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="a5c55-431">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-432">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="a5c55-432">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-433">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-433">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="a5c55-434">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-434">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="a5c55-435">Autres remises</span><span class="sxs-lookup"><span data-stu-id="a5c55-435">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="a5c55-436">(basées sur l’utilisation)</span><span class="sxs-lookup"><span data-stu-id="a5c55-436">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="a5c55-437">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="a5c55-437">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-438">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-438">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="a5c55-439">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-439">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-440">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="a5c55-440">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-441">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="a5c55-441">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="a5c55-442">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="a5c55-442">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-443">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a5c55-443">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="a5c55-444">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="a5c55-444">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-445">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="a5c55-445">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a5c55-446">Autres remises</span><span class="sxs-lookup"><span data-stu-id="a5c55-446">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="a5c55-447">(basées sur une licence)</span><span class="sxs-lookup"><span data-stu-id="a5c55-447">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="a5c55-448">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="a5c55-448">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="a5c55-449">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-449">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a5c55-450"><strong></strong>&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-450"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="a5c55-451">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="a5c55-451">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="a5c55-452">Exception: les taxes sont déjà incluses dans «Décalage d'un élément de la ligne».</span><span class="sxs-lookup"><span data-stu-id="a5c55-452">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="a5c55-453">Consultez les crédits &amp;ajustements ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="a5c55-453">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="a5c55-454">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="a5c55-454">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="a5c55-455">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-455">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="a5c55-456">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="a5c55-456">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
