---
title: Utiliser des webhooks pour recevoir des événements de modification de ressource
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez les API de webhook de l’espace partenaires pour savoir quand des modifications de ressources de références sont effectuées pour Dynamics 365 CRM ou Salesforce CRM.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: références, API webhook, événements de modification de ressource
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43874556b5f3fd355f5c315bf06ca7daee0a699e
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467469"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="c339f-104">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource pour Dynamics 365 CRM et Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c339f-104">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c339f-105">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="c339f-105">Appropriate roles</span></span>

- <span data-ttu-id="c339f-106">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="c339f-106">Referrals admin</span></span>
- <span data-ttu-id="c339f-107">Administrateur système ou personnalisateur de système pour Dynamics 365 CRM ou Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c339f-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="c339f-108">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="c339f-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="c339f-109">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="c339f-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="c339f-110">Cette rubrique explique les API webhook pour Dynamics 365 CRM et Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="c339f-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="c339f-111">Configurer le webhook</span><span class="sxs-lookup"><span data-stu-id="c339f-111">Configure the webhook</span></span>

1. <span data-ttu-id="c339f-112">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="c339f-112">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="c339f-113">Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous</span><span class="sxs-lookup"><span data-stu-id="c339f-113">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. <span data-ttu-id="c339f-115">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="c339f-115">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="c339f-117">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="c339f-117">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="c339f-118">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications d’événement dans les objets d’adresse IP de covente ou de référence indépendante dans l’espace partenaires et les systèmes CRM, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="c339f-118">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="c339f-119">Sélectionnez **espace partenaires pour Dynamics 365 (version préliminaire d’Insider)** ou **espace partenaires pour Salesforce (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="c339f-119">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="c339f-120">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="c339f-120">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="c339f-121">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="c339f-121">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copier l’URL":::

8. <span data-ttu-id="c339f-123">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="c339f-123">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="c339f-124">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="c339f-124">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="c339f-125">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="c339f-125">Enter the following details:</span></span>

    1. <span data-ttu-id="c339f-126">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="c339f-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="c339f-127">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="c339f-127">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="c339f-128">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="c339f-128">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="c339f-129">Le webhook peut maintenant écouter les modifications (créer et mettre à jour des événements).</span><span class="sxs-lookup"><span data-stu-id="c339f-129">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="c339f-130">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="c339f-130">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="c339f-131">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="c339f-131">Customize synchronization steps</span></span>

<span data-ttu-id="c339f-132">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="c339f-132">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="c339f-133">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="c339f-133">Often CRM systems are highly customized.</span></span> <span data-ttu-id="c339f-134">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="c339f-134">You can customize the Power Automate flows.</span></span> <span data-ttu-id="c339f-135">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="c339f-135">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="c339f-136">Les mappages de l’espace partenaires Microsoft aux CRM sont fournis, mais en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="c339f-136">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="c339f-137">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="c339f-137">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="c339f-138">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="c339f-138">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="c339f-139">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="c339f-139">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="c339f-140">Sélectionnez espace partenaires pour Dynamics 365 (version préliminaire d’Insider) ou espace partenaires pour Salesforce (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="c339f-140">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="c339f-141">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="c339f-141">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="c339f-142">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="c339f-142">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="c339f-143">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="c339f-143">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="c339f-144">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="c339f-144">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="c339f-145">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="c339f-145">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="c339f-146">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="c339f-146">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="c339f-147">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="c339f-147">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="c339f-148">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="c339f-148">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="c339f-149">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="c339f-149">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="c339f-150">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="c339f-150">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="c339f-151">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="c339f-151">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="c339f-152">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="c339f-152">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="c339f-153">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="c339f-153">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="c339f-154">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="c339f-154">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="c339f-155">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="c339f-155">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="c339f-156">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="c339f-156">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="c339f-157">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="c339f-157">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="c339f-158">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="c339f-158">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="c339f-159">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="c339f-159">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="c339f-160">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="c339f-160">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="c339f-161">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="c339f-161">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="c339f-162">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 ou Salesforce et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c339f-162">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="c339f-163">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="c339f-163">Pre-requisites</span></span>

<span data-ttu-id="c339f-164">Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM ou entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c339f-164">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="c339f-165">Cela permet à vos équipes de vendeur de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="c339f-165">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="c339f-166">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c339f-166">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="c339f-167">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="c339f-167">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="c339f-168">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="c339f-168">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="c339f-169">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="c339f-169">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="c339f-170">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="c339f-170">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="c339f-171">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="c339f-171">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="c339f-172">**Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="c339f-172">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="c339f-173">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="c339f-173">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="c339f-174">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c339f-174">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="c339f-175">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="c339f-175">SCENARIOS:</span></span>

1. <span data-ttu-id="c339f-176">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="c339f-176">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="c339f-177">Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="c339f-177">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="c339f-178">Assurez-vous que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c339f-178">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Occasion":::

   3. <span data-ttu-id="c339f-180">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="c339f-180">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="c339f-181">**Synchroniser avec l’espace partenaires**: Oui</span><span class="sxs-lookup"><span data-stu-id="c339f-181">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="c339f-182">**Comment Microsoft peut-il vous aider ?**:</span><span class="sxs-lookup"><span data-stu-id="c339f-182">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sélections d’aide":::

      - <span data-ttu-id="c339f-184">**Produits**: ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="c339f-184">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="c339f-185">Une fois que l’opportunité est créée dans Dynamics 365 avec l’option **sync with Partner Center** définie sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c339f-185">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="c339f-186">Vos références seront synchronisées avec Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c339f-186">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="c339f-187">Par conséquent, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c339f-187">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="c339f-188">Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="c339f-188">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="c339f-189">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :</span><span class="sxs-lookup"><span data-stu-id="c339f-189">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="c339f-190">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c339f-190">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="c339f-191">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="c339f-191">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="c339f-192">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="c339f-192">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="c339f-193">Connectez-vous à votre environnement Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="c339f-193">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="c339f-194">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="c339f-194">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="c339f-195">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="c339f-195">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="c339f-196">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="c339f-196">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c339f-197">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c339f-197">Next steps</span></span>

- [<span data-ttu-id="c339f-198">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="c339f-198">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="c339f-199">Événements du webhook de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c339f-199">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="c339f-200">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="c339f-200">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c339f-201">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="c339f-201">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
