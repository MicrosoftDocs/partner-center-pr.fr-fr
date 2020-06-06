---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires avec votre CRM Salesforce
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 2e2cbe4b6f5418cea4d992b9e68daa7e0ed3ec09
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453256"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="f6ef7-103">Connecteur de covente pour Salesforce CRM - vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="f6ef7-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f6ef7-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="f6ef7-104">Appropriate roles</span></span>

- <span data-ttu-id="f6ef7-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="f6ef7-105">Referrals admin</span></span>
- <span data-ttu-id="f6ef7-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="f6ef7-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="f6ef7-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="f6ef7-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="f6ef7-109">À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="f6ef7-110">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="f6ef7-111">Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="f6ef7-112">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="f6ef7-113">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="f6ef7-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="f6ef7-114">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-114">**Topics**</span></span>   |<span data-ttu-id="f6ef7-115">**Détails**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-115">**Details**</span></span>   |<span data-ttu-id="f6ef7-116">**Liens**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="f6ef7-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="f6ef7-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="f6ef7-118">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="f6ef7-118">You need a valid MPN ID</span></span>|<span data-ttu-id="f6ef7-119">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="f6ef7-120">Co-vente prête</span><span class="sxs-lookup"><span data-stu-id="f6ef7-120">Co-sell ready</span></span>|<span data-ttu-id="f6ef7-121">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="f6ef7-122">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="f6ef7-123">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-123">Partner Center account</span></span>|<span data-ttu-id="f6ef7-124">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="f6ef7-125">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="f6ef7-126">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="f6ef7-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f6ef7-127">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-127">Partner Center user roles</span></span>|<span data-ttu-id="f6ef7-128">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="f6ef7-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="f6ef7-129">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="f6ef7-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f6ef7-130">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="f6ef7-130">Salesforce CRM</span></span>|<span data-ttu-id="f6ef7-131">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="f6ef7-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="f6ef7-132">Affecter des rôles dans Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f6ef7-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="f6ef7-133">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="f6ef7-133">Power Automate Flow Account</span></span>|<span data-ttu-id="f6ef7-134">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="f6ef7-135">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="f6ef7-136">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f6ef7-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="f6ef7-137">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="f6ef7-138">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="f6ef7-139">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="f6ef7-140">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="f6ef7-141">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. <span data-ttu-id="f6ef7-143">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="f6ef7-145">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="f6ef7-146">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="f6ef7-147">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRM disponibles":::

8. <span data-ttu-id="f6ef7-149">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="f6ef7-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="f6ef7-150">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="f6ef7-151">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="f6ef7-152">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="f6ef7-153">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="f6ef7-154">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="f6ef7-155">Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="f6ef7-156">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Flux Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="f6ef7-158">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="f6ef7-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="f6ef7-159">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="f6ef7-160">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="f6ef7-161">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="f6ef7-162">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="f6ef7-163">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="f6ef7-164">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="f6ef7-164">Configure the solution</span></span>

1. <span data-ttu-id="f6ef7-165">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="f6ef7-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="f6ef7-166">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="f6ef7-167">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="f6ef7-168">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="f6ef7-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="f6ef7-169">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-169">Partner Center Events</span></span>
   - <span data-ttu-id="f6ef7-170">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="f6ef7-171">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="f6ef7-172">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Créer une connexion":::

   3. <span data-ttu-id="f6ef7-174">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="f6ef7-175">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="f6ef7-176">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="f6ef7-177">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="f6ef7-178">Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="f6ef7-179">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-179">Save the changes.</span></span>

5. <span data-ttu-id="f6ef7-180">**Activez** les flux automate Power.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f6ef7-181">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="f6ef7-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="f6ef7-182">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f6ef7-183">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="f6ef7-184">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f6ef7-185">Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous</span><span class="sxs-lookup"><span data-stu-id="f6ef7-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. <span data-ttu-id="f6ef7-187">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="f6ef7-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="f6ef7-189">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="f6ef7-190">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="f6ef7-191">Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="f6ef7-192">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f6ef7-193">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copier l’URL":::

8. <span data-ttu-id="f6ef7-195">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f6ef7-196">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="f6ef7-197">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-197">Enter the following details:</span></span>

    1. <span data-ttu-id="f6ef7-198">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="f6ef7-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="f6ef7-199">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="f6ef7-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="f6ef7-200">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="f6ef7-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="f6ef7-201">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="f6ef7-202">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f6ef7-203">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="f6ef7-203">Customize synchronization steps</span></span>

