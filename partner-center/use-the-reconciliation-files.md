---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Pour une vue détaillée de l’article de chacun des frais dans un cycle de facturation, télécharger les fichiers de rapprochement à partir de l’espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122276"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="6f0bd-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-103">Use the reconciliation files</span></span>

**<span data-ttu-id="6f0bd-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="6f0bd-104">Applies to</span></span>**

-  <span data-ttu-id="6f0bd-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6f0bd-105">Partner Center</span></span>
-  <span data-ttu-id="6f0bd-106">Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis</span><span class="sxs-lookup"><span data-stu-id="6f0bd-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="6f0bd-107">Pour une vue détaillée de l’article de chacun des frais dans un cycle de facturation, télécharger les fichiers de rapprochement à partir de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="6f0bd-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="6f0bd-109">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="6f0bd-109">Itemize by partner</span></span>


<span data-ttu-id="6f0bd-110">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="6f0bd-111">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="6f0bd-111">MPN ID</span></span></th>
<th><span data-ttu-id="6f0bd-112">Description</span><span class="sxs-lookup"><span data-stu-id="6f0bd-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="6f0bd-113">ID MPN</span><span class="sxs-lookup"><span data-stu-id="6f0bd-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="6f0bd-114">L’ID MicrosoftPartner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-115">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="6f0bd-116">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="6f0bd-117">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6f0bd-118">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="6f0bd-119">Pour afficher ou mettre à jour le revendeur, dans le menu espace partenaires, sélectionnez les <strong>clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="6f0bd-120">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="6f0bd-121">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="6f0bd-122">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="6f0bd-123">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="6f0bd-124">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="6f0bd-125">Champs des fichiers basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="6f0bd-125">License-based file fields</span></span>


