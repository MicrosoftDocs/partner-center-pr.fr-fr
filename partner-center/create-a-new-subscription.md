---
title: Créer des abonnements clients dans l’espace partenaires
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment vendre à vos clients des abonnements à des produits publiés par Microsoft, ainsi qu’à des produits SaaS publiés par des ISV tiers.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 66c8b490e69e9b03ec0db213ca2a5baf3d42635e
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527802"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="c3385-103">Créer, suspendre ou annuler des abonnements client</span><span class="sxs-lookup"><span data-stu-id="c3385-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="c3385-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="c3385-104">**Applies to**</span></span>

- <span data-ttu-id="c3385-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c3385-105">Partner Center</span></span>
- <span data-ttu-id="c3385-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c3385-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="c3385-107">Partenaires fournisseurs de solutions cloud</span><span class="sxs-lookup"><span data-stu-id="c3385-107">CSP partners</span></span>

<span data-ttu-id="c3385-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="c3385-108">**Appropriate roles**</span></span>

- <span data-ttu-id="c3385-109">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="c3385-109">Admin agent</span></span>
- <span data-ttu-id="c3385-110">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="c3385-110">Billing admin</span></span>
- <span data-ttu-id="c3385-111">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="c3385-111">Global admin</span></span>
- <span data-ttu-id="c3385-112">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="c3385-112">Helpdesk agent</span></span>
- <span data-ttu-id="c3385-113">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="c3385-113">Sales agent</span></span>

<span data-ttu-id="c3385-114">Une fois que vous avez créé un enregistrement de votre client dans l’Espace partenaires, vous pouvez lui vendre des abonnements aux produits figurant dans le catalogue.</span><span class="sxs-lookup"><span data-stu-id="c3385-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="c3385-115">Cela comprend les produits publiés par Microsoft, ainsi que les produits SaaS (Software as a service) publiés par des éditeurs de logiciels indépendants tiers sur la place de [marché commerciale](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="c3385-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="c3385-116">Certaines offres sont limitées à un seul abonnement par client.</span><span class="sxs-lookup"><span data-stu-id="c3385-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="c3385-117">Pour voir la liste des offres limitées, consultez la page Tarification et offres de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c3385-118">En tant que partenaire dans le programme CSP, vous pouvez uniquement acheter des abonnements Saas **basés sur une licence** auprès d’éditeurs ISV au sein de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="c3385-119">Cela signifie que vous pouvez acheter une offre SaaS basée sur une **licence** que l’éditeur ISV met à votre disposition, y compris les [offres exclusives](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) auxquelles vous avez accès.</span><span class="sxs-lookup"><span data-stu-id="c3385-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="c3385-120">Pour acheter ou gérer d’autres offres de la place de marché commercial auprès d’éditeurs de logiciels (ISV) (telles que des offres basées sur **l’utilisation**, limitées ou à la consommation impliquant des applications, des conteneurs ou des machines virtuelles Azure), vous devez accéder au [portail de gestion Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c3385-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="c3385-121">Pour plus d’informations, consultez acheter des produits de la place de [marché commercial](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="c3385-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="c3385-122">Créer un abonnement</span><span class="sxs-lookup"><span data-stu-id="c3385-122">Create a new subscription</span></span>

