---
title: Transférer un abonnement Azure dans le cadre d’un plan Azure à un autre partenaire CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment modifier le partenaire du programme fournisseur de solutions Cloud associé aux abonnements Azure d’un client dans le cadre d’un plan Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277315"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="c4c78-103">Transférer les abonnements du plan Azure d’un client à un autre partenaire</span><span class="sxs-lookup"><span data-stu-id="c4c78-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="c4c78-104">**Rôles appropriés**: administrateur de compte | Agent commercial | Agent de facturation</span><span class="sxs-lookup"><span data-stu-id="c4c78-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="c4c78-105">Cet article décrit comment un client peut passer d’un fournisseur de solutions Cloud (CSP) à un autre dans le cadre d’un projet Azure.</span><span class="sxs-lookup"><span data-stu-id="c4c78-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="c4c78-106">Pour faire basculer les abonnements Azure d’un client d’un autre partenaire, procédez comme suit.</span><span class="sxs-lookup"><span data-stu-id="c4c78-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="c4c78-107">Le partenaire et le client ont tous les deux la procédure à suivre.</span><span class="sxs-lookup"><span data-stu-id="c4c78-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="c4c78-108">Seuls les partenaires disposant d’une relation de facturation directe avec Microsoft peuvent accéder aux outils de transition.</span><span class="sxs-lookup"><span data-stu-id="c4c78-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="c4c78-109">Les revendeurs indirects doivent collaborer avec leurs fournisseurs indirects pour tirer parti de cet outil de transition.</span><span class="sxs-lookup"><span data-stu-id="c4c78-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="c4c78-110">Le client doit être en conversation avec les deux partenaires (actuels et futurs) avant de tirer parti de cet outil.</span><span class="sxs-lookup"><span data-stu-id="c4c78-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="c4c78-111">Une conversation hors connexion doit être nécessaire pour éviter les confusions et les évolutions.</span><span class="sxs-lookup"><span data-stu-id="c4c78-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="c4c78-112">En outre, les partenaires et les clients doivent comprendre ces considérations et conditions préalables avant d’initier une transition :</span><span class="sxs-lookup"><span data-stu-id="c4c78-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="c4c78-113">**Points clés :**</span><span class="sxs-lookup"><span data-stu-id="c4c78-113">**Key considerations:**</span></span>

- <span data-ttu-id="c4c78-114">Azure Reservations ne se déplacera pas avec l’abonnement au futur partenaire</span><span class="sxs-lookup"><span data-stu-id="c4c78-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="c4c78-115">La tarification du fournisseur CSP pour les services Azure sous le partenaire actuel n’est pas transition</span><span class="sxs-lookup"><span data-stu-id="c4c78-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="c4c78-116">Les responsabilités de support pour le client seront déplacées vers le futur partenaire</span><span class="sxs-lookup"><span data-stu-id="c4c78-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="c4c78-117">La facturation et la facturation seront déplacées vers le futur partenaire au moment du transfert</span><span class="sxs-lookup"><span data-stu-id="c4c78-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="c4c78-118">Le Access Control de Role-Based Azure (RBAC) n’est pas affecté par le transfert</span><span class="sxs-lookup"><span data-stu-id="c4c78-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="c4c78-119">L’administrateur pour le compte de (ADMINISTRATE) ne sera pas accordé par défaut au partenaire futur</span><span class="sxs-lookup"><span data-stu-id="c4c78-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="c4c78-120">Les produits de la place de marché tiers sont transférés tant que les produits réussissent la vérification du droit de la place de marché.</span><span class="sxs-lookup"><span data-stu-id="c4c78-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="c4c78-121">Il n’existe aucune remise spéciale ou restriction régionale</span><span class="sxs-lookup"><span data-stu-id="c4c78-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="c4c78-122">Les produits ne sont pas basés sur un abonnement</span><span class="sxs-lookup"><span data-stu-id="c4c78-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="c4c78-123">Le futur partenaire devrait travailler avec le serveur de publication pour s’assurer qu’il se trouve dans la liste verte pour le déploiement du produit</span><span class="sxs-lookup"><span data-stu-id="c4c78-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="c4c78-124">Si certaines de ces conditions ne sont pas respectées pour transférer les produits de la place de marché, ils doivent être annulés, les abonnements Azure transférés, puis reacheter les produits de la place de marché auprès du nouveau partenaire.</span><span class="sxs-lookup"><span data-stu-id="c4c78-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="c4c78-125">**Configuration requise :**</span><span class="sxs-lookup"><span data-stu-id="c4c78-125">**Prerequisites:**</span></span>

