---
title: Utiliser l’analytique de l’espace partenaires pour Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment afficher vos données d’entreprise à l’aide de l’application Partner Center Analytics pour Power BI (pour les partenaires directs dans CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633860"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="d00a5-103">Afficher vos données d’entreprise avec l’application Partner Center Analytics pour Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="d00a5-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="d00a5-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="d00a5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d00a5-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="d00a5-105">Global admin</span></span>
- <span data-ttu-id="d00a5-106">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d00a5-106">User management admin</span></span>
- <span data-ttu-id="d00a5-107">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="d00a5-107">Sales agent</span></span>
- <span data-ttu-id="d00a5-108">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="d00a5-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="d00a5-109">Afficher vos données d’entreprise</span><span class="sxs-lookup"><span data-stu-id="d00a5-109">View your business data</span></span>

<span data-ttu-id="d00a5-110">Obtenir une représentation visuelle de vos données d’entreprise avec l’application Partner Center Analytics pour Power BI, notamment :</span><span class="sxs-lookup"><span data-stu-id="d00a5-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="d00a5-111">Croissance de votre base de clients, abonnements et licences</span><span class="sxs-lookup"><span data-stu-id="d00a5-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="d00a5-112">Utilisation de produits Office 365, Microsoft Dynamics et Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="d00a5-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="d00a5-113">Unités de consommation quotidienne par ressource contrôlée de chaque abonnement Azure au cours des 60 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="d00a5-114">Coût estimé (basé sur la carte de taux la plus récente)</span><span class="sxs-lookup"><span data-stu-id="d00a5-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="d00a5-115">Possibilité d’exporter des jeux de données et de créer des rapports personnalisés, notamment par client.</span><span class="sxs-lookup"><span data-stu-id="d00a5-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="d00a5-116">À propos de la version préliminaire de l’application Partner Center Analytics</span><span class="sxs-lookup"><span data-stu-id="d00a5-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="d00a5-117">Cette application est destinée aux partenaires directs dans le programme du fournisseur de solutions Cloud uniquement.</span><span class="sxs-lookup"><span data-stu-id="d00a5-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="d00a5-118">Les autres partenaires du fournisseur CSP (revendeurs indirects, par exemple) ne pourront pas se connecter.</span><span class="sxs-lookup"><span data-stu-id="d00a5-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="d00a5-119">Les coûts estimés sont des données de facturation/facture antérieures, et ne sont pas légalement contraignantes.</span><span class="sxs-lookup"><span data-stu-id="d00a5-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="d00a5-120">Les coûts estimés sont destinés à être utilisés uniquement pour les analyses de données.</span><span class="sxs-lookup"><span data-stu-id="d00a5-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="d00a5-121">Les informations sur les clients sont basées sur des abonnements.</span><span class="sxs-lookup"><span data-stu-id="d00a5-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="d00a5-122">Les clients pour lesquels vous avez récemment créé des comptes, mais qui n’ont pas encore d’abonnement, ne sont pas inclus dans le nombre.</span><span class="sxs-lookup"><span data-stu-id="d00a5-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="d00a5-123">Le coût estimé est basé sur la carte à tarif le plus récent, qui est basé sur la tarification du fournisseur CSP.</span><span class="sxs-lookup"><span data-stu-id="d00a5-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="d00a5-124">Les jours sont les jours civils.</span><span class="sxs-lookup"><span data-stu-id="d00a5-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="d00a5-125">Rapport Business Insights</span><span class="sxs-lookup"><span data-stu-id="d00a5-125">Business Insights report</span></span>

- <span data-ttu-id="d00a5-126">**Locataires client**: nombre de locataires de Azure ad distincts des clients qui ont acheté des abonnements</span><span class="sxs-lookup"><span data-stu-id="d00a5-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="d00a5-127">**Nouveau (30 derniers jours)**: nouveaux clients achetant au moins un abonnement au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="d00a5-128">**Évolution (30 derniers jours)**: clients sans abonnement « actif », « en grâce » ou « désactivé »</span><span class="sxs-lookup"><span data-stu-id="d00a5-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="d00a5-129">**Nouveau (dernières 24 heures)**: nouveaux clients achetant au moins un abonnement au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="d00a5-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="d00a5-130">**Estimation du coût mensuel au cours des 12 derniers mois**: tendance du mois sur le mois du montant estimé des factures en dollars cumulés sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="d00a5-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d00a5-131">**Estimation du coût par produit au cours des 12 derniers mois**: produits vendus triés par montant de facture estimée en dollars cumulé sur la période des 12 derniers mois.</span><span class="sxs-lookup"><span data-stu-id="d00a5-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="d00a5-132">Cet état indique les meilleurs produits qui apportent la plupart des revenus.</span><span class="sxs-lookup"><span data-stu-id="d00a5-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="d00a5-133">**Clients au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients et évolution des clients par mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="d00a5-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d00a5-134">**Estimation du coût par client au cours des 12 derniers mois**: clients triés par estimation de la quantité en dollars de la facture avant impôts cumulés sur la période des 12 derniers mois.</span><span class="sxs-lookup"><span data-stu-id="d00a5-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="d00a5-135">Cet état indique que les meilleurs clients apportent la plupart des revenus.</span><span class="sxs-lookup"><span data-stu-id="d00a5-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="d00a5-136">**Nombre de clients par produit**: produits vendus triés par clients associés.</span><span class="sxs-lookup"><span data-stu-id="d00a5-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="d00a5-137">Cet état indique les meilleurs produits vendus à la plupart des clients.</span><span class="sxs-lookup"><span data-stu-id="d00a5-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="d00a5-138">Rapport sur les informations d’abonnement</span><span class="sxs-lookup"><span data-stu-id="d00a5-138">Subscription Insights report</span></span>

- <span data-ttu-id="d00a5-139">**État** de l’abonnement :</span><span class="sxs-lookup"><span data-stu-id="d00a5-139">**Subscription status**:</span></span>

- <span data-ttu-id="d00a5-140">Actif : abonnements appartenant à l’état « actif » ou « en grâce »</span><span class="sxs-lookup"><span data-stu-id="d00a5-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="d00a5-141">Suspendu : abonnements appartenant à l’état « désactivé »</span><span class="sxs-lookup"><span data-stu-id="d00a5-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="d00a5-142">Désapprovisionnés : abonnements appartenant à l’état « annulé » ou « expiré »</span><span class="sxs-lookup"><span data-stu-id="d00a5-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="d00a5-143">**État** de l’expiration :</span><span class="sxs-lookup"><span data-stu-id="d00a5-143">**Expiry status**:</span></span>

  - <span data-ttu-id="d00a5-144">Expiré : abonnements qui ont déjà expiré (où la date de fin de l’abonnement est passée)</span><span class="sxs-lookup"><span data-stu-id="d00a5-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="d00a5-145">Expiration après 30 jours : abonnements qui expirent au bout de 30 jours (où la date de fin de l’abonnement est ultérieure à 30 jours)</span><span class="sxs-lookup"><span data-stu-id="d00a5-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="d00a5-146">Expiration dans 30 jours : abonnements arrivant à expiration dans les 30 prochains jours (où la date de fin de l’abonnement est comprise entre aujourd’hui et les 30 prochains jours)</span><span class="sxs-lookup"><span data-stu-id="d00a5-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="d00a5-147">**Nombre total d’abonnements**: abonnements dans l’état « actif », « en délai » ou « désactivé »</span><span class="sxs-lookup"><span data-stu-id="d00a5-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="d00a5-148">**Nouveau (30 derniers jours)**: nouveaux abonnements achetés par les clients au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="d00a5-149">**Nouveau (dernières 24 heures)**: nouveaux abonnements achetés par les clients au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="d00a5-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="d00a5-150">**Expiration dans 30 jours**: abonnements arrivant à expiration dans les 30 prochains jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="d00a5-151">**Évolution (30 derniers jours)**: abonnements désapprovisionnés ou suspendus (désactivés) au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="d00a5-152">**Distribution par types d’abonnements**:% distribution du total des abonnements par licence et type d’abonnement basé sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="d00a5-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="d00a5-153">**Nombre d’abonnements actifs par produit**: produits vendus triés par nombre d’abonnements actifs</span><span class="sxs-lookup"><span data-stu-id="d00a5-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="d00a5-154">**Abonnements au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements et des abonnements en cours d’actualisation mensuels sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="d00a5-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d00a5-155">**Détails de l’abonnement client**: vue détaillée des clients, des abonnements et des offres</span><span class="sxs-lookup"><span data-stu-id="d00a5-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="d00a5-156">Rapport sur les informations de licence :</span><span class="sxs-lookup"><span data-stu-id="d00a5-156">License Insights report:</span></span>

- <span data-ttu-id="d00a5-157">**Licences totales**: nombre total de licences agrégées sur tous les abonnements basés sur des licences</span><span class="sxs-lookup"><span data-stu-id="d00a5-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="d00a5-158">**Nouveau (30 derniers jours)**: ajout de licences au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="d00a5-159">**Évolution (30 derniers jours)**: réduction de la licence au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="d00a5-160">**Nouveau (dernières 24 heures)**: ajout de licences au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="d00a5-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="d00a5-161">**Licences au** cours des 90 derniers jours : tendance du mois sur le mois des ajouts et réductions de licences agrégés tous les mois sur la période des 90 derniers jours</span><span class="sxs-lookup"><span data-stu-id="d00a5-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="d00a5-162">**Nombre de licences actives par produit**: produits vendus triés par nombre de licences actives</span><span class="sxs-lookup"><span data-stu-id="d00a5-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="d00a5-163">**Nombre de licences actives par client**: clients triés par nombre de licences actives</span><span class="sxs-lookup"><span data-stu-id="d00a5-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="d00a5-164">**Détails de l’événement de licence client au** cours des 90 derniers jours : vue détaillée des clients, abonnements et événements d’abonnement, y compris la date de l’événement, le nom de l’événement, la quantité et le changement de quantité.</span><span class="sxs-lookup"><span data-stu-id="d00a5-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="d00a5-165">Rapport d’utilisation des licences :</span><span class="sxs-lookup"><span data-stu-id="d00a5-165">Licenses Usage report:</span></span>

- <span data-ttu-id="d00a5-166">**Licences attribuées par produit**: produits vendus triés par nombre d’affectations de licences</span><span class="sxs-lookup"><span data-stu-id="d00a5-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="d00a5-167">**Licences utilisées par produit**: produits vendus triés par nombre d’utilisations de licences</span><span class="sxs-lookup"><span data-stu-id="d00a5-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="d00a5-168">**Distribution client des licences attribuées**:% de la répartition du total des clients dans les compartiments de 20% de la plage par% d’attribution de licence</span><span class="sxs-lookup"><span data-stu-id="d00a5-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="d00a5-169">**Distribution client des licences en cours d’utilisation**:% de la répartition du total des clients dans les compartiments de 20% de la plage par rapport à l’utilisation de la licence%</span><span class="sxs-lookup"><span data-stu-id="d00a5-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="d00a5-170">**Licences attribuées par le client**: vue détaillée des licences vendues et des licences affectées par les clients et les produits</span><span class="sxs-lookup"><span data-stu-id="d00a5-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="d00a5-171">**Licences utilisées par le client**: vue détaillée des licences vendues et des licences utilisées par les clients et les produits</span><span class="sxs-lookup"><span data-stu-id="d00a5-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="d00a5-172">Rapport Azure Insights :</span><span class="sxs-lookup"><span data-stu-id="d00a5-172">Azure Insights report:</span></span>

- <span data-ttu-id="d00a5-173">**Clients basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients basés sur l’utilisation et clients basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="d00a5-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d00a5-174">**Abonnements basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements basés sur l’utilisation et abonnements basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="d00a5-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="d00a5-175">**Estimation du coût d’utilisation par le client au** cours des 60 derniers jours : les clients basés sur l’utilisation sont triés par montant de facture estimée en euros sur la période de 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="d00a5-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="d00a5-176">Cet état indique que les meilleurs clients basés sur l’utilisation apportent la plupart des revenus</span><span class="sxs-lookup"><span data-stu-id="d00a5-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="d00a5-177">**Estimation du coût d’utilisation par catégorie au** cours des 60 derniers jours : les catégories de compteurs d’abonnements basés sur l’utilisation sont triées en fonction du montant de la facture estimée en euros sur la période de 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="d00a5-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="d00a5-178">**Estimation du coût d’utilisation par abonnement au** cours des 60 derniers jours : abonnements basés sur l’utilisation par estimation de l’estimation de la quantité en dollars des factures sur la période des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="d00a5-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="d00a5-179">**Coût d’utilisation estimé par le client par dépense budgétaire**: clients triés par pourcentage de leur budget de dépenses d’utilisation actuel dépassant le seuil (100%).</span><span class="sxs-lookup"><span data-stu-id="d00a5-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="d00a5-180">Rapport d’utilisation des ressources Azure :</span><span class="sxs-lookup"><span data-stu-id="d00a5-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="d00a5-181">**Utilisation des ressources Azure par jour pour la période sélectionnée**: unités de consommation quotidienne pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="d00a5-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="d00a5-182">**Estimation du coût d’utilisation des ressources Azure pour la période sélectionnée**: coût estimé basé sur la carte de taux la plus récente pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="d00a5-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="d00a5-183">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="d00a5-183">Next steps</span></span>

- [<span data-ttu-id="d00a5-184">Présentation de l’analyse de l’espace partenaires pour Power BI application</span><span class="sxs-lookup"><span data-stu-id="d00a5-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="d00a5-185">Installer et prévisualiser l’application Analyse de l’Espace partenaires pour Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="d00a5-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
