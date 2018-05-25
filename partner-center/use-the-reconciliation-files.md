---
title: Utiliser les fichiers de rapprochement | Espace partenaires
description: Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892138374f5730bdc10bdf07f75d0a8e3ef56bea
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/10/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="e3e06-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="e3e06-103">Use the reconciliation files</span></span>

**<span data-ttu-id="e3e06-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="e3e06-104">Applies to</span></span>**

-  <span data-ttu-id="e3e06-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e3e06-105">Partner Center</span></span>
-  <span data-ttu-id="e3e06-106">Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis</span><span class="sxs-lookup"><span data-stu-id="e3e06-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="e3e06-107">Espace partenaires de Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="e3e06-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="e3e06-108">Pour une vue détaillée de chaque élément facturé dans un cycle de facturation, téléchargez les fichiers de rapprochement à partir du tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="e3e06-109">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="e3e06-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="e3e06-110">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="e3e06-110">Itemize by partner</span></span>


<span data-ttu-id="e3e06-111">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="e3e06-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="e3e06-112">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="e3e06-112">MPN ID</span></span></th>
<th><span data-ttu-id="e3e06-113">Description</span><span class="sxs-lookup"><span data-stu-id="e3e06-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="e3e06-114">ID MPN</span><span class="sxs-lookup"><span data-stu-id="e3e06-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="e3e06-115">L’ID MicrosoftPartner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="e3e06-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-116">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="e3e06-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="e3e06-117">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="e3e06-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="e3e06-118">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e3e06-119">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="e3e06-120">Pour afficher ou mettre à jour le revendeur, dans le menu Espace partenaires, sélectionnez <strong>Clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="e3e06-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="e3e06-121">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="e3e06-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="e3e06-122">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="e3e06-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="e3e06-123">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="e3e06-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="e3e06-124">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="e3e06-125">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="e3e06-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="e3e06-126">Champs des fichiers basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="e3e06-126">License-based file fields</span></span>