- <span data-ttu-id="c4c78-126">Le client fait appel au partenaire CSP actuel en cas de transition</span><span class="sxs-lookup"><span data-stu-id="c4c78-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="c4c78-127">Le futur partenaire CSP travaille avec le client pour s’assurer que les besoins des clients peuvent être satisfaits</span><span class="sxs-lookup"><span data-stu-id="c4c78-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="c4c78-128">Le futur partenaire CSP établit une relation avec le client et achète un plan Azure avant le début de la transition</span><span class="sxs-lookup"><span data-stu-id="c4c78-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="c4c78-129">Le client doit signer le contrat du client Microsoft avec un partenaire CSP futur</span><span class="sxs-lookup"><span data-stu-id="c4c78-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="c4c78-130">Le futur partenaire CSP doit avoir signé l’accord de partenariat Microsoft pour utiliser cet outil</span><span class="sxs-lookup"><span data-stu-id="c4c78-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="c4c78-131">Tâches client à effectuer</span><span class="sxs-lookup"><span data-stu-id="c4c78-131">Customer tasks to be completed</span></span>

<span data-ttu-id="c4c78-132">Pour transférer un abonnement Azure dans le cadre d’un plan Azure, le client doit démarrer le processus en contactant son partenaire actuel.</span><span class="sxs-lookup"><span data-stu-id="c4c78-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="c4c78-133">Ils doivent collecter le nom et le domaine de l’entreprise de leur partenaire actuel, de sorte que son partenaire futur puisse remplir le formulaire de demande de transfert en son nom.</span><span class="sxs-lookup"><span data-stu-id="c4c78-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="c4c78-134">Le client doit également identifier les abonnements qu’il souhaite transférer de son partenaire actuel.</span><span class="sxs-lookup"><span data-stu-id="c4c78-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="c4c78-135">Vous ne pouvez pas changer de partenaire pour les abonnements Office 365, Enterprise Mobility suite ou Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="c4c78-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="c4c78-136">Il incombe au futur partenaire de terminer le formulaire de demande de transfert qui initie le processus de transfert.</span><span class="sxs-lookup"><span data-stu-id="c4c78-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="c4c78-137">Microsoft ne peut pas intervenir pour le compte du client ou du partenaire actuel.</span><span class="sxs-lookup"><span data-stu-id="c4c78-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="c4c78-138">Le client doit planifier un travail en étroite collaboration avec son partenaire futur et actuel pour effectuer la transition en douceur.</span><span class="sxs-lookup"><span data-stu-id="c4c78-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="c4c78-139">Futures tâches de partenaire à effectuer</span><span class="sxs-lookup"><span data-stu-id="c4c78-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="c4c78-140">Le futur partenaire de l’abonnement doit remplir un formulaire de demande de transfert de l’espace partenaires pour demander un transfert d’abonnement :</span><span class="sxs-lookup"><span data-stu-id="c4c78-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="c4c78-141">Dans le menu espace partenaires, sélectionnez **clients**, puis sélectionnez le client pour lequel vous souhaitez terminer un formulaire de demande de transfert pour le compte de.</span><span class="sxs-lookup"><span data-stu-id="c4c78-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="c4c78-142">Dans le menu client, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="c4c78-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="c4c78-143">Sélectionnez la section **demande de transfert** .</span><span class="sxs-lookup"><span data-stu-id="c4c78-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="c4c78-144">Dans la **section demande de transfert**, sélectionnez **Ajouter une nouvelle demande**.</span><span class="sxs-lookup"><span data-stu-id="c4c78-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Section des transferts.":::

