---
title: Plan Azure - Facturation | Espace partenaires
ms.topic: article
ms.date: 10/04/2019
description: Décrit la structure des factures et fichiers de rapprochement
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171301"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="1a622-103">Nouvelle expérience de commerce pour les fournisseurs de solutions Cloud - Facturation Azure</span><span class="sxs-lookup"><span data-stu-id="1a622-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="1a622-104">La facturation dans le cadre du plan Azure est une expérience simplifiée grâce à une date de facturation unique et une période de facturation par mois civil.</span><span class="sxs-lookup"><span data-stu-id="1a622-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="1a622-105">Pour plus d’informations sur la plateforme de facturation, consultez le [Guide des opérations de commerce moderne de l’Espace partenaires](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span><span class="sxs-lookup"><span data-stu-id="1a622-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="1a622-106">Résumé des fondamentaux de la facturation</span><span class="sxs-lookup"><span data-stu-id="1a622-106">Summary of billing essentials</span></span>

- <span data-ttu-id="1a622-107">**Date de la facture** : La facture et le fichier de rapprochement sont disponibles dans le tableau de bord/l’API de l’Espace partenaires au plus tard le 8 du mois (minuit UTC).</span><span class="sxs-lookup"><span data-stu-id="1a622-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="1a622-108">**Période de facturation de la facture** : La période de facturation de la facture s’aligne sur le mois civil, par exemple, elle court du 1er au 31 octobre ou du 1er au 30 novembre.</span><span class="sxs-lookup"><span data-stu-id="1a622-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="1a622-109">**Périodes de frais de service** : Les frais s’alignent sur le mois civil.</span><span class="sxs-lookup"><span data-stu-id="1a622-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="1a622-110">Par exemple, si le partenaire facturé ajoute des services Azure par le biais d’un plan Azure le 15 octobre et que le client commence à consommer les services Azure le 15 octobre, alors le partenaire facturé reçoit la facture/le rapprochement le 8 novembre pour la consommation effectuée par le client pendant la période de service allant du 15 au 31 octobre.</span><span class="sxs-lookup"><span data-stu-id="1a622-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="1a622-111">La facture du mois suivant qui va être générée le 8 décembre contient tous les frais relatifs à la période de service allant du 1er au 31 novembre.</span><span class="sxs-lookup"><span data-stu-id="1a622-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="1a622-112">**Conditions de paiement de la facture**  : 60 jours nets.</span><span class="sxs-lookup"><span data-stu-id="1a622-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="1a622-113">**Devise de la facture** : Les partenaires continuent à être facturés dans la devise officielle du pays du client.</span><span class="sxs-lookup"><span data-stu-id="1a622-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="1a622-114">Par exemple, si le partenaire facturé est en Irlande avec des clients au Royaume-Uni, en Norvège et en Allemagne, alors le partenaire facturé reçoit une facture/un rapprochement en GBP, NOK et EUR.</span><span class="sxs-lookup"><span data-stu-id="1a622-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="1a622-115">**Primes incitatives des partenaires** : Payées à 45 jours fin de mois.</span><span class="sxs-lookup"><span data-stu-id="1a622-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="1a622-116">Accéder à vos factures et à vos fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="1a622-116">Access your invoices and recon files</span></span>

<span data-ttu-id="1a622-117">L’administrateur général ou l’administrateur de facturation de votre entreprise reçoit un e-mail dès qu’une facture est consultable.</span><span class="sxs-lookup"><span data-stu-id="1a622-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="1a622-118">**Pour accéder à la facture et au fichier de rapprochement**</span><span class="sxs-lookup"><span data-stu-id="1a622-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="1a622-119">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1a622-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="1a622-120">Dans le menu de l’Espace partenaires, sélectionnez **Facturation**.</span><span class="sxs-lookup"><span data-stu-id="1a622-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="1a622-121">Sélectionnez l’onglet correspondant au **mois civil** et à la devise qui vous intéressent.</span><span class="sxs-lookup"><span data-stu-id="1a622-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![facturation](images/azure/billing1.png)

4. <span data-ttu-id="1a622-123">Sélectionnez la **facture et le fichier de rapprochement**.</span><span class="sxs-lookup"><span data-stu-id="1a622-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="1a622-124">Pour voir l’historique des factures et des fichiers de rapprochement, développez la ligne d’historique de facturation située en dessous.</span><span class="sxs-lookup"><span data-stu-id="1a622-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="1a622-125">Lire la facture</span><span class="sxs-lookup"><span data-stu-id="1a622-125">Read the invoice</span></span>

