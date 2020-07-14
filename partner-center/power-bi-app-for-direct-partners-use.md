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
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302285"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="77495-103">Afficher vos données d’entreprise avec l’application Partner Center Analytics pour Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="77495-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="77495-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="77495-104">**Applies to**</span></span>

- <span data-ttu-id="77495-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="77495-105">Partner Center</span></span>

<span data-ttu-id="77495-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="77495-106">**Appropriate roles**</span></span>

- <span data-ttu-id="77495-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="77495-107">Global admin</span></span>
- <span data-ttu-id="77495-108">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="77495-108">User admin</span></span>
- <span data-ttu-id="77495-109">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="77495-109">Sales agent</span></span>
- <span data-ttu-id="77495-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="77495-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="77495-111">Afficher vos données d’entreprise</span><span class="sxs-lookup"><span data-stu-id="77495-111">View your business data</span></span>

<span data-ttu-id="77495-112">Obtenir une représentation visuelle de vos données d’entreprise avec l’application Partner Center Analytics pour Power BI, notamment :</span><span class="sxs-lookup"><span data-stu-id="77495-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="77495-113">Croissance de votre base de clients, abonnements et licences</span><span class="sxs-lookup"><span data-stu-id="77495-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="77495-114">Utilisation de produits Office 365, Microsoft Dynamics et Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="77495-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="77495-115">Unités de consommation quotidienne par ressource contrôlée de chaque abonnement Azure au cours des 60 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="77495-116">Coût estimé (basé sur la carte de taux la plus récente)</span><span class="sxs-lookup"><span data-stu-id="77495-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="77495-117">Possibilité d’exporter des jeux de données et de créer des rapports personnalisés, notamment par client.</span><span class="sxs-lookup"><span data-stu-id="77495-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="77495-118">À propos de la version préliminaire de l’application Partner Center Analytics</span><span class="sxs-lookup"><span data-stu-id="77495-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="77495-119">Cette application est destinée aux partenaires directs dans le programme du fournisseur de solutions Cloud uniquement.</span><span class="sxs-lookup"><span data-stu-id="77495-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="77495-120">Les autres partenaires du fournisseur CSP (revendeurs indirects, par exemple) ne pourront pas se connecter.</span><span class="sxs-lookup"><span data-stu-id="77495-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="77495-121">Les coûts estimés sont des données de facturation/facture antérieures, et ne sont pas légalement contraignantes.</span><span class="sxs-lookup"><span data-stu-id="77495-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="77495-122">Les coûts estimés sont destinés à être utilisés uniquement pour les analyses de données.</span><span class="sxs-lookup"><span data-stu-id="77495-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="77495-123">Les informations sur les clients sont basées sur des abonnements.</span><span class="sxs-lookup"><span data-stu-id="77495-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="77495-124">Tous les clients pour lesquels vous avez récemment créé des comptes, mais qui n’ont pas encore d’abonnements, ne sont pas inclus dans le nombre.</span><span class="sxs-lookup"><span data-stu-id="77495-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="77495-125">Le coût estimé est basé sur la carte à tarif le plus récent, qui est basé sur la tarification du fournisseur CSP.</span><span class="sxs-lookup"><span data-stu-id="77495-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="77495-126">Les jours sont les jours civils.</span><span class="sxs-lookup"><span data-stu-id="77495-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="77495-127">Rapport Business Insights</span><span class="sxs-lookup"><span data-stu-id="77495-127">Business Insights report</span></span>

- <span data-ttu-id="77495-128">**Locataires client**: nombre de locataires de Azure ad distincts des clients qui ont acheté des abonnements</span><span class="sxs-lookup"><span data-stu-id="77495-128">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="77495-129">**Nouveau (30 derniers jours)**: nouveaux clients achetant au moins un abonnement au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-129">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="77495-130">**Évolution (30 derniers jours)**: clients sans abonnement « actif », « en grâce » ou « désactivé »</span><span class="sxs-lookup"><span data-stu-id="77495-130">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="77495-131">**Nouveau (dernières 24 heures)**: nouveaux clients achetant au moins un abonnement au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="77495-131">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="77495-132">**Estimation du coût mensuel au cours des 12 derniers mois**: tendance du mois sur le mois du montant estimé des factures en dollars cumulés sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="77495-132">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="77495-133">**Estimation du coût par produit au cours des 12 derniers mois**: produits vendus triés par montant de facture estimée en dollars cumulé sur la période des 12 derniers mois.</span><span class="sxs-lookup"><span data-stu-id="77495-133">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="77495-134">Cet état indique les meilleurs produits qui apportent la plupart des revenus.</span><span class="sxs-lookup"><span data-stu-id="77495-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="77495-135">**Clients au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients et évolution des clients par mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="77495-135">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="77495-136">**Estimation du coût par client au cours des 12 derniers mois**: clients triés par estimation de la quantité en dollars de la facture avant impôts cumulés sur la période des 12 derniers mois.</span><span class="sxs-lookup"><span data-stu-id="77495-136">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="77495-137">Cet état indique que les meilleurs clients apportent la plupart des revenus.</span><span class="sxs-lookup"><span data-stu-id="77495-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="77495-138">**Nombre de clients par produit**: produits vendus triés par clients associés.</span><span class="sxs-lookup"><span data-stu-id="77495-138">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="77495-139">Cet état indique les meilleurs produits vendus à la plupart des clients.</span><span class="sxs-lookup"><span data-stu-id="77495-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="77495-140">Rapport sur les informations d’abonnement</span><span class="sxs-lookup"><span data-stu-id="77495-140">Subscription Insights report</span></span>