5.  <span data-ttu-id="c4c78-146">Complétez le formulaire **de demande de transfert** .</span><span class="sxs-lookup"><span data-stu-id="c4c78-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="c4c78-147">Sélectionnez **Envoyer une demande de transfert**  >  **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="c4c78-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Complétez le formulaire de demande de transfert.":::

7.  <span data-ttu-id="c4c78-149">Vérifier la confirmation de demande de transfert</span><span class="sxs-lookup"><span data-stu-id="c4c78-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Vérifiez le transfert en attente.":::

    >[!Note]
    ><span data-ttu-id="c4c78-151">Le futur partenaire peut annuler la demande de transfert en sélectionnant **annuler la demande** dans le coin supérieur droit uniquement lorsque l’état de la demande de transfert est « en attente ».</span><span class="sxs-lookup"><span data-stu-id="c4c78-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="c4c78-152">Une fois que l’état de la demande de transfert est « en cours » ou « terminé », les annulations ne sont pas possibles.</span><span class="sxs-lookup"><span data-stu-id="c4c78-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="c4c78-153">Tâches de partenaire actuelles à effectuer</span><span class="sxs-lookup"><span data-stu-id="c4c78-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="c4c78-154">L’agent admin du partenaire actuel recevra un e-mail indiquant que son client demande un transfert de ses abonnements :</span><span class="sxs-lookup"><span data-stu-id="c4c78-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Révise.":::

<span data-ttu-id="c4c78-156">Passez en revue et acceptez le formulaire de demande de transfert de l’espace partenaires pour terminer le transfert de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c4c78-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="c4c78-157">Si aucune action n’est effectuée par le partenaire actuel dans un délai de 30 jours, la demande expire et le partenaire futur aura un pour créer une demande de transfert.</span><span class="sxs-lookup"><span data-stu-id="c4c78-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="c4c78-158">Sélectionnez **passer en revue la demande de transfert** à partir de l’e-mail ou</span><span class="sxs-lookup"><span data-stu-id="c4c78-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="c4c78-159">Dans le menu espace partenaires, sélectionnez **clients**, puis sélectionnez le client pour lequel une demande de transfert a été soumise pour le compte de.</span><span class="sxs-lookup"><span data-stu-id="c4c78-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="c4c78-160">Dans le menu client, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="c4c78-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="c4c78-161">Sélectionnez la section **demande de transfert** .</span><span class="sxs-lookup"><span data-stu-id="c4c78-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="c4c78-162">Développez les informations de transfert en sélectionnant l' **ID de demande de transfert** choisi sous **demandes reçues** .</span><span class="sxs-lookup"><span data-stu-id="c4c78-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Demande de transfert de révisions de la source.":::

5.  <span data-ttu-id="c4c78-164">Passez en revue la demande de transfert.</span><span class="sxs-lookup"><span data-stu-id="c4c78-164">Review transfer request.</span></span> <span data-ttu-id="c4c78-165">Sélectionnez les abonnements Azure demandés à transférer.</span><span class="sxs-lookup"><span data-stu-id="c4c78-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="c4c78-166">Avant de poursuivre, veuillez noter que vous n’aurez plus accès aux abonnements sélectionnés.</span><span class="sxs-lookup"><span data-stu-id="c4c78-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="c4c78-167">Vous ne serez pas facturé pour une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="c4c78-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="c4c78-168">Les réservations Azure ne sont pas transférées avec les abonnements.</span><span class="sxs-lookup"><span data-stu-id="c4c78-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="c4c78-169">Sélectionnez ensuite **accepter et transférer** pour terminer le processus de transfert.</span><span class="sxs-lookup"><span data-stu-id="c4c78-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sélectionnez les abonnements à transférer sous vos plans Azure.":::

