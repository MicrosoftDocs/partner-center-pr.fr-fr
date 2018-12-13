---
title: Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions | L’espace partenaires
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / du Plan Engagement client à partir des abonnements Basic (offre qualifiés) n’est plus peut être renouvelé.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968269"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="4dcc3-103">Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions</span><span class="sxs-lookup"><span data-stu-id="4dcc3-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="4dcc3-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="4dcc3-104">Applies to</span></span>**

-  <span data-ttu-id="4dcc3-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="4dcc3-105">Partner Center</span></span>

<span data-ttu-id="4dcc3-106">Les clients le 1er janvier 2019 efficaces avec Dynamics 365 for Sales / du Plan Engagement client à partir des abonnements Basic (offre qualifiés) pouvez renouveler n’est plus ces offres hérités; les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="4dcc3-107">Sur la page des détails de l’abonnement, l’état d’abonnement changera par «Expire le [date]» «Renouvellements le [date]».</span><span class="sxs-lookup"><span data-stu-id="4dcc3-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="4dcc3-108">Pour garantir la continuité des activités pour les clients, vous devez passer les ceux dont les abonnements arrivant à expiration à une option pris en charge, répertoriée ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="4dcc3-109">Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="4dcc3-110">Si vous utilisez l’API (CREST ou espace partenaires), vous pouvez trouver renouvellement des abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec l’automatique = False propriété.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="4dcc3-111">Les abonnements en question seront définies automatiquement renouvelé = False le 1er janvier 2019.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="4dcc3-112">Vous pouvez passer les clients vers une nouvelle formule à tout moment.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="4dcc3-113">Le Dynamics 365 propose en cours mis hors service</span><span class="sxs-lookup"><span data-stu-id="4dcc3-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="4dcc3-114">Dynamics 365 pour vente Enterprise Edition CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-115">Dynamics 365 pour vente Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="4dcc3-116">Dynamics 365 pour vente Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-117">Dynamics 365 pour vente Enterprise Edition (tarification du gouvernement des États-Unis) CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-118">Dynamics 365 Édition entreprise de vente à partir de SA pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-119">Dynamics 365 Édition entreprise de vente à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="4dcc3-120">Dynamics 365 Édition entreprise de vente à partir de SA CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-121">Dynamics 365 pour vente Enterprise Edition (tarification du gouvernement des États-Unis) à partir de SA pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-122">Dynamics 365 de vente Enterprise Edition extension pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-123">Dynamics 365 de vente Enterprise Edition extension pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="4dcc3-124">Dynamics 365 de vente Enterprise Edition extension CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-125">Dynamics 365 de vente Enterprise Edition (tarification du gouvernement des États-Unis) extension pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-126">Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-127">Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-128">Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-129">Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="4dcc3-130">Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-131">Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) à partir de SA pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-132">Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-133">Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="4dcc3-134">Dynamics 365 client Engagement Plan Enterprise Edition extension pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-135">Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) module complémentaire pour CRM Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-136">Dynamics 365 client Engagement Plan Enterprise Edition module complémentaire CRM Basic (offre qualifiée) pour les étudiants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="4dcc3-137">Dynamics 365 client Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="4dcc3-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="4dcc3-138">Dynamics 365 for Sales / plans du Plan Engagement client à partir de remplacement Basic (offre qualifiés)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="4dcc3-139">Offres retirés</span><span class="sxs-lookup"><span data-stu-id="4dcc3-139">Retired offers</span></span>**   

- <span data-ttu-id="4dcc3-140">Dynamics 365 for Sales à partir de CRM Basic ou CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="4dcc3-141">Plan d’Engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (qualifiée offre)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="4dcc3-142">Options de remplacement</span><span class="sxs-lookup"><span data-stu-id="4dcc3-142">Replacement options</span></span>**
- <span data-ttu-id="4dcc3-143">Dynamics 365 destinée aux professionnels de vente (nouveau)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="4dcc3-144">Dynamics 365 destinée aux professionnels de vente (nouveau)</span><span class="sxs-lookup"><span data-stu-id="4dcc3-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="4dcc3-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="4dcc3-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="4dcc3-146">Plan d’Engagement client Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="4dcc3-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="4dcc3-147">Membres de l’équipe Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="4dcc3-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4dcc3-148">Accompagner les clients vers des nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="4dcc3-148">Transition customers to new product plans</span></span>

<span data-ttu-id="4dcc3-149">Transfert des clients à partir de références (SKU) retiré vers les plus récentes doit respecter les étapes suivantes dans l’ordre suivant:</span><span class="sxs-lookup"><span data-stu-id="4dcc3-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="4dcc3-150">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="4dcc3-150">Purchase the new subscription</span></span>
- <span data-ttu-id="4dcc3-151">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="4dcc3-151">Reassign current user licenses</span></span>
- <span data-ttu-id="4dcc3-152">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="4dcc3-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="4dcc3-153">Acheter le nouveau plan pour votre client</span><span class="sxs-lookup"><span data-stu-id="4dcc3-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="4dcc3-154">Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous voulez déplacer vers le nouvel abonnement.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="4dcc3-155">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="4dcc3-156">Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="4dcc3-157">Votre client possède alors à la fois l’ancien abonnement et une nouvelle.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="4dcc3-158">L’étape suivante consiste à réaffecter les licences aux utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="4dcc3-159">Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="4dcc3-160">Sélectionnez **Utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="4dcc3-161">Pour réaffecter une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="4dcc3-162">Sur la page **Gérer les licences** , désactivez le Dynamics 365 for Sales / Plan d’Engagement client à partir de Basic (offre qualifiés) licence case à cocher et sélectionnez une nouvelle formule de service de l’abonnement du client est transféré sur.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="4dcc3-163">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-163">Select **Submit**.</span></span> <span data-ttu-id="4dcc3-164">Vous ferez cela pour chaque utilisateur qui ont besoin de la nouvelle licence.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="4dcc3-165">Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="4dcc3-166">Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="4dcc3-167">Sur la page des détails abonnement, définissez l’ancien abonnement sur **suspendu** et sélectionnez **Soumettre**.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="4dcc3-168">L’ancien abonnement est désormais suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="4dcc3-169">L’abonnement suspendu est automatiquement désapprovisionné après 120jours.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4dcc3-170">Votre client n’induit aucun coût supplémentaire pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="4dcc3-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



