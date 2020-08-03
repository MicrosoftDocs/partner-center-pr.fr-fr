---
title: Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutions&nbsp;Cloud
ms.topic: article
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez ces instructions pour consolider des locataires de différents pays/régions. Cela comprend les étapes de migration des comptes client et des abonnements client.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 4389ed675bfc7186aa19e595b14ac9200334c61c
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444924"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="4c1d8-104">Instructions pour le regroupement des locataires disposant de l’autorisation régionale CSP</span><span class="sxs-lookup"><span data-stu-id="4c1d8-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="4c1d8-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="4c1d8-105">**Applies to**</span></span>

-  <span data-ttu-id="4c1d8-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="4c1d8-106">Partner Center</span></span>
-  <span data-ttu-id="4c1d8-107">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="4c1d8-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="4c1d8-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="4c1d8-108">**Appropriate roles**</span></span>

- <span data-ttu-id="4c1d8-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="4c1d8-109">Global admin</span></span>
- <span data-ttu-id="4c1d8-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="4c1d8-110">Admin agent</span></span>

<span data-ttu-id="4c1d8-111">\[Certaines informations relatives aux produits précommercialisés peuvent être substantiellement modifiées avant leur commercialisation.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="4c1d8-112">Microsoft exclut toute garantie, expresse ou implicite, concernant les informations fournies ici.\]</span><span class="sxs-lookup"><span data-stu-id="4c1d8-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="4c1d8-113">Vous pouvez consolider les locataires pour votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="4c1d8-114">Utilisez ces instructions pour consolider des locataires de différents pays/régions.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="4c1d8-115">Vous devez être conscient de tous les abonnements approvisionnés et du nombre de licences pour chacun de vos clients dans le compte à partir duquel vous effectuez la transition.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="4c1d8-116">Vous allez reconfigurer les mêmes abonnements exacts avec le même nombre de licences sous le nouveau compte CSP central dans le cadre du processus de migration.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="4c1d8-117">Utilisez la fonctionnalité d’exportation de liste pour créer une liste de clients à transférer au locataire centralisé.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="4c1d8-118">Une fois la consolidation terminée, vous ne pouvez pas revenir à l’état précédent du locataire.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="4c1d8-119">L’action du client peut également être nécessaire.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="4c1d8-120">Préparation de la migration</span><span class="sxs-lookup"><span data-stu-id="4c1d8-120">Prepare for migration</span></span>

- <span data-ttu-id="4c1d8-121">Connectez-vous à l' **espace partenaires** à l’aide du compte de **transition** (celui que vous allez migrer vers le nouveau compte) et passez en revue tous les clients et tous les services approvisionnés pour ces clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="4c1d8-122">Déconnectez-vous de ce compte.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="4c1d8-123">Migrer des comptes client</span><span class="sxs-lookup"><span data-stu-id="4c1d8-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="4c1d8-124">Connectez-vous à l' **espace partenaires** avec le compte de **transition** (nouveau) (celui vers lequel vous transférez des clients).</span><span class="sxs-lookup"><span data-stu-id="4c1d8-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="4c1d8-125">Sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-125">Select **Customers**.</span></span>

3. <span data-ttu-id="4c1d8-126">Cliquez sur **Demander une relation de revendeur**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="4c1d8-127">Vous êtes invité à envoyer un message électronique par défaut à vos clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="4c1d8-128">Ce message contient une URL avec l’ID d’organisation propre à votre nouveau compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="4c1d8-129">**Action du client&nbsp;:** vérifiez que chaque client actif que vous souhaitez migrer visite cette URL.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="4c1d8-130">À l’ouverture de l’URL, le client est invité à se connecter au portail Office&nbsp;365.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="4c1d8-131">Il se connecte à l’aide du même ID d’organisation que celui utilisé pour accéder aux portails administration Windows Azure et Office&nbsp;365.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="4c1d8-132">Une fois connecté, l’administrateur général du **compte client** est invité à soumettre un accord qui accorde des privilèges d’administrateur délégué au nouveau compte CSP.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="4c1d8-133">S’il accepte, le client active la case à cocher et autorise la relation.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="4c1d8-134">Les clients s’affichent dans la liste des clients du partenaire après l’envoi de l’accord, un par un.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="4c1d8-135">Migration d’abonnements Office&nbsp;365 et non Azure basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="4c1d8-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="4c1d8-136">Lorsque votre client a signé le contrat, vous pouvez recréer ses abonnements sous votre locataire partenaire centralisé.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="4c1d8-137">Dans l' **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="4c1d8-138">Ouvrez le nom de la société du client que vous souhaitez migrer.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="4c1d8-139">Sélectionnez **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="4c1d8-140">Ajoutez les abonnements et le nombre de licences appropriés à partir du catalogue.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="4c1d8-141">Vérifiez avec les informations fournies dans les comptes de partenaire **Transition à partir de**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Liste des clients":::

