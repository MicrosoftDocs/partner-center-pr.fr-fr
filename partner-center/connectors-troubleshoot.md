---
title: Résoudre les problèmes des connecteurs de référencements de covente
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les réponses aux questions courantes sur l’utilisation des connecteurs de co-vente. Lisez ce Forum aux questions sur la résolution des problèmes de co-vente des connecteurs.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354540"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="6da4e-104">Résoudre les problèmes des connecteurs de référencements de covente</span><span class="sxs-lookup"><span data-stu-id="6da4e-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="6da4e-105">**S’applique à :**</span><span class="sxs-lookup"><span data-stu-id="6da4e-105">**Applies to:**</span></span>

- <span data-ttu-id="6da4e-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="6da4e-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="6da4e-107">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="6da4e-107">Salesforce CRM</span></span>

<span data-ttu-id="6da4e-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="6da4e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="6da4e-109">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="6da4e-109">Referrals admin</span></span>
- <span data-ttu-id="6da4e-110">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="6da4e-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="6da4e-111">Questions et réponses sur les conditions préalables</span><span class="sxs-lookup"><span data-stu-id="6da4e-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="6da4e-112">Pouvez-vous utiliser une solution de connecteurs de références de co-vente d’essai pour votre environnement ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="6da4e-113">Si vous êtes dans l’environnement test/intermédiaire, vous pouvez opter pour une solution d’évaluation.</span><span class="sxs-lookup"><span data-stu-id="6da4e-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="6da4e-114">La version payante des connecteurs est disponible dans AppSource au 15 au mois.</span><span class="sxs-lookup"><span data-stu-id="6da4e-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="6da4e-115">Avec la connexion payante, vous obtenez jusqu’à 10 000 appels d’API par jour.</span><span class="sxs-lookup"><span data-stu-id="6da4e-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="6da4e-116">Les connecteurs sont des wrappers par-dessus les API de référence de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6da4e-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="6da4e-117">Chaque fois que les solutions de connecteur s’exécutent pour un événement de **création** ou de **mise à jour** sur les opportunités sur l’espace partenaires ou le côté CRM, un appel d’API est effectué.</span><span class="sxs-lookup"><span data-stu-id="6da4e-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="6da4e-118">Quel rôle avez-vous besoin pour créer des sections dans l’environnement CRM ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="6da4e-119">Les utilisateurs qui sont des administrateurs système ou des personnalisateurs de systèmes peuvent appliquer des modifications pour tout le monde.</span><span class="sxs-lookup"><span data-stu-id="6da4e-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="6da4e-120">Toutefois, tous les utilisateurs de l’application peuvent personnaliser le système et même partager certaines de leurs personnalisations avec d’autres utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6da4e-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="6da4e-121">Les vendeurs partenaires ont-ils besoin de rôles spéciaux pour travailler sur l’espace partenaires ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="6da4e-122">Le rôle « administrateur des références » doit être attribué aux vendeurs partenaires.</span><span class="sxs-lookup"><span data-stu-id="6da4e-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="6da4e-123">Pour plus d’informations, reportez-vous à la [vue d’ensemble des autorisations] (Create-User-Accounts-and-Set-Permissions).</span><span class="sxs-lookup"><span data-stu-id="6da4e-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="6da4e-124">Quels champs doivent être configurés en premier dans votre environnement CRM ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="6da4e-125">• Assurez-vous que votre devise est adaptée à votre emplacement et dans votre environnement CRM avec précision.</span><span class="sxs-lookup"><span data-stu-id="6da4e-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="6da4e-126">• Votre équipe de vente doit être inscrite dans votre environnement CRM en tant qu’utilisateurs CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="6da4e-127">Quelles sont les conditions préalables requises pour la création d’un environnement Power automate ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="6da4e-128">Pour utiliser l’environnement Power automate, vous avez besoin des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6da4e-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="6da4e-129">Une licence Power automate est requise.</span><span class="sxs-lookup"><span data-stu-id="6da4e-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="6da4e-130">Un espace de stockage de 1 Go au minimum est requis.</span><span class="sxs-lookup"><span data-stu-id="6da4e-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="6da4e-131">Avez-vous besoin d’un abonnement Dynamics 365 pour utiliser la solution de connecteurs Salesforce ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="6da4e-132">La solution de connecteur Salesforce est de type « Dynamics Flow » qui prend en charge la synchronisation avec d’autres systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="6da4e-133">La solution ne nécessite pas que vous disposiez d’une instance Dynamics 365 ou d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="6da4e-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="6da4e-134">Lors de l’installation de la solution Salesforce, une liste déroulante contenant les CD existants dans votre entreprise peut s’afficher.</span><span class="sxs-lookup"><span data-stu-id="6da4e-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="6da4e-135">Vous devez sélectionner cet environnement.</span><span class="sxs-lookup"><span data-stu-id="6da4e-135">You need to select that environment.</span></span> <span data-ttu-id="6da4e-136">En outre, si vous obtenez l’erreur « Impossible de trouver une organisation Dynamics 365 connectée à un utilisateur connecté », vous devrez créer un nouvel environnement pour le connecteur.</span><span class="sxs-lookup"><span data-stu-id="6da4e-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="6da4e-137">Questions et réponses sur la configuration</span><span class="sxs-lookup"><span data-stu-id="6da4e-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="6da4e-138">Que devez-vous faire si vous êtes confronté à l’erreur suivante lors de l’activation de flux dans Power Automated Platform ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="6da4e-139">Erreur : la demande de Azure Resource Manager a échoué avec l’erreur : « {erreur » : {« code » : « WorkflowTriggerNotFound », « message » : « le déclencheur «e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 » du workflow « Manual » est introuvable.»}}».</span><span class="sxs-lookup"><span data-stu-id="6da4e-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="6da4e-140">Suivez les étapes de dépannage suivantes :</span><span class="sxs-lookup"><span data-stu-id="6da4e-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6da4e-141">Supprimez la connexion CDS, puis recréez les connexions CDS.</span><span class="sxs-lookup"><span data-stu-id="6da4e-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="6da4e-142">Activer et désactiver le workflow enfant</span><span class="sxs-lookup"><span data-stu-id="6da4e-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="6da4e-143">Supprimez la solution, puis réinstallez la solution.</span><span class="sxs-lookup"><span data-stu-id="6da4e-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="6da4e-144">Que devez-vous faire si vous êtes confronté à l’erreur de connexion lors de l’ajout d’un connecteur de l’espace partenaires dans Power Automated Platform ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Message d’erreur nécessitant une connexion":::

