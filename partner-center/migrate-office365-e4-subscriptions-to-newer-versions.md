---
title: Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365 | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'édition Microsoft Office 365 Entreprise E4 n’est plus disponible depuis le 7 avril 2017. Découvrez comment migrer vos abonnements client vers des versions plus récentes d’Office 365.
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390878"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="06038-104">Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365</span><span class="sxs-lookup"><span data-stu-id="06038-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="06038-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="06038-105">**Applies to**</span></span>

-  <span data-ttu-id="06038-106">Centre pour partenaires</span><span class="sxs-lookup"><span data-stu-id="06038-106">Partner Center</span></span>

<span data-ttu-id="06038-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="06038-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="06038-108">Administrateur global</span><span class="sxs-lookup"><span data-stu-id="06038-108">Global admin</span></span>
-   <span data-ttu-id="06038-109">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="06038-109">User admin</span></span>
-   <span data-ttu-id="06038-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="06038-110">Admin agent</span></span>
-   <span data-ttu-id="06038-111">Commercial</span><span class="sxs-lookup"><span data-stu-id="06038-111">Sales agent</span></span>

<span data-ttu-id="06038-112">La formule Office 365 Entreprise E4 n’est plus disponible depuis le 7 avril 2017.</span><span class="sxs-lookup"><span data-stu-id="06038-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="06038-113">Vous ne pouvez plus acheter de nouveaux abonnements Office 365 E4 après cette date et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration.</span><span class="sxs-lookup"><span data-stu-id="06038-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="06038-114">Lorsque les abonnements E4 prendront fin, ils seront annulés.</span><span class="sxs-lookup"><span data-stu-id="06038-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="06038-115">Pour garantir la continuité des activités pour les clients, vous devez passer les clients ayant des abonnements E4 arrivant à expiration à une option de référence (SKU) prise en charge, répertoriée ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="06038-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="06038-116">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="06038-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="06038-117">Les références SKU commerciales et gouvernementales d’Office 365 Enterprise E4 sont retirées.</span><span class="sxs-lookup"><span data-stu-id="06038-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="06038-118">Sur la page des détails de l’abonnement, le statut de l'abonnement E4 « Renouvellements automatiques le [date] » est remplacé par « Expire le [date] ».</span><span class="sxs-lookup"><span data-stu-id="06038-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="06038-119">Si vous utilisez l’API (CREST ou Espace partenaires), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec la propriété de renouvellement automatique = False.</span><span class="sxs-lookup"><span data-stu-id="06038-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="06038-120">Les abonnements E4 seront définis sur renouvellement automatique = False le 7 avril 2017.</span><span class="sxs-lookup"><span data-stu-id="06038-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="06038-121">Vous pouvez passer les clients vers une nouvelle formule à tout moment.</span><span class="sxs-lookup"><span data-stu-id="06038-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="06038-122">Formules de remplacement pour l'édition Office 365 Entreprise E4</span><span class="sxs-lookup"><span data-stu-id="06038-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="06038-123">Vous pouvez choisir de conserver les mêmes fonctionnalités qu'avec E4 ou de faire bénéficier vos clients des nouvelles fonctions d'Office 365 et de Skype Entreprise Online.</span><span class="sxs-lookup"><span data-stu-id="06038-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="06038-124">Les détails de la tarification figurent sur la liste de prix et le tableau répertoriant les offres dans l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="06038-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="06038-125">Secure Productive Enterprise E3 ou Secure Productive Enterprise E5 peut être remplacé dans les options suivantes respectivement par Office 365 Entreprise E3 ou Office 365 Entreprise E5.</span><span class="sxs-lookup"><span data-stu-id="06038-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="06038-126">Option 1 : Office 365 Entreprise E5</span><span class="sxs-lookup"><span data-stu-id="06038-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="06038-127">Option 2 : Office 365 Entreprise E3 + Cloud PBX de Skype Entreprise</span><span class="sxs-lookup"><span data-stu-id="06038-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="06038-128">Option 3 : Office 365 Entreprise E3 + Skype Entreprise, ainsi que les licences d’accès client (parité de prix et de fonctionnalités avec E4)</span><span class="sxs-lookup"><span data-stu-id="06038-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="06038-129">Option 4 : Office 365 Entreprise E3</span><span class="sxs-lookup"><span data-stu-id="06038-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="06038-130">Composant</span><span class="sxs-lookup"><span data-stu-id="06038-130">Feature</span></span> | <span data-ttu-id="06038-131">Option 1</span><span class="sxs-lookup"><span data-stu-id="06038-131">Option 1</span></span> | <span data-ttu-id="06038-132">Option 2</span><span class="sxs-lookup"><span data-stu-id="06038-132">Option 2</span></span> | <span data-ttu-id="06038-133">Option 3</span><span class="sxs-lookup"><span data-stu-id="06038-133">Option 3</span></span> | <span data-ttu-id="06038-134">Option 4</span><span class="sxs-lookup"><span data-stu-id="06038-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="06038-135">Obtenir toutes les fonctionnalités incluses dans Office 365 Entreprise E4 ?</span><span class="sxs-lookup"><span data-stu-id="06038-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="06038-136">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-136">Yes</span></span> | <span data-ttu-id="06038-137">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-137">Yes</span></span> | <span data-ttu-id="06038-138">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-138">Yes</span></span> | <span data-ttu-id="06038-139">Non</span><span class="sxs-lookup"><span data-stu-id="06038-139">No</span></span> |
| <span data-ttu-id="06038-140">Numéros de téléphone gérés dans Office 365 ?</span><span class="sxs-lookup"><span data-stu-id="06038-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="06038-141">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-141">Yes</span></span> | <span data-ttu-id="06038-142">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-142">Yes</span></span> | <span data-ttu-id="06038-143">Non</span><span class="sxs-lookup"><span data-stu-id="06038-143">No</span></span> | <span data-ttu-id="06038-144">Non</span><span class="sxs-lookup"><span data-stu-id="06038-144">No</span></span> |
| <span data-ttu-id="06038-145">Numéros de téléphone gérés à la fois localement et dans Office 365 (déploiement hybride) ?</span><span class="sxs-lookup"><span data-stu-id="06038-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="06038-146">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-146">Yes</span></span> | <span data-ttu-id="06038-147">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-147">Yes</span></span> | <span data-ttu-id="06038-148">Non</span><span class="sxs-lookup"><span data-stu-id="06038-148">No</span></span> | <span data-ttu-id="06038-149">Non</span><span class="sxs-lookup"><span data-stu-id="06038-149">No</span></span> |
| <span data-ttu-id="06038-150">Option pour ajouter un plan d’appel vocal et RTC ?</span><span class="sxs-lookup"><span data-stu-id="06038-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="06038-151">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-151">Yes</span></span> | <span data-ttu-id="06038-152">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-152">Yes</span></span> | <span data-ttu-id="06038-153">Non</span><span class="sxs-lookup"><span data-stu-id="06038-153">No</span></span> | <span data-ttu-id="06038-154">Non</span><span class="sxs-lookup"><span data-stu-id="06038-154">No</span></span> |
| <span data-ttu-id="06038-155">Conférence RTC ?</span><span class="sxs-lookup"><span data-stu-id="06038-155">PSTN Conferencing?</span></span> | <span data-ttu-id="06038-156">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-156">Yes</span></span> | <span data-ttu-id="06038-157">Non</span><span class="sxs-lookup"><span data-stu-id="06038-157">No</span></span> | <span data-ttu-id="06038-158">Non</span><span class="sxs-lookup"><span data-stu-id="06038-158">No</span></span> | <span data-ttu-id="06038-159">Non</span><span class="sxs-lookup"><span data-stu-id="06038-159">No</span></span> |
| <span data-ttu-id="06038-160">Outils avancés de collaboration, d'analyse et de sécurité ?</span><span class="sxs-lookup"><span data-stu-id="06038-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="06038-161">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-161">Yes</span></span> | <span data-ttu-id="06038-162">Non</span><span class="sxs-lookup"><span data-stu-id="06038-162">No</span></span> | <span data-ttu-id="06038-163">Non</span><span class="sxs-lookup"><span data-stu-id="06038-163">No</span></span> | <span data-ttu-id="06038-164">Non</span><span class="sxs-lookup"><span data-stu-id="06038-164">No</span></span> |
| <span data-ttu-id="06038-165">Rapports interactifs, tableaux de bord et visualisations de données ?</span><span class="sxs-lookup"><span data-stu-id="06038-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="06038-166">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-166">Yes</span></span> | <span data-ttu-id="06038-167">Non</span><span class="sxs-lookup"><span data-stu-id="06038-167">No</span></span> | <span data-ttu-id="06038-168">Non</span><span class="sxs-lookup"><span data-stu-id="06038-168">No</span></span> | <span data-ttu-id="06038-169">Non</span><span class="sxs-lookup"><span data-stu-id="06038-169">No</span></span> | 
| <span data-ttu-id="06038-170">Plus de contrôle sur la sécurité des données et la conformité avec une confidentialité, une transparence et des contrôles utilisateur pointus intégrés ?</span><span class="sxs-lookup"><span data-stu-id="06038-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="06038-171">Oui</span><span class="sxs-lookup"><span data-stu-id="06038-171">Yes</span></span> | <span data-ttu-id="06038-172">Non</span><span class="sxs-lookup"><span data-stu-id="06038-172">No</span></span> | <span data-ttu-id="06038-173">Non</span><span class="sxs-lookup"><span data-stu-id="06038-173">No</span></span> | <span data-ttu-id="06038-174">Non</span><span class="sxs-lookup"><span data-stu-id="06038-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="06038-175">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="06038-175">Transition customers to new product plans</span></span>