<span data-ttu-id="e3e06-127">Pour rapprocher vos frais des commandes des clients, comparez le numéro d’abonnement du partenaire de syndication dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e3e06-128">Colonne</span><span class="sxs-lookup"><span data-stu-id="e3e06-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e3e06-129">Description</span><span class="sxs-lookup"><span data-stu-id="e3e06-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e3e06-130">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="e3e06-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e3e06-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="e3e06-132">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e3e06-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="e3e06-133">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="e3e06-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="e3e06-134">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="e3e06-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="e3e06-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="e3e06-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e3e06-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="e3e06-137">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e3e06-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="e3e06-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="e3e06-139">OrderID</span></span></td>
<td><p><span data-ttu-id="e3e06-140">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3e06-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e3e06-141">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e3e06-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e3e06-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e3e06-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e3e06-144">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3e06-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e3e06-145">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e3e06-146">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="e3e06-147">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="e3e06-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="e3e06-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e3e06-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-149">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="e3e06-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="e3e06-150">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="e3e06-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="e3e06-151">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="e3e06-152">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e3e06-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="e3e06-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="e3e06-154">OfferID</span></span></td>
<td><p><span data-ttu-id="e3e06-155">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="e3e06-155">Unique offer ID.</span></span> <span data-ttu-id="e3e06-156">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="e3e06-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="e3e06-157"><b>Remarque</b>: cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="e3e06-158">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e3e06-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="e3e06-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="e3e06-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="e3e06-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="e3e06-161">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e3e06-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="e3e06-162"><b>Remarque</b>: cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="e3e06-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="e3e06-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="e3e06-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="e3e06-164">OfferName</span></span></td>
<td><p><span data-ttu-id="e3e06-165">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e3e06-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="e3e06-166">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="e3e06-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="e3e06-168">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="e3e06-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="e3e06-169">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="e3e06-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="e3e06-170">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e3e06-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e3e06-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e3e06-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="e3e06-173">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="e3e06-174">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="e3e06-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="e3e06-175">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="e3e06-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="e3e06-176">L’heure indique toujours le début de la journée (0:00).</span><span class="sxs-lookup"><span data-stu-id="e3e06-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e3e06-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e3e06-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e3e06-179">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="e3e06-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="e3e06-180">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="e3e06-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e3e06-181">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e3e06-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e3e06-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="e3e06-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e3e06-184">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="e3e06-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="e3e06-185">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="e3e06-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="e3e06-186">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e3e06-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e3e06-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="e3e06-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e3e06-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="e3e06-189">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-189">The type of charge or adjustment.</span></span> <span data-ttu-id="e3e06-190">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e3e06-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e3e06-191">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e3e06-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e3e06-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="e3e06-193">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="e3e06-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="e3e06-194">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e3e06-195">6.82</span><span class="sxs-lookup"><span data-stu-id="e3e06-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-196">Quantité</span><span class="sxs-lookup"><span data-stu-id="e3e06-196">Quantity</span></span></td>
<td><p><span data-ttu-id="e3e06-197">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="e3e06-197">Number of seats.</span></span> <span data-ttu-id="e3e06-198">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="e3e06-199">2</span><span class="sxs-lookup"><span data-stu-id="e3e06-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-200">Montant</span><span class="sxs-lookup"><span data-stu-id="e3e06-200">Amount</span></span></td>
<td><p><span data-ttu-id="e3e06-201">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="e3e06-201">Total of price for quantity.</span></span> <span data-ttu-id="e3e06-202">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="e3e06-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="e3e06-203">13.32</span><span class="sxs-lookup"><span data-stu-id="e3e06-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="e3e06-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="e3e06-205">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="e3e06-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="e3e06-206">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="e3e06-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="e3e06-207">2.32</span><span class="sxs-lookup"><span data-stu-id="e3e06-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-208">Sous-total</span><span class="sxs-lookup"><span data-stu-id="e3e06-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="e3e06-209">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="e3e06-209">Total before tax.</span></span> <span data-ttu-id="e3e06-210">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="e3e06-211">11</span><span class="sxs-lookup"><span data-stu-id="e3e06-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-212">Taxe</span><span class="sxs-lookup"><span data-stu-id="e3e06-212">Tax</span></span></td>
<td><p><span data-ttu-id="e3e06-213">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="e3e06-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e3e06-214">0</span><span class="sxs-lookup"><span data-stu-id="e3e06-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="e3e06-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="e3e06-216">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="e3e06-216">Total after tax.</span></span> <span data-ttu-id="e3e06-217">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="e3e06-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="e3e06-218">11</span><span class="sxs-lookup"><span data-stu-id="e3e06-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-219">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="e3e06-219">Currency</span></span></td>
<td><p><span data-ttu-id="e3e06-220">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-220">Currency type.</span></span> <span data-ttu-id="e3e06-221">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="e3e06-222">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e3e06-223">EUR</span><span class="sxs-lookup"><span data-stu-id="e3e06-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e3e06-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="e3e06-225">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e3e06-226">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e3e06-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e3e06-227">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="e3e06-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="e3e06-228">MPNID</span></span></td>
<td><p><span data-ttu-id="e3e06-229">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="e3e06-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="e3e06-230">4390934</span><span class="sxs-lookup"><span data-stu-id="e3e06-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e3e06-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e3e06-232">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e3e06-233">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="e3e06-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e3e06-234">4390934</span><span class="sxs-lookup"><span data-stu-id="e3e06-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="e3e06-235">DomainName</span></span></td>
<td><p><span data-ttu-id="e3e06-236">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="e3e06-237">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e3e06-238">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e3e06-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e3e06-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e3e06-240">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-240">Subscription nickname.</span></span> <span data-ttu-id="e3e06-241">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="e3e06-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="e3e06-242">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="e3e06-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e3e06-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e3e06-244">Le nom de l’offre de service achetée par le client, telle que définie dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="e3e06-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="e3e06-245">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="e3e06-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="e3e06-246">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="e3e06-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="e3e06-247">Champs des fichiers basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="e3e06-247">Usage-based file fields</span></span>


