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
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151523"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="ececf-103">Migrer les offres Dynamics 365 Business Edition vers des versions plus récentes</span><span class="sxs-lookup"><span data-stu-id="ececf-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="ececf-104">**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent d’administration | Agent des ventes</span><span class="sxs-lookup"><span data-stu-id="ececf-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="ececf-105">À compter du 1er janvier 2019, les clients disposant d’abonnements Dynamics 365 Business Edition ne peuvent plus renouveler ces offres héritées. les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="ececf-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="ececf-106">Sur la page de détails de l’abonnement, l’état de l’abonnement passe à « expire le [date] » dans « auto Renews on [date] ».</span><span class="sxs-lookup"><span data-stu-id="ececf-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="ececf-107">Pour garantir la continuité des clients, vous devez les transférer avec des abonnements arrivant à expiration vers une option prise en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="ececf-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="ececf-108">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="ececf-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ececf-109">Si vous utilisez l’API (CREST ou Partner Center), vous pouvez rechercher les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux.</span><span class="sxs-lookup"><span data-stu-id="ececf-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="ececf-110">Les abonnements en question seront configurés pour renouveler automatiquement = faux le 1er janvier 2019.</span><span class="sxs-lookup"><span data-stu-id="ececf-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="ececf-111">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="ececf-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="ececf-112">Les éditions Business de Dynamics 365 en cours de retrait</span><span class="sxs-lookup"><span data-stu-id="ececf-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="ececf-113">Dynamics 365 pour les opérations et la finance, édition Business</span><span class="sxs-lookup"><span data-stu-id="ececf-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="ececf-114">Dynamics 365 pour les membres de l’équipe, édition Business</span><span class="sxs-lookup"><span data-stu-id="ececf-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="ececf-115">Dynamics Business central-les nouvelles offres Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="ececf-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="ececf-116">Grâce aux nouvelles offres Dynamics Business central, vos clients peuvent connecter leurs finances, ventes, services et opérations afin de rationaliser les processus d’entreprise, d’améliorer les interactions avec les clients et de prendre de meilleures décisions.</span><span class="sxs-lookup"><span data-stu-id="ececf-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="ececf-117">Dynamics 365 Business central est basé sur le Cloud et disponible uniquement via les partenaires du programme fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="ececf-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="ececf-118">Les clients Dynamics 365 Business Edition peuvent bénéficier d’une tarification avec remise pour les nouvelles offres professionnelles jusqu’au 30 juin 2020.</span><span class="sxs-lookup"><span data-stu-id="ececf-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ececf-119">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="ececf-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="ececf-120">Le déplacement de clients des références SKU hors service vers des versions plus récentes requiert les étapes suivantes dans cet ordre :</span><span class="sxs-lookup"><span data-stu-id="ececf-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="ececf-121">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="ececf-121">Purchase the new subscription</span></span>
- <span data-ttu-id="ececf-122">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="ececf-122">Reassign current user licenses</span></span>
- <span data-ttu-id="ececf-123">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="ececf-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="ececf-124">Acheter le nouveau plan pour votre client</span><span class="sxs-lookup"><span data-stu-id="ececf-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="ececf-125">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous souhaitez déplacer vers le nouvel abonnement.</span><span class="sxs-lookup"><span data-stu-id="ececf-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="ececf-126">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="ececf-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="ececf-127">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="ececf-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="ececf-128">Votre client dispose désormais de l’ancien abonnement et du nouveau.</span><span class="sxs-lookup"><span data-stu-id="ececf-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="ececf-129">L’étape suivante consiste à réattribuer les licences aux utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="ececf-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="ececf-130">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="ececf-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ececf-131">Sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="ececf-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="ececf-132">Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="ececf-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="ececf-133">Sur la page **gérer les licences** , désactivez la case à cocher Dynamics 365 pour le plan Sales/Customer engagement de base (offre qualifiée) et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="ececf-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="ececf-134">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="ececf-134">Select **Submit**.</span></span> <span data-ttu-id="ececf-135">Vous effectuerez cette opération pour chaque utilisateur qui a besoin de la nouvelle licence.</span><span class="sxs-lookup"><span data-stu-id="ececf-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="ececf-136">Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="ececf-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="ececf-137">Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.</span><span class="sxs-lookup"><span data-stu-id="ececf-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ececf-138">Sur la page Détails de l’abonnement, définissez l’ancien abonnement sur **suspendu** , puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="ececf-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="ececf-139">L’ancien abonnement est maintenant suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="ececf-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="ececf-140">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="ececf-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ececf-141">Votre client n’aura aucuns frais supplémentaires pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="ececf-141">Your customer will incur no additional costs for the old subscription.</span></span>