1. <span data-ttu-id="1a622-126">La facture est disponible au plus tard le 8 de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="1a622-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="1a622-127">Les partenaires ont 60 jours pour effectuer le paiement.</span><span class="sxs-lookup"><span data-stu-id="1a622-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="1a622-128">La période de facturation couvre un mois civil donné, par exemple, du 1er au 31 octobre.</span><span class="sxs-lookup"><span data-stu-id="1a622-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="1a622-129">Les frais sont nets d’ajustements (le montant est net de « crédit Partenaires pour les services managés »).</span><span class="sxs-lookup"><span data-stu-id="1a622-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="1a622-130">Consultez le fichier de rapprochement et le fichier d’utilisation quotidienne estimée pour obtenir d’autres informations sur la facturation.</span><span class="sxs-lookup"><span data-stu-id="1a622-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![facture](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="1a622-132">Lire le fichier de rapprochement</span><span class="sxs-lookup"><span data-stu-id="1a622-132">Read the recon file</span></span>

1. <span data-ttu-id="1a622-133">Chaque compteur d’abonnement Azure peut avoir jusqu’à deux lignes de facturation sur le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="1a622-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="1a622-134">Si le compteur est éligible à un type de remise ou crédit (par exemple, des remises de niveau 1 ou le crédit Partenaires pour les services managés) pendant tout le mois civil, alors le fichier de rapprochement ne contient qu’une seule ligne de facturation.</span><span class="sxs-lookup"><span data-stu-id="1a622-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="1a622-135">La colonne **PriceAdjusmentDescription** fait référence à la remise ou au crédit gagné. Le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires ou toute autre remise.</span><span class="sxs-lookup"><span data-stu-id="1a622-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="1a622-136">Si le compteur n’est pas éligible au crédit Partenaires pour les services managés pendant tout le mois civil, alors le fichier de rapprochement ne contient qu’une seule ligne de facturation et le prix unitaire effectif correspond au prix de vente au détail (à savoir, le prix unitaire).</span><span class="sxs-lookup"><span data-stu-id="1a622-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="1a622-137">Si le compteur est éligible au **crédit Partenaires pour les services managés** pendant une partie du mois, le fichier de rapprochement contient deux lignes de facturation.</span><span class="sxs-lookup"><span data-stu-id="1a622-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="1a622-138">Une ligne représente les jours pendant lesquels le compteur est éligible et la seconde ligne représente les jours où il n’est pas éligible.</span><span class="sxs-lookup"><span data-stu-id="1a622-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="1a622-139">Lire le fichier d’utilisation quotidienne</span><span class="sxs-lookup"><span data-stu-id="1a622-139">Read the daily usage file</span></span>

- <span data-ttu-id="1a622-140">Les compteurs d’abonnement dans le cadre d’un plan Azure sont évalués et cumulés quotidiennement.</span><span class="sxs-lookup"><span data-stu-id="1a622-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="1a622-141">Le **crédit Partenaires pour les services managés** est déterminé et appliqué quotidiennement.</span><span class="sxs-lookup"><span data-stu-id="1a622-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="1a622-142">Chaque compteur d’abonnement a une ligne pour chaque jour du mois où une consommation a eu lieu.</span><span class="sxs-lookup"><span data-stu-id="1a622-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="1a622-143">Dans l’exemple ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="1a622-143">In the example below:</span></span>

  - <span data-ttu-id="1a622-144">Le compteur est éligible au **crédit Partenaires pour les services managés** du 1er au 3 juillet. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="1a622-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="1a622-145">Le compteur n’est pas éligible au **crédit Partenaires pour les services managés** du 4 au 7 juillet. Notez que le prix unitaire effectif est le prix de vente au détail.</span><span class="sxs-lookup"><span data-stu-id="1a622-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="1a622-146">Le compteur est éligible au **crédit Partenaires pour les services managés** du 8 au 31 juillet. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="1a622-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="1a622-148">Facture dans la devise du client</span><span class="sxs-lookup"><span data-stu-id="1a622-148">Invoice in customer currency</span></span> 

<span data-ttu-id="1a622-149">Les services Azure fournis par l’intermédiaire d’un plan Azure sont facturés en USD et facturés dans la devise officielle du pays du client.</span><span class="sxs-lookup"><span data-stu-id="1a622-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="1a622-150">Si la devise de facturation n’est pas USD, alors le taux de change utilisé est indiqué à la dernière page de la facture.</span><span class="sxs-lookup"><span data-stu-id="1a622-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="1a622-151">Les taux de change sont déterminés tous les mois et appliqués à la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="1a622-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="1a622-152">Pour obtenir la liste complète des devises des pays, consultez la [grille des devises client et la disponibilité des offres de nouveau commerce par pays](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span><span class="sxs-lookup"><span data-stu-id="1a622-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="1a622-153">Microsoft utilise [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) pour déterminer le taux de change utilisé pour effectuer la conversion des devises.</span><span class="sxs-lookup"><span data-stu-id="1a622-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="1a622-154">Le taux de change est actualisé et disponible le jour précédant le premier jour du mois auquel il s’applique.</span><span class="sxs-lookup"><span data-stu-id="1a622-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="1a622-155">**Exemple**:  Les frais d’utilisation pour la période de service qui va du 1er au 31 août sont facturés à l’aide du taux de change publié le 1er août.</span><span class="sxs-lookup"><span data-stu-id="1a622-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="1a622-156">Ces frais apparaissent dans la facture de septembre et le taux de change est indiqué à la dernière page de la facture.</span><span class="sxs-lookup"><span data-stu-id="1a622-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="1a622-157">Les utilisateurs locataires des partenaires continuent de voir des informations connexes propres à leurs rôles concernant tous les clients et toutes les commandes, quelle que soit la devise de facturation.</span><span class="sxs-lookup"><span data-stu-id="1a622-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="1a622-158">De plus, l’utilisateur peut voir toutes les factures dans toutes les devises.</span><span class="sxs-lookup"><span data-stu-id="1a622-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="1a622-159">Réservations Azure</span><span class="sxs-lookup"><span data-stu-id="1a622-159">Azure reservations</span></span> 

