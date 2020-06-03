---
title: Facturation du plan Azure – Fichiers de facturation et de rapprochement
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment accéder à la structure des fichiers de facturation et de rapprochement liée à la facturation pour le plan Azure et comment la comprendre.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: fa1d1298f0fd3650bdaa4e6fc6b602844ac199c4
ms.sourcegitcommit: 83f9c114910282dc87b3ec22d59a8b24b1d6b368
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "84262873"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="e7666-103">Nouvelle expérience de commerce pour les fournisseurs de solutions Cloud - Facturation Azure</span><span class="sxs-lookup"><span data-stu-id="e7666-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="e7666-104">**Rôles appropriés :**</span><span class="sxs-lookup"><span data-stu-id="e7666-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="e7666-105">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="e7666-105">Admin agent</span></span>
- <span data-ttu-id="e7666-106">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="e7666-106">Billing admin</span></span>
- <span data-ttu-id="e7666-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e7666-107">Global admin</span></span>

<span data-ttu-id="e7666-108">La facturation dans le plan Azure est une expérience simplifiée qui utilise une date de facturation unique et une période de facturation par mois civil.</span><span class="sxs-lookup"><span data-stu-id="e7666-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="e7666-109">Résumé des fondamentaux de la facturation</span><span class="sxs-lookup"><span data-stu-id="e7666-109">Summary of billing essentials</span></span>

- <span data-ttu-id="e7666-110">**Date de la facture** : La facture et le fichier de rapprochement sont disponibles dans le tableau de bord/l’API de l’Espace partenaires au plus tard le 8 du mois (minuit UTC).</span><span class="sxs-lookup"><span data-stu-id="e7666-110">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="e7666-111">**Période de facturation de la facture** : La période de facturation de la facture s’aligne sur le mois civil, par exemple, elle court du 1er au 31 octobre ou du 1er au 30 novembre.</span><span class="sxs-lookup"><span data-stu-id="e7666-111">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="e7666-112">**Périodes de frais de service** : Les frais s’alignent sur le mois civil.</span><span class="sxs-lookup"><span data-stu-id="e7666-112">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="e7666-113">Par exemple, si le partenaire facturé ajoute des services Azure par le biais d’un plan Azure le 15 octobre et que le client commence à consommer les services Azure le 15 octobre, alors le partenaire facturé reçoit la facture/le rapprochement le 8 novembre pour la consommation effectuée par le client pendant la période de service allant du 15 au 31 octobre.</span><span class="sxs-lookup"><span data-stu-id="e7666-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="e7666-114">La facture du mois suivant qui va être générée le 08/12 contient tous les frais relatifs à la période de service 01/11 au 31/11.</span><span class="sxs-lookup"><span data-stu-id="e7666-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="e7666-115">**Conditions de paiement de la facture**  : 60 jours nets.</span><span class="sxs-lookup"><span data-stu-id="e7666-115">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="e7666-116">**Devise de la facture** : Les partenaires continuent à être facturés dans la devise officielle du pays du client.</span><span class="sxs-lookup"><span data-stu-id="e7666-116">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="e7666-117">Par exemple, si le partenaire facturé est en Irlande avec des clients au Royaume-Uni, en Norvège et en Allemagne, alors le partenaire facturé reçoit une facture/un rapprochement en GBP, NOK et EUR.</span><span class="sxs-lookup"><span data-stu-id="e7666-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="e7666-118">**Primes incitatives des partenaires** : Payées à 45 jours fin de mois.</span><span class="sxs-lookup"><span data-stu-id="e7666-118">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="e7666-119">Accéder à vos factures et à vos fichiers de rapprochement</span><span class="sxs-lookup"><span data-stu-id="e7666-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="e7666-120">L’administrateur général ou l’administrateur de facturation de votre entreprise reçoit un e-mail dès qu’une facture est consultable.</span><span class="sxs-lookup"><span data-stu-id="e7666-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="e7666-121">**Pour accéder à la facture et au fichier de rapprochement**</span><span class="sxs-lookup"><span data-stu-id="e7666-121">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="e7666-122">Connectez-vous au [tableau de bord](https://partner.microsoft.com/en-us/dashboard/) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="e7666-123">Dans le menu de l’Espace partenaires, sélectionnez **Facturation**.</span><span class="sxs-lookup"><span data-stu-id="e7666-123">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="e7666-124">Sélectionnez l’onglet correspondant à **Recurring** (Périodique) et **One-time** (Ponctuelle) ainsi qu’à la devise qui vous intéresse.</span><span class="sxs-lookup"><span data-stu-id="e7666-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![facturation](images/azure/billing3.png)