- <span data-ttu-id="77495-141">**État**de l’abonnement :</span><span class="sxs-lookup"><span data-stu-id="77495-141">**Subscription status**:</span></span>

- <span data-ttu-id="77495-142">Actif : abonnements appartenant à l’état « actif » ou « en grâce »</span><span class="sxs-lookup"><span data-stu-id="77495-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="77495-143">Suspendu : abonnements appartenant à l’état « désactivé »</span><span class="sxs-lookup"><span data-stu-id="77495-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="77495-144">Désapprovisionnés : abonnements appartenant à l’état « annulé » ou « expiré »</span><span class="sxs-lookup"><span data-stu-id="77495-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="77495-145">**État**de l’expiration :</span><span class="sxs-lookup"><span data-stu-id="77495-145">**Expiry status**:</span></span>

  - <span data-ttu-id="77495-146">Expiré : abonnements qui ont déjà expiré (où la date de fin de l’abonnement est passée)</span><span class="sxs-lookup"><span data-stu-id="77495-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="77495-147">Expiration après 30 jours : abonnements qui expirent au bout de 30 jours (où la date de fin de l’abonnement est ultérieure à 30 jours)</span><span class="sxs-lookup"><span data-stu-id="77495-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="77495-148">Expiration dans 30 jours : abonnements arrivant à expiration dans les 30 prochains jours (où la date de fin de l’abonnement est comprise entre aujourd’hui et les 30 prochains jours)</span><span class="sxs-lookup"><span data-stu-id="77495-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="77495-149">**Nombre total d’abonnements**: abonnements dans l’état « actif », « en délai » ou « désactivé »</span><span class="sxs-lookup"><span data-stu-id="77495-149">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="77495-150">**Nouveau (30 derniers jours)**: nouveaux abonnements achetés par les clients au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-150">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="77495-151">**Nouveau (dernières 24 heures)**: nouveaux abonnements achetés par les clients au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="77495-151">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="77495-152">**Expiration dans 30 jours**: abonnements arrivant à expiration dans les 30 prochains jours</span><span class="sxs-lookup"><span data-stu-id="77495-152">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="77495-153">**Évolution (30 derniers jours)**: abonnements désapprovisionnés ou suspendus (désactivés) au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-153">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="77495-154">**Distribution par types d’abonnements**:% distribution du total des abonnements par licence et type d’abonnement basé sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="77495-154">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="77495-155">**Nombre d’abonnements actifs par produit**: produits vendus triés par nombre d’abonnements actifs</span><span class="sxs-lookup"><span data-stu-id="77495-155">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="77495-156">**Abonnements au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements et des abonnements en cours d’actualisation mensuels sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="77495-156">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="77495-157">**Détails de l’abonnement client**: vue détaillée des clients, des abonnements et des offres</span><span class="sxs-lookup"><span data-stu-id="77495-157">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="77495-158">Rapport sur les informations de licence :</span><span class="sxs-lookup"><span data-stu-id="77495-158">License Insights report:</span></span>

