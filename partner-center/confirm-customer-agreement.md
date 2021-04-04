---
title: Comment vérifier que votre client a accepté le Contrat client Microsoft pour le programme Fournisseur de solutions Microsoft Cloud
description: Les partenaires fournisseurs de solutions Cloud (CSP) doivent confirmer l’acceptation par le client du Contrat client Microsoft avant de leur commander des services Microsoft.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633776"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="0743f-103">Comment vérifier que votre client a accepté le Contrat client Microsoft pour le programme Fournisseur de solutions Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="0743f-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="0743f-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="0743f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0743f-105">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="0743f-105">Admin agent</span></span>
- <span data-ttu-id="0743f-106">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="0743f-106">Sales agent</span></span>


<span data-ttu-id="0743f-107">Les clients disposent de deux options pour accepter le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="0743f-108">**Option 1** : Attestation du partenaire de l’acceptation par les clients - Le partenaire peut confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires ou via le tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0743f-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="0743f-109">**Option 2** : Acceptation directe par le client - Le partenaire peut inviter le client via une URL à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="0743f-110">Accéder au modèle de Contrat client Microsoft</span><span class="sxs-lookup"><span data-stu-id="0743f-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="0743f-111">Vous pouvez télécharger manuellement la dernière version du modèle de Contrat client Microsoft à partir d’[ici](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="0743f-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="0743f-112">Le Contrat client Microsoft est spécifique au pays.</span><span class="sxs-lookup"><span data-stu-id="0743f-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="0743f-113">Quand vous demandez le modèle de Contrat client Microsoft, veillez à sélectionner le pays approprié en fonction de la localisation du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="0743f-114">Option 1 : Confirmer l’acceptation du client dans l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0743f-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="0743f-115">Les partenaires de facturation directe peuvent confirmer l’acceptation par les clients du Contrat client Microsoft dans l’Espace partenaires pour les clients nouveaux et existants.</span><span class="sxs-lookup"><span data-stu-id="0743f-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="0743f-116">Les revendeurs indirects ne peuvent pas effectuer d’attestation au nom de leurs clients. Ils doivent collaborer avec leur fournisseur indirect pour obtenir l’attestation.</span><span class="sxs-lookup"><span data-stu-id="0743f-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="0743f-117">Confirmer l’acceptation par les nouveaux clients</span><span class="sxs-lookup"><span data-stu-id="0743f-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="0743f-118">Lorsque vous créez un locataire client dans l’Espace partenaires, suivez les étapes ci-dessous pour confirmer l’acceptation par le client du contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="0743f-119">Vous devez être Agent administrateur ou Commercial pour suivre ces étapes.</span><span class="sxs-lookup"><span data-stu-id="0743f-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="0743f-120">Sélectionnez **Clients**, puis **Nouveau client**.</span><span class="sxs-lookup"><span data-stu-id="0743f-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="0743f-121">Sous **Informations sur le compte**, entrez les informations relatives à l’entreprise et à son contact principal.</span><span class="sxs-lookup"><span data-stu-id="0743f-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="0743f-122">Sous **Contrat Microsoft**, cochez la case permettant d’attester que le client a accepté le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="0743f-123">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="0743f-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="0743f-124">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0743f-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="0743f-125">Assurez-vous que les coordonnées de l’utilisateur principal affichées sont correctes.</span><span class="sxs-lookup"><span data-stu-id="0743f-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="0743f-126">Si ce n’est pas le cas, sélectionnez **Mettre à jour** et entrez les informations exactes de la personne qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="0743f-127">Sélectionnez **Suivant** pour continuer à créer le locataire du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nouveau client":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="0743f-129">Confirmer l’acceptation par les clients existants</span><span class="sxs-lookup"><span data-stu-id="0743f-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="0743f-130">Pour ce faire, vous devez être un agent d’administration ou un commercial :</span><span class="sxs-lookup"><span data-stu-id="0743f-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="0743f-131">Sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="0743f-131">Select **Customers**.</span></span> <span data-ttu-id="0743f-132">Recherchez et sélectionnez le client.</span><span class="sxs-lookup"><span data-stu-id="0743f-132">Find and select the customer.</span></span>

