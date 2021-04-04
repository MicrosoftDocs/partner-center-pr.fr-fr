---
title: Migrer Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment migrer les offres Dynamics 365 Business Edition qualifiées vers des versions plus récentes avant qu’elles n’expirent.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132636"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="b00f5-103">Migrer les offres Dynamics 365 Business Edition vers des versions plus récentes</span><span class="sxs-lookup"><span data-stu-id="b00f5-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="b00f5-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="b00f5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b00f5-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="b00f5-105">Global admin</span></span>
- <span data-ttu-id="b00f5-106">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b00f5-106">User management admin</span></span>
- <span data-ttu-id="b00f5-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="b00f5-107">Admin agent</span></span>
- <span data-ttu-id="b00f5-108">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="b00f5-108">Sales agent</span></span>

<span data-ttu-id="b00f5-109">À compter du 1er janvier 2019, les clients disposant d’abonnements Dynamics 365 Business Edition ne peuvent plus renouveler ces offres héritées. les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="b00f5-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b00f5-110">Sur la page de détails de l’abonnement, l’état de l’abonnement passe à « expire le [date] » dans « auto Renews on [date] ».</span><span class="sxs-lookup"><span data-stu-id="b00f5-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="b00f5-111">Pour garantir la continuité des clients, vous devez les transférer avec des abonnements arrivant à expiration vers une option prise en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="b00f5-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b00f5-112">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="b00f5-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b00f5-113">Si vous utilisez l’API (CREST ou Partner Center), vous pouvez rechercher les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux.</span><span class="sxs-lookup"><span data-stu-id="b00f5-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b00f5-114">Les abonnements en question seront configurés pour renouveler automatiquement = faux le 1er janvier 2019.</span><span class="sxs-lookup"><span data-stu-id="b00f5-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="b00f5-115">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="b00f5-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="b00f5-116">Les éditions Business de Dynamics 365 en cours de retrait</span><span class="sxs-lookup"><span data-stu-id="b00f5-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="b00f5-117">Dynamics 365 pour les opérations et la finance, édition Business</span><span class="sxs-lookup"><span data-stu-id="b00f5-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="b00f5-118">Dynamics 365 pour les membres de l’équipe, édition Business</span><span class="sxs-lookup"><span data-stu-id="b00f5-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="b00f5-119">Dynamics Business central-les nouvelles offres Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="b00f5-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="b00f5-120">Grâce aux nouvelles offres Dynamics Business central, vos clients peuvent connecter leurs finances, ventes, services et opérations afin de rationaliser les processus d’entreprise, d’améliorer les interactions avec les clients et de prendre de meilleures décisions.</span><span class="sxs-lookup"><span data-stu-id="b00f5-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="b00f5-121">Dynamics 365 Business central est basé sur le Cloud et disponible uniquement via les partenaires du programme fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="b00f5-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="b00f5-122">Les clients Dynamics 365 Business Edition peuvent bénéficier d’une tarification avec remise pour les nouvelles offres professionnelles jusqu’au 30 juin 2020.</span><span class="sxs-lookup"><span data-stu-id="b00f5-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b00f5-123">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="b00f5-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="b00f5-124">Le déplacement de clients des références SKU hors service vers des versions plus récentes requiert les étapes suivantes dans cet ordre :</span><span class="sxs-lookup"><span data-stu-id="b00f5-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b00f5-125">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="b00f5-125">Purchase the new subscription</span></span>
- <span data-ttu-id="b00f5-126">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="b00f5-126">Reassign current user licenses</span></span>
- <span data-ttu-id="b00f5-127">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="b00f5-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b00f5-128">Acheter le nouveau plan pour votre client</span><span class="sxs-lookup"><span data-stu-id="b00f5-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b00f5-129">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous souhaitez déplacer vers le nouvel abonnement.</span><span class="sxs-lookup"><span data-stu-id="b00f5-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b00f5-130">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b00f5-131">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b00f5-132">Votre client dispose désormais de l’ancien abonnement et du nouveau.</span><span class="sxs-lookup"><span data-stu-id="b00f5-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b00f5-133">L’étape suivante consiste à réattribuer les licences aux utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="b00f5-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b00f5-134">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="b00f5-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b00f5-135">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b00f5-136">Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b00f5-137">Sur la page **gérer les licences** , désactivez la case à cocher Dynamics 365 pour le plan Sales/Customer engagement de base (offre qualifiée) et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="b00f5-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b00f5-138">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-138">Select **Submit**.</span></span> <span data-ttu-id="b00f5-139">Vous effectuerez cette opération pour chaque utilisateur qui a besoin de la nouvelle licence.</span><span class="sxs-lookup"><span data-stu-id="b00f5-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b00f5-140">Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="b00f5-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b00f5-141">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="b00f5-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b00f5-142">Sur la page Détails de l’abonnement, définissez l’ancien abonnement sur **suspendu** , puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="b00f5-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b00f5-143">L’ancien abonnement est maintenant suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="b00f5-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b00f5-144">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="b00f5-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b00f5-145">Votre client n’aura aucuns frais supplémentaires pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="b00f5-145">Your customer will incur no additional costs for the old subscription.</span></span>