- <span data-ttu-id="77495-159">**Licences totales**: nombre total de licences agrégées sur tous les abonnements basés sur des licences</span><span class="sxs-lookup"><span data-stu-id="77495-159">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="77495-160">**Nouveau (30 derniers jours)**: ajout de licences au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-160">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="77495-161">**Évolution (30 derniers jours)**: réduction de la licence au cours des 30 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-161">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="77495-162">**Nouveau (dernières 24 heures)**: ajout de licences au cours des dernières 24 heures</span><span class="sxs-lookup"><span data-stu-id="77495-162">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="77495-163">**Licences au**cours des 90 derniers jours : tendance du mois sur le mois des ajouts et réductions de licences agrégés tous les mois sur la période des 90 derniers jours</span><span class="sxs-lookup"><span data-stu-id="77495-163">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="77495-164">**Nombre de licences actives par produit**: produits vendus triés par nombre de licences actives</span><span class="sxs-lookup"><span data-stu-id="77495-164">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="77495-165">**Nombre de licences actives par client**: clients triés par nombre de licences actives</span><span class="sxs-lookup"><span data-stu-id="77495-165">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="77495-166">**Détails de l’événement de licence client au**cours des 90 derniers jours : vue détaillée des clients, abonnements et événements d’abonnement, y compris la date de l’événement, le nom de l’événement, la quantité et le changement de quantité.</span><span class="sxs-lookup"><span data-stu-id="77495-166">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="77495-167">Rapport d’utilisation des licences :</span><span class="sxs-lookup"><span data-stu-id="77495-167">Licenses Usage report:</span></span>

- <span data-ttu-id="77495-168">**Licences attribuées par produit**: produits vendus triés par nombre d’affectations de licences</span><span class="sxs-lookup"><span data-stu-id="77495-168">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="77495-169">**Licences utilisées par produit**: produits vendus triés par nombre d’utilisations de licences</span><span class="sxs-lookup"><span data-stu-id="77495-169">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="77495-170">**Distribution client des licences attribuées**:% de la répartition du total des clients dans les compartiments de 20% de la plage par% d’attribution de licence</span><span class="sxs-lookup"><span data-stu-id="77495-170">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="77495-171">**Distribution client des licences en cours d’utilisation**:% de la répartition du total des clients dans les compartiments de 20% de la plage par rapport à l’utilisation de la licence%</span><span class="sxs-lookup"><span data-stu-id="77495-171">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="77495-172">**Licences attribuées par le client**: vue détaillée des licences vendues et des licences affectées par les clients et les produits</span><span class="sxs-lookup"><span data-stu-id="77495-172">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="77495-173">**Licences utilisées par le client**: vue détaillée des licences vendues et des licences utilisées par les clients et les produits</span><span class="sxs-lookup"><span data-stu-id="77495-173">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="77495-174">Rapport Azure Insights :</span><span class="sxs-lookup"><span data-stu-id="77495-174">Azure Insights report:</span></span>

- <span data-ttu-id="77495-175">**Clients basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients basés sur l’utilisation et clients basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="77495-175">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="77495-176">**Abonnements basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements basés sur l’utilisation et abonnements basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois</span><span class="sxs-lookup"><span data-stu-id="77495-176">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="77495-177">**Estimation du coût d’utilisation par le client au**cours des 60 derniers jours : les clients basés sur l’utilisation sont triés par montant de facture estimée en euros sur la période de 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="77495-177">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="77495-178">Cet état indique que les meilleurs clients basés sur l’utilisation apportent la plupart des revenus</span><span class="sxs-lookup"><span data-stu-id="77495-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="77495-179">**Estimation du coût d’utilisation par catégorie au**cours des 60 derniers jours : les catégories de compteurs d’abonnements basés sur l’utilisation sont triées en fonction du montant de la facture estimée en euros sur la période de 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="77495-179">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="77495-180">**Estimation du coût d’utilisation par abonnement au**cours des 60 derniers jours : abonnements basés sur l’utilisation par estimation de l’estimation de la quantité en dollars des factures sur la période des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="77495-180">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="77495-181">**Coût d’utilisation estimé par le client par dépense budgétaire**: clients triés par pourcentage de leur budget de dépenses d’utilisation actuel dépassant le seuil (100%).</span><span class="sxs-lookup"><span data-stu-id="77495-181">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="77495-182">Rapport d’utilisation des ressources Azure :</span><span class="sxs-lookup"><span data-stu-id="77495-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="77495-183">**Utilisation des ressources Azure par jour pour la période sélectionnée**: unités de consommation quotidienne pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="77495-183">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="77495-184">**Estimation du coût d’utilisation des ressources Azure pour la période sélectionnée**: coût estimé basé sur la carte de taux la plus récente pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours.</span><span class="sxs-lookup"><span data-stu-id="77495-184">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="77495-185">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="77495-185">Next steps</span></span>

- [<span data-ttu-id="77495-186">Présentation de l’analyse de l’espace partenaires pour Power BI application</span><span class="sxs-lookup"><span data-stu-id="77495-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="77495-187">Installer et prévisualiser l’application Analyse de l’Espace partenaires pour Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="77495-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