2. <span data-ttu-id="0743f-133">Sélectionnez **Informations sur le compte**.</span><span class="sxs-lookup"><span data-stu-id="0743f-133">Select **Account info**.</span></span>

3. <span data-ttu-id="0743f-134">Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="0743f-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="0743f-135">Saisissez les **Prénom**, **Nom**, **Adresse e-mail** et **Numéro de téléphone** (facultatif) de la personne qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="0743f-136">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="0743f-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="0743f-137">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0743f-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="0743f-138">Sélectionnez **Enregistrer** et continuez.</span><span class="sxs-lookup"><span data-stu-id="0743f-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Client existant":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="0743f-140">Récupérer la confirmation de l’acceptation par le client</span><span class="sxs-lookup"><span data-stu-id="0743f-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="0743f-141">Pour récupérer la confirmation qu’un client existant a accepté le Contrat client Microsoft, procédez comme suit.</span><span class="sxs-lookup"><span data-stu-id="0743f-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="0743f-142">Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="0743f-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="0743f-143">Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="0743f-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="0743f-144">Sélectionnez **Informations sur le compte**.</span><span class="sxs-lookup"><span data-stu-id="0743f-144">Select **Account info**.</span></span>

3. <span data-ttu-id="0743f-145">Sous **Contrat client Microsoft**, vérifiez si la confirmation a été fournie ou n’a pas été fournie par ce client.</span><span class="sxs-lookup"><span data-stu-id="0743f-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="0743f-146">Confirmer l’acceptation par les clients à l’aide de l’API/du kit SDK de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0743f-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="0743f-147">Vous pouvez utiliser l’API/le kit SDK de l’Espace partenaires pour confirmer l’acceptation du Contrat client Microsoft par les clients.</span><span class="sxs-lookup"><span data-stu-id="0743f-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="0743f-148">Pour plus d’informations sur l’API/le SDK, consultez :</span><span class="sxs-lookup"><span data-stu-id="0743f-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="0743f-149">Obtenir les métadonnées du Contrat client Microsoft</span><span class="sxs-lookup"><span data-stu-id="0743f-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="0743f-150">Confirmer que le client a accepté le Contrat client Microsoft</span><span class="sxs-lookup"><span data-stu-id="0743f-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="0743f-151">Obtenir la confirmation de l’acceptation du Contrat client Microsoft par le client</span><span class="sxs-lookup"><span data-stu-id="0743f-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="0743f-152">Obtenir un lien de téléchargement pour le modèle de Contrat client Microsoft</span><span class="sxs-lookup"><span data-stu-id="0743f-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="0743f-153">Option 2 : Acceptation par les clients dans le Centre d’administration Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0743f-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="0743f-154">Les partenaires peuvent inviter de nouveaux clients et des clients existants, via une URL, à passer en revue et accepter le contrat dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="0743f-155">Les sections suivantes vous montrent comment :</span><span class="sxs-lookup"><span data-stu-id="0743f-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="0743f-156">Créer un client, puis l’inviter à passer en revue et accepter le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="0743f-157">Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="0743f-158">Inviter un client existant à passer en revue et accepter le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="0743f-159">Vous pouvez utiliser l’[API ou le SDK de l’Espace partenaires](/partner-center/develop/get-direct-sign-status-of-customer-agreement) pour savoir si le client a accepté directement le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="0743f-160">Créer un client, puis l’inviter à passer en revue et accepter le contrat</span><span class="sxs-lookup"><span data-stu-id="0743f-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="0743f-161">Effectuez les étapes suivantes pour créer un client dans l’Espace partenaires, puis invitez-le à passer en revue et accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="0743f-162">Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez **Ajouter un client**.</span><span class="sxs-lookup"><span data-stu-id="0743f-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="0743f-163">Sous **Informations sur le compte**, entrez les informations relatives au nouveau client dans tous les champs obligatoires, notamment le nom de l’entreprise et le contact principal du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="0743f-164">Sous **Contrat client**, sélectionnez **Le client va être invité à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="0743f-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="0743f-165">Remplissez tous les autres champs obligatoires de la page.</span><span class="sxs-lookup"><span data-stu-id="0743f-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="0743f-166">Sélectionnez **Suivant : Passer en revue**, puis poursuivez les étapes permettant de créer le locataire du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="0743f-167">Les nouveaux clients ne peuvent pas effectuer d’achat tant qu’ils n’ont pas accepté le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Créer un client":::