<span data-ttu-id="6f0bd-126">Pour rapprocher vos frais des commandes des clients, comparez le numéro d’abonnement du partenaire de syndication dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="6f0bd-127">Colonne</span><span class="sxs-lookup"><span data-stu-id="6f0bd-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="6f0bd-128">Description</span><span class="sxs-lookup"><span data-stu-id="6f0bd-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="6f0bd-129">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="6f0bd-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="6f0bd-131">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="6f0bd-132">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="6f0bd-133">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="6f0bd-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="6f0bd-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="6f0bd-136">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="6f0bd-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="6f0bd-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-138">OrderID</span></span></td>
<td><p><span data-ttu-id="6f0bd-139">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="6f0bd-140">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="6f0bd-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="6f0bd-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="6f0bd-143">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="6f0bd-144">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="6f0bd-145">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="6f0bd-146">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="6f0bd-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="6f0bd-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-148">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="6f0bd-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="6f0bd-149">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="6f0bd-150">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="6f0bd-151">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="6f0bd-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="6f0bd-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-153">OfferID</span></span></td>
<td><p><span data-ttu-id="6f0bd-154">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-154">Unique offer ID.</span></span> <span data-ttu-id="6f0bd-155">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="6f0bd-156"><b>Remarque</b>: cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="6f0bd-157">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="6f0bd-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="6f0bd-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="6f0bd-160">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="6f0bd-161"><b>Remarque</b>: cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="6f0bd-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="6f0bd-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-163">OfferName</span></span></td>
<td><p><span data-ttu-id="6f0bd-164">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="6f0bd-165">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-167">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="6f0bd-168">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="6f0bd-169">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6f0bd-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6f0bd-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-172">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="6f0bd-173">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="6f0bd-174">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="6f0bd-175">L’heure indique toujours le début de la journée (0:00).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6f0bd-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6f0bd-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-178">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="6f0bd-179">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="6f0bd-180">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6f0bd-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="6f0bd-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-183">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="6f0bd-184">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="6f0bd-185">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="6f0bd-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="6f0bd-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="6f0bd-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="6f0bd-188">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-188">The type of charge or adjustment.</span></span> <span data-ttu-id="6f0bd-189">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6f0bd-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="6f0bd-190">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6f0bd-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="6f0bd-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="6f0bd-192">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="6f0bd-193">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="6f0bd-194">6.82</span><span class="sxs-lookup"><span data-stu-id="6f0bd-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-195">Quantité</span><span class="sxs-lookup"><span data-stu-id="6f0bd-195">Quantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-196">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-196">Number of seats.</span></span> <span data-ttu-id="6f0bd-197">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="6f0bd-198">2</span><span class="sxs-lookup"><span data-stu-id="6f0bd-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-199">Montant</span><span class="sxs-lookup"><span data-stu-id="6f0bd-199">Amount</span></span></td>
<td><p><span data-ttu-id="6f0bd-200">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-200">Total of price for quantity.</span></span> <span data-ttu-id="6f0bd-201">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="6f0bd-202">13.32</span><span class="sxs-lookup"><span data-stu-id="6f0bd-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="6f0bd-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="6f0bd-204">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="6f0bd-205">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="6f0bd-206">2.32</span><span class="sxs-lookup"><span data-stu-id="6f0bd-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-207">Sous-total</span><span class="sxs-lookup"><span data-stu-id="6f0bd-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="6f0bd-208">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-208">Total before tax.</span></span> <span data-ttu-id="6f0bd-209">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="6f0bd-210">11</span><span class="sxs-lookup"><span data-stu-id="6f0bd-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-211">Taxe</span><span class="sxs-lookup"><span data-stu-id="6f0bd-211">Tax</span></span></td>
<td><p><span data-ttu-id="6f0bd-212">Taxe sur les frais de quantité, selon votre market& #39; les règles de taxe s et les circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="6f0bd-213">0</span><span class="sxs-lookup"><span data-stu-id="6f0bd-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="6f0bd-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="6f0bd-215">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-215">Total after tax.</span></span> <span data-ttu-id="6f0bd-216">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="6f0bd-217">11</span><span class="sxs-lookup"><span data-stu-id="6f0bd-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-218">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="6f0bd-218">Currency</span></span></td>
<td><p><span data-ttu-id="6f0bd-219">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-219">Currency type.</span></span> <span data-ttu-id="6f0bd-220">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="6f0bd-221">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="6f0bd-222">EUR</span><span class="sxs-lookup"><span data-stu-id="6f0bd-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="6f0bd-224">Customer& #39; nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="6f0bd-225">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="6f0bd-226">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="6f0bd-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-227">MPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-228">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="6f0bd-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="6f0bd-229">4390934</span><span class="sxs-lookup"><span data-stu-id="6f0bd-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-231">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6f0bd-232">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="6f0bd-233">4390934</span><span class="sxs-lookup"><span data-stu-id="6f0bd-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-234">DomainName</span></span></td>
<td><p><span data-ttu-id="6f0bd-235">Customer& #39; nom de domaine s, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="6f0bd-236">Cela ne doit pas être utilisée pour identifier de manière unique le client que le client/partenaire peut mettre à jour le domaine de redirection vers un microsite/par défaut via le portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="6f0bd-237">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="6f0bd-238">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6f0bd-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="6f0bd-240">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-240">Subscription nickname.</span></span> <span data-ttu-id="6f0bd-241">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="6f0bd-242">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="6f0bd-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="6f0bd-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="6f0bd-244">Le nom de l’offre de service achetée par le client, telle que définie dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="6f0bd-245">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="6f0bd-246">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="6f0bd-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="6f0bd-247">Champs des fichiers basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-247">Usage-based file fields</span></span>