<span data-ttu-id="1a622-160">Si vous achetez des [réservations Azure](https://docs.microsoft.com/partner-center/azure-reservations) par le biais d’un plan Azure, il est uniquement possible de choisir la facturation ponctuelle dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1a622-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="1a622-161">La facturation mensuelle est disponible sur le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="1a622-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="1a622-162">La facturation mensuelle sera disponible dans l’Espace partenaires à une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1a622-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="1a622-163">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="1a622-163">Azure cost management</span></span> 

<span data-ttu-id="1a622-164">Les outils Azure Cost Management permettent aux organisations de visualiser, gérer et optimiser les coûts sur Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="1a622-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="1a622-165">Cette fonctionnalité sera disponible sur la portail Azure.</span><span class="sxs-lookup"><span data-stu-id="1a622-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="1a622-166">Les partenaires disposeront d’une solution toujours active à faible latence avec les fonctionnalités suivantes disponibles :</span><span class="sxs-lookup"><span data-stu-id="1a622-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="1a622-167">Analyses plus précises et alertes budgétaires</span><span class="sxs-lookup"><span data-stu-id="1a622-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="1a622-168">API et connecteurs Power BI</span><span class="sxs-lookup"><span data-stu-id="1a622-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="1a622-169">Vue multiclient</span><span class="sxs-lookup"><span data-stu-id="1a622-169">Multi-customer view</span></span> 
- <span data-ttu-id="1a622-170">Gratuité de la gestion des coûts Azure</span><span class="sxs-lookup"><span data-stu-id="1a622-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="1a622-171">Élargissement des rôles/utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1a622-171">Expansion of roles/users</span></span> 

<span data-ttu-id="1a622-172">Pour plus d’informations sur cette fonctionnalité disponible pour les contrats Entreprise depuis février 2019, consultez [Azure Cost Management](https://azure.microsoft.com/services/cost-management).</span><span class="sxs-lookup"><span data-stu-id="1a622-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="1a622-173">Cette fonctionnalité est disponible uniquement avec les services Azure achetés dans le cadre de cette nouvelle expérience de commerce Azure pour les fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="1a622-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="1a622-174">Dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="1a622-174">Azure spending</span></span> 

<span data-ttu-id="1a622-175">Un outil relatif aux dépenses Azure sera disponible dans l’Espace partenaires pour la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="1a622-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="1a622-176">Quand cette expérience sera appliquée, cet outil permettra aux partenaires de voir :</span><span class="sxs-lookup"><span data-stu-id="1a622-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="1a622-177">Le budget total d’un client</span><span class="sxs-lookup"><span data-stu-id="1a622-177">Total budget on a customer</span></span> 
- <span data-ttu-id="1a622-178">Les dépenses totales estimées sur un plan Azure existant</span><span class="sxs-lookup"><span data-stu-id="1a622-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="1a622-179">Le pourcentage d’utilisation des clients à chaque période de facturation</span><span class="sxs-lookup"><span data-stu-id="1a622-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="1a622-180">Étant donné que le modèle de facturation des services Azure par le biais d’un plan Azure correspond à une consommation après paiement, pour éviter une facture plus importante que prévu, les partenaires peuvent appliquer un budget mensuel et suivre le pourcentage d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="1a622-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="1a622-181">Un budget peut être appliqué à un seul client ou à plusieurs clients à la fois.</span><span class="sxs-lookup"><span data-stu-id="1a622-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Dépenses Azure](images/azure/azurespend.png)

<span data-ttu-id="1a622-183">**Pour plus d’informations**</span><span class="sxs-lookup"><span data-stu-id="1a622-183">**For more information**</span></span>

-  <span data-ttu-id="1a622-184">Le mode de calcul du crédit Partenaires se trouve dans la liste de tarifs disponible dans le tableau de bord de votre Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1a622-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="1a622-185">Acheter le plan Azure</span><span class="sxs-lookup"><span data-stu-id="1a622-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="1a622-186">Tarifs de la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="1a622-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
