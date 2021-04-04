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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132619"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="198d6-104">Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365</span><span class="sxs-lookup"><span data-stu-id="198d6-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="198d6-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="198d6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="198d6-106">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="198d6-106">Global admin</span></span>
- <span data-ttu-id="198d6-107">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="198d6-107">User management admin</span></span>
- <span data-ttu-id="198d6-108">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="198d6-108">Admin agent</span></span>
- <span data-ttu-id="198d6-109">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="198d6-109">Sales agent</span></span>

<span data-ttu-id="198d6-110">Le plan Office 365 Enterprise E4 est retiré, à compter du 7 avril 2017.</span><span class="sxs-lookup"><span data-stu-id="198d6-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="198d6-111">Vous ne pouvez plus acheter de nouveaux abonnements Office 365 E4 après cette date, et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="198d6-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="198d6-112">Lorsque les abonnements E4 se terminent, ils sont annulés.</span><span class="sxs-lookup"><span data-stu-id="198d6-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="198d6-113">Pour garantir la continuité des clients, vous devez faire passer les clients avec des abonnements E4 arrivant à expiration à une option SKU prise en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="198d6-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="198d6-114">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="198d6-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="198d6-115">Les références SKU commerciales et gouvernementales d’Office 365 Enterprise E4 sont retirées.</span><span class="sxs-lookup"><span data-stu-id="198d6-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="198d6-116">Sur la page de détails de l’abonnement, l’état de l’abonnement E4 est passé à « expire le [date] » de « auto Renews on [date] ».</span><span class="sxs-lookup"><span data-stu-id="198d6-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="198d6-117">Si vous utilisez l’API (CREST ou Partner Center), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = false.</span><span class="sxs-lookup"><span data-stu-id="198d6-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="198d6-118">Les abonnements E4 seront configurés pour un renouvellement automatique = false en avril 7, 2017.</span><span class="sxs-lookup"><span data-stu-id="198d6-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="198d6-119">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="198d6-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="198d6-120">Plans de remplacement Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="198d6-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="198d6-121">Vous pouvez choisir de conserver la même fonctionnalité avec E4 ou de faire en sorte que vos clients tirent parti des fonctionnalités et fonctionnalités plus récentes dans Office 365 et Skype entreprise online.</span><span class="sxs-lookup"><span data-stu-id="198d6-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="198d6-122">Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="198d6-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="198d6-123">Secure Product Enterprise E3 ou Secure productive Enterprise E5 peut être remplacé par les options suivantes pour Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivement.</span><span class="sxs-lookup"><span data-stu-id="198d6-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="198d6-124">Option 1 : Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="198d6-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="198d6-125">Option 2 : Office 365 Enterprise E3 + PBX Cloud de Skype entreprise</span><span class="sxs-lookup"><span data-stu-id="198d6-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="198d6-126">Option 3 : Office 365 Enterprise E3 + licences d’accès client Skype entreprise plus (parité prix et fonctionnalité avec E4)</span><span class="sxs-lookup"><span data-stu-id="198d6-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="198d6-127">Option 4 : Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="198d6-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="198d6-128">Fonctionnalité</span><span class="sxs-lookup"><span data-stu-id="198d6-128">Feature</span></span> | <span data-ttu-id="198d6-129">Option 1 :</span><span class="sxs-lookup"><span data-stu-id="198d6-129">Option 1</span></span> | <span data-ttu-id="198d6-130">Option 2 :</span><span class="sxs-lookup"><span data-stu-id="198d6-130">Option 2</span></span> | <span data-ttu-id="198d6-131">Option 3</span><span class="sxs-lookup"><span data-stu-id="198d6-131">Option 3</span></span> | <span data-ttu-id="198d6-132">Option 4</span><span class="sxs-lookup"><span data-stu-id="198d6-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="198d6-133">Bénéficier de toutes les fonctionnalités incluses dans Office 365 Enterprise E4 ?</span><span class="sxs-lookup"><span data-stu-id="198d6-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="198d6-134">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-134">Yes</span></span> | <span data-ttu-id="198d6-135">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-135">Yes</span></span> | <span data-ttu-id="198d6-136">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-136">Yes</span></span> | <span data-ttu-id="198d6-137">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-137">No</span></span> |
| <span data-ttu-id="198d6-138">Numéros de téléphone gérés dans Office 365 ?</span><span class="sxs-lookup"><span data-stu-id="198d6-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="198d6-139">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-139">Yes</span></span> | <span data-ttu-id="198d6-140">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-140">Yes</span></span> | <span data-ttu-id="198d6-141">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-141">No</span></span> | <span data-ttu-id="198d6-142">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-142">No</span></span> |
| <span data-ttu-id="198d6-143">Numéros de téléphone gérés localement et dans Office 365 (déploiement hybride) ?</span><span class="sxs-lookup"><span data-stu-id="198d6-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="198d6-144">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-144">Yes</span></span> | <span data-ttu-id="198d6-145">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-145">Yes</span></span> | <span data-ttu-id="198d6-146">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-146">No</span></span> | <span data-ttu-id="198d6-147">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-147">No</span></span> |
| <span data-ttu-id="198d6-148">Option permettant d’ajouter un plan d’appel vocal RTPC ?</span><span class="sxs-lookup"><span data-stu-id="198d6-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="198d6-149">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-149">Yes</span></span> | <span data-ttu-id="198d6-150">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-150">Yes</span></span> | <span data-ttu-id="198d6-151">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-151">No</span></span> | <span data-ttu-id="198d6-152">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-152">No</span></span> |
| <span data-ttu-id="198d6-153">La Conférence RTPC ?</span><span class="sxs-lookup"><span data-stu-id="198d6-153">PSTN Conferencing?</span></span> | <span data-ttu-id="198d6-154">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-154">Yes</span></span> | <span data-ttu-id="198d6-155">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-155">No</span></span> | <span data-ttu-id="198d6-156">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-156">No</span></span> | <span data-ttu-id="198d6-157">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-157">No</span></span> |
| <span data-ttu-id="198d6-158">Outils avancés pour la collaboration, l’analyse et la sécurité ?</span><span class="sxs-lookup"><span data-stu-id="198d6-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="198d6-159">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-159">Yes</span></span> | <span data-ttu-id="198d6-160">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-160">No</span></span> | <span data-ttu-id="198d6-161">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-161">No</span></span> | <span data-ttu-id="198d6-162">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-162">No</span></span> |
| <span data-ttu-id="198d6-163">Des rapports interactifs, des tableaux de bord et des visualisations de données ?</span><span class="sxs-lookup"><span data-stu-id="198d6-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="198d6-164">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-164">Yes</span></span> | <span data-ttu-id="198d6-165">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-165">No</span></span> | <span data-ttu-id="198d6-166">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-166">No</span></span> | <span data-ttu-id="198d6-167">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-167">No</span></span> | 
| <span data-ttu-id="198d6-168">Contrôle accru de la sécurité et de la conformité des données grâce à la confidentialité intégrée, à la transparence et aux contrôles utilisateur affinés ?</span><span class="sxs-lookup"><span data-stu-id="198d6-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="198d6-169">Oui</span><span class="sxs-lookup"><span data-stu-id="198d6-169">Yes</span></span> | <span data-ttu-id="198d6-170">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-170">No</span></span> | <span data-ttu-id="198d6-171">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-171">No</span></span> | <span data-ttu-id="198d6-172">Non</span><span class="sxs-lookup"><span data-stu-id="198d6-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="198d6-173">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="198d6-173">Transition customers to new product plans</span></span>