<span data-ttu-id="e3e06-248">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="e3e06-249">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="e3e06-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="e3e06-250">Colonne</span><span class="sxs-lookup"><span data-stu-id="e3e06-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="e3e06-251">Description</span><span class="sxs-lookup"><span data-stu-id="e3e06-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="e3e06-252">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="e3e06-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="e3e06-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="e3e06-254">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e3e06-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="e3e06-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e3e06-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="e3e06-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="e3e06-257">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="e3e06-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="e3e06-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="e3e06-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="e3e06-260">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="e3e06-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="e3e06-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e3e06-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="e3e06-263">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e3e06-264">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e3e06-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="e3e06-265">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="e3e06-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="e3e06-266">MPNID</span></span></td>
<td><p><span data-ttu-id="e3e06-267">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="e3e06-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="e3e06-268">4390934</span><span class="sxs-lookup"><span data-stu-id="e3e06-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="e3e06-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="e3e06-270">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="e3e06-271">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="e3e06-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="e3e06-272">4390934</span><span class="sxs-lookup"><span data-stu-id="e3e06-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e3e06-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="e3e06-274">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="e3e06-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="e3e06-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="e3e06-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="e3e06-277">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e3e06-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e3e06-278">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="e3e06-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="e3e06-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e3e06-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="e3e06-281">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="e3e06-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="e3e06-282">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="e3e06-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="e3e06-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="e3e06-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="e3e06-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="e3e06-285">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3e06-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="e3e06-286">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="e3e06-287">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="e3e06-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="e3e06-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="e3e06-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="e3e06-290">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="e3e06-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="e3e06-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e3e06-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="e3e06-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="e3e06-293">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="e3e06-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="e3e06-294">Microsoft&nbsp;Azure</span><span class="sxs-lookup"><span data-stu-id="e3e06-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-295">OrderId</span><span class="sxs-lookup"><span data-stu-id="e3e06-295">OrderID</span></span></td>
<td><p><span data-ttu-id="e3e06-296">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3e06-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e3e06-297">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="e3e06-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="e3e06-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="e3e06-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="e3e06-300">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="e3e06-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="e3e06-301">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="e3e06-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="e3e06-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="e3e06-303">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="e3e06-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e3e06-304">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="e3e06-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="e3e06-305">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="e3e06-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="e3e06-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="e3e06-307">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="e3e06-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="e3e06-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="e3e06-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-309">Nom de la ressource</span><span class="sxs-lookup"><span data-stu-id="e3e06-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="e3e06-310">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="e3e06-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="e3e06-311">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="e3e06-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="e3e06-312">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="e3e06-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-313">Région</span><span class="sxs-lookup"><span data-stu-id="e3e06-313">Region</span></span></td>
<td><p><span data-ttu-id="e3e06-314">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-314">The region the usage applies to.</span></span> <span data-ttu-id="e3e06-315">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="e3e06-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="e3e06-316">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="e3e06-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-317">SKU</span><span class="sxs-lookup"><span data-stu-id="e3e06-317">SKU</span></span></td>
<td><p><span data-ttu-id="e3e06-318">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="e3e06-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="e3e06-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="e3e06-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="e3e06-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="e3e06-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="e3e06-321">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="e3e06-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="e3e06-322">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="e3e06-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="e3e06-323">1</span><span class="sxs-lookup"><span data-stu-id="e3e06-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="e3e06-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="e3e06-325">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="e3e06-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="e3e06-326">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="e3e06-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="e3e06-327">11</span><span class="sxs-lookup"><span data-stu-id="e3e06-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="e3e06-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="e3e06-329">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="e3e06-329">Units included as part of the offer.</span></span> <span data-ttu-id="e3e06-330">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="e3e06-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="e3e06-331">0</span><span class="sxs-lookup"><span data-stu-id="e3e06-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="e3e06-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="e3e06-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="e3e06-333">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="e3e06-334">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="e3e06-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="e3e06-335">11</span><span class="sxs-lookup"><span data-stu-id="e3e06-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="e3e06-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="e3e06-337">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="e3e06-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="e3e06-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="e3e06-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="e3e06-340">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e3e06-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e3e06-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="e3e06-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="e3e06-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="e3e06-343">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="e3e06-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="e3e06-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="e3e06-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="e3e06-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="e3e06-346">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="e3e06-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="e3e06-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="e3e06-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-348">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="e3e06-348">Currency</span></span></td>
<td><p><span data-ttu-id="e3e06-349">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-349">Currency type.</span></span> <span data-ttu-id="e3e06-350">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="e3e06-351">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="e3e06-352">EUR</span><span class="sxs-lookup"><span data-stu-id="e3e06-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e3e06-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e3e06-354">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="e3e06-354">Pretax price per unit.</span></span> <span data-ttu-id="e3e06-355">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e3e06-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e3e06-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="e3e06-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="e3e06-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="e3e06-358">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="e3e06-358">Post tax price per unit.</span></span> <span data-ttu-id="e3e06-359">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="e3e06-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="e3e06-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="e3e06-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e3e06-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="e3e06-362">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-362">The type of charge or adjustment.</span></span> <span data-ttu-id="e3e06-363">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e3e06-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="e3e06-364">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="e3e06-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="e3e06-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="e3e06-366">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="e3e06-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="e3e06-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="e3e06-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="e3e06-369">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="e3e06-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="e3e06-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="e3e06-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="e3e06-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="e3e06-372">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="e3e06-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="e3e06-373">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="e3e06-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="e3e06-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="e3e06-375">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="e3e06-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="e3e06-376">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="e3e06-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="e3e06-377">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="e3e06-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="e3e06-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="e3e06-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="e3e06-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="e3e06-380">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="e3e06-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="e3e06-381">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="e3e06-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-382">Projet</span><span class="sxs-lookup"><span data-stu-id="e3e06-382">Project</span></span></td>
<td><p><span data-ttu-id="e3e06-383">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="e3e06-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="e3e06-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e3e06-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="e3e06-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="e3e06-386">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="e3e06-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="e3e06-387">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="e3e06-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="e3e06-388">Si vous avez un pack de 25 connexions ServiceBus et que vous en avez utilisé 1 ce jour-là, votre relevé d’utilisation quotidienne indiquera « 25 connexions/30 jours - Utilisées : 1 ».</span><span class="sxs-lookup"><span data-stu-id="e3e06-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="e3e06-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="e3e06-390">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="e3e06-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="e3e06-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="e3e06-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="e3e06-392">DomainName</span></span></td>
<td><p><span data-ttu-id="e3e06-393">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="e3e06-394">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="e3e06-395">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e3e06-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="e3e06-396">Unit</span><span class="sxs-lookup"><span data-stu-id="e3e06-396">Unit</span></span></td>
<td><p><span data-ttu-id="e3e06-397">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="e3e06-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="e3e06-398">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="e3e06-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="e3e06-399">Champs du fichier d’achat ponctuel</span><span class="sxs-lookup"><span data-stu-id="e3e06-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="e3e06-400">Champ</span><span class="sxs-lookup"><span data-stu-id="e3e06-400">Field</span></span>** |**<span data-ttu-id="e3e06-401">Définition</span><span class="sxs-lookup"><span data-stu-id="e3e06-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="e3e06-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="e3e06-402">PartnerId</span></span> |<span data-ttu-id="e3e06-403">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="e3e06-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="e3e06-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="e3e06-404">CustomerId</span></span> |<span data-ttu-id="e3e06-405">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="e3e06-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="e3e06-406">CustomerName</span></span> |<span data-ttu-id="e3e06-407">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="e3e06-408">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="e3e06-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="e3e06-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="e3e06-409">CustomerDomainName</span></span> |<span data-ttu-id="e3e06-410">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="e3e06-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="e3e06-411">CustomerCountry</span></span> |<span data-ttu-id="e3e06-412">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="e3e06-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="e3e06-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="e3e06-413">InvoiceNumber</span></span> |<span data-ttu-id="e3e06-414">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="e3e06-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="e3e06-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="e3e06-415">MpnId</span></span> |<span data-ttu-id="e3e06-416">L'identifiant MPN du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="e3e06-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="e3e06-417">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="e3e06-417">Reseller MPN ID</span></span> |<span data-ttu-id="e3e06-418">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="e3e06-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="e3e06-419">IDMPN du revendeur de référence pour la réservation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="e3e06-420">Cet ID correspond à l’ID de revendeur indiqué pour la réservation dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e3e06-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="e3e06-421">Si un partenaire fournisseur de solutions Cloud a vendu la réservation directement au client, son ID MPN est indiqué deux fois, en tant qu’ID MPN et ID MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="e3e06-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="e3e06-422">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="e3e06-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="e3e06-423">Si le partenaire fournisseur de solutions Cloud supprime un D revendeur, cette valeur est définie sur -1.</span><span class="sxs-lookup"><span data-stu-id="e3e06-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="e3e06-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="e3e06-424">OrderId</span></span> |<span data-ttu-id="e3e06-425">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e3e06-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="e3e06-426">Peut être utile pour identifier la réservation Azure lors de tout contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="e3e06-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="e3e06-427">OrderDate</span></span> |<span data-ttu-id="e3e06-428">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="e3e06-428">The date the order was placed.</span></span> |
|<span data-ttu-id="e3e06-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="e3e06-429">ProductId</span></span> |<span data-ttu-id="e3e06-430">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="e3e06-430">The ID for the product.</span></span> |
|<span data-ttu-id="e3e06-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="e3e06-431">SkuId</span></span>  |<span data-ttu-id="e3e06-432">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="e3e06-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="e3e06-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="e3e06-433">AvailabilityId</span></span> |<span data-ttu-id="e3e06-434">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="e3e06-434">The ID for a particular Availability.</span></span> <span data-ttu-id="e3e06-435">La «Disponibilité» indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="e3e06-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="e3e06-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="e3e06-436">SkuName</span></span>  |<span data-ttu-id="e3e06-437">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="e3e06-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="e3e06-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="e3e06-438">ProductName</span></span> |<span data-ttu-id="e3e06-439">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="e3e06-439">The name of the product.</span></span> |
|<span data-ttu-id="e3e06-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="e3e06-440">ChargeType</span></span> |<span data-ttu-id="e3e06-441">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="e3e06-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="e3e06-442">UnitPrice</span></span> |<span data-ttu-id="e3e06-443">Prix par produit commandé.</span><span class="sxs-lookup"><span data-stu-id="e3e06-443">Price per product ordered.</span></span> |
|<span data-ttu-id="e3e06-444">Quantité</span><span class="sxs-lookup"><span data-stu-id="e3e06-444">Quantity</span></span> |<span data-ttu-id="e3e06-445">Nombre de produits commandés.</span><span class="sxs-lookup"><span data-stu-id="e3e06-445">Number of products ordered.</span></span> |
|<span data-ttu-id="e3e06-446">Sous-total</span><span class="sxs-lookup"><span data-stu-id="e3e06-446">Subtotal</span></span> |<span data-ttu-id="e3e06-447">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="e3e06-447">Total before tax.</span></span> <span data-ttu-id="e3e06-448">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="e3e06-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="e3e06-449">TaxTotal</span></span> |<span data-ttu-id="e3e06-450">La somme totale de toutes les taxes applicables.</span><span class="sxs-lookup"><span data-stu-id="e3e06-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="e3e06-451">Total</span><span class="sxs-lookup"><span data-stu-id="e3e06-451">Total</span></span> |<span data-ttu-id="e3e06-452">Le montant total de cet achat.</span><span class="sxs-lookup"><span data-stu-id="e3e06-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="e3e06-453">Devise</span><span class="sxs-lookup"><span data-stu-id="e3e06-453">Currency</span></span> |<span data-ttu-id="e3e06-454">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-454">Currency type.</span></span> <span data-ttu-id="e3e06-455">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="e3e06-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="e3e06-456">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="e3e06-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="e3e06-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="e3e06-457">DiscountDetails</span></span> |<span data-ttu-id="e3e06-458">Liste détaillée des remises éventuelles pertinentes.</span><span class="sxs-lookup"><span data-stu-id="e3e06-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="e3e06-459">Mise en correspondance des frais entre une facture et le fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="e3e06-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="e3e06-460">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="e3e06-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="e3e06-461">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de MicrosoftExcel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="e3e06-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="e3e06-462">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="e3e06-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="e3e06-463">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’«ajustements» ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="e3e06-464">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e3e06-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="e3e06-465">Description des frais indiqués sur les factures</span><span class="sxs-lookup"><span data-stu-id="e3e06-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e3e06-466">Description des frais figurant sur le fichier de rapprochement (colonne ChargeType)</span><span class="sxs-lookup"><span data-stu-id="e3e06-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e3e06-467">À quoi correspondent ces frais?</span><span class="sxs-lookup"><span data-stu-id="e3e06-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="e3e06-468">Comment faire correspondre ces types de frais ChargeType sur la facture?</span><span class="sxs-lookup"><span data-stu-id="e3e06-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="e3e06-469">Frais récurrents</span><span class="sxs-lookup"><span data-stu-id="e3e06-469">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e3e06-470">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="e3e06-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-471">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="e3e06-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="e3e06-472">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-473">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="e3e06-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-474">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="e3e06-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-475">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="e3e06-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-476">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-477">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="e3e06-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-478">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="e3e06-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-479">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="e3e06-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-480">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="e3e06-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-481">Frais au prorata en cas d’achat</span><span class="sxs-lookup"><span data-stu-id="e3e06-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-482">Frais au prorata lors de l’achat</span><span class="sxs-lookup"><span data-stu-id="e3e06-482">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-483">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-484">Frais initiaux de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-484">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-485">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="e3e06-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-486">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-487">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="e3e06-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-488">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e3e06-489">Autres produits et services</span><span class="sxs-lookup"><span data-stu-id="e3e06-489">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e3e06-490">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="e3e06-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-491">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="e3e06-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-492">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-492">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="e3e06-493">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="e3e06-493">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e3e06-494">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="e3e06-494">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-495">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="e3e06-495">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="e3e06-496">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-496">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-497">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="e3e06-497">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-498">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="e3e06-498">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e3e06-499">Crédits &amp; ajustements</span><span class="sxs-lookup"><span data-stu-id="e3e06-499">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="e3e06-500">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="e3e06-500">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-501">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="e3e06-501">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-502">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-502">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="e3e06-503">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-503">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="e3e06-504">Autres remises</span><span class="sxs-lookup"><span data-stu-id="e3e06-504">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="e3e06-505">(basées sur l’utilisation)</span><span class="sxs-lookup"><span data-stu-id="e3e06-505">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="e3e06-506">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="e3e06-506">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-507">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-507">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="e3e06-508">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-508">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-509">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="e3e06-509">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-510">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="e3e06-510">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e3e06-511">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="e3e06-511">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-512">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="e3e06-512">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="e3e06-513">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="e3e06-513">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-514">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="e3e06-514">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="e3e06-515">Autres remises</span><span class="sxs-lookup"><span data-stu-id="e3e06-515">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="e3e06-516">(basées sur une licence)</span><span class="sxs-lookup"><span data-stu-id="e3e06-516">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="e3e06-517">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="e3e06-517">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="e3e06-518">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-518">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="e3e06-519"><strong></strong>&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-519"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="e3e06-520">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="e3e06-520">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="e3e06-521">Exception: les taxes sont déjà incluses dans «Décalage d'un élément de la ligne».</span><span class="sxs-lookup"><span data-stu-id="e3e06-521">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="e3e06-522">Consultez les crédits &amp;ajustements ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="e3e06-522">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="e3e06-523">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="e3e06-523">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="e3e06-524">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-524">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="e3e06-525">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="e3e06-525">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