<span data-ttu-id="f6ef7-204">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f6ef7-205">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f6ef7-206">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f6ef7-207">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f6ef7-208">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f6ef7-209">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f6ef7-210">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f6ef7-211">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="f6ef7-212">Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="f6ef7-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="f6ef7-213">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="f6ef7-214">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f6ef7-215">Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f6ef7-216">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f6ef7-217">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="f6ef7-218">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="f6ef7-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="f6ef7-219">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f6ef7-220">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="f6ef7-221">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="f6ef7-222">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="f6ef7-223">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f6ef7-224">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="f6ef7-225">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="f6ef7-226">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="f6ef7-227">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f6ef7-228">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="f6ef7-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="f6ef7-229">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f6ef7-230">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="f6ef7-231">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="f6ef7-232">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="f6ef7-233">Créer une section distincte dans la disposition des opportunités CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="f6ef7-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="f6ef7-234">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f6ef7-235">Cela permet à vos équipes de vendeur de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f6ef7-236">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="f6ef7-237">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="f6ef7-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="f6ef7-238">L’utilisateur administrateur CRM Salesforce devra créer une section CRM distincte.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="f6ef7-239">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f6ef7-240">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f6ef7-241">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f6ef7-242">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f6ef7-243">**Comment Microsoft peut-il vous aider ?**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-243">**How can Microsoft help?**</span></span> <span data-ttu-id="f6ef7-244">Aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="f6ef7-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f6ef7-245">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="f6ef7-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f6ef7-246">**Audit**: piste d’audit en lecture seule pour la synchronisation avec la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="f6ef7-247">Définir des champs et des relations</span><span class="sxs-lookup"><span data-stu-id="f6ef7-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="f6ef7-248">Connectez-vous à votre compte Salesforce et accédez à **opportunité**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="f6ef7-249">Cliquez sur les options **d’installation** et de **modification d’objet** pour ajouter les champs nécessaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="f6ef7-250">Sélectionner les **champs & les relations** dans le volet de navigation gauche</span><span class="sxs-lookup"><span data-stu-id="f6ef7-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="f6ef7-252">Ajoutez les champs suivants dans la table **fields & Relationship** :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="f6ef7-253">**Étiquette du champ**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-253">**Field label**</span></span>   |<span data-ttu-id="f6ef7-254">**Nom du champ**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-254">**Field name**</span></span>|<span data-ttu-id="f6ef7-255">**Type de données**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-255">**Data type**</span></span>|<span data-ttu-id="f6ef7-256">**Indexée**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="f6ef7-257">Audit</span><span class="sxs-lookup"><span data-stu-id="f6ef7-257">Audit</span></span>|  <span data-ttu-id="f6ef7-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="f6ef7-258">Audit__c</span></span>|<span data-ttu-id="f6ef7-259">Longue zone de texte (100000) (ligne visible 4)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="f6ef7-260">Comment Microsoft peut-il vous aider ?</span><span class="sxs-lookup"><span data-stu-id="f6ef7-260">How can Microsoft help?</span></span>|<span data-ttu-id="f6ef7-261">H ow_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="f6ef7-261">H   ow_can_Microsoft_help__c</span></span>|<span data-ttu-id="f6ef7-262">Liste déroulante</span><span class="sxs-lookup"><span data-stu-id="f6ef7-262">Picklist\*</span></span>|
   |<span data-ttu-id="f6ef7-263">Produits</span><span class="sxs-lookup"><span data-stu-id="f6ef7-263">Products</span></span>|<span data-ttu-id="f6ef7-264">Produits-c</span><span class="sxs-lookup"><span data-stu-id="f6ef7-264">Products-c</span></span>|<span data-ttu-id="f6ef7-265">texte (255)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-265">text (255)</span></span>||
   |<span data-ttu-id="f6ef7-266">Referral</span><span class="sxs-lookup"><span data-stu-id="f6ef7-266">Referral</span></span> |  <span data-ttu-id="f6ef7-267">Referral_Identi fier__c</span><span class="sxs-lookup"><span data-stu-id="f6ef7-267">Referral_Identi   fier__c</span></span>|<span data-ttu-id="f6ef7-268">Texte (100) (ID externe)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-268">Text(100)(External ID)</span></span>|<span data-ttu-id="f6ef7-269">Oui</span><span class="sxs-lookup"><span data-stu-id="f6ef7-269">yes</span></span>|
   |<span data-ttu-id="f6ef7-270">Lien de référence</span><span class="sxs-lookup"><span data-stu-id="f6ef7-270">Referral    Link</span></span>|   <span data-ttu-id="f6ef7-271">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="f6ef7-271">Referral_Link__c_</span></span>|<span data-ttu-id="f6ef7-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-272">URL(255)</span></span>||
   |<span data-ttu-id="f6ef7-273">Synchroniser avec le CEN de partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-273">Sync with Partner Cen   ter</span></span>|<span data-ttu-id="f6ef7-274">synchronisation avec Partner-Center-c</span><span class="sxs-lookup"><span data-stu-id="f6ef7-274">sync-with-partner-center-c</span></span>|<span data-ttu-id="f6ef7-275">Case à cocher (désactivé par défaut)</span><span class="sxs-lookup"><span data-stu-id="f6ef7-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="f6ef7-276">\* Valeurs de liste déroulante :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-276">\*Picklist values:</span></span>

   - <span data-ttu-id="f6ef7-277">Proposition de valeur spécifique à la charge de travail</span><span class="sxs-lookup"><span data-stu-id="f6ef7-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="f6ef7-278">Architecture technique du client</span><span class="sxs-lookup"><span data-stu-id="f6ef7-278">Customer technical architecture</span></span>
   - <span data-ttu-id="f6ef7-279">Preuve de concept ou démonstration</span><span class="sxs-lookup"><span data-stu-id="f6ef7-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="f6ef7-280">Devis ou licences</span><span class="sxs-lookup"><span data-stu-id="f6ef7-280">Quotes or licensing</span></span>
   - <span data-ttu-id="f6ef7-281">Succès du client après la vente</span><span class="sxs-lookup"><span data-stu-id="f6ef7-281">Post sales customer success</span></span>
   - <span data-ttu-id="f6ef7-282">Général ou autre</span><span class="sxs-lookup"><span data-stu-id="f6ef7-282">General or other</span></span>