<span data-ttu-id="6da4e-146">Suivez cette étape de résolution des problèmes :</span><span class="sxs-lookup"><span data-stu-id="6da4e-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="6da4e-147">Utilisez vos informations d’identification de l’espace partenaires pour vous connecter à l’environnement Flow une seule fois (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="6da4e-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="6da4e-148">Que devez-vous faire si vous recevez l’erreur suivante lors de l’activation de l’espace partenaires sur le Flow CRM dans Power Automated Platform ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Message d’erreur nécessitant des mises à jour":::

<span data-ttu-id="6da4e-150">Suivez les étapes de dépannage suivantes :</span><span class="sxs-lookup"><span data-stu-id="6da4e-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="6da4e-151">Commencez par activer les deux flux enfants suivants avant d’activer l’espace partenaires dans le flux CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="6da4e-152">Espace partenaires vers CRM-Helper (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="6da4e-153">Espace partenaires Microsoft : mises à jour de référence de la co-vente à CRM (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="6da4e-154">Que devez-vous faire lorsque vous n’êtes pas en mesure d’ajouter des connexions au Flow lorsque vous essayez de modifier le Flow ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="6da4e-155">Vous ajoutez des connexions au workflow pendant l’exécution du workflow et vous ajoutez à chaque Flow séparément.</span><span class="sxs-lookup"><span data-stu-id="6da4e-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="6da4e-156">Si la boîte de dialogue d’ajout de connexions ne s’ouvre pas automatiquement pendant la modification du flux, vous pouvez modifier individuellement chacune des étapes et des sous-étapes des flux.</span><span class="sxs-lookup"><span data-stu-id="6da4e-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="6da4e-157">Sélectionnez chaque Flow et modifiez-les individuellement.</span><span class="sxs-lookup"><span data-stu-id="6da4e-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="6da4e-158">Développer toutes les étapes du Flow</span><span class="sxs-lookup"><span data-stu-id="6da4e-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Étapes nécessitant des connexions":::

- <span data-ttu-id="6da4e-160">Sélectionnez les étapes dans lesquelles une icône d’avertissement s’affiche et vous invite à associer des connexions et à ajouter des connexions.</span><span class="sxs-lookup"><span data-stu-id="6da4e-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modifier le Flow étape par étape":::