1. <span data-ttu-id="c3385-123">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c3385-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c3385-124">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c3385-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c3385-125">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="c3385-125">Select **Add subscription**.</span></span> <span data-ttu-id="c3385-126">L’onglet **services en ligne** affiche toutes les offres SaaS disponibles sur la place de marché.</span><span class="sxs-lookup"><span data-stu-id="c3385-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="c3385-127">Pour afficher uniquement certains types d’abonnements, effectuez les sélections dans les filtres disponibles :</span><span class="sxs-lookup"><span data-stu-id="c3385-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="c3385-128">**Éditeur**: choisissez **Microsoft** pour afficher uniquement les offres de Microsoft ou le **partenaire** pour consulter les produits de la place de marché commercialisés publiés par les éditeurs de logiciels indépendants.</span><span class="sxs-lookup"><span data-stu-id="c3385-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="c3385-129">**Type de facturation**: sélectionnez le type de facturation d’abonnement que vous souhaitez utiliser : **licence** ou **utilisation**.</span><span class="sxs-lookup"><span data-stu-id="c3385-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="c3385-130">Consultez [facturation basée sur une licence](license-based-billing.md) pour obtenir des informations qui vous aideront à déterminer la fréquence de facturation mensuelle et annuelle.</span><span class="sxs-lookup"><span data-stu-id="c3385-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="c3385-131">**Catégorie**: choisissez **Enterprise**, **Small Business**ou **version d’évaluation**.</span><span class="sxs-lookup"><span data-stu-id="c3385-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="c3385-132">Pour obtenir des informations sur les abonnements d’essai, consultez [Proposer à vos clients des abonnements d’essai aux produits Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="c3385-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="c3385-133">Sélectionnez les abonnements de produits que vous souhaitez acheter pour votre client.</span><span class="sxs-lookup"><span data-stu-id="c3385-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="c3385-134">Les produits que vous voyez dépendent du type de segment client (éducation, gouvernement, etc.) et des filtres que vous avez appliqués.</span><span class="sxs-lookup"><span data-stu-id="c3385-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="c3385-135">Certaines offres affichées sur la place de marché ne sont pas toujours disponibles pour un client spécifique ou un partenaire CSP spécifique.</span><span class="sxs-lookup"><span data-stu-id="c3385-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="c3385-136">Cela peut être dû aux raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3385-136">This can be because:</span></span>

   - <span data-ttu-id="c3385-137">Le client a déjà un abonnement à ce produit et n’est autorisé qu’un seul</span><span class="sxs-lookup"><span data-stu-id="c3385-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="c3385-138">L’abonnement du client a peut-être été suspendu (dans ce cas, vous pouvez réactiver l’abonnement au lieu d’en acheter un nouveau.)</span><span class="sxs-lookup"><span data-stu-id="c3385-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="c3385-139">Pour les offres SaaS ISV, il peut y avoir plusieurs raisons pour lesquelles l’offre n’est pas disponible à l’achat : l’ISV peut ne pas prendre en charge le pays ou la région de facturation du client. l’éditeur de logiciels indépendant peut avoir choisi de ne pas rendre l’offre disponible par le biais du programme CSP. ou, l’ISV a peut-être rendu l’offre [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) uniquement à certains partenaires CSP.</span><span class="sxs-lookup"><span data-stu-id="c3385-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="c3385-140">L’offre ISV n’est pas non plus utilisable via l’espace partenaires (par exemple, des conteneurs ou des offres basées sur l’utilisation).</span><span class="sxs-lookup"><span data-stu-id="c3385-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="c3385-141">Pour chaque abonnement que vous souhaitez ajouter, entrez le nombre de licences (si nécessaire), puis sélectionnez **Ajouter au panier**.</span><span class="sxs-lookup"><span data-stu-id="c3385-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="c3385-142">Lorsque vous avez terminé d’ajouter des abonnements, sélectionnez **passer en revue** et passer en revue votre commande.</span><span class="sxs-lookup"><span data-stu-id="c3385-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="c3385-143">Une fois que vous avez consulté vos commandes et que vous êtes prêt à acheter ces abonnements, sélectionnez **acheter**.</span><span class="sxs-lookup"><span data-stu-id="c3385-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="c3385-144">Une fois que vous avez acheté un abonnement pour un client, voici ce qui se produit :</span><span class="sxs-lookup"><span data-stu-id="c3385-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="c3385-145">Vous pouvez consulter ou modifier l’abonnement en sélectionnant le nom de l’abonnement dans la page **abonnements** du client.</span><span class="sxs-lookup"><span data-stu-id="c3385-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="c3385-146">À partir de là, vous pouvez sélectionner des licences de module complémentaire, le cas échéant, modifier le nombre de licences ou suspendre l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3385-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="c3385-147">**Pour les abonnements ISV SaaS (basés sur une licence) :**</span><span class="sxs-lookup"><span data-stu-id="c3385-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="c3385-148">Vous recevrez un lien vers le site de l’éditeur ISV.</span><span class="sxs-lookup"><span data-stu-id="c3385-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="c3385-149">Ce lien doit vous aider à effectuer la configuration du déploiement ou du compte de l’abonnement du client.</span><span class="sxs-lookup"><span data-stu-id="c3385-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="c3385-150">Ni vous ni votre client ne recevrez un e-mail contenant des instructions pour terminer l’installation/la configuration de compte pour ce type d’abonnement ISV.)</span><span class="sxs-lookup"><span data-stu-id="c3385-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="c3385-151">Si votre abonnement est fourni avec une version d’évaluation gratuite de 30 jours, la période d’essai gratuite sera appliquée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="c3385-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="c3385-152">En tant que partenaire dans le programme CSP, vous ne pouvez pas renoncer à la période d’évaluation gratuite sur les offres que vous achetez pour les clients.</span><span class="sxs-lookup"><span data-stu-id="c3385-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="c3385-153">Une fois la période d’essai gratuite terminée, la durée de l’abonnement commence et l’abonnement est converti en état payant.</span><span class="sxs-lookup"><span data-stu-id="c3385-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="c3385-154">L’abonnement est ensuite renouvelé automatiquement en fonction de la même planification.</span><span class="sxs-lookup"><span data-stu-id="c3385-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="c3385-155">Mettre à jour les abonnements avec des modules complémentaires</span><span class="sxs-lookup"><span data-stu-id="c3385-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="c3385-156">Pour acheter un module complémentaire, le client doit d’abord disposer d’un abonnement de base actif.</span><span class="sxs-lookup"><span data-stu-id="c3385-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="c3385-157">Vous ne pouvez pas acheter des modules complémentaires par le biais du catalogue.</span><span class="sxs-lookup"><span data-stu-id="c3385-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="c3385-158">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c3385-159">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c3385-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c3385-160">Choisissez l’abonnement que vous souhaitez gérer.</span><span class="sxs-lookup"><span data-stu-id="c3385-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c3385-161">Sous la section **État** , vous trouverez la liste des modules complémentaires disponibles pour l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3385-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="c3385-162">Mettez à jour le nombre de licences pour chaque module complémentaire requis.</span><span class="sxs-lookup"><span data-stu-id="c3385-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="c3385-163">Ensuite, **envoyez** vos modifications.</span><span class="sxs-lookup"><span data-stu-id="c3385-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="c3385-164">La possibilité d’acheter des modules complémentaires via l’espace partenaires n’est disponible que pour les fournisseurs directs et indirects.</span><span class="sxs-lookup"><span data-stu-id="c3385-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="c3385-165">Seuls les modules complémentaires éligibles sont affichés en fonction des exigences de base et de la disponibilité régionale.</span><span class="sxs-lookup"><span data-stu-id="c3385-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="c3385-166">Pour plus d’informations sur la tarification et les offres, reportez-vous à la matrice de l’offre du revendeur Cloud.</span><span class="sxs-lookup"><span data-stu-id="c3385-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="c3385-167">La suspension de l’abonnement de base interrompt également tous les modules complémentaires associés.</span><span class="sxs-lookup"><span data-stu-id="c3385-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="c3385-168">Les dates de début des modules complémentaires s’alignent sur l’abonnement de base et les frais sont calculés à partir de la date de début et de la date de fin des frais avec des frais au prorata sur la première facture.</span><span class="sxs-lookup"><span data-stu-id="c3385-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="c3385-169">Pour plus d’informations, consultez [facturation basée sur une licence](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="c3385-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="c3385-170">Suspendre ou annuler un abonnement</span><span class="sxs-lookup"><span data-stu-id="c3385-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="c3385-171">Les partenaires peuvent suspendre ou annuler un abonnement à la demande du client ou dans les cas de fraude ou de défaut de paiement.</span><span class="sxs-lookup"><span data-stu-id="c3385-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="c3385-172">Suspendre un abonnement</span><span class="sxs-lookup"><span data-stu-id="c3385-172">Suspend a subscription</span></span>

