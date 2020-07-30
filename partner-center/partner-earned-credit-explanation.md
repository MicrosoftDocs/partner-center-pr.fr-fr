---
title: Crédit Partenaires pour les services managés
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les crédits Partenaires Microsoft pour les services managés sont calculés et payés, et comment vérifier que vous êtes éligible.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: db2dc98d3f40dbb29bd00111d8787a4a8cb0e082
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943616"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="17ffe-103">Calcul et paiement du crédit Partenaires</span><span class="sxs-lookup"><span data-stu-id="17ffe-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="17ffe-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="17ffe-104">**Appropriate roles**</span></span>

- <span data-ttu-id="17ffe-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="17ffe-105">Global admin</span></span>
- <span data-ttu-id="17ffe-106">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="17ffe-106">User admin</span></span>
- <span data-ttu-id="17ffe-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="17ffe-107">Admin agent</span></span>
- <span data-ttu-id="17ffe-108">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="17ffe-108">Billing admin</span></span>
- <span data-ttu-id="17ffe-109">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="17ffe-109">Sales agent</span></span>

<span data-ttu-id="17ffe-110">Le crédit Partenaires (PEC, partner earned credit) pour les services managés reconnaît et récompense les partenaires qui gère et contrôle les opérations informatiques 24h/24 et 7j/7 de tout ou partie de l’environnent Azure de leurs clients.</span><span class="sxs-lookup"><span data-stu-id="17ffe-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="17ffe-111">Par défaut, les partenaires engagés dans le programme Fournisseur de solutions Cloud bénéficient de droits d’accès à l’abonnement du client, ce qui leur permet de gérer et de contrôler les opérations 24 h/24 et 7 j/7 des ressources de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="17ffe-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="17ffe-112">Les autres moyens dont dispose le client pour accorder un accès au partenaire de transactions sont décrits dans la section suivante.</span><span class="sxs-lookup"><span data-stu-id="17ffe-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="17ffe-113">Le montant de facturation mensuelle s’entend hors crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="17ffe-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="17ffe-114">Le partenaire peut consulter le détail du crédit PEC dans le fichier de rapprochement mensuel.</span><span class="sxs-lookup"><span data-stu-id="17ffe-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="17ffe-115">Pour connaître les autres moyens dont dispose les clients pour provisionner un accès au partenaire de transactions, consultez [Gérer les abonnements et les ressources dans le plan Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="17ffe-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="17ffe-116">Lire également [Rétablir les privilèges d’administrateur pour les abonnements Azure CSP](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="17ffe-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="17ffe-117">Informations importantes sur l’éligibilité et le calcul</span><span class="sxs-lookup"><span data-stu-id="17ffe-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="17ffe-118">Le partenaire doit avoir un contrat MPN actif et un rôle RBAC valide pour bénéficier d’un crédit Partenaires pour les ressources Azure qu’il gère.</span><span class="sxs-lookup"><span data-stu-id="17ffe-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="17ffe-119">Dans le cas des fournisseurs indirects et de leurs revendeurs indirects, le fournisseur indirect est éligible au crédit PEC si le fournisseur indirect, le revendeur indirect ou les deux gèrent et contrôlent les opérations 24 h/24 et 7 j/7 des ressources Azure du client dans le programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="17ffe-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="17ffe-120">Le crédit PEC est associé à la consommation facturée de l’espace Azure du client relevant du programme Fournisseur de solutions Cloud managé par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="17ffe-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="17ffe-121">Il est réservé uniquement aux partenaires du programme CSP qui sont facturés par Microsoft (fournisseur indirect et partenaire à facturation directe).</span><span class="sxs-lookup"><span data-stu-id="17ffe-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="17ffe-122">Services éligibles : Le crédit Partenaires s’applique aux services figurant dans les **tarifs de la consommation de plan Azure** que les partenaires peuvent exporter à partir de la page des [tarifs du plan Azure](https://partner.microsoft.com/commerce/sales).</span><span class="sxs-lookup"><span data-stu-id="17ffe-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="17ffe-123">Notez qu’il existe des exceptions, telles que notamment les produits tiers identifiés comme **Tiers** dans la colonne **Étiquettes** des tarifs de consommation de plan Azure et les réservations de plan Azure ainsi que les produits des tarifs de la Place de marché.</span><span class="sxs-lookup"><span data-stu-id="17ffe-123">Note, there are exceptions including, but not limited to, third-party products identified as **Third Party** in  the **Tags** column of the Azure plan consumption price list and Azure Plan reservations, and products in the Marketplace price list.</span></span>

- <span data-ttu-id="17ffe-124">Le crédit PEC est calculé tous les jours et peut être consulté dans le fichier d’utilisation quotidienne et dans le fichier de rapprochement de facturation mensuelle.</span><span class="sxs-lookup"><span data-stu-id="17ffe-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="17ffe-125">Pour obtenir un crédit PEC, le partenaire (fournisseur indirect ou revendeur indirect) doit bénéficier d’un accès tout au long de la journée (24h/24, 7j/7).</span><span class="sxs-lookup"><span data-stu-id="17ffe-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>  

- <span data-ttu-id="17ffe-126">Il est possible d’obtenir un crédit PEC jusqu’au niveau des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="17ffe-126">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="17ffe-127">Si le partenaire a un accès valide au niveau de l’abonnement ou du groupe de ressources, chaque ressource qui atteint l’entité supérieure obtient un crédit PEC.</span><span class="sxs-lookup"><span data-stu-id="17ffe-127">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="17ffe-128">Les détails du crédit PEC se trouvent aussi dans [Azure Cost Management](https://go.microsoft.com/fwlink/?linkid=2106482).</span><span class="sxs-lookup"><span data-stu-id="17ffe-128">PEC details will also be available on [Azure Cost management](https://go.microsoft.com/fwlink/?linkid=2106482)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="17ffe-129">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="17ffe-129">Azure Cost Management</span></span>

<span data-ttu-id="17ffe-130">Azure Cost Management (ACM) avec Cost Analysis vous permet, en tant que partenaire, de voir les coûts qui ont bénéficié du crédit PEC.</span><span class="sxs-lookup"><span data-stu-id="17ffe-130">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="17ffe-131">Dans le [portail Azure](https://portal.azure.com), connectez-vous à votre locataire partenaire, puis sélectionnez **Cost Management + Facturation**.</span><span class="sxs-lookup"><span data-stu-id="17ffe-131">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="17ffe-132">Sélectionnez **Cost Management**</span><span class="sxs-lookup"><span data-stu-id="17ffe-132">Select **Cost management**</span></span>

3. <span data-ttu-id="17ffe-133">Sélectionnez **Cost Analysis**</span><span class="sxs-lookup"><span data-stu-id="17ffe-133">Select **Cost Analysis**</span></span>

   <span data-ttu-id="17ffe-134">La vue Cost Analysis montre les coûts de votre compte de facturation, pour tous les services achetés et consommés aux prix que vous payez Microsoft.</span><span class="sxs-lookup"><span data-stu-id="17ffe-134">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="17ffe-135">Sélectionnez **PartnerEarnedCreditApplied** dans la liste déroulante d’un graphique croisé dynamique pour voir les coûts auxquels un crédit PEC est appliqué.</span><span class="sxs-lookup"><span data-stu-id="17ffe-135">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="17ffe-136">Quand la propriété **PartnerEarnedCreditApplied** a la valeur True, le coût associé bénéficie du crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="17ffe-136">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="17ffe-137">Quand la propriété PartnerEarnedCreditApplied a la valeur False, le coût associé n’a pas répondu aux critères d’éligibilité requise pour le crédit ou le service acheté n’est pas éligible au crédit Partenaires.</span><span class="sxs-lookup"><span data-stu-id="17ffe-137">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="17ffe-138">En règle générale, l’utilisation des services prend de 8 à 24 heures pour s’afficher dans **Cost Management**, et les crédits PEC apparaîtront dans les 48 heures à partir de l’heure d’accès dans Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="17ffe-138">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="17ffe-139">Vous pouvez également regrouper et filtrer selon la propriété **PartnerEarnedCreditApplied** à l’aide des fonctionnalités de filtre **Group by and Add** (Regrouper par et ajouter) pour analyser les coûts avec un crédit PEC et les coûts auxquels aucun PEC n’est appliqué.</span><span class="sxs-lookup"><span data-stu-id="17ffe-139">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17ffe-140">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="17ffe-140">Next steps</span></span>

- [<span data-ttu-id="17ffe-141">Crédit Partenaires – Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="17ffe-141">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="17ffe-142">Vous trouverez des exemples détaillés de calculs de crédit PEC dans la liste des tarifs à laquelle vous pouvez accéder via le tableau de bord de l’Espace partenaires (connexion nécessaire).</span><span class="sxs-lookup"><span data-stu-id="17ffe-142">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="17ffe-143">Passer au plan Azure – Démarrer</span><span class="sxs-lookup"><span data-stu-id="17ffe-143">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="17ffe-144">Gérer les abonnements et les ressources dans le cadre du plan Azure</span><span class="sxs-lookup"><span data-stu-id="17ffe-144">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="17ffe-145">Révoquer ou rétablir les privilèges d’administrateur pour les abonnements Azure CSP</span><span class="sxs-lookup"><span data-stu-id="17ffe-145">Revoke or re-instate admin privileges for Azure CSP subscriptions  </span></span>](revoke-reinstate-csp.md)