4. <span data-ttu-id="e7666-126">Sélectionnez **Facture** ou **Fichier de rapprochement**.</span><span class="sxs-lookup"><span data-stu-id="e7666-126">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="e7666-127">Pour voir l’historique des factures et des fichiers de rapprochement, développez la ligne d’historique de facturation située en dessous.</span><span class="sxs-lookup"><span data-stu-id="e7666-127">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="e7666-128">Fonctionnement des données d’utilisation</span><span class="sxs-lookup"><span data-stu-id="e7666-128">Understanding usage data</span></span> 

1. <span data-ttu-id="e7666-129">Le plan Azure est le conteneur racine ou de niveau supérieur pour l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e7666-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="e7666-130">Toute utilisation est liée à un seul plan Azure.</span><span class="sxs-lookup"><span data-stu-id="e7666-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="e7666-131">Dans un plan, il y aura un ou plusieurs abonnements Azure.</span><span class="sxs-lookup"><span data-stu-id="e7666-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="e7666-132">Il s’agit de conteneurs utilisés pour la gestion et le déploiement des ressources.</span><span class="sxs-lookup"><span data-stu-id="e7666-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="e7666-133">Dans un abonnement, les groupes de ressources s’ajoutent aux ressources de groupe.</span><span class="sxs-lookup"><span data-stu-id="e7666-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="e7666-134">Chaque ressource est déployée sur un groupe de ressources.</span><span class="sxs-lookup"><span data-stu-id="e7666-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="e7666-135">Les machines virtuelles et les comptes de stockage sont des exemples de ressources.</span><span class="sxs-lookup"><span data-stu-id="e7666-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="e7666-136">Les ressources émettent des compteurs : Les compteurs sont des mesures de consommation d’une ressource et une ressource peut émettre l’utilisation de plusieurs compteurs.</span><span class="sxs-lookup"><span data-stu-id="e7666-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="e7666-137">Les compteurs sont identifiés par un ProductId, un SKUId et un AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="e7666-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="e7666-138">Hiérarchie des groupes de ressources et du contrôle des abonnements</span><span class="sxs-lookup"><span data-stu-id="e7666-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="e7666-139">**Compte Azure (locataire)**</span><span class="sxs-lookup"><span data-stu-id="e7666-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="e7666-140">Abonnement A</span><span class="sxs-lookup"><span data-stu-id="e7666-140">Subscription A</span></span>
    - <span data-ttu-id="e7666-141">Groupe de ressources 1</span><span class="sxs-lookup"><span data-stu-id="e7666-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="e7666-142">Machine virtuelle (ressource)</span><span class="sxs-lookup"><span data-stu-id="e7666-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e7666-143">Compteur de calcul</span><span class="sxs-lookup"><span data-stu-id="e7666-143">Compute meter</span></span>
        - <span data-ttu-id="e7666-144">Réseau virtuel (ressource)</span><span class="sxs-lookup"><span data-stu-id="e7666-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="e7666-145">Aucun compteur de facturation</span><span class="sxs-lookup"><span data-stu-id="e7666-145">No billing meter</span></span>

    - <span data-ttu-id="e7666-146">Groupe de ressources 2</span><span class="sxs-lookup"><span data-stu-id="e7666-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="e7666-147">Machine virtuelle (ressource)</span><span class="sxs-lookup"><span data-stu-id="e7666-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="e7666-148">Compteur de calcul</span><span class="sxs-lookup"><span data-stu-id="e7666-148">Computer meter</span></span>
        - <span data-ttu-id="e7666-149">Disque managé SSD Premium (ressource)</span><span class="sxs-lookup"><span data-stu-id="e7666-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="e7666-150">Compteur de capacité de stockage</span><span class="sxs-lookup"><span data-stu-id="e7666-150">Storage capacity meter</span></span>
            - <span data-ttu-id="e7666-151">Compteur des opérations de stockage</span><span class="sxs-lookup"><span data-stu-id="e7666-151">Storage operations meter</span></span>

