---
title: Utiliser les fichiers de rapprochement | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Pour une vue détaillée de l’article de chacun des frais dans un cycle de facturation, télécharger les fichiers de rapprochement à partir de l’espace partenaires.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 50af14ab0e8edf6cd4576be6615cd7238b23bd99
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990991"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="365c8-103">Utiliser les fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="365c8-103">Use the reconciliation files</span></span>

**<span data-ttu-id="365c8-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="365c8-104">Applies to</span></span>**

-  <span data-ttu-id="365c8-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="365c8-105">Partner Center</span></span>
-  <span data-ttu-id="365c8-106">Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis</span><span class="sxs-lookup"><span data-stu-id="365c8-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="365c8-107">Pour une vue détaillée de l’article de chacun des frais dans un cycle de facturation, télécharger les fichiers de rapprochement à partir de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="365c8-108">Vous y trouverez des informations sur les frais pour chaque abonnement client et les événements détaillés (par exemple, l’ajout intermédiaire de sièges à un abonnement).</span><span class="sxs-lookup"><span data-stu-id="365c8-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="365c8-109">Détailler par partenaire</span><span class="sxs-lookup"><span data-stu-id="365c8-109">Itemize by partner</span></span>


<span data-ttu-id="365c8-110">Dans le modèle indirect, les partenaires peuvent utiliser ces champs supplémentaires dans les fichiers de rapprochement basés sur l’utilisation ou basés sur les licences pour détailler les informations par revendeur.</span><span class="sxs-lookup"><span data-stu-id="365c8-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="365c8-111">ID&nbsp;MPN</span><span class="sxs-lookup"><span data-stu-id="365c8-111">MPN ID</span></span></th>
<th><span data-ttu-id="365c8-112">Description</span><span class="sxs-lookup"><span data-stu-id="365c8-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="365c8-113">ID MPN</span><span class="sxs-lookup"><span data-stu-id="365c8-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="365c8-114">L’ID MicrosoftPartner Network (MPN) du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="365c8-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-115">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="365c8-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="365c8-116">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="365c8-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="365c8-117">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="365c8-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="365c8-118">Cet&nbsp;ID correspond à l’ID de revendeur indiqué pour l’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="365c8-119">Pour afficher ou mettre à jour le revendeur, dans le menu espace partenaires, sélectionnez les <strong>clients</strong>, puis choisissez le client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="365c8-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="365c8-120">Dans le menu client, sélectionnez <strong>Abonnements</strong>, puis choisissez l’abonnement dans la liste.</span><span class="sxs-lookup"><span data-stu-id="365c8-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="365c8-121">Sélectionnez <strong>Mettre à jour</strong> pour modifier le <strong>Revendeur (ID&nbsp;MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="365c8-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="365c8-122">Si un partenaire&nbsp;Fournisseur de solutions&nbsp;Cloud a vendu l’abonnement directement au client, son ID&nbsp;MPN est indiqué deux&nbsp;fois, en tant qu’ID&nbsp;MPN et ID&nbsp;MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="365c8-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="365c8-123">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="365c8-124">Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1.</span><span class="sxs-lookup"><span data-stu-id="365c8-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="365c8-125">Champs des fichiers basés sur les licences</span><span class="sxs-lookup"><span data-stu-id="365c8-125">License-based file fields</span></span>