5. <span data-ttu-id="f6ef7-283">Les champs sont créés sous les **champs & les relations**</span><span class="sxs-lookup"><span data-stu-id="f6ef7-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Champs créés":::

6. <span data-ttu-id="f6ef7-285">Dans la disposition opportunité, créez une section distincte avec les champs comme indiqué ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="f6ef7-286">Cette section doit être disponible pour les vendeurs dans la disposition opportunité.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Disposition des champs de l’espace partenaires":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f6ef7-288">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="f6ef7-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="f6ef7-289">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f6ef7-290">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="f6ef7-290">Pre-requisites</span></span>

<span data-ttu-id="f6ef7-291">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f6ef7-292">Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f6ef7-293">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="f6ef7-294">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="f6ef7-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f6ef7-295">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f6ef7-296">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f6ef7-297">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f6ef7-298">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6ef7-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f6ef7-299">**Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="f6ef7-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f6ef7-300">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="f6ef7-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f6ef7-301">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f6ef7-302">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="f6ef7-302">SCENARIOS:</span></span>

1. <span data-ttu-id="f6ef7-303">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f6ef7-304">Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f6ef7-305">Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="f6ef7-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Environnement Salesforce":::

   3. <span data-ttu-id="f6ef7-307">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="f6ef7-308">« Synchroniser avec l’espace partenaires » : Oui</span><span class="sxs-lookup"><span data-stu-id="f6ef7-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="f6ef7-309">« Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="f6ef7-310">Produits : ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="f6ef7-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="f6ef7-311">Une fois que vous avez défini l’option **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f6ef7-312">Vos références seront synchronisées avec Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="f6ef7-313">Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="f6ef7-314">Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="f6ef7-315">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :</span><span class="sxs-lookup"><span data-stu-id="f6ef7-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="f6ef7-316">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="f6ef7-317">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="f6ef7-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="f6ef7-318">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="f6ef7-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="f6ef7-319">Connectez-vous à votre environnement CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="f6ef7-320">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f6ef7-321">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Écran d’opportunités Salesforce":::

    6. <span data-ttu-id="f6ef7-323">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="f6ef7-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f6ef7-324">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="f6ef7-324">Next steps</span></span>

- [<span data-ttu-id="f6ef7-325">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="f6ef7-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="f6ef7-326">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="f6ef7-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f6ef7-327">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="f6ef7-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="f6ef7-328">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f6ef7-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)