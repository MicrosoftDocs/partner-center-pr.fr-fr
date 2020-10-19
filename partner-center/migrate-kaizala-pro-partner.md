---
title: Migrer les abonnements Kaizala Pro vers Microsoft365
description: Découvrez comment migrer des abonnements Kaizala Pro vers des versions Microsoft365 ou Office 365. Lisez cet article pour plus d’informations sur la transition de vos clients.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175176"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="e797b-104">Migrer des abonnements Kaizala Pro autonomes vers des versions Microsoft365 ou Office 365</span><span class="sxs-lookup"><span data-stu-id="e797b-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="e797b-105">À compter du 1er juillet 2020, Microsoft met fin aux ventes du service autonome Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="e797b-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="e797b-106">Les clients ne seront plus en mesure d’acheter de nouveaux abonnements Kaizala Pro après cette date, et les abonnements Kaizala Pro existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.</span><span class="sxs-lookup"><span data-stu-id="e797b-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="e797b-107">Pour garantir la continuité des clients, vous devez faire en sorte que les clients qui expirent les abonnements Kaizala Pro autonomes soient pris en charge, comme indiqué ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="e797b-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="e797b-108">Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.</span><span class="sxs-lookup"><span data-stu-id="e797b-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="e797b-109">Si vous utilisez l’API (à la fois CREST ou Partner Center), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique définie sur false : `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="e797b-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="e797b-110">Les abonnements E4 seront définis `auto renew=False` sur le 1er juillet 2020.</span><span class="sxs-lookup"><span data-stu-id="e797b-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="e797b-111">Vous pouvez déplacer les clients vers un nouveau plan à tout moment.</span><span class="sxs-lookup"><span data-stu-id="e797b-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="e797b-112">Plans de remplacement autonomes Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="e797b-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="e797b-113">Avec les nouveaux plans, vos clients peuvent tirer parti des fonctionnalités et fonctionnalités plus récentes dans Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e797b-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="e797b-114">Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e797b-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="e797b-115">[**Microsoft 365 pour les entreprises**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), notamment :</span><span class="sxs-lookup"><span data-stu-id="e797b-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="e797b-116">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="e797b-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="e797b-117">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="e797b-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="e797b-118">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="e797b-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="e797b-119">[**Microsoft 365 pour la Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), notamment :</span><span class="sxs-lookup"><span data-stu-id="e797b-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="e797b-120">Microsoft 365 F3 (anciennement Microsoft 365 F1) et Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="e797b-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="e797b-121">[**Microsoft 365 pour les entreprises**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), notamment :</span><span class="sxs-lookup"><span data-stu-id="e797b-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="e797b-122">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="e797b-122">Office 365 E1</span></span>
   - <span data-ttu-id="e797b-123">Microsoft 365 E3 et Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="e797b-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="e797b-124">Microsoft 365 E5 et Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="e797b-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="e797b-125">[**Microsoft 365 pour l’éducation**](https://www.microsoft.com/education/buy-license/microsoft365), notamment :</span><span class="sxs-lookup"><span data-stu-id="e797b-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="e797b-126">Microsoft 365 A1 et Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="e797b-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="e797b-127">Microsoft 365 A3 et Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="e797b-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="e797b-128">Microsoft 365 A5 et Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="e797b-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="e797b-129">Accompagner les clients vers les nouvelles formules de produit</span><span class="sxs-lookup"><span data-stu-id="e797b-129">Transition customers to new product plans</span></span>

<span data-ttu-id="e797b-130">Microsoft offre en permanence de nouveaux produits et services à nos partenaires.</span><span class="sxs-lookup"><span data-stu-id="e797b-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="e797b-131">Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées.</span><span class="sxs-lookup"><span data-stu-id="e797b-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="e797b-132">La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e797b-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="e797b-133">R.</span><span class="sxs-lookup"><span data-stu-id="e797b-133">A.</span></span> <span data-ttu-id="e797b-134">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="e797b-134">Purchase the new subscription</span></span>

<span data-ttu-id="e797b-135">B.</span><span class="sxs-lookup"><span data-stu-id="e797b-135">B.</span></span> <span data-ttu-id="e797b-136">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="e797b-136">Reassign current user licenses</span></span>

<span data-ttu-id="e797b-137">C.</span><span class="sxs-lookup"><span data-stu-id="e797b-137">C.</span></span> <span data-ttu-id="e797b-138">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="e797b-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="e797b-139">Migrer vos clients vers de nouveaux plans</span><span class="sxs-lookup"><span data-stu-id="e797b-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="e797b-140">R.</span><span class="sxs-lookup"><span data-stu-id="e797b-140">A.</span></span> <span data-ttu-id="e797b-141">Acheter le nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="e797b-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="e797b-142">Pour acheter le nouvel abonnement, dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.</span><span class="sxs-lookup"><span data-stu-id="e797b-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="e797b-143">Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="e797b-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="e797b-144">Votre client doit maintenant avoir les anciens et les nouveaux abonnements, l’ancien abonnement Kaizala Pro standalone et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 entreprise F1.</span><span class="sxs-lookup"><span data-stu-id="e797b-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="e797b-145">B.</span><span class="sxs-lookup"><span data-stu-id="e797b-145">B.</span></span> <span data-ttu-id="e797b-146">Réaffecter les licences utilisateur actuelles</span><span class="sxs-lookup"><span data-stu-id="e797b-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="e797b-147">Pour réaffecter les licences des utilisateurs du client, dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous déplacez, puis sélectionnez **utilisateurs et licences**.</span><span class="sxs-lookup"><span data-stu-id="e797b-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="e797b-148">La page utilisateurs et licences du client s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="e797b-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="e797b-149">Pour réaffecter la licence utilisateur, sélectionnez l’utilisateur à réassigner, puis sélectionnez **gérer les licences**.</span><span class="sxs-lookup"><span data-stu-id="e797b-149">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="e797b-150">Sur la page **gérer les licences** , désactivez la case à cocher licence autonome Kaizala Pro, puis sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.</span><span class="sxs-lookup"><span data-stu-id="e797b-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="e797b-151">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="e797b-151">Select **Submit**.</span></span> <span data-ttu-id="e797b-152">Une page de confirmation indique les nouvelles licences attribuées.</span><span class="sxs-lookup"><span data-stu-id="e797b-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="e797b-153">Poursuivez ce même processus pour les autres utilisateurs qui ont besoin d’attributions de licence.</span><span class="sxs-lookup"><span data-stu-id="e797b-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="e797b-154">C.</span><span class="sxs-lookup"><span data-stu-id="e797b-154">C.</span></span> <span data-ttu-id="e797b-155">Annuler l’ancien abonnement</span><span class="sxs-lookup"><span data-stu-id="e797b-155">Cancel old subscription</span></span>

<span data-ttu-id="e797b-156">Après avoir déplacé la licence utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client.</span><span class="sxs-lookup"><span data-stu-id="e797b-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="e797b-157">Dans le menu **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="e797b-157">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="e797b-158">Sélectionnez le client dont vous annulez l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="e797b-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="e797b-159">Dans la page Détails de l’abonnement, définissez l’abonnement sur **suspendu**.</span><span class="sxs-lookup"><span data-stu-id="e797b-159">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="e797b-160">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="e797b-160">Select **Submit**.</span></span>

<span data-ttu-id="e797b-161">L’ancien abonnement est suspendu et le nouveau est activé.</span><span class="sxs-lookup"><span data-stu-id="e797b-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="e797b-162">L’abonnement suspendu est désapprovisionné automatiquement après 120 jours.</span><span class="sxs-lookup"><span data-stu-id="e797b-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="e797b-163">Aucun frais n’est facturé au client pour l’ancien abonnement.</span><span class="sxs-lookup"><span data-stu-id="e797b-163">The customer incurs no additional costs for the old subscription.</span></span>
