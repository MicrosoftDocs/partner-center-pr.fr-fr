---
title: Consolidation des locataires disposant de l’autorisation régionale Fournisseur de solutions&nbsp;Cloud
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez ces instructions pour consolider des locataires de différents pays/régions. Cela comprend les étapes de migration des comptes client et des abonnements client.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: migrer des clients, approvisionnement, compte de locataire, consolider les locataires
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d361a220ce798863eaeec73e6ff093f135bc4ae1
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453226"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="9c348-105">Instructions pour la consolidation des locataires d’autorisation régionale du CSP</span><span class="sxs-lookup"><span data-stu-id="9c348-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="9c348-106">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="9c348-106">**Applies to**</span></span>

-  <span data-ttu-id="9c348-107">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="9c348-107">Partner Center</span></span>
-  <span data-ttu-id="9c348-108">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="9c348-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="9c348-109">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="9c348-109">**Appropriate roles**</span></span>

- <span data-ttu-id="9c348-110">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="9c348-110">Global admin</span></span>
- <span data-ttu-id="9c348-111">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="9c348-111">Admin agent</span></span>

<span data-ttu-id="9c348-112">\[Certaines informations relatives aux produits précommercialisés peuvent être substantiellement modifiées avant leur commercialisation.</span><span class="sxs-lookup"><span data-stu-id="9c348-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="9c348-113">Microsoft exclut toute garantie, expresse ou implicite, concernant les informations fournies ici.\]</span><span class="sxs-lookup"><span data-stu-id="9c348-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="9c348-114">Utilisez ces instructions pour consolider des locataires de différents pays/régions.</span><span class="sxs-lookup"><span data-stu-id="9c348-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="9c348-115">**Remarque** Vous devez connaître tous les abonnements et le nombre de sièges de vos clients approvisionnés à partir des comptes de transition.</span><span class="sxs-lookup"><span data-stu-id="9c348-115">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="9c348-116">Vous allez reconfigurer les mêmes abonnements exacts avec le même nombre de sièges sous le nouveau compte CSP central dans le cadre du processus de migration.</span><span class="sxs-lookup"><span data-stu-id="9c348-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="9c348-117">Utilisez la fonctionnalité d’exportation de liste pour créer une liste de clients à transférer au locataire centralisé.</span><span class="sxs-lookup"><span data-stu-id="9c348-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="9c348-118">Les partenaires choisissent de consolider leurs locataires.</span><span class="sxs-lookup"><span data-stu-id="9c348-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="9c348-119">Une fois la consolidation terminée, les partenaires ne peuvent pas revenir à leur état antérieur.</span><span class="sxs-lookup"><span data-stu-id="9c348-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="9c348-120">Notez que l’action du client peut également être nécessaire.</span><span class="sxs-lookup"><span data-stu-id="9c348-120">Note that customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="9c348-121">Préparation de la migration</span><span class="sxs-lookup"><span data-stu-id="9c348-121">Prepare for migration</span></span>

- <span data-ttu-id="9c348-122">Connectez-vous à votre **espace partenaires** à l’aide du compte de **transition** (existant) (celui que vous allez passer) et prenez note de tous les clients et de tous les services configurés pour ces clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-122">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="liste de clients régionaux":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="9c348-124">Migrer des comptes client</span><span class="sxs-lookup"><span data-stu-id="9c348-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="9c348-125">Connectez-vous à votre **espace partenaires** à l’aide du compte de **transition** (nouveau) (celui dans lequel vous effectuez la transition) et accédez à la liste Customers **(clients).**</span><span class="sxs-lookup"><span data-stu-id="9c348-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="9c348-126">Sélectionnez Clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-126">Select Customers.</span></span>

3. <span data-ttu-id="9c348-127">Cliquez sur **Demander une relation de revendeur**.</span><span class="sxs-lookup"><span data-stu-id="9c348-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="9c348-128">Un message électronique par défaut à présenter à vos clients s’affiche.</span><span class="sxs-lookup"><span data-stu-id="9c348-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="9c348-129">Ce message contient une URL avec l’ID d’organisation propre à votre nouveau compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="9c348-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="9c348-130">**Action du client&nbsp;:** vérifiez que chaque client actif que vous souhaitez migrer visite cette URL.</span><span class="sxs-lookup"><span data-stu-id="9c348-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="9c348-131">À l’ouverture de l’URL, le client est invité à se connecter au portail Office&nbsp;365.</span><span class="sxs-lookup"><span data-stu-id="9c348-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="9c348-132">Il se connecte à l’aide du même ID d’organisation que celui utilisé pour accéder aux portails administration Windows Azure et Office&nbsp;365.</span><span class="sxs-lookup"><span data-stu-id="9c348-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="9c348-133">Une fois connecté, l’administrateur global du compte client est invité à valider l’attribution de privilèges d’administration délégué pour le nouveau compte Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="9c348-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="9c348-134">S’il accepte, le client active la case à cocher et autorise la relation.</span><span class="sxs-lookup"><span data-stu-id="9c348-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="9c348-135">Les clients s’affichent dans la liste des clients du partenaire après l’envoi de l’accord, un par un.</span><span class="sxs-lookup"><span data-stu-id="9c348-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="9c348-136">Migration d’abonnements Office&nbsp;365 et non Azure basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="9c348-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="9c348-137">Lorsque votre client a signé le contrat, vous pouvez recréer ses abonnements sous votre locataire partenaire centralisé.</span><span class="sxs-lookup"><span data-stu-id="9c348-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="9c348-138">Dans l' **espace partenaires** , sélectionnez **clients**.</span><span class="sxs-lookup"><span data-stu-id="9c348-138">From the **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="9c348-139">Ouvrez le nom de la société du client que vous souhaitez migrer.</span><span class="sxs-lookup"><span data-stu-id="9c348-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="9c348-140">Cliquez sur **Ajouter un abonnement**.</span><span class="sxs-lookup"><span data-stu-id="9c348-140">Click **Add subscription**.</span></span>

5. <span data-ttu-id="9c348-141">Ajoutez les abonnements et le nombre de sièges corrects à partir du catalogue.</span><span class="sxs-lookup"><span data-stu-id="9c348-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="9c348-142">Vérifiez avec les informations fournies dans les comptes de partenaire **Transition à partir de**.</span><span class="sxs-lookup"><span data-stu-id="9c348-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="Liste des clients":::

6. <span data-ttu-id="9c348-144">Cliquez sur **Envoyer.**</span><span class="sxs-lookup"><span data-stu-id="9c348-144">Click **Submit.**</span></span>

   <span data-ttu-id="9c348-145">Les services sont maintenant fournis au client à partir du compte de partenaire **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="9c348-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="9c348-146">Répétez ces étapes pour migrer les abonnements de tous les clients supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="9c348-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="9c348-147">Avant de passer à la section suivante, vérifiez que tous les abonnements client existant sous les comptes de partenaire **Transition à partir de** sont ré-approvisionnées sous le compte de partenaire **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="9c348-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="9c348-148">Les partenaires doivent suspendre les abonnements lors de la transition **à partir du** compte de locataire partenaire dans l’espace partenaires le même jour que ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="9c348-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="9c348-149">Les demandes de support seront refusées pour les crédits résultant d’un chevauchement dans la facturation à cause d’une désactivation incorrecte des abonnements **Transition à partir de**.</span><span class="sxs-lookup"><span data-stu-id="9c348-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="9c348-150">Désactivation des abonnements Office&nbsp;365 sous le compte de partenaire Transition à partir de</span><span class="sxs-lookup"><span data-stu-id="9c348-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="9c348-151">La désactivation de l’abonnement Fournisseur de solutions Cloud sous les comptes de partenaire **Transition à partir de** interrompt toute facturation future.</span><span class="sxs-lookup"><span data-stu-id="9c348-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="9c348-152">Il est inutile de désactiver manuellement les abonnements Azure, car le processus de migration les désactive automatiquement.</span><span class="sxs-lookup"><span data-stu-id="9c348-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="9c348-153">Connectez-vous à l' **espace partenaires** à l’aide de la **transition à partir du** compte CSP et accédez à la liste des clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="9c348-154">Ouvrez le client avec les abonnements à désactiver, et sélectionnez la première offre à désactiver.</span><span class="sxs-lookup"><span data-stu-id="9c348-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="9c348-155">Réglez l’abonnement sur **suspendu**, puis cliquez sur **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="9c348-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   >  <span data-ttu-id="9c348-156">La suspension de l’abonnement garantit que la double facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="9c348-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="9c348-157">L’abonnement affiche la mention **suspendu** dans la liste des abonnements.</span><span class="sxs-lookup"><span data-stu-id="9c348-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="9c348-158">Répétez ces étapes pour tous les abonnements sous le client.</span><span class="sxs-lookup"><span data-stu-id="9c348-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="9c348-159">Vérifiez que tous les abonnements indiquent la mention **suspendu**.</span><span class="sxs-lookup"><span data-stu-id="9c348-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="9c348-160">Sélectionnez le client suivant sur la liste et répétez le processus de désactivation de tous les abonnements.</span><span class="sxs-lookup"><span data-stu-id="9c348-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="9c348-161">Migration d’abonnements Azure basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="9c348-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="9c348-162">Azure, les abonnements CSP basés sur l’utilisation n’ont pas besoin d’être migrés manuellement comme c’est le cas avec les abonnements CSP Office 365.</span><span class="sxs-lookup"><span data-stu-id="9c348-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="9c348-163">Le support Microsoft Azure peut migrer les abonnements Azure ainsi que tous les services ou ressources déployés entre les comptes de revendeur Fournisseur de solutions Cloud **Transition à partir de** et le compte de revendeur Fournisseur de solutions Cloud **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="9c348-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="9c348-164">Il n’y a aucune interruption de service pour le client pendant cette transition.</span><span class="sxs-lookup"><span data-stu-id="9c348-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="9c348-165">Vérifiez que les comptes client qui ont besoin d’abonnements Azure migrés ont accepté le contrat à associer au nouveau compte Fournisseur de solutions Cloud **Transition vers**.</span><span class="sxs-lookup"><span data-stu-id="9c348-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="9c348-166">Les partenaires notifient à Microsoft les comptes client dont les abonnements Azure sont prêts à migrer, et fournit les noms de société de ces clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="9c348-167">Microsoft migre les abonnements Azure basés sur l’utilisation et avertit le partenaire lorsque la migration est terminée.</span><span class="sxs-lookup"><span data-stu-id="9c348-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="9c348-168">Le partenaire confirme que l’abonnement Azure sous les comptes de revendeur Fournisseur de solutions&nbsp;Cloud **Transition à partir de** affiche la mention Suspendu dans l’Espace partenaires sous la section des abonnements du client.</span><span class="sxs-lookup"><span data-stu-id="9c348-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="9c348-169">Le partenaire confirme que l’abonnement Azure sous le compte de revendeur Fournisseur de solutions&nbsp;Cloud **Transition à partir de** affiche la mention **Actif** dans l’Espace partenaires sous la section des abonnements du client.</span><span class="sxs-lookup"><span data-stu-id="9c348-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="9c348-170">La désactivation des abonnements sous le client ne modifie pas l’apparence du client dans la liste des clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="9c348-171">Il n’y a actuellement aucune possibilité de supprimer des clients de la liste.</span><span class="sxs-lookup"><span data-stu-id="9c348-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="9c348-172">Les partenaires doivent éviter de rajouter des abonnements à ces clients à partir de leur compte **Transition à partir de** à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="9c348-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="9c348-173">Répétez ces étapes pour tous les abonnements sous l’ensemble de vos clients pour arrêter les prochaines facturations sur le ou les comptes **Transition à partir de**.</span><span class="sxs-lookup"><span data-stu-id="9c348-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="9c348-174">Le partenaire reçoit une facture finale avec un crédit pour le nombre de jours inutilisés entre le jour de l’annulation et le dernier jour de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="9c348-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="9c348-175">Aucune facture n’est générée après cette période de facturation finale.</span><span class="sxs-lookup"><span data-stu-id="9c348-175">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="9c348-176">Notes</span><span class="sxs-lookup"><span data-stu-id="9c348-176">Notes</span></span>

- <span data-ttu-id="9c348-177">La désactivation de l’abonnement de la **transition à partir** du compte CSP n’a pas d’impact sur le service du client final tant que le service a été approvisionné à partir du compte de **transition vers** le fournisseur CSP avant de désactiver l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="9c348-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="9c348-178">Les abonnements ne peuvent pas être utilisés par le client et ne génèrent pas de frais lorsqu’ils sont suspendus ou annulés.</span><span class="sxs-lookup"><span data-stu-id="9c348-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="9c348-179">Il est actuellement impossible de supprimer complètement un client de la liste de clients.</span><span class="sxs-lookup"><span data-stu-id="9c348-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

>[!Note]
> <span data-ttu-id="9c348-180">Les partenaires doivent suspendre les abonnements lors de la transition à **partir du** compte de locataire partenaire dans l’espace partenaires le même jour auquel ces abonnements sont migrés et configurés dans le cadre du compte de locataire de partenaire dans l’espace partenaires pour s’assurer **que la double** facturation n’a pas lieu.</span><span class="sxs-lookup"><span data-stu-id="9c348-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="9c348-181">Microsoft ne prend pas en charge les demandes de crédits en raison d’un chevauchement de la facturation qui résulte de la définition incorrecte du **passage des** abonnements à l’état suspendu.</span><span class="sxs-lookup"><span data-stu-id="9c348-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="9c348-182">Simplifier la migration avec l’exportation</span><span class="sxs-lookup"><span data-stu-id="9c348-182">Simplify migration using Export</span></span>

<span data-ttu-id="9c348-183">Grâce à la **fonction Exporter**, vous pouvez capturer les abonnements que vous devez utiliser dans votre nouvelle structure consolidée&nbsp;:</span><span class="sxs-lookup"><span data-stu-id="9c348-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="9c348-184">Cliquez sur **clients** dans l’espace partenaires pour afficher la liste des clients dans votre structure existante.</span><span class="sxs-lookup"><span data-stu-id="9c348-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="9c348-185">Ouvrez le nom de client souhaité.</span><span class="sxs-lookup"><span data-stu-id="9c348-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="9c348-186">Dans la page **Abonnements**, cliquez sur **Exporter les abonnements** pour exporter les détails des abonnements dans un fichier Excel.</span><span class="sxs-lookup"><span data-stu-id="9c348-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="9c348-187">Utilisez cette liste pour recréer les abonnements dans votre nouveau locataire consolidé.</span><span class="sxs-lookup"><span data-stu-id="9c348-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="9c348-188">Inscription d’API</span><span class="sxs-lookup"><span data-stu-id="9c348-188">API registration</span></span>

<span data-ttu-id="9c348-189">Pour plus d’informations sur l’inscription d’API, consultez [configurer l’accès aux API dans l’espace partenaires](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="9c348-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