<span data-ttu-id="198d6-174">Microsoft offre en permanence de nouveaux produits et services à nos partenaires.</span><span class="sxs-lookup"><span data-stu-id="198d6-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="198d6-175">Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées.</span><span class="sxs-lookup"><span data-stu-id="198d6-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="198d6-176">La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="198d6-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="198d6-177">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="198d6-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="198d6-178">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="198d6-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="198d6-179">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="198d6-179">Cancel the old subscription</span></span>

<span data-ttu-id="198d6-180">Suivez ces étapes pour migrer l’abonnement Office 365 Enterprise E4 d’un client vers l’une des options du tableau ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="198d6-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="198d6-181">Étape 1 : acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="198d6-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="198d6-182">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.</span><span class="sxs-lookup"><span data-stu-id="198d6-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="198d6-183">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="198d6-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="198d6-184">Votre client doit maintenant avoir des abonnements anciens et nouveaux, l’ancien abonnement Office 365 Enterprise E4 et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="198d6-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="198d6-185">Étape 2 : réattribuer les licences des utilisateurs du client</span><span class="sxs-lookup"><span data-stu-id="198d6-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="198d6-186">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="198d6-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="198d6-187">La page utilisateurs et licences du client s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="198d6-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="198d6-188">Pour réaffecter des licences utilisateur, sélectionnez l’utilisateur à réassigner, puis sélectionnez **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="198d6-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="198d6-189">Sur la page **gérer les licences** , désactivez la case à cocher **Office 365 Enterprise E4** et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="198d6-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="198d6-190">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="198d6-190">Select **Submit**.</span></span> <span data-ttu-id="198d6-191">Une page de confirmation indique les nouvelles licences attribuées.</span><span class="sxs-lookup"><span data-stu-id="198d6-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="198d6-192">Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.</span><span class="sxs-lookup"><span data-stu-id="198d6-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="198d6-193">Après avoir déplacé les licences utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client le plus élevé.</span><span class="sxs-lookup"><span data-stu-id="198d6-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="198d6-194">Étape 3 : annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="198d6-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="198d6-195">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="198d6-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="198d6-196">Sélectionnez le client que vous souhaitez déplacer, puis sélectionnez l’abonnement que vous souhaitez annuler.</span><span class="sxs-lookup"><span data-stu-id="198d6-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="198d6-197">Dans la page Détails de l’abonnement, définissez l’état de l’abonnement sur **suspendu**.</span><span class="sxs-lookup"><span data-stu-id="198d6-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="198d6-198">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="198d6-198">Select **Submit**.</span></span>

<span data-ttu-id="198d6-199">L’ancien abonnement est suspendu et le nouvel abonnement est actif.</span><span class="sxs-lookup"><span data-stu-id="198d6-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="198d6-200">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="198d6-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="198d6-201">Aucun frais n’est facturé au client pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="198d6-201">The customer incurs no additional costs for the old subscription.</span></span>



 



