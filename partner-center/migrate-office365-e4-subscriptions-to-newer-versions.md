---
title: Migrer des abonnements Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition est mis hors service depuis le 7 avril 2017. Découvrez comment migrer vos abonnements client vers des versions plus récentes d’Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949042"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="2c913-104">Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365</span><span class="sxs-lookup"><span data-stu-id="2c913-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="2c913-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="2c913-105">**Applies to**</span></span>

-  <span data-ttu-id="2c913-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="2c913-106">Partner Center</span></span>

<span data-ttu-id="2c913-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="2c913-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="2c913-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="2c913-108">Global admin</span></span>
-   <span data-ttu-id="2c913-109">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2c913-109">User admin</span></span>
-   <span data-ttu-id="2c913-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="2c913-110">Admin agent</span></span>
-   <span data-ttu-id="2c913-111">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="2c913-111">Sales agent</span></span>

<span data-ttu-id="2c913-112">Le plan Office 365 Enterprise E4 est retiré, à compter du 7 avril 2017.</span><span class="sxs-lookup"><span data-stu-id="2c913-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="2c913-113">Vous ne pouvez plus acheter de nouveaux abonnements Office 365 E4 après cette date, et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="2c913-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2c913-114">Lorsque les abonnements E4 se terminent, ils sont annulés.</span><span class="sxs-lookup"><span data-stu-id="2c913-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="2c913-115">Pour garantir la continuité des clients, vous devez faire passer les clients avec des abonnements E4 arrivant à expiration à une option SKU prise en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="2c913-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2c913-116">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="2c913-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="2c913-117">Les références SKU commerciales et gouvernementales d’Office 365 Enterprise E4 sont retirées.</span><span class="sxs-lookup"><span data-stu-id="2c913-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="2c913-118">Sur la page de détails de l’abonnement, l’état de l’abonnement E4 est passé à « expire le [date] » de « auto Renews on [date] ».</span><span class="sxs-lookup"><span data-stu-id="2c913-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2c913-119">Si vous utilisez l’API (CREST ou Partner Center), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = false.</span><span class="sxs-lookup"><span data-stu-id="2c913-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="2c913-120">Les abonnements E4 seront configurés pour un renouvellement automatique = false en avril 7, 2017.</span><span class="sxs-lookup"><span data-stu-id="2c913-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="2c913-121">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="2c913-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="2c913-122">Plans de remplacement Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="2c913-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="2c913-123">Vous pouvez choisir de conserver la même fonctionnalité avec E4 ou de faire en sorte que vos clients tirent parti des fonctionnalités et fonctionnalités plus récentes dans Office 365 et Skype entreprise online.</span><span class="sxs-lookup"><span data-stu-id="2c913-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="2c913-124">Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c913-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="2c913-125">Secure Product Enterprise E3 ou Secure productive Enterprise E5 peut être remplacé par les options suivantes pour Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivement.</span><span class="sxs-lookup"><span data-stu-id="2c913-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="2c913-126">Option 1 : Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="2c913-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="2c913-127">Option 2 : Office 365 Enterprise E3 + PBX Cloud de Skype entreprise</span><span class="sxs-lookup"><span data-stu-id="2c913-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="2c913-128">Option 3 : Office 365 Enterprise E3 + licences d’accès client Skype entreprise plus (parité prix et fonctionnalité avec E4)</span><span class="sxs-lookup"><span data-stu-id="2c913-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="2c913-129">Option 4 : Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="2c913-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="2c913-130">Fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="2c913-130">Feature</span></span> | <span data-ttu-id="2c913-131">Option 1 :</span><span class="sxs-lookup"><span data-stu-id="2c913-131">Option 1</span></span> | <span data-ttu-id="2c913-132">Option 2 :</span><span class="sxs-lookup"><span data-stu-id="2c913-132">Option 2</span></span> | <span data-ttu-id="2c913-133">Option 3</span><span class="sxs-lookup"><span data-stu-id="2c913-133">Option 3</span></span> | <span data-ttu-id="2c913-134">Option 4</span><span class="sxs-lookup"><span data-stu-id="2c913-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="2c913-135">Bénéficier de toutes les fonctionnalités incluses dans Office 365 Enterprise E4 ?</span><span class="sxs-lookup"><span data-stu-id="2c913-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="2c913-136">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-136">Yes</span></span> | <span data-ttu-id="2c913-137">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-137">Yes</span></span> | <span data-ttu-id="2c913-138">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-138">Yes</span></span> | <span data-ttu-id="2c913-139">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-139">No</span></span> |
| <span data-ttu-id="2c913-140">Numéros de téléphone gérés dans Office 365 ?</span><span class="sxs-lookup"><span data-stu-id="2c913-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="2c913-141">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-141">Yes</span></span> | <span data-ttu-id="2c913-142">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-142">Yes</span></span> | <span data-ttu-id="2c913-143">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-143">No</span></span> | <span data-ttu-id="2c913-144">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-144">No</span></span> |
| <span data-ttu-id="2c913-145">Numéros de téléphone gérés localement et dans Office 365 (déploiement hybride) ?</span><span class="sxs-lookup"><span data-stu-id="2c913-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="2c913-146">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-146">Yes</span></span> | <span data-ttu-id="2c913-147">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-147">Yes</span></span> | <span data-ttu-id="2c913-148">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-148">No</span></span> | <span data-ttu-id="2c913-149">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-149">No</span></span> |
| <span data-ttu-id="2c913-150">Option permettant d’ajouter un plan d’appel vocal RTPC ?</span><span class="sxs-lookup"><span data-stu-id="2c913-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="2c913-151">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-151">Yes</span></span> | <span data-ttu-id="2c913-152">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-152">Yes</span></span> | <span data-ttu-id="2c913-153">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-153">No</span></span> | <span data-ttu-id="2c913-154">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-154">No</span></span> |
| <span data-ttu-id="2c913-155">La Conférence RTPC ?</span><span class="sxs-lookup"><span data-stu-id="2c913-155">PSTN Conferencing?</span></span> | <span data-ttu-id="2c913-156">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-156">Yes</span></span> | <span data-ttu-id="2c913-157">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-157">No</span></span> | <span data-ttu-id="2c913-158">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-158">No</span></span> | <span data-ttu-id="2c913-159">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-159">No</span></span> |
| <span data-ttu-id="2c913-160">Outils avancés pour la collaboration, l’analyse et la sécurité ?</span><span class="sxs-lookup"><span data-stu-id="2c913-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="2c913-161">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-161">Yes</span></span> | <span data-ttu-id="2c913-162">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-162">No</span></span> | <span data-ttu-id="2c913-163">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-163">No</span></span> | <span data-ttu-id="2c913-164">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-164">No</span></span> |
| <span data-ttu-id="2c913-165">Des rapports interactifs, des tableaux de bord et des visualisations de données ?</span><span class="sxs-lookup"><span data-stu-id="2c913-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="2c913-166">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-166">Yes</span></span> | <span data-ttu-id="2c913-167">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-167">No</span></span> | <span data-ttu-id="2c913-168">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-168">No</span></span> | <span data-ttu-id="2c913-169">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-169">No</span></span> | 
| <span data-ttu-id="2c913-170">Contrôle accru de la sécurité et de la conformité des données grâce à la confidentialité intégrée, à la transparence et aux contrôles utilisateur affinés ?</span><span class="sxs-lookup"><span data-stu-id="2c913-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="2c913-171">Oui</span><span class="sxs-lookup"><span data-stu-id="2c913-171">Yes</span></span> | <span data-ttu-id="2c913-172">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-172">No</span></span> | <span data-ttu-id="2c913-173">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-173">No</span></span> | <span data-ttu-id="2c913-174">Non</span><span class="sxs-lookup"><span data-stu-id="2c913-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2c913-175">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="2c913-175">Transition customers to new product plans</span></span>