6. <span data-ttu-id="4c1d8-143">Cliquez sur **Envoyer.**</span><span class="sxs-lookup"><span data-stu-id="4c1d8-143">Click **Submit.**</span></span>

   <span data-ttu-id="4c1d8-144">Les services sont maintenant fournis au client à partir du compte de partenaire **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="4c1d8-145">Répétez ces étapes pour migrer les abonnements de tous les clients supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="4c1d8-146">Avant de passer à la section suivante, vérifiez que tous les abonnements client existant sous les comptes de partenaire **Transition à partir de** sont ré-approvisionnées sous le compte de partenaire **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="4c1d8-147">Les partenaires doivent suspendre les abonnements lors de la transition **à partir du** compte de locataire partenaire dans l’espace partenaires le même jour que ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="4c1d8-148">Les demandes de support sont refusées pour les crédits en raison du chevauchement de la facturation résultant de la désactivation incorrecte **de la transition des** abonnements.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="4c1d8-149">Désactivation des abonnements Office&nbsp;365 sous le compte de partenaire Transition à partir de</span><span class="sxs-lookup"><span data-stu-id="4c1d8-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="4c1d8-150">La désactivation de l’abonnement Fournisseur de solutions Cloud sous les comptes de partenaire **Transition à partir de** interrompt toute facturation future.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="4c1d8-151">Vous n’avez pas besoin de désactiver manuellement les abonnements Azure, car les abonnements Azure sont automatiquement désactivés pendant le processus de migration.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="4c1d8-152">Connectez-vous à l' **espace partenaires** à l’aide de la **transition à partir du** compte CSP et accédez à la liste des clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="4c1d8-153">Ouvrez le client avec les abonnements à désactiver, et sélectionnez la première offre à désactiver.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="4c1d8-154">Réglez l’abonnement sur **suspendu**, puis cliquez sur **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="4c1d8-155">La suspension de l’abonnement garantit que la double facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="4c1d8-156">L’abonnement affiche **suspendu** dans la liste des abonnements.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="4c1d8-157">Répétez ces étapes pour tous les abonnements sous le client.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="4c1d8-158">Vérifiez que tous les abonnements indiquent la mention **suspendu**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="4c1d8-159">Sélectionnez le client suivant sur la liste et répétez le processus de désactivation de tous les abonnements.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="4c1d8-160">Migration d’abonnements Azure basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="4c1d8-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="4c1d8-161">Contrairement aux abonnements CSP Office 365, Azure, les abonnements CSP basés sur l’utilisation n’ont pas besoin d’être migrés manuellement.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="4c1d8-162">Microsoft Azure prise en charge migre les abonnements Azure, ainsi que tous les services ou ressources déployés à partir de la **transition des** comptes du revendeur CSP vers le compte du revendeur de la **transition vers** le revendeur CSP.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="4c1d8-163">Il n’y a aucune interruption de service pour le client pendant cette transition.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="4c1d8-164">Assurez-vous que les comptes clients pour lesquels des abonnements Azure ont été migrés ont accepté le contrat à associer à la nouvelle **transition vers** le compte CSP.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="4c1d8-165">Vous informerez Microsoft des comptes client prêts à migrer et fournissez les noms de société de ces clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="4c1d8-166">Microsoft migre les abonnements basés sur l’utilisation d’Azure et vous avertit lorsque la migration est terminée.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="4c1d8-167">Vous devez vérifier que l’abonnement Azure sous le compte **de** revendeur du revendeur CSP est désormais marqué comme **suspendu** dans l’espace partenaires dans la section abonnements client.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="4c1d8-168">Confirmez que l’abonnement Azure sous le compte du revendeur **de la transition au** revendeur CSP affiche maintenant l’état **actif** dans l’espace partenaires dans la section abonnements client.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="4c1d8-169">La désactivation des abonnements sous le client ne modifie pas l’apparence du client dans la liste des clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="4c1d8-170">Il n’y a actuellement aucune possibilité de supprimer des clients de la liste.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="4c1d8-171">Les partenaires doivent éviter de rajouter des abonnements à ces clients à partir de leur compte **Transition à partir de** à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="4c1d8-172">Répétez ces étapes pour tous les abonnements sous l’ensemble de vos clients pour arrêter les prochaines facturations sur le ou les comptes **Transition à partir de**.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="4c1d8-173">Le partenaire reçoit une facture finale avec un crédit pour le nombre de jours inutilisés entre le jour de l’annulation et le dernier jour de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="4c1d8-174">Aucune facture n’est générée après cette période de facturation finale.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="4c1d8-175">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="4c1d8-175">Additional information</span></span>