<span data-ttu-id="365c8-126">Pour rapprocher vos frais des commandes des clients, comparez le numéro d’abonnement du partenaire de syndication dans le fichier de rapprochement à l’ID d’abonnement dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="365c8-127">Colonne</span><span class="sxs-lookup"><span data-stu-id="365c8-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="365c8-128">Description</span><span class="sxs-lookup"><span data-stu-id="365c8-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="365c8-129">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="365c8-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="365c8-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="365c8-131">Identificateur unique de l’entité de facturation spécifique, au format GUID.</span><span class="sxs-lookup"><span data-stu-id="365c8-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="365c8-132">Non requis pour le rapprochement, peut contenir des informations utiles.</span><span class="sxs-lookup"><span data-stu-id="365c8-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="365c8-133">Identique dans toutes les lignes.</span><span class="sxs-lookup"><span data-stu-id="365c8-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="365c8-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="365c8-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="365c8-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="365c8-136">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="365c8-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="365c8-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="365c8-138">OrderID</span></span></td>
<td><p><span data-ttu-id="365c8-139">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="365c8-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="365c8-140">Peut être utile pour identifier la commande lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="365c8-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="365c8-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="365c8-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="365c8-143">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="365c8-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="365c8-144">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="365c8-145">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="365c8-146">Voir Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="365c8-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="365c8-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="365c8-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-148">Syndication_Partner_Subscription_Number</span><span class="sxs-lookup"><span data-stu-id="365c8-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="365c8-149">Identificateur unique des abonnements.</span><span class="sxs-lookup"><span data-stu-id="365c8-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="365c8-150">Un client pouvant avoir plusieurs abonnements pour la même formule, cet élément est important pour l’analyse des fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="365c8-151">Ce champ correspond à l’ID d’abonnement dans la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="365c8-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="365c8-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="365c8-153">OfferID</span></span></td>
<td><p><span data-ttu-id="365c8-154">ID d’offre unique.</span><span class="sxs-lookup"><span data-stu-id="365c8-154">Unique offer ID.</span></span> <span data-ttu-id="365c8-155">ID d’offre standard conformément à la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="365c8-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="365c8-156"><b>Remarque</b>: cette valeur ne correspond pas à l’ID d’offre indiquée dans la liste tarifaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="365c8-157">Voir DurableOfferID ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="365c8-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="365c8-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="365c8-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="365c8-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="365c8-160">ID d’offre unique durable, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="365c8-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="365c8-161"><b>Remarque</b>: cette valeur correspond à l’ID d’offre de la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="365c8-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="365c8-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="365c8-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="365c8-163">OfferName</span></span></td>
<td><p><span data-ttu-id="365c8-164">Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="365c8-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="365c8-165">Microsoft Office 365 (Plan&nbsp;E3)</span><span class="sxs-lookup"><span data-stu-id="365c8-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="365c8-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="365c8-167">La date de début d’abonnement, définie sur le jour suivant la soumission de la commande.</span><span class="sxs-lookup"><span data-stu-id="365c8-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="365c8-168">En fonction de la date de début et de la date de fin de l’abonnement, vous pouvez déterminer s’il s’agit toujours de la première année de l’abonnement ou si l’abonnement a été renouvelé pour l’année suivante.</span><span class="sxs-lookup"><span data-stu-id="365c8-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="365c8-169">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="365c8-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="365c8-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="365c8-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="365c8-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="365c8-172">Date de fin d’abonnement&nbsp;: 12&nbsp;mois + x&nbsp;jours après la date de début (pour s’aligner sur la date de facturation du partenaire) ou 12&nbsp;mois à partir de la date de renouvellement.</span><span class="sxs-lookup"><span data-stu-id="365c8-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="365c8-173">Lors du renouvellement, les prix sont mis à jour selon la liste des prix en vigueur.</span><span class="sxs-lookup"><span data-stu-id="365c8-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="365c8-174">La communication avec les clients peut être nécessaire avant le renouvellement automatique.</span><span class="sxs-lookup"><span data-stu-id="365c8-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="365c8-175">L’heure indique toujours le début de la journée (0:00).</span><span class="sxs-lookup"><span data-stu-id="365c8-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="365c8-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="365c8-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="365c8-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="365c8-178">Date de début des frais.</span><span class="sxs-lookup"><span data-stu-id="365c8-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="365c8-179">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="365c8-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="365c8-180">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="365c8-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="365c8-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="365c8-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="365c8-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="365c8-183">Jour de fin des frais.</span><span class="sxs-lookup"><span data-stu-id="365c8-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="365c8-184">Quand un client change le nombre de sièges, ce nombre est utilisé pour calculer les frais (prorata) par jour.</span><span class="sxs-lookup"><span data-stu-id="365c8-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="365c8-185">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="365c8-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="365c8-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="365c8-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="365c8-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="365c8-188">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="365c8-188">The type of charge or adjustment.</span></span> <span data-ttu-id="365c8-189">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="365c8-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="365c8-190">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="365c8-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="365c8-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="365c8-192">Prix par siège, tel que publié dans la liste de prix au moment de l’achat.</span><span class="sxs-lookup"><span data-stu-id="365c8-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="365c8-193">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="365c8-194">6.82</span><span class="sxs-lookup"><span data-stu-id="365c8-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-195">Quantité</span><span class="sxs-lookup"><span data-stu-id="365c8-195">Quantity</span></span></td>
<td><p><span data-ttu-id="365c8-196">Nombre de sièges.</span><span class="sxs-lookup"><span data-stu-id="365c8-196">Number of seats.</span></span> <span data-ttu-id="365c8-197">Assurez-vous que cela correspond aux informations stockées dans votre système de facturation pendant le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="365c8-198">2</span><span class="sxs-lookup"><span data-stu-id="365c8-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-199">Montant</span><span class="sxs-lookup"><span data-stu-id="365c8-199">Amount</span></span></td>
<td><p><span data-ttu-id="365c8-200">Prix total pour la quantité.</span><span class="sxs-lookup"><span data-stu-id="365c8-200">Total of price for quantity.</span></span> <span data-ttu-id="365c8-201">Permet de vérifier que la méthode de calcul du montant est identique à celle utilisée pour les clients.</span><span class="sxs-lookup"><span data-stu-id="365c8-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="365c8-202">13.32</span><span class="sxs-lookup"><span data-stu-id="365c8-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="365c8-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="365c8-204">Montant de la remise appliquée à ces frais.</span><span class="sxs-lookup"><span data-stu-id="365c8-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="365c8-205">Les nouveaux abonnements ou abonnements IUR pouvant bénéficier d’un incitatif comprennent également le montant de la remise dans cette colonne.</span><span class="sxs-lookup"><span data-stu-id="365c8-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="365c8-206">2.32</span><span class="sxs-lookup"><span data-stu-id="365c8-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-207">Sous-total</span><span class="sxs-lookup"><span data-stu-id="365c8-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="365c8-208">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="365c8-208">Total before tax.</span></span> <span data-ttu-id="365c8-209">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="365c8-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="365c8-210">11</span><span class="sxs-lookup"><span data-stu-id="365c8-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-211">Taxe</span><span class="sxs-lookup"><span data-stu-id="365c8-211">Tax</span></span></td>
<td><p><span data-ttu-id="365c8-212">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="365c8-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="365c8-213">0</span><span class="sxs-lookup"><span data-stu-id="365c8-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="365c8-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="365c8-215">Total après impôts.</span><span class="sxs-lookup"><span data-stu-id="365c8-215">Total after tax.</span></span> <span data-ttu-id="365c8-216">Vérifie si les impôts sont retenus sur la facture.</span><span class="sxs-lookup"><span data-stu-id="365c8-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="365c8-217">11</span><span class="sxs-lookup"><span data-stu-id="365c8-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-218">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="365c8-218">Currency</span></span></td>
<td><p><span data-ttu-id="365c8-219">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-219">Currency type.</span></span> <span data-ttu-id="365c8-220">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="365c8-221">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="365c8-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="365c8-222">EUR</span><span class="sxs-lookup"><span data-stu-id="365c8-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="365c8-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="365c8-224">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="365c8-225">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="365c8-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="365c8-226">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="365c8-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="365c8-227">MPNID</span></span></td>
<td><p><span data-ttu-id="365c8-228">ID&nbsp;MPN du partenaire&nbsp;CSP</span><span class="sxs-lookup"><span data-stu-id="365c8-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="365c8-229">4390934</span><span class="sxs-lookup"><span data-stu-id="365c8-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="365c8-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="365c8-231">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="365c8-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="365c8-232">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="365c8-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="365c8-233">4390934</span><span class="sxs-lookup"><span data-stu-id="365c8-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="365c8-234">DomainName</span></span></td>
<td><p><span data-ttu-id="365c8-235">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="365c8-236">Cela ne doit pas être utilisée pour identifier de manière unique le client que le client/partenaire peut mettre à jour le domaine de redirection vers un microsite/par défaut via le portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="365c8-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="365c8-237">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="365c8-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="365c8-238">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="365c8-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="365c8-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="365c8-240">Pseudo d'abonnement.</span><span class="sxs-lookup"><span data-stu-id="365c8-240">Subscription nickname.</span></span> <span data-ttu-id="365c8-241">Si aucun pseudo n’est spécifié, l'Espace partenaires utilise le OfferName.</span><span class="sxs-lookup"><span data-stu-id="365c8-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="365c8-242">PROJET EN LIGNE</span><span class="sxs-lookup"><span data-stu-id="365c8-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="365c8-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="365c8-244">Le nom de l’offre de service achetée par le client, telle que définie dans la liste des prix.</span><span class="sxs-lookup"><span data-stu-id="365c8-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="365c8-245">(Il s'agit d'un champ identique au nom Offre).</span><span class="sxs-lookup"><span data-stu-id="365c8-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="365c8-246">PROJET EN LIGNE PREMIUM SANS CLIENT DE PROJET</span><span class="sxs-lookup"><span data-stu-id="365c8-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="365c8-247">Champs des fichiers basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="365c8-247">Usage-based file fields</span></span>


