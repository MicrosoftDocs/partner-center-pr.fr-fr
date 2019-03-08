---
title: Migrer Dynamics 365 et le Plan d’Engagement client à partir de Basic (offres qualifiés) aux versions plus récentes | Partenaires
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 pour les ventes / Customer Engagement Plan à partir des abonnements de base (offre qualifié) peut ne plus être renouvelé.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Offres Dynamics 365, renouveler les offres, les nouvelles références SKU de Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586942"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="0c350-104">Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions</span><span class="sxs-lookup"><span data-stu-id="0c350-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="0c350-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="0c350-105">**Applies to**</span></span>

-  <span data-ttu-id="0c350-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0c350-106">Partner Center</span></span>

<span data-ttu-id="0c350-107">À compter du 1 janvier 2019, les clients avec Dynamics 365 pour les ventes / Customer Engagement Plan à partir des abonnements de base (offre qualifié) ne pouvez plus renouveler ces offres hérités ; les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="0c350-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="0c350-108">Sur la page de détails de l’abonnement, l’état de l’abonnement passe « Expire le [date] » à partir de « Auto renouvelle le [date] ».</span><span class="sxs-lookup"><span data-stu-id="0c350-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="0c350-109">Pour garantir la continuité des activités pour les clients, vous devez passer celles avec des abonnements arrivant à expiration à une option de prise en charge, répertoriés ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="0c350-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="0c350-110">Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service.</span><span class="sxs-lookup"><span data-stu-id="0c350-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="0c350-111">Si vous utilisez l’API (CREST ou partenaires), vous pouvez trouver d’abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que l’automatiquement renouvelés = propriété False.</span><span class="sxs-lookup"><span data-stu-id="0c350-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="0c350-112">Les abonnements en question seront définies sur auto renouveler = False sur le 1 janvier 2019.</span><span class="sxs-lookup"><span data-stu-id="0c350-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="0c350-113">Vous pouvez passer les clients vers une nouvelle formule à tout moment.</span><span class="sxs-lookup"><span data-stu-id="0c350-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="0c350-114">Le Dynamics 365 offre en cours de retrait</span><span class="sxs-lookup"><span data-stu-id="0c350-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="0c350-115">Dynamics 365 pour les ventes Enterprise Edition CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-116">Dynamics 365 pour l’édition entreprise de vente CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="0c350-117">Dynamics 365 pour l’édition entreprise de vente CRMOL Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-118">Dynamics 365 pour les ventes Enterprise Edition (tarification secteur public) CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-119">Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-120">Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="0c350-121">Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-122">Dynamics 365 pour les ventes, Édition entreprise (tarification secteur public) à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-123">Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-124">Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="0c350-125">Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-126">Dynamics 365 pour le module complémentaire de vente Enterprise Edition (tarification secteur public) pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (tarification secteur public) CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="0c350-131">Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-132">Dynamics 365 Customer Engagement Plan, Édition entreprise (tarification secteur public) à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-133">Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-134">Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="0c350-135">Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (tarification secteur public) module complémentaire pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-137">Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="0c350-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="0c350-138">Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="0c350-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="0c350-139">Dynamics 365 pour les ventes / plans de Customer Engagement Plan à partir de remplacement de Basic (offre qualifié)</span><span class="sxs-lookup"><span data-stu-id="0c350-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="0c350-140">**Offres supprimées**</span><span class="sxs-lookup"><span data-stu-id="0c350-140">**Retired offers**</span></span>   

- <span data-ttu-id="0c350-141">Dynamics 365 pour les ventes de CRM Basic ou CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="0c350-142">Plan d’Engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="0c350-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="0c350-143">**Options de remplacement**</span><span class="sxs-lookup"><span data-stu-id="0c350-143">**Replacement options**</span></span>
- <span data-ttu-id="0c350-144">Dynamics 365 pour les professionnels de vente (nouveau)</span><span class="sxs-lookup"><span data-stu-id="0c350-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="0c350-145">Dynamics 365 pour les professionnels de vente (nouveau)</span><span class="sxs-lookup"><span data-stu-id="0c350-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="0c350-146">Dynamics 365 pour le Service client</span><span class="sxs-lookup"><span data-stu-id="0c350-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="0c350-147">Plan d’Engagement client Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="0c350-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="0c350-148">Membres de l’équipe Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="0c350-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="0c350-149">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="0c350-149">Transition customers to new product plans</span></span>

<span data-ttu-id="0c350-150">Déplacement des clients à partir de références (SKU) retirée vers les plus récents nécessite les étapes suivantes dans cet ordre :</span><span class="sxs-lookup"><span data-stu-id="0c350-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="0c350-151">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="0c350-151">Purchase the new subscription</span></span>
- <span data-ttu-id="0c350-152">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="0c350-152">Reassign current user licenses</span></span>
- <span data-ttu-id="0c350-153">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="0c350-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="0c350-154">Le nouveau plan d’achat pour votre client</span><span class="sxs-lookup"><span data-stu-id="0c350-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="0c350-155">Sélectionnez **clients** à partir de la navigation de gauche puis le client que vous souhaitez déplacer vers un nouvel abonnement.</span><span class="sxs-lookup"><span data-stu-id="0c350-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="0c350-156">Sélectionnez **ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="0c350-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="0c350-157">Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="0c350-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="0c350-158">Votre client aura maintenant à l’ancien abonnement et le nouveau.</span><span class="sxs-lookup"><span data-stu-id="0c350-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="0c350-159">L’étape suivante consiste à réassigner des licences pour les utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="0c350-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="0c350-160">Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client vous font la transition.</span><span class="sxs-lookup"><span data-stu-id="0c350-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0c350-161">Sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="0c350-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="0c350-162">Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="0c350-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="0c350-163">Sur le **gérer les licences** page, désactivez la Dynamics 365 pour les ventes / Plan d’Engagement client à partir de Basic (offre qualifié) licence case à cocher et sélectionnez un nouveau plan de service pour l’abonnement que le client se déplace vers.</span><span class="sxs-lookup"><span data-stu-id="0c350-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="0c350-164">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="0c350-164">Select **Submit**.</span></span> <span data-ttu-id="0c350-165">Vous effectuerez ceci pour chaque utilisateur qui a besoin de la nouvelle licence.</span><span class="sxs-lookup"><span data-stu-id="0c350-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="0c350-166">Une fois que vous avez déplacé les licences vers un nouvel abonnement, vous pouvez annuler l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="0c350-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="0c350-167">Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client vous font la transition.</span><span class="sxs-lookup"><span data-stu-id="0c350-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0c350-168">Dans la page de détails d’abonnement, la valeur est l’ancien abonnement **Suspended** et sélectionnez **envoyer**.</span><span class="sxs-lookup"><span data-stu-id="0c350-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="0c350-169">L’ancien abonnement est interrompu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="0c350-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="0c350-170">L’abonnement suspendu est automatiquement désapprovisionné après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="0c350-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="0c350-171">Votre client n’entraîne aucun coût supplémentaire pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="0c350-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