<span data-ttu-id="c3385-173">Lorsque vous attribuez à un abonnement l’état **Suspendu**, les utilisateurs ne peuvent plus se connecter aux services ou y accéder.</span><span class="sxs-lookup"><span data-stu-id="c3385-173">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="c3385-174">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c3385-175">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c3385-175">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c3385-176">Choisissez l’abonnement que vous souhaitez gérer.</span><span class="sxs-lookup"><span data-stu-id="c3385-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c3385-177">Dans la section **État**, choisissez **Suspendu**.</span><span class="sxs-lookup"><span data-stu-id="c3385-177">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="c3385-178">Ensuite, **envoyez** vos modifications.</span><span class="sxs-lookup"><span data-stu-id="c3385-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c3385-179">Toutes les données seront supprimées, sauf si l’abonnement est réactivé dans les 90 jours, ou 90 jours en plus du nombre de jours écoulés entre la date d'ouverture du compte et la première période de facturation (120 jours maximum).</span><span class="sxs-lookup"><span data-stu-id="c3385-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="c3385-180">Lorsque vous suspendez un abonnement, la date affichée sous le bouton **Suspendu** indique quand l’abonnement va automatiquement expirer si vous ne le réactivez pas.</span><span class="sxs-lookup"><span data-stu-id="c3385-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="c3385-181">Annuler un abonnement</span><span class="sxs-lookup"><span data-stu-id="c3385-181">Cancel a subscription</span></span>