7.  <span data-ttu-id="c4c78-171">Affichez la confirmation de l’acceptation du transfert.</span><span class="sxs-lookup"><span data-stu-id="c4c78-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="c4c78-172">À ce stade, le futur partenaire, le client et le partenaire actuel seront avertis de la demande de transfert acceptée par courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="c4c78-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="c4c78-173">Après, la transition a été acceptée, l’état du transfert peut rester en attente pendant 15 minutes maximum pendant la mise à jour du système.</span><span class="sxs-lookup"><span data-stu-id="c4c78-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="c4c78-174">Si cela prend plus de temps, le système continuera à essayer pendant trois jours.</span><span class="sxs-lookup"><span data-stu-id="c4c78-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="c4c78-175">Si l’état du transfert reste toujours en attente, le partenaire doit soumettre une demande de service.</span><span class="sxs-lookup"><span data-stu-id="c4c78-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="c4c78-176">Une fois le transfert terminé, les abonnements inclus dans la demande s’affichent dans le plan Azure du futur partenaire et ne sont plus répertoriés avec vous.</span><span class="sxs-lookup"><span data-stu-id="c4c78-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="c4c78-177">Pour les fournisseurs indirects : Veuillez informer votre revendeur indirect que la demande de transfert a été acceptée.</span><span class="sxs-lookup"><span data-stu-id="c4c78-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="c4c78-178">Gestion de vos abonnements client transférés</span><span class="sxs-lookup"><span data-stu-id="c4c78-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="c4c78-179">L’accès aux utilisateurs, groupes ou principaux de service existants auxquels a été affecté le contrôle d’accès en fonction du rôle Azure (RBAC) n’est pas affecté pendant la transition.</span><span class="sxs-lookup"><span data-stu-id="c4c78-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="c4c78-180">Le contrôle d’accès en fonction du rôle [(RBAC)](/azure/role-based-access-control/overview) Azure permet à votre client de gérer qui a accès aux ressources Azure, ce qu’il peut faire avec ces ressources et les domaines auxquels ils ont accès.</span><span class="sxs-lookup"><span data-stu-id="c4c78-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="c4c78-181">En tant que nouveau partenaire, vous ne disposez d’aucun accès RBAC aux ressources de votre client après le transfert de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="c4c78-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="c4c78-182">Le partenaire précédent de votre client conserve son accès RBAC.</span><span class="sxs-lookup"><span data-stu-id="c4c78-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="c4c78-183">Collaborez avec votre client pour comprendre qui a un aperçu de ses abonnements et comment apporter les modifications souhaitées.</span><span class="sxs-lookup"><span data-stu-id="c4c78-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="c4c78-184">Par conséquent, il est important que votre client supprime l’accès RBAC Azure pour son partenaire précédent et ajoute un accès pour le nouveau partenaire.</span><span class="sxs-lookup"><span data-stu-id="c4c78-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="c4c78-185">Pour plus d’informations sur votre client donnant accès à un nouvel accès, consultez [qu’est-ce que le contrôle d’accès en fonction du rôle Azure (Azure RBAC) ?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="c4c78-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="c4c78-186">Pour plus d’informations sur votre client qui supprime l’accès RBAC de votre partenaire précédent, consultez [supprimer une attribution de rôle](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="c4c78-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="c4c78-187">En outre, vous ne disposez pas automatiquement de l’accès de l’administrateur pour le [compte de (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) à vos abonnements.</span><span class="sxs-lookup"><span data-stu-id="c4c78-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="c4c78-188">ADMINISTRATE est nécessaire pour que le partenaire gère les abonnements Azure de ses clients en leur nom.</span><span class="sxs-lookup"><span data-stu-id="c4c78-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="c4c78-189">Pour plus d’informations sur les privilèges Azure, consultez [obtenir des autorisations pour gérer le service ou l’abonnement d’un client.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="c4c78-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="c4c78-190">Étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="c4c78-190">Next steps:</span></span>

- [<span data-ttu-id="c4c78-191">(RBAC Azure)</span><span class="sxs-lookup"><span data-stu-id="c4c78-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="c4c78-192">Obtenir des autorisations pour gérer le service ou l’abonnement d’un client.</span><span class="sxs-lookup"><span data-stu-id="c4c78-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