<span data-ttu-id="365c8-248">Pour rapprocher vos frais de l’utilisation des clients, comparez le champ ResellerID/ResellerName/ResellerBillableAccount du fichier de rapprochement, le nom du client et l’ID d’abonnement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="365c8-249">Les champs suivants décrivent les services utilisés et leurs taux.</span><span class="sxs-lookup"><span data-stu-id="365c8-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="365c8-250">Colonne</span><span class="sxs-lookup"><span data-stu-id="365c8-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="365c8-251">Description</span><span class="sxs-lookup"><span data-stu-id="365c8-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="365c8-252">Valeur échantillon</span><span class="sxs-lookup"><span data-stu-id="365c8-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="365c8-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="365c8-254">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="365c8-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="365c8-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="365c8-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="365c8-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="365c8-257">Nom du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="365c8-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="365c8-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="365c8-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="365c8-260">ID de compte partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="365c8-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="365c8-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="365c8-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="365c8-263">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="365c8-264">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="365c8-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="365c8-265">Client test&nbsp;A</span><span class="sxs-lookup"><span data-stu-id="365c8-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="365c8-266">MPNID</span></span></td>
<td><p><span data-ttu-id="365c8-267">ID&nbsp;MPN du partenaire&nbsp;CSP.</span><span class="sxs-lookup"><span data-stu-id="365c8-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="365c8-268">4390934</span><span class="sxs-lookup"><span data-stu-id="365c8-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="365c8-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="365c8-270">ID&nbsp;MPN du revendeur de référence pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="365c8-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="365c8-271">Voir [Détailler par partenaire](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="365c8-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="365c8-272">4390934</span><span class="sxs-lookup"><span data-stu-id="365c8-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="365c8-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="365c8-274">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="365c8-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="365c8-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="365c8-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="365c8-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="365c8-277">Date de début du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="365c8-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="365c8-278">L’heure indique toujours le début de la journée, 0:00.</span><span class="sxs-lookup"><span data-stu-id="365c8-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="365c8-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="365c8-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="365c8-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="365c8-281">Date de fin du cycle de facturation, sauf pour les dates de données d’utilisation latentes jamais facturées (à partir du cycle de facturation précédent).</span><span class="sxs-lookup"><span data-stu-id="365c8-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="365c8-282">L’heure indique toujours la fin de la journée, 23:59.</span><span class="sxs-lookup"><span data-stu-id="365c8-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="365c8-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="365c8-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="365c8-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="365c8-285">Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="365c8-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="365c8-286">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="365c8-287">Ce numéro est différent de l’ID d’abonnement sur la Console d’administration du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="365c8-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="365c8-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="365c8-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="365c8-290">Pseudo de l’offre de service.</span><span class="sxs-lookup"><span data-stu-id="365c8-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="365c8-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="365c8-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="365c8-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="365c8-293">Cœur de métier de l’offre de service</span><span class="sxs-lookup"><span data-stu-id="365c8-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="365c8-294">Microsoft&nbsp;Azure</span><span class="sxs-lookup"><span data-stu-id="365c8-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-295">OrderId</span><span class="sxs-lookup"><span data-stu-id="365c8-295">OrderID</span></span></td>
<td><p><span data-ttu-id="365c8-296">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="365c8-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="365c8-297">Peut être utile pour identifier l’abonnement lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="365c8-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="365c8-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="365c8-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="365c8-300">Nom du service Azure en question.</span><span class="sxs-lookup"><span data-stu-id="365c8-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="365c8-301">MACHINES VIRTUELLES</span><span class="sxs-lookup"><span data-stu-id="365c8-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="365c8-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="365c8-303">Type spécifique de service Windows&nbsp;Azure.</span><span class="sxs-lookup"><span data-stu-id="365c8-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="365c8-304">Service Bus - Individuel ou Pack</span><span class="sxs-lookup"><span data-stu-id="365c8-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="365c8-305">Base de données SQL Azure - Entreprise ou Web Edition</span><span class="sxs-lookup"><span data-stu-id="365c8-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="365c8-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="365c8-307">Identificateur unique spécifique pour toutes les données de service et la structure de tarification.</span><span class="sxs-lookup"><span data-stu-id="365c8-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="365c8-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="365c8-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-309">Nom de la ressource</span><span class="sxs-lookup"><span data-stu-id="365c8-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="365c8-310">Nom de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="365c8-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="365c8-311">Transfert de données entrantes (Go)</span><span class="sxs-lookup"><span data-stu-id="365c8-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="365c8-312">Transfert de données sortantes (Go)</span><span class="sxs-lookup"><span data-stu-id="365c8-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-313">Région</span><span class="sxs-lookup"><span data-stu-id="365c8-313">Region</span></span></td>
<td><p><span data-ttu-id="365c8-314">Région dans laquelle s’applique l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="365c8-314">The region the usage applies to.</span></span> <span data-ttu-id="365c8-315">Principalement utilisée pour affecter des taux aux transferts de données, car les taux varient selon la région.</span><span class="sxs-lookup"><span data-stu-id="365c8-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="365c8-316">Asie-Pacifique, Europe, Amérique latine, Amérique du Nord</span><span class="sxs-lookup"><span data-stu-id="365c8-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-317">SKU</span><span class="sxs-lookup"><span data-stu-id="365c8-317">SKU</span></span></td>
<td><p><span data-ttu-id="365c8-318">Identificateur unique MSFT de l’offre</span><span class="sxs-lookup"><span data-stu-id="365c8-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="365c8-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="365c8-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="365c8-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="365c8-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="365c8-321">ID et quantité permettant de détailler les différents taux pour un service ou une ressource sur une période de facturation donnée.</span><span class="sxs-lookup"><span data-stu-id="365c8-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="365c8-322">Pour l’évaluation par niveau d’Azure, il peut y avoir un taux jusqu’à une certaine quantité d’unités facturées, puis un autre pour les quantités plus élevées.</span><span class="sxs-lookup"><span data-stu-id="365c8-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="365c8-323">1</span><span class="sxs-lookup"><span data-stu-id="365c8-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="365c8-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="365c8-325">Quantité de service utilisé (heures, Go, etc.) pendant la période en question.</span><span class="sxs-lookup"><span data-stu-id="365c8-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="365c8-326">Inclut également toute utilisation non facturée pour les périodes précédentes.</span><span class="sxs-lookup"><span data-stu-id="365c8-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="365c8-327">11</span><span class="sxs-lookup"><span data-stu-id="365c8-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="365c8-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="365c8-329">Unités incluses dans le cadre de l’offre.</span><span class="sxs-lookup"><span data-stu-id="365c8-329">Units included as part of the offer.</span></span> <span data-ttu-id="365c8-330">Généralement non présent pour le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="365c8-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="365c8-331">0</span><span class="sxs-lookup"><span data-stu-id="365c8-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="365c8-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="365c8-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="365c8-333">Unités non incluses dans le cadre de l’offre, qui doivent être payées par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="365c8-334">Correspond à ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="365c8-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="365c8-335">11</span><span class="sxs-lookup"><span data-stu-id="365c8-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="365c8-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="365c8-337">Prix de l’offre en vigueur à la date de début de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="365c8-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="365c8-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="365c8-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="365c8-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="365c8-340">ListPrist fois OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="365c8-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="365c8-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="365c8-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="365c8-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="365c8-343">Montant de la taxe sur les frais, selon les règles fiscales et les circonstances spécifiques de votre marché.</span><span class="sxs-lookup"><span data-stu-id="365c8-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="365c8-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="365c8-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="365c8-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="365c8-346">Total après impôts, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="365c8-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="365c8-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="365c8-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-348">Symbole monétaire</span><span class="sxs-lookup"><span data-stu-id="365c8-348">Currency</span></span></td>
<td><p><span data-ttu-id="365c8-349">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-349">Currency type.</span></span> <span data-ttu-id="365c8-350">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="365c8-351">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="365c8-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="365c8-352">EUR</span><span class="sxs-lookup"><span data-stu-id="365c8-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="365c8-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="365c8-354">Prix avant impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="365c8-354">Pretax price per unit.</span></span> <span data-ttu-id="365c8-355">Correspond à PretaxCharges / OverageQuantity, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="365c8-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="365c8-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="365c8-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="365c8-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="365c8-358">Prix après impôts par unité.</span><span class="sxs-lookup"><span data-stu-id="365c8-358">Post tax price per unit.</span></span> <span data-ttu-id="365c8-359">Correspond à PostTaxTotal / OverageQuantity, ou à PretaxEffectiveRate + taux d’imposition par unité, arrondi au centime près.</span><span class="sxs-lookup"><span data-stu-id="365c8-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="365c8-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="365c8-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="365c8-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="365c8-362">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="365c8-362">The type of charge or adjustment.</span></span> <span data-ttu-id="365c8-363">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="365c8-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="365c8-364">Voir <a href="#charge_types">Frais de mappage entre une facture et le fichier de rapprochement</a></span><span class="sxs-lookup"><span data-stu-id="365c8-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="365c8-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="365c8-366">ID de compte unique dans la plateforme de facturation MSFT.</span><span class="sxs-lookup"><span data-stu-id="365c8-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="365c8-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="365c8-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="365c8-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="365c8-369">Date du déploiement du service.</span><span class="sxs-lookup"><span data-stu-id="365c8-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="365c8-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="365c8-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="365c8-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="365c8-372">Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant).</span><span class="sxs-lookup"><span data-stu-id="365c8-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="365c8-373">Asie de l’Est, Asie du Sud-Est, Europe du Nord, Europe de l’Ouest, États-Unis Centre Nord, États-Unis Centre Sud</span><span class="sxs-lookup"><span data-stu-id="365c8-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="365c8-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="365c8-375">Cette colonne permet de suivre le service Microsoft Azure qui peut ne pas être spécifiquement identifié dans la colonne ServiceName.</span><span class="sxs-lookup"><span data-stu-id="365c8-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="365c8-376">Par exemple, les transferts de données sont signalés comme &quot;Microsoft Azure - Tous les services&quot; dans la colonne de ServiceName.</span><span class="sxs-lookup"><span data-stu-id="365c8-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="365c8-377">Cette colonne MeteredService indiquera à quel service l’utilisation se rapporte.</span><span class="sxs-lookup"><span data-stu-id="365c8-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="365c8-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="365c8-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="365c8-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="365c8-380">Sous-titre qui clarifie le service Microsoft&nbsp;Azure individuel plus précisément que dans le champ MeteredService.</span><span class="sxs-lookup"><span data-stu-id="365c8-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="365c8-381">EXTERNE</span><span class="sxs-lookup"><span data-stu-id="365c8-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-382">Projet</span><span class="sxs-lookup"><span data-stu-id="365c8-382">Project</span></span></td>
<td><p><span data-ttu-id="365c8-383">Nom défini par le client pour son instance de service</span><span class="sxs-lookup"><span data-stu-id="365c8-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="365c8-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="365c8-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="365c8-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="365c8-386">Nombre de connexions ServiceBus qui ont été configurées et utilisées sur un jour donné.</span><span class="sxs-lookup"><span data-stu-id="365c8-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="365c8-387">Exemple : si vous avez utilisé une connexion configurée individuellement pendant un mois de 30 jours, Service Info 1 indique « 1 connexion/30 jours ».</span><span class="sxs-lookup"><span data-stu-id="365c8-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="365c8-388">Si vous avez un pack de 25 connexions ServiceBus et que vous en avez utilisé 1 ce jour-là, votre relevé d’utilisation quotidienne indiquera « 25 connexions/30 jours - Utilisées : 1 ».</span><span class="sxs-lookup"><span data-stu-id="365c8-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="365c8-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="365c8-390">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="365c8-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="365c8-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="365c8-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="365c8-392">DomainName</span></span></td>
<td><p><span data-ttu-id="365c8-393">Nom de domaine du client, afin d’identifier le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="365c8-394">Ce champ peut rester vide jusqu'au deuxième cycle de facturation.</span><span class="sxs-lookup"><span data-stu-id="365c8-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="365c8-395">exemple.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="365c8-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="365c8-396">Unit</span><span class="sxs-lookup"><span data-stu-id="365c8-396">Unit</span></span></td>
<td><p><span data-ttu-id="365c8-397">Unité de la ressource.</span><span class="sxs-lookup"><span data-stu-id="365c8-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="365c8-398">Go ou heures</span><span class="sxs-lookup"><span data-stu-id="365c8-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="365c8-399">Champs du fichier d’achat ponctuel</span><span class="sxs-lookup"><span data-stu-id="365c8-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="365c8-400">Champ</span><span class="sxs-lookup"><span data-stu-id="365c8-400">Field</span></span>** |**<span data-ttu-id="365c8-401">Définition</span><span class="sxs-lookup"><span data-stu-id="365c8-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="365c8-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="365c8-402">PartnerId</span></span> |<span data-ttu-id="365c8-403">ID partenaire au format GUID.</span><span class="sxs-lookup"><span data-stu-id="365c8-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="365c8-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="365c8-404">CustomerId</span></span> |<span data-ttu-id="365c8-405">ID unique de Microsoft, au format GUID, utilisé pour identifier le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="365c8-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="365c8-406">CustomerName</span></span> |<span data-ttu-id="365c8-407">Nom de l’entreprise du client comme indiqué dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="365c8-408">Cela est très important pour rapprocher la facture des informations de votre système.</span><span class="sxs-lookup"><span data-stu-id="365c8-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="365c8-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="365c8-409">CustomerDomainName</span></span> |<span data-ttu-id="365c8-410">Le nom de domaine du client.</span><span class="sxs-lookup"><span data-stu-id="365c8-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="365c8-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="365c8-411">CustomerCountry</span></span> |<span data-ttu-id="365c8-412">Le pays dans lequel se trouve le client.</span><span class="sxs-lookup"><span data-stu-id="365c8-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="365c8-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="365c8-413">InvoiceNumber</span></span> |<span data-ttu-id="365c8-414">Le numéro de la facture dans laquelle la transaction spécifiée apparaît.</span><span class="sxs-lookup"><span data-stu-id="365c8-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="365c8-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="365c8-415">MpnId</span></span> |<span data-ttu-id="365c8-416">L'identifiant MPN du partenaire fournisseur de solutions Cloud (direct ou indirect).</span><span class="sxs-lookup"><span data-stu-id="365c8-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="365c8-417">ID MPN revendeur</span><span class="sxs-lookup"><span data-stu-id="365c8-417">Reseller MPN ID</span></span> |<span data-ttu-id="365c8-418">Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect.</span><span class="sxs-lookup"><span data-stu-id="365c8-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="365c8-419">IDMPN du revendeur de référence pour la réservation.</span><span class="sxs-lookup"><span data-stu-id="365c8-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="365c8-420">Cet ID correspond à l’ID de revendeur indiqué pour la réservation dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="365c8-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="365c8-421">Si un partenaire Fournisseur de solutions Cloud a vendu la réservation directement au client, son ID MPN est indiqué deux fois, en tant qu’ID MPN et ID MPN revendeur.</span><span class="sxs-lookup"><span data-stu-id="365c8-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="365c8-422">Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire.</span><span class="sxs-lookup"><span data-stu-id="365c8-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="365c8-423">Si le partenaire fournisseur de solutions Cloud supprime un ID revendeur, cette valeur est définie sur-1.</span><span class="sxs-lookup"><span data-stu-id="365c8-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="365c8-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="365c8-424">OrderId</span></span> |<span data-ttu-id="365c8-425">Identificateur unique pour une commande dans la plateforme de facturation Microsoft.</span><span class="sxs-lookup"><span data-stu-id="365c8-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="365c8-426">Peut être utile pour identifier la réservation Azure lors du contact avec le support technique, mais pas pour le rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="365c8-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="365c8-427">OrderDate</span></span> |<span data-ttu-id="365c8-428">La date à laquelle la commande a été passée.</span><span class="sxs-lookup"><span data-stu-id="365c8-428">The date the order was placed.</span></span> |
|<span data-ttu-id="365c8-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="365c8-429">ProductId</span></span> |<span data-ttu-id="365c8-430">ID du produit.</span><span class="sxs-lookup"><span data-stu-id="365c8-430">The ID for the product.</span></span> |
|<span data-ttu-id="365c8-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="365c8-431">SkuId</span></span>  |<span data-ttu-id="365c8-432">L’ID d'une référence SKU spécifique.</span><span class="sxs-lookup"><span data-stu-id="365c8-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="365c8-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="365c8-433">AvailabilityId</span></span> |<span data-ttu-id="365c8-434">L’ID d'une disponibilité spécifique.</span><span class="sxs-lookup"><span data-stu-id="365c8-434">The ID for a particular Availability.</span></span> <span data-ttu-id="365c8-435">La «Disponibilité» indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc.</span><span class="sxs-lookup"><span data-stu-id="365c8-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="365c8-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="365c8-436">SkuName</span></span>  |<span data-ttu-id="365c8-437">Le titre d'une référence spécifique.</span><span class="sxs-lookup"><span data-stu-id="365c8-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="365c8-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="365c8-438">ProductName</span></span> |<span data-ttu-id="365c8-439">Le nom du produit.</span><span class="sxs-lookup"><span data-stu-id="365c8-439">The name of the product.</span></span> |
|<span data-ttu-id="365c8-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="365c8-440">ChargeType</span></span> |<span data-ttu-id="365c8-441">Le type de frais ou d’ajustement.</span><span class="sxs-lookup"><span data-stu-id="365c8-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="365c8-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="365c8-442">UnitPrice</span></span> |<span data-ttu-id="365c8-443">Prix par produit commandé.</span><span class="sxs-lookup"><span data-stu-id="365c8-443">Price per product ordered.</span></span> |
|<span data-ttu-id="365c8-444">Quantité</span><span class="sxs-lookup"><span data-stu-id="365c8-444">Quantity</span></span> |<span data-ttu-id="365c8-445">Nombre de produits commandés.</span><span class="sxs-lookup"><span data-stu-id="365c8-445">Number of products ordered.</span></span> |
|<span data-ttu-id="365c8-446">Sous-total</span><span class="sxs-lookup"><span data-stu-id="365c8-446">Subtotal</span></span> |<span data-ttu-id="365c8-447">Total avant impôt.</span><span class="sxs-lookup"><span data-stu-id="365c8-447">Total before tax.</span></span> <span data-ttu-id="365c8-448">Vérifiez que le sous-total correspond au total prévu, en cas de remise.</span><span class="sxs-lookup"><span data-stu-id="365c8-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="365c8-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="365c8-449">TaxTotal</span></span> |<span data-ttu-id="365c8-450">La somme totale de toutes les taxes applicables.</span><span class="sxs-lookup"><span data-stu-id="365c8-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="365c8-451">Total</span><span class="sxs-lookup"><span data-stu-id="365c8-451">Total</span></span> |<span data-ttu-id="365c8-452">Le montant total de cet achat.</span><span class="sxs-lookup"><span data-stu-id="365c8-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="365c8-453">Devise</span><span class="sxs-lookup"><span data-stu-id="365c8-453">Currency</span></span> |<span data-ttu-id="365c8-454">Type de devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-454">Currency type.</span></span> <span data-ttu-id="365c8-455">Chaque entité de facturation n’a qu’une devise.</span><span class="sxs-lookup"><span data-stu-id="365c8-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="365c8-456">Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation.</span><span class="sxs-lookup"><span data-stu-id="365c8-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="365c8-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="365c8-457">DiscountDetails</span></span> |<span data-ttu-id="365c8-458">Liste détaillée des remises éventuelles pertinentes.</span><span class="sxs-lookup"><span data-stu-id="365c8-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="365c8-459">Mise en correspondance des frais entre une facture et le fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="365c8-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="365c8-460">Votre facture inclut un récapitulatif des frais, tandis que votre fichier de rapprochement fournit une description détaillée des transactions de chaque ligne d'élément, et indique également les types de frais.</span><span class="sxs-lookup"><span data-stu-id="365c8-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="365c8-461">Afin de comparer les frais indiqués sur la facture et le fichier de rapprochement, vous pouvez utiliser les options de filtre de MicrosoftExcel pour trier les types de frais du fichier de rapprochement et les faire correspondre à un ensemble de frais détaillés sur ce même fichier.</span><span class="sxs-lookup"><span data-stu-id="365c8-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="365c8-462">Les fichiers de rapprochement, à la fois basés sur les licences et sur l’utilisation, affichent uniquement les transactions et les frais basés sur l’utilisation (unités consommées et frais associés).</span><span class="sxs-lookup"><span data-stu-id="365c8-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="365c8-463">Les crédits, remises ou remboursements ponctuels qui apparaissent sur la facture en tant qu’«ajustements» ne sont pas affichés dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="365c8-464">Le tableau ci-dessous indique les correspondances entre une section de la facture et les types de frais associés qui peuvent figurer sur les fichiers de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="365c8-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="365c8-465">Description des frais indiqués sur les factures</span><span class="sxs-lookup"><span data-stu-id="365c8-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="365c8-466">Description des frais figurant sur le fichier de rapprochement (colonne ChargeType)</span><span class="sxs-lookup"><span data-stu-id="365c8-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="365c8-467">À quoi correspondent ces frais?</span><span class="sxs-lookup"><span data-stu-id="365c8-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="365c8-468">Comment faire correspondre ces types de frais ChargeType sur la facture?</span><span class="sxs-lookup"><span data-stu-id="365c8-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="365c8-469">Frais basé sur les licences</span><span class="sxs-lookup"><span data-stu-id="365c8-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="365c8-470">Frais d'activation</span><span class="sxs-lookup"><span data-stu-id="365c8-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-471">Montant facturé au client lorsqu’il utilise l’abonnement après l'avoir acheté</span><span class="sxs-lookup"><span data-stu-id="365c8-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="365c8-472">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Montant</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-473">Frais d'annulation</span><span class="sxs-lookup"><span data-stu-id="365c8-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-474">Frais au prorata remboursés au client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="365c8-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-475">Frais de cycle</span><span class="sxs-lookup"><span data-stu-id="365c8-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-476">Frais périodiques de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-477">Instance de cycle au prorata</span><span class="sxs-lookup"><span data-stu-id="365c8-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-478">Les frais au prorata évalués du client lorsque des sièges associés sont modifiés</span><span class="sxs-lookup"><span data-stu-id="365c8-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-479">Frais au prorata en cas d'annulation</span><span class="sxs-lookup"><span data-stu-id="365c8-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-480">Remboursement au prorata pour la partie inutilisée du service lors de l’annulation</span><span class="sxs-lookup"><span data-stu-id="365c8-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-481">Frais au prorata en cas d’achat</span><span class="sxs-lookup"><span data-stu-id="365c8-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-482">Le type de frais pour un abonnement lors de l’utilisation de la facturation annuelle</span><span class="sxs-lookup"><span data-stu-id="365c8-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-483">Frais d’abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-484">Le type de frais pour un abonnement lorsque vous utilisez une facturation mensuelle</span><span class="sxs-lookup"><span data-stu-id="365c8-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-485">Frais au prorata lors du renouvellement</span><span class="sxs-lookup"><span data-stu-id="365c8-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-486">Frais au prorata lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="365c8-487">Frais de renouvellement</span><span class="sxs-lookup"><span data-stu-id="365c8-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-488">Frais de renouvellement d'un abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-489">Frais au prorata lors de l'activation</span><span class="sxs-lookup"><span data-stu-id="365c8-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-490">Frais au prorata de l’activation à la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="365c8-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="365c8-491">Frais d’utilisation</span><span class="sxs-lookup"><span data-stu-id="365c8-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="365c8-492">Évaluer les frais d’utilisation lors de l'annulation</span><span class="sxs-lookup"><span data-stu-id="365c8-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-493">Frais d’utilisation de l’accès lors de l’annulation pour une utilisation impayée pendant la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="365c8-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="365c8-494">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-495">Évaluer les frais d’utilisation pour le cycle actuel</span><span class="sxs-lookup"><span data-stu-id="365c8-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-496">Frais d’utilisation de l’accès pour la période de facturation en cours</span><span class="sxs-lookup"><span data-stu-id="365c8-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="365c8-497">Crédits</span><span class="sxs-lookup"><span data-stu-id="365c8-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="365c8-498">Décalage d’un élément de ligne</span><span class="sxs-lookup"><span data-stu-id="365c8-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-499">Remboursement partiel ou total d'un élément de ligne, taxes incluses</span><span class="sxs-lookup"><span data-stu-id="365c8-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-500">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="365c8-501">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="365c8-502">Sur l’utilisation des remises</span><span class="sxs-lookup"><span data-stu-id="365c8-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="365c8-503">Remise sur l’activation</span><span class="sxs-lookup"><span data-stu-id="365c8-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-504">Remise appliquée lors de l’activation de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="365c8-505">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-506">Remise sur le cycle</span><span class="sxs-lookup"><span data-stu-id="365c8-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-507">Remise appliquée sur les frais périodiques</span><span class="sxs-lookup"><span data-stu-id="365c8-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-508">Renouveler la remise</span><span class="sxs-lookup"><span data-stu-id="365c8-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-509">Remise appliquée lors du renouvellement de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="365c8-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-510">Annuler la remise</span><span class="sxs-lookup"><span data-stu-id="365c8-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-511">Frais appliqués lors de l’annulation des remises</span><span class="sxs-lookup"><span data-stu-id="365c8-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="365c8-512">Basé sur les licences des remises</span><span class="sxs-lookup"><span data-stu-id="365c8-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="365c8-513">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="365c8-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="365c8-514">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="365c8-515"><strong></strong>&nbsp;ou&nbsp;<strong>TVA</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="365c8-516">Peuvent être appliquées à plusieurs types de frais</span><span class="sxs-lookup"><span data-stu-id="365c8-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="365c8-517">Exception: les taxes sont déjà incluses dans «Décalage d'un élément de la ligne».</span><span class="sxs-lookup"><span data-stu-id="365c8-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="365c8-518">Consultez les crédits, ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="365c8-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="365c8-519">Taxes ou taxe sur la valeur ajoutée (TVA)</span><span class="sxs-lookup"><span data-stu-id="365c8-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="365c8-520">Reportez-vous au fichier basé sur les licences pour faire la somme des montants de la colonne <strong>Taxes</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="365c8-521">À partir d'un fichier basé sur l’utilisation, faites la somme des montants indiqués dans la colonne <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="365c8-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