<span data-ttu-id="c3385-182">Vous avez la possibilité d’annuler les abonnements SaaS basés sur des licences à partir d’éditeurs ISV tiers au sein de la place de [marché commerciale](csp-commercial-marketplace-overview.md)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="c3385-183">Tant que vous annulez l’opération pendant la période d’annulation, vous recevrez un remboursement intégral.</span><span class="sxs-lookup"><span data-stu-id="c3385-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="c3385-184">Pour les éditeurs de logiciels, les offres sont facturées tous les mois :</span><span class="sxs-lookup"><span data-stu-id="c3385-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="c3385-185">Si vous annulez moins de 24 heures après avoir passé la commande, vous recevrez un crédit complet sur la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="c3385-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c3385-186">Si vous annulez plus de 24 heures après avoir passé la commande, l’annulation sera planifiée pour être renouvelée.</span><span class="sxs-lookup"><span data-stu-id="c3385-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c3385-187">Pour les offres facturées annuellement :</span><span class="sxs-lookup"><span data-stu-id="c3385-187">For offers billed annually:</span></span>

- <span data-ttu-id="c3385-188">Si vous annulez moins de 14 jours après avoir placé la commande, vous recevrez un crédit complet sur la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="c3385-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c3385-189">Si vous annulez plus de 14 jours après avoir placé la commande, l’annulation sera planifiée au renouvellement.</span><span class="sxs-lookup"><span data-stu-id="c3385-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c3385-190">Une fois ces périodes supérieures, vous ne verrez plus l’option permettant d’annuler l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3385-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="c3385-191">Les services ISV tiers basés sur l’utilisation et contrôlés (qui utilisent des machines virtuelles ou des conteneurs, par exemple) ne peuvent pas être retournés.</span><span class="sxs-lookup"><span data-stu-id="c3385-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="c3385-192">Les services basés sur l’utilisation peuvent être désapprovisionnés en tant que méthode d’annulation.</span><span class="sxs-lookup"><span data-stu-id="c3385-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="c3385-193">Étant donné que les frais sont facturés après utilisation, ces services ne peuvent pas être remboursés.</span><span class="sxs-lookup"><span data-stu-id="c3385-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="c3385-194">Pour annuler un abonnement SaaS basé sur une licence auprès d’un éditeur de logiciels indépendant, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c3385-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="c3385-195">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c3385-196">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c3385-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c3385-197">Recherchez l’abonnement que vous souhaitez annuler.</span><span class="sxs-lookup"><span data-stu-id="c3385-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="c3385-198">Dans la colonne **État** , sélectionnez **Annuler**.</span><span class="sxs-lookup"><span data-stu-id="c3385-198">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="c3385-199">Ensuite, **envoyez** vos modifications.</span><span class="sxs-lookup"><span data-stu-id="c3385-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c3385-200">Si une boîte de dialogue s’affiche, renseignez les détails pertinents, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="c3385-200">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="c3385-201">Pour confirmer l’annulation, sélectionnez **Oui, annuler**.</span><span class="sxs-lookup"><span data-stu-id="c3385-201">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="c3385-202">Vous pouvez également choisir d’annuler un abonnement à la place de marché Azure à l’aide d’API.</span><span class="sxs-lookup"><span data-stu-id="c3385-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="c3385-203">Pour ce faire, consultez [annuler un abonnement Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="c3385-203">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="c3385-204">Choisir de renouveler automatiquement un abonnement à la place marché commerciale</span><span class="sxs-lookup"><span data-stu-id="c3385-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="c3385-205">Par défaut, les abonnements actifs sont définis pour se renouveler automatiquement à l’expiration de la période d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3385-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="c3385-206">Pour les [abonnements aux produits de la place de marché commercial](csp-commercial-marketplace-overview.md), vous pouvez éventuellement choisir de ne pas renouveler automatiquement l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c3385-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="c3385-207">Pour arrêter le renouvellement automatique d’un abonnement au marché commercial actif :</span><span class="sxs-lookup"><span data-stu-id="c3385-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="c3385-208">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c3385-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c3385-209">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c3385-209">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c3385-210">Sélectionnez **Abonnements**.</span><span class="sxs-lookup"><span data-stu-id="c3385-210">Select **Subscriptions**.</span></span> <span data-ttu-id="c3385-211">Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.</span><span class="sxs-lookup"><span data-stu-id="c3385-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="c3385-212">Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez modifier.</span><span class="sxs-lookup"><span data-stu-id="c3385-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="c3385-213">Dans la page Détails de l’abonnement, recherchez la section **État** et désactivez la case à cocher **renouvellement automatique** .</span><span class="sxs-lookup"><span data-stu-id="c3385-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="c3385-214">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="c3385-214">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c3385-215">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c3385-215">Next steps</span></span>

- [<span data-ttu-id="c3385-216">Acheter des produits de la place de marché commerciale pour vos clients</span><span class="sxs-lookup"><span data-stu-id="c3385-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="c3385-217">Gérer les produits de la place de marché commerciale pour vos clients</span><span class="sxs-lookup"><span data-stu-id="c3385-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="c3385-218">Vue d’ensemble de la Place de marché commerciale</span><span class="sxs-lookup"><span data-stu-id="c3385-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