<span data-ttu-id="06038-176">Microsoft offre en permanence de nouveaux produits et services à nos partenaires.</span><span class="sxs-lookup"><span data-stu-id="06038-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="06038-177">Dans ces cas, vous pouvez avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître.</span><span class="sxs-lookup"><span data-stu-id="06038-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="06038-178">La migration de clients depuis des références supprimées vers des références plus récentes doit respecter les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="06038-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="06038-179">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="06038-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="06038-180">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="06038-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="06038-181">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="06038-181">Cancel the old subscription</span></span>

<span data-ttu-id="06038-182">Suivez ces étapes pour migrer l’abonnement Office 365 Entreprise E4 d’un client vers l'une des options indiquées dans le tableau ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="06038-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="06038-183">Étape 1 : acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="06038-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="06038-184">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.</span><span class="sxs-lookup"><span data-stu-id="06038-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="06038-185">Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="06038-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="06038-186">Votre client doit maintenant avoir des abonnements anciens et nouveaux, l’ancien abonnement Office 365 Enterprise E4 et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="06038-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="06038-187">Étape 2 : réaffecter les licences des utilisateurs du client</span><span class="sxs-lookup"><span data-stu-id="06038-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="06038-188">Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="06038-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="06038-189">La page utilisateurs et licences du client s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="06038-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="06038-190">Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="06038-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="06038-191">Dans la page **Gérer les licences**, désactivez la case à cocher de la licence **Office 365 Entreprise E4**, puis sélectionnez une nouvelle formule de service pour l’abonnement auquel passe le client.</span><span class="sxs-lookup"><span data-stu-id="06038-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="06038-192">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="06038-192">Select **Submit**.</span></span> <span data-ttu-id="06038-193">Une page de confirmation indique les nouvelles licences attribuées.</span><span class="sxs-lookup"><span data-stu-id="06038-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="06038-194">Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.</span><span class="sxs-lookup"><span data-stu-id="06038-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="06038-195">Une fois les licences utilisateur attribuées au nouveau service, vous pouvez en toute sécurité annuler l'abonnement retiré au premier niveau du client.</span><span class="sxs-lookup"><span data-stu-id="06038-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="06038-196">Étape 3 : annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="06038-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="06038-197">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="06038-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="06038-198">Sélectionnez le client que vous voulez déplacer, puis l’abonnement à annuler.</span><span class="sxs-lookup"><span data-stu-id="06038-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="06038-199">Dans la page des détails de l’abonnement, définissez l'état d'abonnement sur **Suspendu**.</span><span class="sxs-lookup"><span data-stu-id="06038-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="06038-200">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="06038-200">Select **Submit**.</span></span>

<span data-ttu-id="06038-201">L’ancien abonnement est suspendu et le nouveau est activé.</span><span class="sxs-lookup"><span data-stu-id="06038-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="06038-202">L’abonnement suspendu est automatiquement désapprovisionné après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="06038-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="06038-203">Aucun frais n’est facturé au client pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="06038-203">The customer incurs no additional costs for the old subscription.</span></span>



 



