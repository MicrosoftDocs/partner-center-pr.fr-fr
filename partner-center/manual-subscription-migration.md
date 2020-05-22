---
title: Migrer des abonnements Dynamics 365 qualifiés
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment migrer des abonnements Dynamics 365 de base qualifiés vers un nouvel abonnement avant l’expiration des abonnements existants.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 offres, renouvellement d’offres, nouvelles références (SKU) Dynamics 365
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795991"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="8a76b-104">Migrer Dynamics 365 et Plan Customer Engagement à partir de Basic (offres qualifiées) vers une version plus récente</span><span class="sxs-lookup"><span data-stu-id="8a76b-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="8a76b-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="8a76b-105">**Applies to**</span></span>

-  <span data-ttu-id="8a76b-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8a76b-106">Partner Center</span></span>

<span data-ttu-id="8a76b-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8a76b-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="8a76b-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="8a76b-108">Global admin</span></span>
-   <span data-ttu-id="8a76b-109">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8a76b-109">User admin</span></span>
-   <span data-ttu-id="8a76b-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="8a76b-110">Admin agent</span></span>
-   <span data-ttu-id="8a76b-111">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="8a76b-111">Sales agent</span></span>

<span data-ttu-id="8a76b-112">À compter du 1er janvier 2019, les clients disposant de Dynamics 365 pour le plan d’engagement commercial/client des abonnements de base (offres qualifiées) ne peuvent plus renouveler ces offres héritées. les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="8a76b-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="8a76b-113">Sur la page de détails de l’abonnement, l’état de l’abonnement passe à « expire le [date] » dans « auto Renews on [date] ».</span><span class="sxs-lookup"><span data-stu-id="8a76b-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="8a76b-114">Pour garantir la continuité des clients, vous devez les transférer avec des abonnements arrivant à expiration vers une option prise en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8a76b-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="8a76b-115">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="8a76b-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="8a76b-116">Si vous utilisez l’API (CREST ou Partner Center), vous pouvez rechercher les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux.</span><span class="sxs-lookup"><span data-stu-id="8a76b-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="8a76b-117">Les abonnements en question seront configurés pour renouveler automatiquement = false le 1er janvier 2019.</span><span class="sxs-lookup"><span data-stu-id="8a76b-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="8a76b-118">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="8a76b-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="8a76b-119">Les offres Dynamics 365 en cours de retrait</span><span class="sxs-lookup"><span data-stu-id="8a76b-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="8a76b-120">Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-121">Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="8a76b-122">Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-123">Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-124">Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-125">Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="8a76b-126">Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-127">Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-128">Dynamics 365 pour le module complémentaire Sales Enterprise Edition pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-129">Dynamics 365 pour le module complémentaire Sales Enterprise Edition pour CRM de base (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="8a76b-130">Dynamics 365 pour le module complémentaire Sales Enterprise Edition pour CRM de base (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-131">Module complémentaire Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-132">Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-133">Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-134">Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-135">Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="8a76b-136">Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-137">Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) à partir de SA pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-138">Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-139">Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="8a76b-140">Dynamics 365 Customer engagement plan Enterprise Edition pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-141">Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) complémentaire pour CRM Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-142">Dynamics 365 Customer engagement plan Enterprise Edition pour CRM Basic (offre qualifiée) pour les élèves</span><span class="sxs-lookup"><span data-stu-id="8a76b-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="8a76b-143">Dynamics 365 Customer engagement plan Enterprise Edition pour CRM Basic (offre qualifiée) pour les enseignants</span><span class="sxs-lookup"><span data-stu-id="8a76b-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="8a76b-144">Dynamics 365 pour les ventes/le plan d’engagement des clients des plans de remplacement de base (offres qualifiées)</span><span class="sxs-lookup"><span data-stu-id="8a76b-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="8a76b-145">**Offres mises hors service**</span><span class="sxs-lookup"><span data-stu-id="8a76b-145">**Retired offers**</span></span>   

- <span data-ttu-id="8a76b-146">Dynamics 365 pour les ventes à partir de CRM Basic ou CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="8a76b-147">Plan d’engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (offre qualifiée)</span><span class="sxs-lookup"><span data-stu-id="8a76b-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="8a76b-148">**Options de remplacement**</span><span class="sxs-lookup"><span data-stu-id="8a76b-148">**Replacement options**</span></span>
- <span data-ttu-id="8a76b-149">Dynamics 365 pour le professionnel des ventes (nouveauté)</span><span class="sxs-lookup"><span data-stu-id="8a76b-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="8a76b-150">Dynamics 365 pour le professionnel des ventes (nouveauté)</span><span class="sxs-lookup"><span data-stu-id="8a76b-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="8a76b-151">Dynamics 365 pour le service client</span><span class="sxs-lookup"><span data-stu-id="8a76b-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="8a76b-152">Plan d’engagement client Dynamics 365 ou</span><span class="sxs-lookup"><span data-stu-id="8a76b-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="8a76b-153">Membres de l’équipe Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8a76b-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="8a76b-154">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="8a76b-154">Transition customers to new product plans</span></span>

<span data-ttu-id="8a76b-155">Le déplacement de clients des références SKU hors service vers des versions plus récentes requiert les étapes suivantes dans cet ordre :</span><span class="sxs-lookup"><span data-stu-id="8a76b-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="8a76b-156">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="8a76b-156">Purchase the new subscription</span></span>
- <span data-ttu-id="8a76b-157">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="8a76b-157">Reassign current user licenses</span></span>
- <span data-ttu-id="8a76b-158">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="8a76b-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="8a76b-159">Acheter le nouveau plan pour votre client</span><span class="sxs-lookup"><span data-stu-id="8a76b-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="8a76b-160">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous souhaitez déplacer vers le nouvel abonnement.</span><span class="sxs-lookup"><span data-stu-id="8a76b-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="8a76b-161">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="8a76b-162">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="8a76b-163">Votre client dispose désormais de l’ancien abonnement et du nouveau.</span><span class="sxs-lookup"><span data-stu-id="8a76b-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="8a76b-164">L’étape suivante consiste à réattribuer les licences aux utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="8a76b-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="8a76b-165">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="8a76b-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8a76b-166">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="8a76b-167">Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="8a76b-168">Sur la page **gérer les licences** , désactivez la case à cocher Dynamics 365 pour le plan Sales/Customer engagement de base (offre qualifiée) et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="8a76b-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="8a76b-169">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-169">Select **Submit**.</span></span> <span data-ttu-id="8a76b-170">Vous effectuerez cette opération pour chaque utilisateur qui a besoin de la nouvelle licence.</span><span class="sxs-lookup"><span data-stu-id="8a76b-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="8a76b-171">Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="8a76b-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="8a76b-172">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="8a76b-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="8a76b-173">Sur la page Détails de l’abonnement, définissez l’ancien abonnement sur **suspendu** , puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="8a76b-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="8a76b-174">L’ancien abonnement est maintenant suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="8a76b-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="8a76b-175">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="8a76b-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="8a76b-176">Votre client n’aura aucuns frais supplémentaires pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="8a76b-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