5. <span data-ttu-id="6da4e-162">Que devez-vous faire si les flux de la solution de références de covente des connexions ne sont pas activés ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="6da4e-163">R.</span><span class="sxs-lookup"><span data-stu-id="6da4e-163">A.</span></span> <span data-ttu-id="6da4e-164">Dans Power automate, vous devez modifier les flux dans l’ordre suivant et les mettre à jour pour qu’ils utilisent les bonnes connexions :</span><span class="sxs-lookup"><span data-stu-id="6da4e-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="6da4e-165">Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-166">Créer une référence de covente-Salesforce à l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-167">Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-168">Espace partenaires vers Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-169">Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-170">Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6da4e-171">Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="6da4e-172">B.</span><span class="sxs-lookup"><span data-stu-id="6da4e-172">B.</span></span> <span data-ttu-id="6da4e-173">Pour chaque Flow, sélectionnez l’option **exécuter uniquement les utilisateurs** .</span><span class="sxs-lookup"><span data-stu-id="6da4e-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="6da4e-174">Sélectionnez **utiliser la connexion** au lieu de **fourni par l’utilisateur en exécution seule**.</span><span class="sxs-lookup"><span data-stu-id="6da4e-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Pour activer un Flow":::


<span data-ttu-id="6da4e-176">C.</span><span class="sxs-lookup"><span data-stu-id="6da4e-176">C.</span></span> <span data-ttu-id="6da4e-177">Activez les flux indiqués ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="6da4e-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="6da4e-178">Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="6da4e-179">Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6da4e-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="6da4e-180">D.</span><span class="sxs-lookup"><span data-stu-id="6da4e-180">D.</span></span> <span data-ttu-id="6da4e-181">Activez tous les flux restants.</span><span class="sxs-lookup"><span data-stu-id="6da4e-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="6da4e-182">E.</span><span class="sxs-lookup"><span data-stu-id="6da4e-182">E.</span></span> <span data-ttu-id="6da4e-183">Dans l’inscription au webhook de l’espace partenaires, sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="6da4e-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="6da4e-184">Fournissez l' **URL http** à partir de la première action dans **Partner Center vers Salesforce** Flow.</span><span class="sxs-lookup"><span data-stu-id="6da4e-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="6da4e-185">Sélectionnez les quatre options sous **événements à inscrire** , puis sélectionnez **Oui** pour le remplacement.</span><span class="sxs-lookup"><span data-stu-id="6da4e-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="6da4e-186">Questions et réponses sur l’exécution et la maintenance</span><span class="sxs-lookup"><span data-stu-id="6da4e-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="6da4e-187">Comment résoudre les problèmes en cas de défaillances lors de l’exécution d’automate Power ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="6da4e-188">Pour vous assurer que vos flux d’automati s’exécutent comme prévu et pour résoudre les problèmes d’échec lors de l’exécution, reportez-vous à [corriger les échecs de flux](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="6da4e-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="6da4e-189">Que devez-vous faire si vous voyez des références qui ne sont pas correctement synchronisées dans l’espace partenaires ou l’environnement CRM ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="6da4e-190">Pour déterminer l’état de synchronisation de la référence, sélectionnez **audit**.</span><span class="sxs-lookup"><span data-stu-id="6da4e-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronisation des références":::

<span data-ttu-id="6da4e-192">Assurez-vous que les conditions suivantes sont remplies :</span><span class="sxs-lookup"><span data-stu-id="6da4e-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="6da4e-193">L’ID de solution est fourni dans le cadre de l’opportunité.</span><span class="sxs-lookup"><span data-stu-id="6da4e-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="6da4e-194">Un code de pays à deux lettres est requis.</span><span class="sxs-lookup"><span data-stu-id="6da4e-194">Two letter country code is required.</span></span>

- <span data-ttu-id="6da4e-195">Lorsque l’aide de Microsoft est sélectionnée pour l’opportunité, les coordonnées du client sont requises.</span><span class="sxs-lookup"><span data-stu-id="6da4e-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="6da4e-196">Comment s’assurer qu’une référence sera synchronisée de manière bidirectionnelle ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="6da4e-197">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6da4e-197">Do the following steps:</span></span>

- <span data-ttu-id="6da4e-198">Les vendeurs partenaires doivent s’assurer qu’ils ont activé l’option **synchroniser avec l’espace partenaires** dans la section CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Vérifiez que vous avez activé la synchronisation":::

- <span data-ttu-id="6da4e-200">Les vendeurs doivent fournir un chiffre d’affaires et une date de clôture lorsqu’ils qualifient un prospect.</span><span class="sxs-lookup"><span data-stu-id="6da4e-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="6da4e-201">Si l’ID CRM est fourni à l’étape de **création** ou de **mise à jour** d’une opportunité de covente, mais qu’une opportunité de prospect avec cet ID est introuvable dans CRM, la mise à jour ou la création sera ignorée.</span><span class="sxs-lookup"><span data-stu-id="6da4e-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="6da4e-202">Assurez-vous que le champ devise de référence est configuré dans l’environnement Salesforce.</span><span class="sxs-lookup"><span data-stu-id="6da4e-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="6da4e-203">Que devez-vous faire si le connecteur est déconnecté et que vous manquez une synchronisation de référence.</span><span class="sxs-lookup"><span data-stu-id="6da4e-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="6da4e-204">Voici quelques-unes des options que vous pouvez essayer :</span><span class="sxs-lookup"><span data-stu-id="6da4e-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="6da4e-205">Vérifiez si le nom d’utilisateur ou le mot de passe a expiré pour l’utilisateur de l’espace partenaires avec des rôles d’administrateur de référence.</span><span class="sxs-lookup"><span data-stu-id="6da4e-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="6da4e-206">Vous pouvez accéder à l’opportunité non synchronisée, effectuer une mise à jour mineure et observer si la référence a été synchronisée.</span><span class="sxs-lookup"><span data-stu-id="6da4e-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="6da4e-207">Si les flux ont été exécutés et ont échoué, sélectionnez le flux et soumettez à nouveau l’exécution qui a échoué.</span><span class="sxs-lookup"><span data-stu-id="6da4e-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="6da4e-208">Que devez-vous faire lorsque vous recevez des erreurs d’accès refusé ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="6da4e-209">Assurez-vous que les rôles appropriés existent</span><span class="sxs-lookup"><span data-stu-id="6da4e-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="6da4e-210">Rôle d’administrateur de référence pour le vendeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6da4e-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="6da4e-211">Rôle d’administrateur système ou de personnalisateur de système sur votre instance CRM</span><span class="sxs-lookup"><span data-stu-id="6da4e-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="6da4e-212">Assurez-vous que l’utilisateur du compte de gestion de l’alimentation se connecte https://flow.microsoft.com au moins une fois au préalable</span><span class="sxs-lookup"><span data-stu-id="6da4e-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="6da4e-213">Si vous voyez que l' **indicatif du pays du compte client** est manquant lors de la création d’une opportunité de covente, que devez-vous faire ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="6da4e-214">Vous devez ajouter le code du pays ISO à deux lettres au compte client dans CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="6da4e-215">Que devez-vous faire si vous voyez l’erreur indiquant que l' **ID de solution est requis** lors de la création d’une opportunité de covente ?</span><span class="sxs-lookup"><span data-stu-id="6da4e-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="6da4e-216">Pour créer une référence de covente, vous avez besoin d’une solution Microsoft de co-vente prête.</span><span class="sxs-lookup"><span data-stu-id="6da4e-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="6da4e-217">Que devez-vous faire lorsque vous voyez des opportunités de covente créées dans l’espace partenaires qui ne sont pas synchronisées avec CRM, même s’il n’y a pas d’erreurs de flow :</span><span class="sxs-lookup"><span data-stu-id="6da4e-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="6da4e-218">Effectuez les actions suivantes :</span><span class="sxs-lookup"><span data-stu-id="6da4e-218">Do the following:</span></span>

- <span data-ttu-id="6da4e-219">Une fois que vous avez créé une nouvelle vente de covente dans l’espace partenaires, vérifiez si l’option espace partenaires pour Dynamics 365 Flow est invoquée (elle peut être appelée plusieurs fois).</span><span class="sxs-lookup"><span data-stu-id="6da4e-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="6da4e-220">Si le flux est appelé, vérifiez tous les flux appelés et identifiez l’exécution du flux qui met à jour le CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="6da4e-221">Vous pouvez suivre les actions et vérifier si le service CRM a été mis à jour ou si un problème s’est produit.</span><span class="sxs-lookup"><span data-stu-id="6da4e-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="6da4e-222">Cochez *nouveau contrat*\* dans l’espace partenaires pour voir s’il est rempli avec l’ID CRM.</span><span class="sxs-lookup"><span data-stu-id="6da4e-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="6da4e-223">Assurez-vous que la transaction n’est pas fermée par erreur en tant que « gagné » ou « perdue » dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6da4e-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6da4e-224">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6da4e-224">Next steps</span></span>

- [<span data-ttu-id="6da4e-225">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="6da4e-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="6da4e-226">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="6da4e-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