- <span data-ttu-id="e7666-152">Abonnement B   -Groupe de ressources 1       - Azure SQL (ressource)           - Compteur DTU       - Passerelle VPN (ressource)           - Compteur de passerelle VPN</span><span class="sxs-lookup"><span data-stu-id="e7666-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="e7666-153">Groupe de ressources 2</span><span class="sxs-lookup"><span data-stu-id="e7666-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="e7666-154">Interface réseau virtuelle (ressource)</span><span class="sxs-lookup"><span data-stu-id="e7666-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="e7666-155">Aucun compteur de facturation</span><span class="sxs-lookup"><span data-stu-id="e7666-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="e7666-156">Lire la facture</span><span class="sxs-lookup"><span data-stu-id="e7666-156">Read the invoice</span></span>

1. <span data-ttu-id="e7666-157">La facture est disponible au plus tard le huit de chaque mois.</span><span class="sxs-lookup"><span data-stu-id="e7666-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="e7666-158">Les partenaires ont 60 jours pour effectuer le paiement.</span><span class="sxs-lookup"><span data-stu-id="e7666-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="e7666-159">La période de facturation couvre un mois civil donné, par exemple, du 1er au 31 octobre.</span><span class="sxs-lookup"><span data-stu-id="e7666-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="e7666-160">Les frais sont nets d’ajustements (le montant est net de « crédit Partenaires pour les services managés »).</span><span class="sxs-lookup"><span data-stu-id="e7666-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="e7666-161">Consultez le fichier de rapprochement et le fichier d’utilisation quotidienne estimée pour obtenir d’autres informations sur la facturation.</span><span class="sxs-lookup"><span data-stu-id="e7666-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![facture](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="e7666-163">Lire le fichier de rapprochement des factures</span><span class="sxs-lookup"><span data-stu-id="e7666-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="e7666-164">Chaque combinaison de compteur et de plan Azure peut avoir jusqu’à deux lignes de facturation sur le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="e7666-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="e7666-165">Si le compteur est éligible à un type de remise ou crédit (par exemple, des remises différenciées ou le crédit Partenaires pour les services managés) pendant tout le mois civil, le fichier de rapprochement ne contient qu’une seule ligne de facturation.</span><span class="sxs-lookup"><span data-stu-id="e7666-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="e7666-166">La colonne **PriceAdjusmentDescription** référencera la remise ou le crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="e7666-167">Si aucune ressource d’un compteur particulier n’est éligible à une remise ou au crédit Partenaires, le fichier de rapprochement ne contient qu’une seule ligne de facturation et le prix unitaire effectif correspond au prix de vente au détail (à savoir, le prix unitaire).</span><span class="sxs-lookup"><span data-stu-id="e7666-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="e7666-168">Si le compteur, ou n’importe quelle ressource émettant ce compteur, est éligible au **crédit Partenaires pour les services managés** pendant une partie du mois, le fichier de rapprochement contient deux lignes de facturation.</span><span class="sxs-lookup"><span data-stu-id="e7666-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="e7666-169">Une ligne représente les jours pendant lesquels le compteur est éligible et la seconde ligne représente les jours où il n’est pas éligible.</span><span class="sxs-lookup"><span data-stu-id="e7666-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="e7666-170">Lire le fichier d’utilisation quotidienne</span><span class="sxs-lookup"><span data-stu-id="e7666-170">Read the daily usage file</span></span>

- <span data-ttu-id="e7666-171">Les compteurs d’abonnement dans le cadre d’un plan Azure sont évalués et cumulés quotidiennement.</span><span class="sxs-lookup"><span data-stu-id="e7666-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="e7666-172">Le **crédit Partenaires pour les services managés** est déterminé et appliqué quotidiennement.</span><span class="sxs-lookup"><span data-stu-id="e7666-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="e7666-173">Chaque compteur d’abonnement a une ligne pour chaque jour du mois où une consommation a eu lieu.</span><span class="sxs-lookup"><span data-stu-id="e7666-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="e7666-174">Dans l’exemple ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="e7666-174">In the example below:</span></span>

  - <span data-ttu-id="e7666-175">Le compteur est éligible au **crédit Partenaires pour les services managés** du 01/07 au 03/07. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="e7666-176">Le compteur n’est pas éligible au **crédit Partenaires pour les services managés** du 04/07 au 07/07. Notez que le prix unitaire effectif est le prix de vente au détail.</span><span class="sxs-lookup"><span data-stu-id="e7666-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="e7666-177">Le compteur est éligible au **crédit Partenaires pour les services managés** du 08/07 au 31/07. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="e7666-179">Facture dans la devise du client</span><span class="sxs-lookup"><span data-stu-id="e7666-179">Invoice in customer currency</span></span> 