<span data-ttu-id="2c913-176">Microsoft offre en permanence de nouveaux produits et services à nos partenaires.</span><span class="sxs-lookup"><span data-stu-id="2c913-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2c913-177">Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées.</span><span class="sxs-lookup"><span data-stu-id="2c913-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2c913-178">La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="2c913-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="2c913-179">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="2c913-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="2c913-180">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="2c913-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="2c913-181">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="2c913-181">Cancel the old subscription</span></span>

<span data-ttu-id="2c913-182">Suivez ces étapes pour migrer l’abonnement Office 365 Enterprise E4 d’un client vers l’une des options du tableau ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="2c913-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="2c913-183">Étape 1 : acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="2c913-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="2c913-184">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.</span><span class="sxs-lookup"><span data-stu-id="2c913-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2c913-185">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="2c913-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="2c913-186">Votre client doit maintenant avoir des abonnements anciens et nouveaux, l’ancien abonnement Office 365 Enterprise E4 et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2c913-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="2c913-187">Étape 2 : réattribuer les licences des utilisateurs du client</span><span class="sxs-lookup"><span data-stu-id="2c913-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="2c913-188">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="2c913-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="2c913-189">La page utilisateurs et licences du client s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="2c913-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2c913-190">Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="2c913-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2c913-191">Sur la page **gérer les licences** , désactivez la case à cocher **Office 365 Enterprise E4** et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="2c913-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="2c913-192">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="2c913-192">Select **Submit**.</span></span> <span data-ttu-id="2c913-193">Une page de confirmation indique les nouvelles licences attribuées.</span><span class="sxs-lookup"><span data-stu-id="2c913-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="2c913-194">Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.</span><span class="sxs-lookup"><span data-stu-id="2c913-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="2c913-195">Après avoir déplacé les licences utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client le plus élevé.</span><span class="sxs-lookup"><span data-stu-id="2c913-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="2c913-196">Étape 3 : annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="2c913-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="2c913-197">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="2c913-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2c913-198">Sélectionnez le client que vous souhaitez déplacer, puis sélectionnez l’abonnement que vous souhaitez annuler.</span><span class="sxs-lookup"><span data-stu-id="2c913-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="2c913-199">Dans la page Détails de l’abonnement, définissez l’état de l’abonnement sur **suspendu**.</span><span class="sxs-lookup"><span data-stu-id="2c913-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="2c913-200">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="2c913-200">Select **Submit**.</span></span>

<span data-ttu-id="2c913-201">L’ancien abonnement est suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="2c913-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="2c913-202">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="2c913-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2c913-203">Aucun frais n’est facturé au client pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c913-203">The customer incurs no additional costs for the old subscription.</span></span>



 