<span data-ttu-id="6f0bd-248">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="6f0bd-249">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="6f0bd-250">Colonne</span><span class="sxs-lookup"><span data-stu-id="6f0bd-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="6f0bd-251">Description</span><span class="sxs-lookup"><span data-stu-id="6f0bd-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="6f0bd-252">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="6f0bd-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="6f0bd-254">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="6f0bd-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="6f0bd-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="6f0bd-257">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="6f0bd-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="6f0bd-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="6f0bd-260">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="6f0bd-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="6f0bd-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="6f0bd-263">Customer& #39; nom de l’organisation s comme indiqué dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="6f0bd-264">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="6f0bd-265">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="6f0bd-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-266">MPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-267">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="6f0bd-268">4390934</span><span class="sxs-lookup"><span data-stu-id="6f0bd-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-270">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6f0bd-271">Voir <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Détailler par partenaire</a>.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="6f0bd-272">4390934</span><span class="sxs-lookup"><span data-stu-id="6f0bd-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="6f0bd-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="6f0bd-274">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="6f0bd-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="6f0bd-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-277">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="6f0bd-278">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="6f0bd-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="6f0bd-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-281">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="6f0bd-282">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="6f0bd-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="6f0bd-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="6f0bd-285">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="6f0bd-286">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="6f0bd-287">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="6f0bd-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="6f0bd-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="6f0bd-290">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="6f0bd-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="6f0bd-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="6f0bd-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="6f0bd-293">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="6f0bd-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="6f0bd-294">Microsoft&nbsp;Azure</span><span class="sxs-lookup"><span data-stu-id="6f0bd-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-295">OrderId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-295">OrderID</span></span></td>
<td><p><span data-ttu-id="6f0bd-296">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="6f0bd-297">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="6f0bd-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="6f0bd-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="6f0bd-300">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="6f0bd-301">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="6f0bd-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="6f0bd-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="6f0bd-303">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="6f0bd-304">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="6f0bd-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="6f0bd-305">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="6f0bd-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="6f0bd-307">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="6f0bd-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="6f0bd-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-309">Nom de la ressource</span><span class="sxs-lookup"><span data-stu-id="6f0bd-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="6f0bd-310">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="6f0bd-311">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="6f0bd-312">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-313">Région</span><span class="sxs-lookup"><span data-stu-id="6f0bd-313">Region</span></span></td>
<td><p><span data-ttu-id="6f0bd-314">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-314">The region the usage applies to.</span></span> <span data-ttu-id="6f0bd-315">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="6f0bd-316">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="6f0bd-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-317">SKU</span><span class="sxs-lookup"><span data-stu-id="6f0bd-317">SKU</span></span></td>
<td><p><span data-ttu-id="6f0bd-318">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="6f0bd-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="6f0bd-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="6f0bd-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="6f0bd-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="6f0bd-321">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="6f0bd-322">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="6f0bd-323">1</span><span class="sxs-lookup"><span data-stu-id="6f0bd-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="6f0bd-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-325">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="6f0bd-326">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="6f0bd-327">11</span><span class="sxs-lookup"><span data-stu-id="6f0bd-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="6f0bd-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-329">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-329">Units included as part of the offer.</span></span> <span data-ttu-id="6f0bd-330">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="6f0bd-331">0</span><span class="sxs-lookup"><span data-stu-id="6f0bd-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="6f0bd-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="6f0bd-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="6f0bd-333">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="6f0bd-334">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="6f0bd-335">11</span><span class="sxs-lookup"><span data-stu-id="6f0bd-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="6f0bd-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="6f0bd-337">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="6f0bd-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="6f0bd-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="6f0bd-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="6f0bd-340">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6f0bd-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="6f0bd-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="6f0bd-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="6f0bd-343">Taxe sur les frais de quantité, selon votre market& #39; les règles de taxe s et les circonstances spécifiques.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="6f0bd-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="6f0bd-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="6f0bd-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="6f0bd-346">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="6f0bd-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="6f0bd-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-348">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="6f0bd-348">Currency</span></span></td>
<td><p><span data-ttu-id="6f0bd-349">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-349">Currency type.</span></span> <span data-ttu-id="6f0bd-350">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="6f0bd-351">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="6f0bd-352">EUR</span><span class="sxs-lookup"><span data-stu-id="6f0bd-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="6f0bd-354">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-354">Pretax price per unit.</span></span> <span data-ttu-id="6f0bd-355">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6f0bd-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="6f0bd-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="6f0bd-358">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-358">Post tax price per unit.</span></span> <span data-ttu-id="6f0bd-359">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="6f0bd-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="6f0bd-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="6f0bd-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="6f0bd-362">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-362">The type of charge or adjustment.</span></span> <span data-ttu-id="6f0bd-363">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6f0bd-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="6f0bd-364">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="6f0bd-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="6f0bd-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="6f0bd-366">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="6f0bd-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="6f0bd-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-369">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="6f0bd-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="6f0bd-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="6f0bd-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="6f0bd-372">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="6f0bd-373">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="6f0bd-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="6f0bd-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="6f0bd-375">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="6f0bd-376">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="6f0bd-377">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="6f0bd-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="6f0bd-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="6f0bd-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="6f0bd-380">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="6f0bd-381">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="6f0bd-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-382">Projet</span><span class="sxs-lookup"><span data-stu-id="6f0bd-382">Project</span></span></td>
<td><p><span data-ttu-id="6f0bd-383">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="6f0bd-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="6f0bd-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="6f0bd-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="6f0bd-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="6f0bd-386">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="6f0bd-387">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="6f0bd-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="6f0bd-388">Si vous avez un pack de 25 connexions ServiceBus et que vous en avez utilisé 1 ce jour-là, votre relevé d’utilisation quotidienne indiquera « 25 connexions/30 jours - Utilisées : 1 ».</span><span class="sxs-lookup"><span data-stu-id="6f0bd-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="6f0bd-390">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="6f0bd-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="6f0bd-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="6f0bd-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-392">DomainName</span></span></td>
<td><p><span data-ttu-id="6f0bd-393">Customer& #39; nom de domaine s, utilisé pour aider à identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="6f0bd-394">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="6f0bd-395">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="6f0bd-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="6f0bd-396">Unit</span><span class="sxs-lookup"><span data-stu-id="6f0bd-396">Unit</span></span></td>
<td><p><span data-ttu-id="6f0bd-397">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="6f0bd-398">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="6f0bd-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="6f0bd-399">Champs des fichiers à usage unique et périodique</span><span class="sxs-lookup"><span data-stu-id="6f0bd-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="6f0bd-400">Colonne</span><span class="sxs-lookup"><span data-stu-id="6f0bd-400">Column</span></span></th>
<th><span data-ttu-id="6f0bd-401">Description</span><span class="sxs-lookup"><span data-stu-id="6f0bd-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="6f0bd-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="6f0bd-403">Identificateur unique de client Microsoft Azure Active Directory pour une entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="6f0bd-404">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="6f0bd-405">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-406">Id de client</span><span class="sxs-lookup"><span data-stu-id="6f0bd-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="6f0bd-407">Microsoft Azure Active Directory client ID unique, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-408">Nom du client</span><span class="sxs-lookup"><span data-stu-id="6f0bd-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="6f0bd-409">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="6f0bd-411">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="6f0bd-412">Cela ne doit pas être utilisée pour identifier de manière unique le client que le client/partenaire peut mettre à jour le domaine de redirection vers un microsite/par défaut via le portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="6f0bd-413">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-414">Pays client</span><span class="sxs-lookup"><span data-stu-id="6f0bd-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="6f0bd-415">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-416">Numéro de facture</span><span class="sxs-lookup"><span data-stu-id="6f0bd-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="6f0bd-417">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-418">MpnId</span></span></td>
<td><p><span data-ttu-id="6f0bd-419">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-420">MpnId revendeur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="6f0bd-421">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-422">ID de commande</span><span class="sxs-lookup"><span data-stu-id="6f0bd-422">Order ID</span></span></td>
<td><p><span data-ttu-id="6f0bd-423">Identificateur unique pour une commande dans la plateforme Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="6f0bd-424">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-425">Date de la commande</span><span class="sxs-lookup"><span data-stu-id="6f0bd-425">Order date</span></span></td>
<td><p><span data-ttu-id="6f0bd-426">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-427">ProductId</span></span></td>
<td><p><span data-ttu-id="6f0bd-428">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-429">SkuId</span></span></td>
<td><p><span data-ttu-id="6f0bd-430">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="6f0bd-432">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-432">The ID for a particular Availability.</span></span> <span data-ttu-id="6f0bd-433">La «Disponibilité» indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-434">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="6f0bd-435">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-436">Nom du produit</span><span class="sxs-lookup"><span data-stu-id="6f0bd-436">Product name</span></span></td>
<td><p><span data-ttu-id="6f0bd-437">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-438">Nom de l’éditeur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="6f0bd-439">Le nom de l’Éditeur du produit.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="6f0bd-441">ID unique pour cet éditeur.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-442">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="6f0bd-443">Nom convivial de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-444">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="6f0bd-445">Identificateur unique pour un abonnement dans la plateforme Microsoft commerce.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="6f0bd-446">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="6f0bd-447">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-449">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-449">Start day of the charges.</span></span> <span data-ttu-id="6f0bd-450">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-452">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-452">End day of the charges.</span></span> <span data-ttu-id="6f0bd-453">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-454">Terme et Billingcycle</span><span class="sxs-lookup"><span data-stu-id="6f0bd-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="6f0bd-455">La durée et le cycle de facturation de l’achat.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="6f0bd-456">Par exemple, «1 an, chaque mois.»</span><span class="sxs-lookup"><span data-stu-id="6f0bd-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-457">Type de facturation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="6f0bd-458">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-459">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="6f0bd-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="6f0bd-460">Le prix tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="6f0bd-461">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-462">Prix unitaire effectifs</span><span class="sxs-lookup"><span data-stu-id="6f0bd-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="6f0bd-463">Le prix unitaire une fois les ajustements.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-464">Quantité</span><span class="sxs-lookup"><span data-stu-id="6f0bd-464">Quantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-465">Nombre d’unités.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-465">Number of units.</span></span> <span data-ttu-id="6f0bd-466">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-467">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="6f0bd-467">Unit type</span></span></td>
<td><p><span data-ttu-id="6f0bd-468">Le type d’unité achetée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="6f0bd-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="6f0bd-470">Explication les remises applicables.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-471">Sous-total</span><span class="sxs-lookup"><span data-stu-id="6f0bd-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="6f0bd-472">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-472">Total before tax.</span></span> <span data-ttu-id="6f0bd-473">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-474">Total des taxes</span><span class="sxs-lookup"><span data-stu-id="6f0bd-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="6f0bd-475">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-476">Total</span><span class="sxs-lookup"><span data-stu-id="6f0bd-476">Total</span></span></td>
<td><p><span data-ttu-id="6f0bd-477">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-477">Total after tax.</span></span> <span data-ttu-id="6f0bd-478">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-479">Devise</span><span class="sxs-lookup"><span data-stu-id="6f0bd-479">Currency</span></span></td>
<td><p><span data-ttu-id="6f0bd-480">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-480">Currency type.</span></span> <span data-ttu-id="6f0bd-481">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="6f0bd-482">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="6f0bd-484">Un identificateur de remplacement pour un ID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="6f0bd-485">Champs des fichiers utilisation quotidienne-évalués</span><span class="sxs-lookup"><span data-stu-id="6f0bd-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="6f0bd-486">Colonne</span><span class="sxs-lookup"><span data-stu-id="6f0bd-486">Column</span></span></th>
<th><span data-ttu-id="6f0bd-487">Description</span><span class="sxs-lookup"><span data-stu-id="6f0bd-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="6f0bd-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="6f0bd-489">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="6f0bd-491">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="6f0bd-493">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="6f0bd-495">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="6f0bd-496">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="6f0bd-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="6f0bd-498">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-498">The customer’s domain name.</span></span> <span data-ttu-id="6f0bd-499">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-500">Pays client</span><span class="sxs-lookup"><span data-stu-id="6f0bd-500">Customer country</span></span></td>
<td><p><span data-ttu-id="6f0bd-501">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-502">MPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-503">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-504">Revendeur MPNID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="6f0bd-505">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="6f0bd-506">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="6f0bd-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="6f0bd-508">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="6f0bd-509">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-510">ProductId</span></span></td>
<td><p><span data-ttu-id="6f0bd-511">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-512">SkuId</span></span></td>
<td><p><span data-ttu-id="6f0bd-513">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="6f0bd-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="6f0bd-515">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-515">The ID for a particular Availability.</span></span> <span data-ttu-id="6f0bd-516">La «Disponibilité» indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-517">Nom de la référence (SKU)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="6f0bd-518">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-519">Nom de l’éditeur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="6f0bd-520">Le nom de l’éditeur.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="6f0bd-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="6f0bd-522">L’ID de l’éditeur, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="6f0bd-523">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="6f0bd-524">Description de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="6f0bd-525">Le nom de l’offre de service achetée par le client, telle que définie dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="6f0bd-526">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-527">ID d’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="6f0bd-528">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="6f0bd-529">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="6f0bd-530">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-532">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="6f0bd-533">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="6f0bd-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="6f0bd-535">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="6f0bd-536">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-537">Date d’utilisation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="6f0bd-538">Date de l’utilisation du service.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-539">Type d’indicateur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="6f0bd-540">Le type de mètres.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-541">Catégorie de compteur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="6f0bd-542">Le service de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-543">Id compteur</span><span class="sxs-lookup"><span data-stu-id="6f0bd-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="6f0bd-544">L’ID de la jauge utilisée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-545">Jauge sous-catégorie</span><span class="sxs-lookup"><span data-stu-id="6f0bd-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="6f0bd-546">Le type de service Azure qui affecte le taux.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-547">Nom de la jauge</span><span class="sxs-lookup"><span data-stu-id="6f0bd-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="6f0bd-548">L’unité de mesure relative à la jauge consommée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-549">Région de la jauge</span><span class="sxs-lookup"><span data-stu-id="6f0bd-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="6f0bd-550">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-551">Unit</span><span class="sxs-lookup"><span data-stu-id="6f0bd-551">Unit</span></span></td>
<td><p><span data-ttu-id="6f0bd-552">Unité de la ressource nom.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-553">Quantité consommée</span><span class="sxs-lookup"><span data-stu-id="6f0bd-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-554">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="6f0bd-555">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-556">Emplacement de la ressource</span><span class="sxs-lookup"><span data-stu-id="6f0bd-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="6f0bd-557">Le centre de données dans laquelle la jauge est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-558">Service consommé</span><span class="sxs-lookup"><span data-stu-id="6f0bd-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="6f0bd-559">Le service de plateforme Azure que vous avez utilisé.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-560">Groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="6f0bd-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="6f0bd-561">Le groupe de ressources dans lequel la jauge déployée est en cours d’exécution.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-562">URI de ressource</span><span class="sxs-lookup"><span data-stu-id="6f0bd-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="6f0bd-563">L’URI de la ressource utilisée.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-564">Type de frais</span><span class="sxs-lookup"><span data-stu-id="6f0bd-564">Charge type</span></span></td>
<td><p><span data-ttu-id="6f0bd-565">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-565">The type of charge or adjustment.</span></span> <span data-ttu-id="6f0bd-566">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-567">Prix unitaire</span><span class="sxs-lookup"><span data-stu-id="6f0bd-567">Unit price</span></span></td>
<td><p><span data-ttu-id="6f0bd-568">Prix par licence, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="6f0bd-569">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-570">Quantité</span><span class="sxs-lookup"><span data-stu-id="6f0bd-570">Quantity</span></span></td>
<td><p><span data-ttu-id="6f0bd-571">Nombre de licences.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-571">Number of licenses.</span></span> <span data-ttu-id="6f0bd-572">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-573">Type d’unité</span><span class="sxs-lookup"><span data-stu-id="6f0bd-573">Unit type</span></span></td>
<td><p><span data-ttu-id="6f0bd-574">Le type d’unité la jauge est facturé dans.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="6f0bd-575">Non disponible pour l’activité en cours.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-576">Facturation avant impôts</span><span class="sxs-lookup"><span data-stu-id="6f0bd-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="6f0bd-577">Montant total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-578">Devise de facturation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="6f0bd-579">La devise dans une région géographique du client</span><span class="sxs-lookup"><span data-stu-id="6f0bd-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-580">Prix total avant impôt</span><span class="sxs-lookup"><span data-stu-id="6f0bd-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="6f0bd-581">La tarification avant les taxes sont ajoutées.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-582">Devise de tarification</span><span class="sxs-lookup"><span data-stu-id="6f0bd-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="6f0bd-583">La devise dans la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-584">Service Info 1</span><span class="sxs-lookup"><span data-stu-id="6f0bd-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="6f0bd-585">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-586">Informations relatives au service 2</span><span class="sxs-lookup"><span data-stu-id="6f0bd-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="6f0bd-587">Un champ hérité qui capture les métadonnées spécifiques au service facultatives.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="6f0bd-588">étiquettes</span><span class="sxs-lookup"><span data-stu-id="6f0bd-588">Tags</span></span></td>
<td><p><span data-ttu-id="6f0bd-589">Balises que vous affectez à la jauge dans l’ordre pour regrouper les enregistrements de facturation.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="6f0bd-590">Par exemple, vous pouvez utiliser des balises pour distribuer des coûts par le département informatique qui utilise la jauge.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="6f0bd-591">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="6f0bd-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="6f0bd-592">Toute information supplémentaire non couverte dans d’autres colonnes.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="6f0bd-593">Mise en correspondance des frais entre une facture et le fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="6f0bd-594">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="6f0bd-595">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de MicrosoftExcel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="6f0bd-596">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="6f0bd-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="6f0bd-597">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’«ajustements» ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="6f0bd-598">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="6f0bd-599">Description des frais indiqués sur les factures</span><span class="sxs-lookup"><span data-stu-id="6f0bd-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="6f0bd-600">Description des frais figurant sur le fichier de rapprochement (colonne ChargeType)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="6f0bd-601">À quoi correspondent ces frais?</span><span class="sxs-lookup"><span data-stu-id="6f0bd-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="6f0bd-602">Comment faire correspondre ces types de frais ChargeType sur la facture?</span><span class="sxs-lookup"><span data-stu-id="6f0bd-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="6f0bd-603">Frais basé sur les licences</span><span class="sxs-lookup"><span data-stu-id="6f0bd-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-604">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-605">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="6f0bd-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="6f0bd-606">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-607">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-608">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="6f0bd-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-609">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="6f0bd-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-610">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-611">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="6f0bd-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-612">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="6f0bd-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-613">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-614">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-615">Frais au prorata en cas d’achat</span><span class="sxs-lookup"><span data-stu-id="6f0bd-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-616">Le type de frais pour un abonnement lors de l’utilisation de la facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="6f0bd-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-617">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-618">Le type de frais pour un abonnement lorsque vous utilisez une facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="6f0bd-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-619">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-620">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="6f0bd-621">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-622">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-623">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-624">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="6f0bd-625">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-626">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-627">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="6f0bd-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="6f0bd-628">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-629">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="6f0bd-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-630">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="6f0bd-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="6f0bd-631">Crédits</span><span class="sxs-lookup"><span data-stu-id="6f0bd-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-632">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="6f0bd-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-633">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="6f0bd-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-634">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="6f0bd-635">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="6f0bd-636">Sur l’utilisation des remises</span><span class="sxs-lookup"><span data-stu-id="6f0bd-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-637">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="6f0bd-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-638">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="6f0bd-639">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-640">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="6f0bd-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-641">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="6f0bd-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-642">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="6f0bd-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-643">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="6f0bd-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-644">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="6f0bd-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-645">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="6f0bd-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="6f0bd-646">Basé sur les licences des remises</span><span class="sxs-lookup"><span data-stu-id="6f0bd-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="6f0bd-647">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="6f0bd-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-648">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="6f0bd-649"><strong></strong>&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="6f0bd-650">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="6f0bd-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="6f0bd-651">Exception: &quot;décalage d’un élément de ligne&quot; taxes sont déjà incluses.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="6f0bd-652">Consultez les crédits, ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="6f0bd-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-653">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="6f0bd-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="6f0bd-654">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="6f0bd-655">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="6f0bd-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