<span data-ttu-id="e7666-180">Les services Azure fournis par l’intermédiaire d’un plan Azure sont facturés en USD et facturés dans la devise officielle du pays du client.</span><span class="sxs-lookup"><span data-stu-id="e7666-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="e7666-181">Si la devise de facturation n’est pas USD, le taux de change utilisé est indiqué à la dernière page de la facture.</span><span class="sxs-lookup"><span data-stu-id="e7666-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="e7666-182">Les taux de change sont déterminés tous les mois et appliqués à la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="e7666-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="e7666-183">Pour obtenir la liste complète des devises des pays, consultez la [grille des devises client et la disponibilité des offres de nouveau commerce par pays](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="e7666-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span> 

<span data-ttu-id="e7666-184">Microsoft utilise Thomson Reuters pour déterminer les taux de change permettant d’effectuer la conversion de la devise de tarification en devise de facturation.</span><span class="sxs-lookup"><span data-stu-id="e7666-184">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="e7666-185">Les taux de change sont actualisés et disponibles le jour précédant le premier jour du mois auquel ils s’appliquent.</span><span class="sxs-lookup"><span data-stu-id="e7666-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="e7666-186">**Exemple**:  Les frais d’utilisation pour la période de service qui va du 1er au 31 août sont facturés à l’aide du taux de change publié le 31 juillet.</span><span class="sxs-lookup"><span data-stu-id="e7666-186">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="e7666-187">Ces frais apparaissent dans la facture de septembre et le taux de change est indiqué à la dernière page de la facture.</span><span class="sxs-lookup"><span data-stu-id="e7666-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="e7666-188">Réservations Azure</span><span class="sxs-lookup"><span data-stu-id="e7666-188">Azure reservations</span></span> 

<span data-ttu-id="e7666-189">Si vous achetez des [réservations Azure](https://docs.microsoft.com/partner-center/azure-reservations) par le biais d’un plan Azure, il est uniquement possible de choisir la facturation ponctuelle dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-189">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="e7666-190">La facturation mensuelle est disponible sur le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="e7666-190">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="e7666-191">La facturation mensuelle sera disponible dans l’Espace partenaires à une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="e7666-191">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="e7666-192">Dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="e7666-192">Azure spending</span></span> 

<span data-ttu-id="e7666-193">L’expérience des dépenses Azure existante est mise à jour pour prendre en charge la facturation du nouveau plan Azure dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e7666-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="e7666-194">Cela permet aux partenaires d’effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="e7666-194">This enables partners to:</span></span>

- <span data-ttu-id="e7666-195">Voir, gérer et recevoir des alertes pour le budget défini au niveau d’un client</span><span class="sxs-lookup"><span data-stu-id="e7666-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="e7666-196">Voir les dépenses totales estimées sur un plan Azure (ventilées par niveau de ressource et de compteur)</span><span class="sxs-lookup"><span data-stu-id="e7666-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="e7666-197">Étant donné que le modèle de facturation des services Azure par le biais d’un plan Azure correspond à une consommation après paiement, pour éviter une facture plus importante que prévu, les partenaires peuvent appliquer un budget mensuel et suivre le pourcentage d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="e7666-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="e7666-198">Un budget peut être appliqué à un seul client ou à plusieurs clients à la fois.</span><span class="sxs-lookup"><span data-stu-id="e7666-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Dépenses Azure](images/azure/azurespend.png)

<span data-ttu-id="e7666-200">**Pour plus d’informations**</span><span class="sxs-lookup"><span data-stu-id="e7666-200">**For more information**</span></span>

-  <span data-ttu-id="e7666-201">Le mode de calcul du crédit Partenaires se trouve dans la liste de tarifs disponible dans le [tableau de bord](https://partner.microsoft.com/en-us/dashboard/) de votre Espace partenaires (connexion requise).</span><span class="sxs-lookup"><span data-stu-id="e7666-201">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="e7666-202">Acheter le plan Azure</span><span class="sxs-lookup"><span data-stu-id="e7666-202">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="e7666-203">Tarifs de la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="e7666-203">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