5. <span data-ttu-id="0743f-169">Une fois que vous avez atteint l’écran **Confirmation** dans le workflow de nouveau client, enregistrez les informations d’identification de ce client.</span><span class="sxs-lookup"><span data-stu-id="0743f-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="0743f-170">Vous devrez plus tard fournir ces informations d’identification à votre client.</span><span class="sxs-lookup"><span data-stu-id="0743f-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="0743f-171">En dehors de l’Espace partenaires, créez et envoyez un e-mail invitant le client à accepter le Contrat client Microsoft dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="0743f-172">Veillez à inclure ces éléments dans l’e-mail :</span><span class="sxs-lookup"><span data-stu-id="0743f-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="0743f-173">Lien vers cette [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (connexion obligatoire)</span><span class="sxs-lookup"><span data-stu-id="0743f-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="0743f-174">Informations d’identification du client, que vous avez enregistrées à l’étape 5.</span><span class="sxs-lookup"><span data-stu-id="0743f-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="0743f-175">Le client va ensuite recevoir l’invitation par e-mail de la part du partenaire et sélectionner l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="0743f-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="0743f-176">Le client se connecte au Centre d’administration Microsoft 365 à l’aide des informations d’identification que vous avez fournies.</span><span class="sxs-lookup"><span data-stu-id="0743f-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="0743f-177">Le client coche la case pour accepter le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="0743f-178">Inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft</span><span class="sxs-lookup"><span data-stu-id="0743f-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="0743f-179">Effectuez les étapes suivantes pour inviter un nouveau client à passer en revue et accepter la relation de revendeur et le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="0743f-180">Sous l’onglet **Clients** de l’Espace partenaires, sélectionnez le lien **Demander une relation de revendeur**.</span><span class="sxs-lookup"><span data-stu-id="0743f-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="0743f-181">Un modèle d’e-mail automatique est généré. Il comprend notamment du texte et une URL paramétrable qui dirige le client vers le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="0743f-182">Vous pouvez personnaliser le modèle d’e-mail généré automatiquement, puis sélectionner **Copier dans le Presse-papiers** ou **Ouvrir un e-mail**.</span><span class="sxs-lookup"><span data-stu-id="0743f-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="0743f-183">Utilisez ce modèle d’e-mail pour inviter le client à accepter la **demande de relation de revendeur** et le **Contrat client Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="0743f-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="0743f-184">(Remarque : Dans l’invitation par e-mail, vérifiez que le partenaire ajoute également l’URL fournie automatiquement ainsi que les informations d’identification client créées.)</span><span class="sxs-lookup"><span data-stu-id="0743f-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="créer une relation":::