- <span data-ttu-id="4c1d8-176">La désactivation de l’abonnement de la **transition à partir** du compte CSP n’a pas d’impact sur le service du client final tant que le service a été approvisionné à partir du compte de **transition vers** le fournisseur CSP avant de désactiver l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="4c1d8-177">Les abonnements ne peuvent pas être utilisés par le client et ne génèrent pas de frais lorsqu’ils sont suspendus ou annulés.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="4c1d8-178">Il n’existe actuellement aucun moyen de supprimer complètement un client de la liste des **clients** .</span><span class="sxs-lookup"><span data-stu-id="4c1d8-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="4c1d8-179">Les partenaires doivent suspendre les abonnements lors de la transition à **partir du** compte de locataire partenaire dans l’espace partenaires le même jour que celui vers lequel les abonnements sont migrés et configurés sous le compte de **transition** pour s’assurer que la double facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="4c1d8-180">Microsoft ne prend pas en charge les demandes de crédits en raison d’un chevauchement de la facturation qui résulte de la définition incorrecte du **passage des** abonnements à l’état suspendu.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="4c1d8-181">Simplifier la migration avec l’exportation</span><span class="sxs-lookup"><span data-stu-id="4c1d8-181">Simplify migration using Export</span></span>

<span data-ttu-id="4c1d8-182">Grâce à la **fonction Exporter**, vous pouvez capturer les abonnements que vous devez utiliser dans votre nouvelle structure consolidée&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="4c1d8-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="4c1d8-183">Cliquez sur **clients** dans l’espace partenaires pour afficher la liste des clients.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="4c1d8-184">Ouvrez le nom de client souhaité.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="4c1d8-185">Dans la page **Abonnements**, cliquez sur **Exporter les abonnements** pour exporter les détails des abonnements dans un fichier Excel.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="4c1d8-186">Utilisez cette liste pour recréer les abonnements dans votre nouveau locataire consolidé.</span><span class="sxs-lookup"><span data-stu-id="4c1d8-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="4c1d8-187">Inscription d’API</span><span class="sxs-lookup"><span data-stu-id="4c1d8-187">API registration</span></span>

<span data-ttu-id="4c1d8-188">Pour plus d’informations sur l’inscription d’API, consultez [configurer l’accès aux API dans l’espace partenaires](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="4c1d8-188">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c1d8-189">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="4c1d8-189">Next steps</span></span>

- [<span data-ttu-id="4c1d8-190">Configuration et gestion des comptes clients pour les partenaires revendeurs dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="4c1d8-190">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)
