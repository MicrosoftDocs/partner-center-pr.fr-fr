---
title: Créer des abonnements clients dans l’espace partenaires
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment vendre à vos clients des abonnements à des produits publiés par Microsoft, ainsi qu’à des produits SaaS publiés par des ISV tiers.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 47291be42523cbcc3aafbb76a6fd9512191ca806
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435248"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="74461-103">Créer, suspendre ou annuler des abonnements client</span><span class="sxs-lookup"><span data-stu-id="74461-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="74461-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="74461-104">**Applies to**</span></span>

- <span data-ttu-id="74461-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="74461-105">Partner Center</span></span>
- <span data-ttu-id="74461-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="74461-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="74461-107">Partenaires fournisseurs de solutions cloud</span><span class="sxs-lookup"><span data-stu-id="74461-107">CSP partners</span></span>

<span data-ttu-id="74461-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="74461-108">**Appropriate roles**</span></span>

- <span data-ttu-id="74461-109">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="74461-109">Admin agent</span></span>
- <span data-ttu-id="74461-110">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="74461-110">Billing admin</span></span>
- <span data-ttu-id="74461-111">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="74461-111">Global admin</span></span>
- <span data-ttu-id="74461-112">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="74461-112">Helpdesk agent</span></span>
- <span data-ttu-id="74461-113">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="74461-113">Sales agent</span></span>

