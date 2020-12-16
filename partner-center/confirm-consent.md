---
title: Confirmer que le client a accepté le Contrat client Microsoft
description: Découvrez comment confirmer l’acceptation du Contrat client Microsoft par les clients. Cela peut être nécessaire pour commander des produits et services Microsoft pour les clients.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354608"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="d6dfd-104">Mise à jour de la méthode permettant de confirmer l’acceptation du Contrat client Microsoft par les clients</span><span class="sxs-lookup"><span data-stu-id="d6dfd-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="d6dfd-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="d6dfd-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d6dfd-106">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="d6dfd-106">Admin agent</span></span>
- <span data-ttu-id="d6dfd-107">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="d6dfd-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="d6dfd-108">La ressource Contrat est actuellement prise en charge par l’Espace partenaires dans le cloud public Microsoft uniquement.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="d6dfd-109">Elle n’est pas applicable aux éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d6dfd-109">It is not applicable to:</span></span>
> * <span data-ttu-id="d6dfd-110">Espace partenaires géré par 21Vianet</span><span class="sxs-lookup"><span data-stu-id="d6dfd-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="d6dfd-111">Espace partenaires de Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="d6dfd-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="d6dfd-112">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d6dfd-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="d6dfd-113">À compter du 31 janvier 2020, tous les clients, nouveaux et existants, doivent signer le nouveau Contrat client Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="d6dfd-114">Pour en savoir plus, consultez [Confirmer l’acceptation du Contrat client Microsoft par les clients](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="d6dfd-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="d6dfd-115">En tant que partenaire, vous devez obtenir l’acceptation du Contrat client Microsoft par le client pour pouvoir lui commander des produits et des services Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="d6dfd-116">Pour permettre aux partenaires à mieux répondre aux exigences de conformité, Microsoft demande aux partenaires de confirmer l’acceptation en fournissant les informations suivantes sur la personne qui a accepté le contrat :</span><span class="sxs-lookup"><span data-stu-id="d6dfd-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="d6dfd-117">Prénom</span><span class="sxs-lookup"><span data-stu-id="d6dfd-117">First name</span></span>

- <span data-ttu-id="d6dfd-118">Nom</span><span class="sxs-lookup"><span data-stu-id="d6dfd-118">Last name</span></span>

- <span data-ttu-id="d6dfd-119">Adresse de messagerie</span><span class="sxs-lookup"><span data-stu-id="d6dfd-119">Email address</span></span>

- <span data-ttu-id="d6dfd-120">Numéro de téléphone (facultatif)</span><span class="sxs-lookup"><span data-stu-id="d6dfd-120">Phone number (optional)</span></span>

- <span data-ttu-id="d6dfd-121">Date d’acceptation</span><span class="sxs-lookup"><span data-stu-id="d6dfd-121">Date of acceptance</span></span>

<span data-ttu-id="d6dfd-122">Les partenaires associés à une facturation directe et les fournisseurs indirects peuvent confirmer l’acceptation du Contrat client Microsoft par le client quand ils effectuent des transactions par le biais de l’Espace partenaires ou de l’API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="d6dfd-123">La confirmation est *obligatoire*.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="d6dfd-124">Si la confirmation n’est pas fournie pour un client donné :</span><span class="sxs-lookup"><span data-stu-id="d6dfd-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="d6dfd-125">Vous ne pourrez pas créer de commandes pour ce client.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="d6dfd-126">Vous ne pourrez pas changer le nombre de licences des abonnements existants basés sur les licences pour ce client.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="d6dfd-127">La confirmation de l’acceptation du client peut être effectuée par le biais de l’Espace partenaires ou de l’API de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="d6dfd-128">Pour effectuer cette opération via l’API de l’Espace partenaires, consultez les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="d6dfd-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="d6dfd-129">Obtenir la confirmation du consentement du client</span><span class="sxs-lookup"><span data-stu-id="d6dfd-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="d6dfd-130">Obtenir les métadonnées d’un contrat</span><span class="sxs-lookup"><span data-stu-id="d6dfd-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="d6dfd-131">Confirmer le consentement du client</span><span class="sxs-lookup"><span data-stu-id="d6dfd-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="d6dfd-132">Cela s’applique à la fois aux environnements de production et aux environnements de bac à sable (sandbox).</span><span class="sxs-lookup"><span data-stu-id="d6dfd-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="d6dfd-133">Confirmer l’acceptation par un nouveau client</span><span class="sxs-lookup"><span data-stu-id="d6dfd-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="d6dfd-134">Utilisez la procédure suivante pour confirmer l’acceptation du client quand vous créez un locataire du client dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="d6dfd-135">Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d6dfd-136">Sélectionnez **Clients**, **Nouveau client**, puis **Informations sur le compte**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="d6dfd-137">Entrez les informations relatives à la **Société** et au **Contact principal**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informations sur la société":::

3. <span data-ttu-id="d6dfd-139">Sous **Contrat client Microsoft**, sélectionnez **Le client a accepté le dernier Contrat client Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="d6dfd-140">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d6dfd-141">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="d6dfd-142">Entrez les détails de l’utilisateur qui a fourni l’acceptation.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Ajouter une date d’acceptation":::

   <span data-ttu-id="d6dfd-144">Par défaut, les informations d’utilisateur du contact principal sont affichées.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="d6dfd-145">Si elles ne sont pas correctes, sélectionnez **Mettre à jour**, puis entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le \**Numéro de téléphone* (facultatif) de la personne qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="d6dfd-146">Sélectionnez **Suivant** pour effectuer le reste des étapes afin de créer le locataire du client.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d6dfd-147">Confirmer l’acceptation par un client existant</span><span class="sxs-lookup"><span data-stu-id="d6dfd-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="d6dfd-148">Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d6dfd-149">Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d6dfd-150">Sélectionnez **Informations sur le compte**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-150">Select **Account info**.</span></span>

3. <span data-ttu-id="d6dfd-151">Sous **Contrat client Microsoft**, sélectionnez **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Mettre à jour":::

4. <span data-ttu-id="d6dfd-153">Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="d6dfd-154">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d6dfd-155">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="d6dfd-156">Sélectionnez **Enregistrer et continuer**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="d6dfd-157">Confirmer l’acceptation du client lors de la création d’une commande pour un client existant</span><span class="sxs-lookup"><span data-stu-id="d6dfd-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="d6dfd-158">Si vous essayez de créer une commande pour un client existant que vous n’avez pas encore confirmé, vous recevrez une invite pour effectuer la confirmation.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="d6dfd-159">Pour ce faire, utilisez la procédure suivante.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="d6dfd-160">Entrez le **Prénom**, le **Nom**, l’**Adresse e-mail** et le **Numéro de téléphone** (facultatif) de l’utilisateur qui a accepté le contrat.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="d6dfd-161">Sous **Date d'acceptation du contrat**, entrez la date appropriée.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d6dfd-162">Vous ne pouvez pas la définir sur une date ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="d6dfd-163">Sélectionnez **Enregistrer et continuer**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d6dfd-164">Récupérer la confirmation de l’acceptation d’un client existant</span><span class="sxs-lookup"><span data-stu-id="d6dfd-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="d6dfd-165">Vous pouvez récupérer la confirmation de l’acceptation d’un client existant que vous avez fournie précédemment à l’aide de la procédure ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="d6dfd-166">Vous devez être Agent administrateur ou Commercial pour effectuer cette opération.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d6dfd-167">Sélectionnez **Clients**, puis recherchez et sélectionnez le client que vous souhaitez afficher.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="d6dfd-168">Sélectionnez **Informations sur le compte**.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-168">Select **Account info**.</span></span>

3. <span data-ttu-id="d6dfd-169">Sous **Contrat client Microsoft**, vous voyez si la confirmation a été fournie, ou non, pour ce client.</span><span class="sxs-lookup"><span data-stu-id="d6dfd-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d6dfd-170">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="d6dfd-170">Next steps</span></span>

- [<span data-ttu-id="d6dfd-171">Confirmer l’acceptation du Contrat client Microsoft par le client dans le cadre du programme des partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="d6dfd-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="d6dfd-172">Attester l’acceptation du Contrat client Microsoft au nom de votre client</span><span class="sxs-lookup"><span data-stu-id="d6dfd-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)