5. <span data-ttu-id="0743f-186">Le client reçoit une invitation par e-mail, et clique sur l’URL paramétrable.</span><span class="sxs-lookup"><span data-stu-id="0743f-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="0743f-187">Le client utilise les informations d’identification que vous avez fournies dans l’e-mail pour se connecter au Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="0743f-188">Le client coche la case pour accepter la **relation de revendeur** et le **Contrat client Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="0743f-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="0743f-189">Dans la même URL, le client peut voir une liste centralisée des différents partenaires avec lesquels il travaille.</span><span class="sxs-lookup"><span data-stu-id="0743f-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="0743f-190">Il peut sélectionner un partenaire pour voir les détails correspondants.</span><span class="sxs-lookup"><span data-stu-id="0743f-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Accepter le contrat":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="0743f-192">Inviter un client existant à passer en revue et accepter le contrat</span><span class="sxs-lookup"><span data-stu-id="0743f-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="0743f-193">Effectuez les étapes suivantes pour inviter un client existant à passer en revue et accepter le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="0743f-194">Créez l’e-mail destiné au client avec l’URL intégrée invitant le client à accepter le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="0743f-195">Votre client reçoit l’invitation par e-mail, puis clique sur l’[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="0743f-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="0743f-196">Le client entre ses informations d’identification dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="0743f-197">Votre client coche la case pour accepter le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="0743f-198">Dans la même URL, le client peut voir la liste centralisée des différents partenaires avec lesquels il travaille.</span><span class="sxs-lookup"><span data-stu-id="0743f-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="0743f-199">Il peut sélectionner un partenaire pour voir les détails correspondants.</span><span class="sxs-lookup"><span data-stu-id="0743f-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="client":::

>[!NOTE]
><span data-ttu-id="0743f-201">Dans certains scénarios, les clients ne peuvent pas toujours accepter directement le Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0743f-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="0743f-202">Pour en savoir plus sur ces situations, consultez ci-après Deux scénarios où vous devez effectuer l’attestation au nom de votre client.</span><span class="sxs-lookup"><span data-stu-id="0743f-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="0743f-203">Deux scénarios où vous devez effectuer l’attestation au nom de votre client</span><span class="sxs-lookup"><span data-stu-id="0743f-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="0743f-204">Il existe deux scénarios où les clients ne peuvent pas toujours accepter directement le Contrat client Microsoft dans le Centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0743f-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="0743f-205">**Scénario 1** : Un client existant a acheté l’un des produits suivants via une relation partenaire existante : offres, logiciels ou abonnements logiciels, instances réservées ou plan Azure.</span><span class="sxs-lookup"><span data-stu-id="0743f-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="0743f-206">Le client tente à présent d’effectuer un nouvel achat (en dehors du renouvellement automatique).</span><span class="sxs-lookup"><span data-stu-id="0743f-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="0743f-207">Quand ce client clique sur l’URL, il reçoit un message de ce type : « Contactez votre partenaire pour confirmer votre acceptation du Contrat client Microsoft ».</span><span class="sxs-lookup"><span data-stu-id="0743f-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="0743f-208">**Solution** : Vous devez effectuer l’attestation au nom du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Capture d’écran de la page du Centre d’administration Microsoft 365 vous invitant à contacter votre partenaire pour confirmer l’acceptation du Contrat client Microsoft.":::

<span data-ttu-id="0743f-210">**Scénario 2** : Un client existant a acheté des offres, des logiciels ou des abonnements logiciels, des instances réservées ou un plan Azure.</span><span class="sxs-lookup"><span data-stu-id="0743f-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="0743f-211">Le client tente à présent d’effectuer un nouvel achat auprès d’un nouveau partenaire.</span><span class="sxs-lookup"><span data-stu-id="0743f-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="0743f-212">Quand le client clique sur l’URL du Centre d’administration Microsoft 365 pour accepter la nouvelle relation partenaire et le contrat, il reçoit un message de ce type : « Contactez votre partenaire pour confirmer votre acceptation du Contrat client Microsoft ».</span><span class="sxs-lookup"><span data-stu-id="0743f-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="0743f-213">**Solution** : Vous devez effectuer l’attestation au nom du client.</span><span class="sxs-lookup"><span data-stu-id="0743f-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="0743f-214">Confirmer qu’un client a accepté le contrat</span><span class="sxs-lookup"><span data-stu-id="0743f-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="0743f-215">Si vous essayez de créer une commande pour un client existant que vous n’avez pas encore confirmé, vous recevrez une invite pour effectuer la confirmation.</span><span class="sxs-lookup"><span data-stu-id="0743f-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="0743f-216">Pour ce faire, utilisez la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="0743f-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="0743f-217">Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="0743f-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="0743f-218">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="0743f-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="0743f-219">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0743f-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="0743f-220">Sélectionnez **Enregistrer et continuer**.</span><span class="sxs-lookup"><span data-stu-id="0743f-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0743f-221">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0743f-221">Next steps</span></span>

- [<span data-ttu-id="0743f-222">Vérifier ou mettre à jour les informations du profil de votre entreprise</span><span class="sxs-lookup"><span data-stu-id="0743f-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="0743f-223">Contrats client Microsoft (par région, par langue)</span><span class="sxs-lookup"><span data-stu-id="0743f-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