<span data-ttu-id="74461-114">Une fois que vous avez créé un enregistrement de votre client dans l’Espace partenaires, vous pouvez lui vendre des abonnements aux produits figurant dans le catalogue.</span><span class="sxs-lookup"><span data-stu-id="74461-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="74461-115">Cela comprend les produits publiés par Microsoft, ainsi que les produits SaaS (Software as a service) publiés par des éditeurs de logiciels indépendants tiers sur la place de [marché commerciale](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="74461-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="74461-116">Certaines offres sont limitées à un seul abonnement par client.</span><span class="sxs-lookup"><span data-stu-id="74461-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="74461-117">Pour voir la liste des offres limitées, consultez la page Tarification et offres de l'Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="74461-118">En tant que partenaire dans le programme CSP, vous pouvez uniquement acheter des abonnements Saas **basés sur une licence** auprès d’éditeurs ISV au sein de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="74461-119">Cela signifie que vous pouvez acheter une offre SaaS basée sur une **licence** que l’éditeur ISV met à votre disposition, y compris les [offres exclusives](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) auxquelles vous avez accès.</span><span class="sxs-lookup"><span data-stu-id="74461-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="74461-120">Pour acheter ou gérer d’autres offres de la place de marché commercial auprès d’éditeurs de logiciels (ISV) (telles que des offres basées sur **l’utilisation**, limitées ou à la consommation impliquant des applications, des conteneurs ou des machines virtuelles Azure), vous devez accéder au [portail de gestion Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="74461-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="74461-121">Pour plus d’informations, consultez acheter des produits de la place de [marché commercial](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="74461-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="74461-122">Créer un abonnement</span><span class="sxs-lookup"><span data-stu-id="74461-122">Create a new subscription</span></span>

1. <span data-ttu-id="74461-123">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="74461-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="74461-124">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="74461-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="74461-125">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="74461-125">Select **Add subscription**.</span></span> <span data-ttu-id="74461-126">L’onglet **services en ligne** affiche toutes les offres SaaS disponibles sur la place de marché.</span><span class="sxs-lookup"><span data-stu-id="74461-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="74461-127">Pour afficher uniquement certains types d’abonnements, effectuez les sélections dans les filtres disponibles :</span><span class="sxs-lookup"><span data-stu-id="74461-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="74461-128">**Éditeur**: choisissez **Microsoft** pour afficher uniquement les offres de Microsoft ou le **partenaire** pour consulter les produits de la place de marché commercialisés publiés par les éditeurs de logiciels indépendants.</span><span class="sxs-lookup"><span data-stu-id="74461-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="74461-129">**Type de facturation**: sélectionnez le type de facturation d’abonnement que vous souhaitez utiliser : **licence** ou **utilisation**.</span><span class="sxs-lookup"><span data-stu-id="74461-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="74461-130">Consultez [FAQ sur les nouvelles fonctionnalités de facturation](faq-about-new-billing-features.md) pour obtenir des informations qui vous aideront à décider entre la fréquence de facturation mensuelle et annuelle.</span><span class="sxs-lookup"><span data-stu-id="74461-130">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="74461-131">**Catégorie**: choisissez **Enterprise**, **Small Business**ou **version d’évaluation**.</span><span class="sxs-lookup"><span data-stu-id="74461-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="74461-132">Pour obtenir des informations sur les abonnements d’essai, consultez [Proposer à vos clients des abonnements d’essai aux produits Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="74461-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="74461-133">Sélectionnez les abonnements de produits que vous souhaitez acheter pour votre client.</span><span class="sxs-lookup"><span data-stu-id="74461-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="74461-134">Les produits que vous voyez dépendent du type de segment client (éducation, gouvernement, etc.) et des filtres que vous avez appliqués.</span><span class="sxs-lookup"><span data-stu-id="74461-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="74461-135">Certaines offres affichées sur la place de marché ne sont pas toujours disponibles pour un client spécifique ou un partenaire CSP spécifique.</span><span class="sxs-lookup"><span data-stu-id="74461-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="74461-136">Cela peut être dû aux raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="74461-136">This can be because:</span></span>

   - <span data-ttu-id="74461-137">Le client a déjà un abonnement à ce produit et n’est autorisé qu’un seul</span><span class="sxs-lookup"><span data-stu-id="74461-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="74461-138">L’abonnement du client a peut-être été suspendu (dans ce cas, vous pouvez réactiver l’abonnement au lieu d’en acheter un nouveau.)</span><span class="sxs-lookup"><span data-stu-id="74461-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="74461-139">Pour les offres SaaS ISV, il peut y avoir plusieurs raisons pour lesquelles l’offre n’est pas disponible à l’achat : l’ISV peut ne pas prendre en charge le pays ou la région de facturation du client. l’éditeur de logiciels indépendant peut avoir choisi de ne pas rendre l’offre disponible par le biais du programme CSP. ou, l’ISV a peut-être rendu l’offre [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) uniquement à certains partenaires CSP.</span><span class="sxs-lookup"><span data-stu-id="74461-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="74461-140">L’offre ISV n’est pas non plus utilisable via l’espace partenaires (par exemple, des conteneurs ou des offres basées sur l’utilisation).</span><span class="sxs-lookup"><span data-stu-id="74461-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="74461-141">Pour chaque abonnement que vous souhaitez ajouter, entrez le nombre de licences (si nécessaire), puis sélectionnez **Ajouter au panier**.</span><span class="sxs-lookup"><span data-stu-id="74461-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="74461-142">Lorsque vous avez terminé d’ajouter des abonnements, sélectionnez **passer en revue** et passer en revue votre commande.</span><span class="sxs-lookup"><span data-stu-id="74461-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="74461-143">Une fois que vous avez consulté vos commandes et que vous êtes prêt à acheter ces abonnements, sélectionnez **acheter**.</span><span class="sxs-lookup"><span data-stu-id="74461-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="74461-144">Une fois que vous avez acheté un abonnement pour un client, voici ce qui se produit :</span><span class="sxs-lookup"><span data-stu-id="74461-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="74461-145">Vous pouvez consulter ou modifier l’abonnement en sélectionnant le nom de l’abonnement dans la page **abonnements** du client.</span><span class="sxs-lookup"><span data-stu-id="74461-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="74461-146">À partir de là, vous pouvez sélectionner des licences de module complémentaire, le cas échéant, modifier le nombre de licences ou suspendre l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="74461-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="74461-147">**Pour les abonnements ISV SaaS (basés sur une licence) :**</span><span class="sxs-lookup"><span data-stu-id="74461-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="74461-148">Vous recevrez un lien vers le site de l’éditeur ISV.</span><span class="sxs-lookup"><span data-stu-id="74461-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="74461-149">Ce lien doit vous aider à effectuer la configuration du déploiement ou du compte de l’abonnement du client.</span><span class="sxs-lookup"><span data-stu-id="74461-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="74461-150">Ni vous ni votre client ne recevrez un e-mail contenant des instructions pour terminer l’installation/la configuration de compte pour ce type d’abonnement ISV.)</span><span class="sxs-lookup"><span data-stu-id="74461-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="74461-151">Si votre abonnement est fourni avec une version d’évaluation gratuite de 30 jours, la période d’essai gratuite sera appliquée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="74461-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="74461-152">En tant que partenaire dans le programme CSP, vous ne pouvez pas renoncer à la période d’évaluation gratuite sur les offres que vous achetez pour les clients.</span><span class="sxs-lookup"><span data-stu-id="74461-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="74461-153">Une fois la période d’essai gratuite terminée, la durée de l’abonnement commence et l’abonnement est converti en état payant.</span><span class="sxs-lookup"><span data-stu-id="74461-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="74461-154">L’abonnement est ensuite renouvelé en fonction de la même planification.</span><span class="sxs-lookup"><span data-stu-id="74461-154">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="74461-155">Suspendre ou annuler un abonnement</span><span class="sxs-lookup"><span data-stu-id="74461-155">Suspend or cancel a subscription</span></span>

<span data-ttu-id="74461-156">Les partenaires peuvent suspendre ou annuler un abonnement à la demande du client ou dans les cas de fraude ou de défaut de paiement.</span><span class="sxs-lookup"><span data-stu-id="74461-156">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="74461-157">Suspendre un abonnement</span><span class="sxs-lookup"><span data-stu-id="74461-157">Suspend a subscription</span></span>

<span data-ttu-id="74461-158">Lorsque vous attribuez à un abonnement l’état **Suspendu**, les utilisateurs ne peuvent plus se connecter aux services ou y accéder.</span><span class="sxs-lookup"><span data-stu-id="74461-158">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="74461-159">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="74461-160">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="74461-160">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="74461-161">Choisissez l’abonnement que vous souhaitez gérer.</span><span class="sxs-lookup"><span data-stu-id="74461-161">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="74461-162">Dans la section **État**, choisissez **Suspendu**.</span><span class="sxs-lookup"><span data-stu-id="74461-162">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="74461-163">Ensuite, **envoyez** vos modifications.</span><span class="sxs-lookup"><span data-stu-id="74461-163">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="74461-164">Toutes les données seront supprimées, sauf si l’abonnement est réactivé dans les 90 jours, ou 90 jours en plus du nombre de jours écoulés entre la date d'ouverture du compte et la première période de facturation (120 jours maximum).</span><span class="sxs-lookup"><span data-stu-id="74461-164">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="74461-165">Lorsque vous suspendez un abonnement, la date affichée sous le bouton **Suspendu** indique quand l’abonnement va automatiquement expirer si vous ne le réactivez pas.</span><span class="sxs-lookup"><span data-stu-id="74461-165">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="74461-166">Pour plus d’informations, consultez [FAQ sur les nouvelles fonctionnalités de facturation](faq-about-new-billing-features.md).</span><span class="sxs-lookup"><span data-stu-id="74461-166">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="74461-167">Annuler un abonnement</span><span class="sxs-lookup"><span data-stu-id="74461-167">Cancel a subscription</span></span>

<span data-ttu-id="74461-168">Vous avez la possibilité d’annuler les abonnements SaaS basés sur des licences à partir d’éditeurs ISV tiers au sein de la place de [marché commerciale](csp-commercial-marketplace-overview.md)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-168">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="74461-169">Tant que vous annulez l’opération pendant la période d’annulation, vous recevrez un remboursement intégral.</span><span class="sxs-lookup"><span data-stu-id="74461-169">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="74461-170">Pour les éditeurs de logiciels, les offres sont facturées tous les mois :</span><span class="sxs-lookup"><span data-stu-id="74461-170">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="74461-171">Si vous annulez moins de 24 heures après avoir passé la commande, vous recevrez un crédit complet sur la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="74461-171">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="74461-172">Si vous annulez plus de 24 heures après avoir passé la commande, l’annulation sera planifiée pour être renouvelée.</span><span class="sxs-lookup"><span data-stu-id="74461-172">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="74461-173">Pour les offres facturées annuellement :</span><span class="sxs-lookup"><span data-stu-id="74461-173">For offers billed annually:</span></span>

- <span data-ttu-id="74461-174">Si vous annulez moins de 14 jours après avoir placé la commande, vous recevrez un crédit complet sur la facture suivante.</span><span class="sxs-lookup"><span data-stu-id="74461-174">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="74461-175">Si vous annulez plus de 14 jours après avoir placé la commande, l’annulation sera planifiée au renouvellement.</span><span class="sxs-lookup"><span data-stu-id="74461-175">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="74461-176">Une fois ces périodes supérieures, vous ne verrez plus l’option permettant d’annuler l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="74461-176">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="74461-177">Les services ISV tiers basés sur l’utilisation et contrôlés (qui utilisent des machines virtuelles ou des conteneurs, par exemple) ne peuvent pas être retournés.</span><span class="sxs-lookup"><span data-stu-id="74461-177">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="74461-178">Les services basés sur l’utilisation peuvent être désapprovisionnés en tant que méthode d’annulation.</span><span class="sxs-lookup"><span data-stu-id="74461-178">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="74461-179">Étant donné que les frais sont facturés après utilisation, ces services ne peuvent pas être remboursés.</span><span class="sxs-lookup"><span data-stu-id="74461-179">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="74461-180">Pour annuler un abonnement SaaS basé sur une licence auprès d’un éditeur de logiciels indépendant, effectuez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="74461-180">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="74461-181">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-181">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="74461-182">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="74461-182">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="74461-183">Recherchez l’abonnement que vous souhaitez annuler.</span><span class="sxs-lookup"><span data-stu-id="74461-183">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="74461-184">Dans la colonne **État** , sélectionnez **Annuler**.</span><span class="sxs-lookup"><span data-stu-id="74461-184">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="74461-185">Ensuite, **envoyez** vos modifications.</span><span class="sxs-lookup"><span data-stu-id="74461-185">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="74461-186">Si une boîte de dialogue s’affiche, renseignez les détails pertinents, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="74461-186">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="74461-187">Pour confirmer l’annulation, sélectionnez **Oui, annuler**.</span><span class="sxs-lookup"><span data-stu-id="74461-187">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="74461-188">Vous pouvez également choisir d’annuler un abonnement à la place de marché Azure à l’aide d’API.</span><span class="sxs-lookup"><span data-stu-id="74461-188">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="74461-189">Pour ce faire, consultez [annuler un abonnement Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="74461-189">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="74461-190">Choisir de renouveler automatiquement un abonnement à la place marché commerciale</span><span class="sxs-lookup"><span data-stu-id="74461-190">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="74461-191">Par défaut, les abonnements actifs sont définis pour se renouveler automatiquement à l’expiration de la période d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="74461-191">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="74461-192">Pour les [abonnements aux produits de la place de marché commercial](csp-commercial-marketplace-overview.md), vous pouvez éventuellement choisir de ne pas renouveler automatiquement l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="74461-192">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="74461-193">Pour arrêter le renouvellement automatique d’un abonnement au marché commercial actif :</span><span class="sxs-lookup"><span data-stu-id="74461-193">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="74461-194">Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="74461-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="74461-195">Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.</span><span class="sxs-lookup"><span data-stu-id="74461-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="74461-196">Sélectionnez **Abonnements**.</span><span class="sxs-lookup"><span data-stu-id="74461-196">Select **Subscriptions**.</span></span> <span data-ttu-id="74461-197">Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.</span><span class="sxs-lookup"><span data-stu-id="74461-197">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="74461-198">Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez modifier.</span><span class="sxs-lookup"><span data-stu-id="74461-198">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="74461-199">Dans la page Détails de l’abonnement, recherchez la section **État** et désactivez la case à cocher **renouvellement automatique** .</span><span class="sxs-lookup"><span data-stu-id="74461-199">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="74461-200">Sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="74461-200">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="74461-201">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="74461-201">Next steps</span></span>

- [<span data-ttu-id="74461-202">Acheter des produits de la place de marché commerciale pour vos clients</span><span class="sxs-lookup"><span data-stu-id="74461-202">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="74461-203">Gérer les produits de la place de marché commerciale pour vos clients</span><span class="sxs-lookup"><span data-stu-id="74461-203">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="74461-204">Vue d’ensemble de la Place de marché commerciale</span><span class="sxs-lookup"><span data-stu-id="74461-204">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
