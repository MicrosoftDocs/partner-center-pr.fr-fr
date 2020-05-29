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
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145103"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b43a6-103">Connecteur de co-vente pour Salesforce CRM-vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="b43a6-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="b43a6-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="b43a6-104">Appropriate roles</span></span>

- <span data-ttu-id="b43a6-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="b43a6-105">Referrals admin</span></span>
- <span data-ttu-id="b43a6-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="b43a6-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b43a6-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b43a6-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b43a6-109">À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="b43a6-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b43a6-110">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b43a6-111">Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b43a6-112">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b43a6-113">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="b43a6-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b43a6-114">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="b43a6-114">**Topics**</span></span>   |<span data-ttu-id="b43a6-115">**Détails**</span><span class="sxs-lookup"><span data-stu-id="b43a6-115">**Details**</span></span>   |<span data-ttu-id="b43a6-116">**Liens**</span><span class="sxs-lookup"><span data-stu-id="b43a6-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b43a6-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="b43a6-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b43a6-118">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="b43a6-118">You need a valid MPN ID</span></span>|<span data-ttu-id="b43a6-119">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="b43a6-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b43a6-120">Co-vente prête</span><span class="sxs-lookup"><span data-stu-id="b43a6-120">Co-sell ready</span></span>|<span data-ttu-id="b43a6-121">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b43a6-122">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b43a6-123">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-123">Partner Center account</span></span>|<span data-ttu-id="b43a6-124">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b43a6-125">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="b43a6-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b43a6-126">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="b43a6-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b43a6-127">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-127">Partner Center user roles</span></span>|<span data-ttu-id="b43a6-128">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="b43a6-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b43a6-129">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b43a6-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b43a6-130">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="b43a6-130">Salesforce CRM</span></span>|<span data-ttu-id="b43a6-131">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="b43a6-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b43a6-132">Affecter des rôles dans Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b43a6-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="b43a6-133">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="b43a6-133">Power Automate Flow Account</span></span>|<span data-ttu-id="b43a6-134">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b43a6-135">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="b43a6-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b43a6-136">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b43a6-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b43a6-137">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="b43a6-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b43a6-138">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="b43a6-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b43a6-139">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="b43a6-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="b43a6-140">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="b43a6-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b43a6-141">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="b43a6-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Ouvrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="b43a6-143">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="b43a6-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

![Salesforce](images/salesforce/salesforce1.png)

6. <span data-ttu-id="b43a6-145">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-145">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="b43a6-146">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="b43a6-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b43a6-147">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="b43a6-147">Agree to terms and conditions.</span></span>

![CRM disponibles](images/salesforce/available-crm.png)

8. <span data-ttu-id="b43a6-149">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="b43a6-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b43a6-150">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="b43a6-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b43a6-151">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b43a6-152">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="b43a6-152">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="b43a6-153">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="b43a6-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b43a6-154">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="b43a6-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b43a6-155">Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b43a6-156">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="b43a6-156">The following Power Automate flows and entities are available:</span></span>

![Flux Salesforce](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b43a6-158">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="b43a6-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b43a6-159">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="b43a6-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b43a6-160">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b43a6-161">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="b43a6-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b43a6-162">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b43a6-163">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="b43a6-163">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="b43a6-164">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="b43a6-164">Configure the solution</span></span>

1. <span data-ttu-id="b43a6-165">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="b43a6-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b43a6-166">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="b43a6-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="b43a6-167">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="b43a6-167">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="b43a6-168">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="b43a6-168">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="b43a6-169">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-169">Partner Center Events</span></span>
- <span data-ttu-id="b43a6-170">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="b43a6-170">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="b43a6-171">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-171">a.</span></span> <span data-ttu-id="b43a6-172">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="b43a6-172">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="b43a6-173">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-173">b.</span></span> <span data-ttu-id="b43a6-174">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-174">Create a connection by clicking **Create a connection**.</span></span> 

    ![Créer une connexion](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="b43a6-176">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-176">c.</span></span> <span data-ttu-id="b43a6-177">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="b43a6-177">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

    <span data-ttu-id="b43a6-178">d.</span><span class="sxs-lookup"><span data-stu-id="b43a6-178">d.</span></span> <span data-ttu-id="b43a6-179">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="b43a6-179">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="b43a6-180">e.</span><span class="sxs-lookup"><span data-stu-id="b43a6-180">e.</span></span> <span data-ttu-id="b43a6-181">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="b43a6-181">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>
    
    <span data-ttu-id="b43a6-182">f.</span><span class="sxs-lookup"><span data-stu-id="b43a6-182">f.</span></span> <span data-ttu-id="b43a6-183">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-183">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="b43a6-184">Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-184">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="b43a6-185">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="b43a6-185">Save the changes.</span></span>

5. <span data-ttu-id="b43a6-186">**Activez** les flux automate Power.</span><span class="sxs-lookup"><span data-stu-id="b43a6-186">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b43a6-187">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="b43a6-187">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b43a6-188">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="b43a6-188">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b43a6-189">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="b43a6-189">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b43a6-190">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="b43a6-190">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b43a6-191">Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous</span><span class="sxs-lookup"><span data-stu-id="b43a6-191">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Déclencheur](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="b43a6-193">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="b43a6-193">When you make these updates, you'll see</span></span>

![Webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="b43a6-195">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-195">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="b43a6-196">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="b43a6-196">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b43a6-197">Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-197">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b43a6-198">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-198">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b43a6-199">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="b43a6-199">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copier l’URL](images/salesforce/copy-url.png)

8. <span data-ttu-id="b43a6-201">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-201">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b43a6-202">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-202">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="b43a6-203">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="b43a6-203">Enter the following details:</span></span> 

    <span data-ttu-id="b43a6-204">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-204">a.</span></span> <span data-ttu-id="b43a6-205">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="b43a6-205">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="b43a6-206">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-206">b.</span></span> <span data-ttu-id="b43a6-207">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="b43a6-207">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="b43a6-208">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-208">c.</span></span> <span data-ttu-id="b43a6-209">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="b43a6-209">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="b43a6-210">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="b43a6-210">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b43a6-211">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="b43a6-211">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b43a6-212">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="b43a6-212">Customize synchronization steps</span></span>

<span data-ttu-id="b43a6-213">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="b43a6-213">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b43a6-214">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="b43a6-214">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b43a6-215">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="b43a6-215">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b43a6-216">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="b43a6-216">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b43a6-217">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="b43a6-217">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b43a6-218">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="b43a6-218">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b43a6-219">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="b43a6-219">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b43a6-220">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="b43a6-220">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="b43a6-221">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-221">a.</span></span> <span data-ttu-id="b43a6-222">Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="b43a6-222">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

    <span data-ttu-id="b43a6-223">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-223">b.</span></span> <span data-ttu-id="b43a6-224">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="b43a6-224">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="b43a6-225">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-225">c.</span></span> <span data-ttu-id="b43a6-226">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-226">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b43a6-227">Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-227">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b43a6-228">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-228">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b43a6-229">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="b43a6-229">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="b43a6-230">d.</span><span class="sxs-lookup"><span data-stu-id="b43a6-230">d.</span></span> <span data-ttu-id="b43a6-231">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="b43a6-231">To customize CRM field mappings for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="b43a6-232">e.</span><span class="sxs-lookup"><span data-stu-id="b43a6-232">e.</span></span> <span data-ttu-id="b43a6-233">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-233">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b43a6-234">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-234">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="b43a6-235">f.</span><span class="sxs-lookup"><span data-stu-id="b43a6-235">f.</span></span> <span data-ttu-id="b43a6-236">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="b43a6-236">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="b43a6-237">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="b43a6-237">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="b43a6-238">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-238">a.</span></span> <span data-ttu-id="b43a6-239">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="b43a6-239">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="b43a6-240">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-240">b.</span></span> <span data-ttu-id="b43a6-241">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-241">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="b43a6-242">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-242">c.</span></span> <span data-ttu-id="b43a6-243">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-243">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="b43a6-244">d.</span><span class="sxs-lookup"><span data-stu-id="b43a6-244">d.</span></span> <span data-ttu-id="b43a6-245">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-245">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="b43a6-246">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="b43a6-246">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b43a6-247">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="b43a6-247">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="b43a6-248">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-248">a.</span></span> <span data-ttu-id="b43a6-249">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="b43a6-249">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="b43a6-250">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-250">b.</span></span> <span data-ttu-id="b43a6-251">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="b43a6-251">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="b43a6-252">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-252">c.</span></span> <span data-ttu-id="b43a6-253">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-253">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="b43a6-254">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="b43a6-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="b43a6-255">Créer une section distincte dans la disposition des opportunités CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="b43a6-255">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="b43a6-256">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b43a6-256">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b43a6-257">Cela permet à vos équipes de vendeur de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-257">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b43a6-258">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="b43a6-258">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="b43a6-259">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="b43a6-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="b43a6-260">L’utilisateur administrateur CRM Salesforce devra créer une section CRM distincte.</span><span class="sxs-lookup"><span data-stu-id="b43a6-260">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="b43a6-261">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="b43a6-261">The following custom fields should be part of the CRM section:</span></span>

<span data-ttu-id="b43a6-262">• **Synchronisation avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-262">• **Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

<span data-ttu-id="b43a6-263">• **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-263">• **Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

<span data-ttu-id="b43a6-264">• **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-264">• **Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

<span data-ttu-id="b43a6-265">• **Comment Microsoft peut-il vous aider ?**</span><span class="sxs-lookup"><span data-stu-id="b43a6-265">• **How can Microsoft help?**</span></span> <span data-ttu-id="b43a6-266">Aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="b43a6-266">Help required from Microsoft for the referral</span></span>

<span data-ttu-id="b43a6-267">• **Products**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="b43a6-267">• **Products**: List of products associated with this opportunity</span></span>

<span data-ttu-id="b43a6-268">• **Audit**: une piste d’audit en lecture seule pour la synchronisation avec la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-268">• **Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="b43a6-269">Définir des champs et des relations</span><span class="sxs-lookup"><span data-stu-id="b43a6-269">Set up fields and relationships</span></span>

1. <span data-ttu-id="b43a6-270">Connectez-vous à votre compte Salesforce et accédez à **opportunité**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-270">Sign into your Salesforce account and go to **Opportunity**.</span></span> 

2. <span data-ttu-id="b43a6-271">Cliquez sur les options **d’installation** et de **modification d’objet** pour ajouter les champs nécessaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-271">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>


3. <span data-ttu-id="b43a6-272">Sélectionner les **champs & les relations** dans le volet de navigation gauche</span><span class="sxs-lookup"><span data-stu-id="b43a6-272">Select **Fields & Relationships** from the left navigation</span></span>

![Champs](images/salesforce/fields1.png)

4. <span data-ttu-id="b43a6-274">Ajoutez les champs suivants dans la table « Field & Relationship » :</span><span class="sxs-lookup"><span data-stu-id="b43a6-274">Add the following fields in the “Fields & Relationship” table:</span></span>

|<span data-ttu-id="b43a6-275">**Étiquette du champ**</span><span class="sxs-lookup"><span data-stu-id="b43a6-275">**Field label**</span></span>   |<span data-ttu-id="b43a6-276">**Nom du champ**</span><span class="sxs-lookup"><span data-stu-id="b43a6-276">**Field name**</span></span>|<span data-ttu-id="b43a6-277">**Type de données**</span><span class="sxs-lookup"><span data-stu-id="b43a6-277">**Data type**</span></span>|<span data-ttu-id="b43a6-278">**Indexée**</span><span class="sxs-lookup"><span data-stu-id="b43a6-278">**Indexed**</span></span>|
|---------------------|:-------------------|:--------------|:----------------|
|<span data-ttu-id="b43a6-279">Synchroniser avec l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-279">Sync with Partner Center</span></span>|<span data-ttu-id="b43a6-280">synchronisation avec Partner-Center-c</span><span class="sxs-lookup"><span data-stu-id="b43a6-280">sync-with-partner-center-c</span></span>|<span data-ttu-id="b43a6-281">Case à cocher (désactivé par défaut)</span><span class="sxs-lookup"><span data-stu-id="b43a6-281">Checkbox (default unchecked)</span></span>||
|<span data-ttu-id="b43a6-282">Products</span><span class="sxs-lookup"><span data-stu-id="b43a6-282">Products</span></span>|<span data-ttu-id="b43a6-283">Produits-c</span><span class="sxs-lookup"><span data-stu-id="b43a6-283">Products-c</span></span>|<span data-ttu-id="b43a6-284">texte (255)</span><span class="sxs-lookup"><span data-stu-id="b43a6-284">text (255)</span></span>||
|<span data-ttu-id="b43a6-285">Referral</span><span class="sxs-lookup"><span data-stu-id="b43a6-285">Referral</span></span> | <span data-ttu-id="b43a6-286">Referral_Identifier__c</span><span class="sxs-lookup"><span data-stu-id="b43a6-286">Referral_Identifier__c</span></span>|<span data-ttu-id="b43a6-287">Texte (100) (ID externe)</span><span class="sxs-lookup"><span data-stu-id="b43a6-287">Text(100)(External ID)</span></span>|<span data-ttu-id="b43a6-288">Oui</span><span class="sxs-lookup"><span data-stu-id="b43a6-288">yes</span></span>|
|<span data-ttu-id="b43a6-289">Lien de référence</span><span class="sxs-lookup"><span data-stu-id="b43a6-289">Referral Link</span></span>| <span data-ttu-id="b43a6-290">Referral_Link__c_</span><span class="sxs-lookup"><span data-stu-id="b43a6-290">Referral_Link__c_</span></span>|<span data-ttu-id="b43a6-291">URL (255)</span><span class="sxs-lookup"><span data-stu-id="b43a6-291">URL(255)</span></span>||
|<span data-ttu-id="b43a6-292">Audit</span><span class="sxs-lookup"><span data-stu-id="b43a6-292">Audit</span></span>| <span data-ttu-id="b43a6-293">Audit__c</span><span class="sxs-lookup"><span data-stu-id="b43a6-293">Audit__c</span></span>|<span data-ttu-id="b43a6-294">Longue zone de texte (100000) (ligne visible 4)</span><span class="sxs-lookup"><span data-stu-id="b43a6-294">Long Text Area(100000)(visible line 4)</span></span>||
|<span data-ttu-id="b43a6-295">Comment Microsoft peut-il vous aider ?</span><span class="sxs-lookup"><span data-stu-id="b43a6-295">How can Microsoft help?</span></span>|<span data-ttu-id="b43a6-296">How_can_Microsoft_help__c</span><span class="sxs-lookup"><span data-stu-id="b43a6-296">How_can_Microsoft_help__c</span></span>|<span data-ttu-id="b43a6-297">Liste déroulante</span><span class="sxs-lookup"><span data-stu-id="b43a6-297">Picklist\*</span></span>|

<span data-ttu-id="b43a6-298">\* Valeurs de liste déroulante :</span><span class="sxs-lookup"><span data-stu-id="b43a6-298">\*Picklist values:</span></span>

<span data-ttu-id="b43a6-299">• Proposition de valeur spécifique à la charge de travail</span><span class="sxs-lookup"><span data-stu-id="b43a6-299">• Workload specific value proposition</span></span>

<span data-ttu-id="b43a6-300">• Architecture technique du client</span><span class="sxs-lookup"><span data-stu-id="b43a6-300">• Customer technical architecture</span></span>

<span data-ttu-id="b43a6-301">• Preuve de concept ou de démonstration</span><span class="sxs-lookup"><span data-stu-id="b43a6-301">• Proof of concept or demo</span></span>

<span data-ttu-id="b43a6-302">• Devis ou licences</span><span class="sxs-lookup"><span data-stu-id="b43a6-302">• Quotes or licensing</span></span>

<span data-ttu-id="b43a6-303">• Succès du client après la vente</span><span class="sxs-lookup"><span data-stu-id="b43a6-303">• Post sales customer success</span></span>

<span data-ttu-id="b43a6-304">• Général ou autre</span><span class="sxs-lookup"><span data-stu-id="b43a6-304">• General or other</span></span>

<span data-ttu-id="b43a6-305">5. les champs sont créés sous « champs & relations ».</span><span class="sxs-lookup"><span data-stu-id="b43a6-305">5.The fields would get created under “Fields & Relationships”</span></span>

![Champs créés](images/salesforce/fields2.png)

6. <span data-ttu-id="b43a6-307">Dans la disposition opportunité, créez une section distincte avec les champs comme indiqué ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="b43a6-307">In the Opportunity layout, create a separate section with the fields as listed above.</span></span> 

    <span data-ttu-id="b43a6-308">• Cette section doit être disponible pour les vendeurs dans la disposition des opportunités</span><span class="sxs-lookup"><span data-stu-id="b43a6-308">• This section should be available for the sellers in the Opportunity layout</span></span>


![Disposition des champs de l’espace partenaires](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b43a6-310">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="b43a6-310">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b43a6-311">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-311">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b43a6-312">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="b43a6-312">Pre-requisites</span></span>

<span data-ttu-id="b43a6-313">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b43a6-313">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b43a6-314">Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="b43a6-314">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b43a6-315">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="b43a6-315">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b43a6-316">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="b43a6-316">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b43a6-317">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="b43a6-317">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b43a6-318">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-318">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b43a6-319">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-319">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b43a6-320">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="b43a6-320">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b43a6-321">**Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="b43a6-321">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b43a6-322">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="b43a6-322">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b43a6-323">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-323">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="b43a6-324">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="b43a6-324">SCENARIOS:</span></span>

1. <span data-ttu-id="b43a6-325">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="b43a6-325">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="b43a6-326">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-326">a.</span></span> <span data-ttu-id="b43a6-327">Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-327">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="b43a6-328">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-328">b.</span></span> <span data-ttu-id="b43a6-329">Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="b43a6-329">Ensure that the following section is present when you create a “New Opportunity” in Salesforce CRM environment</span></span>

    ![Environnement Salesforce](images/salesforce/salesforce-scenario-1.png)

   

    <span data-ttu-id="b43a6-331">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-331">c.</span></span> <span data-ttu-id="b43a6-332">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="b43a6-332">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="b43a6-333">« Synchroniser avec l’espace partenaires » : Oui</span><span class="sxs-lookup"><span data-stu-id="b43a6-333">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="b43a6-334">« Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="b43a6-334">"How can Microsoft help?”: Select from the following options:</span></span>

   

    - <span data-ttu-id="b43a6-335">Produits : ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="b43a6-335">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="b43a6-336">d.</span><span class="sxs-lookup"><span data-stu-id="b43a6-336">d.</span></span> <span data-ttu-id="b43a6-337">Une fois que vous avez défini l’option **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-337">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b43a6-338">Vos références seront synchronisées avec Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-338">Your referrals will be synchronized with Salesforce CRM.</span></span>

    <span data-ttu-id="b43a6-339">e.</span><span class="sxs-lookup"><span data-stu-id="b43a6-339">e.</span></span> <span data-ttu-id="b43a6-340">Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-340">When the “Sync with Partner Center” option is set to “Yes”, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

    <span data-ttu-id="b43a6-341">f.</span><span class="sxs-lookup"><span data-stu-id="b43a6-341">f.</span></span> <span data-ttu-id="b43a6-342">Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-342">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b43a6-343">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :</span><span class="sxs-lookup"><span data-stu-id="b43a6-343">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span> 

    <span data-ttu-id="b43a6-344">a.</span><span class="sxs-lookup"><span data-stu-id="b43a6-344">a.</span></span> <span data-ttu-id="b43a6-345">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b43a6-345">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="b43a6-346">b.</span><span class="sxs-lookup"><span data-stu-id="b43a6-346">b.</span></span> <span data-ttu-id="b43a6-347">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="b43a6-347">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="b43a6-348">c.</span><span class="sxs-lookup"><span data-stu-id="b43a6-348">c.</span></span> <span data-ttu-id="b43a6-349">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="b43a6-349">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="b43a6-350">d.</span><span class="sxs-lookup"><span data-stu-id="b43a6-350">d.</span></span> <span data-ttu-id="b43a6-351">Connectez-vous à votre environnement CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="b43a6-351">Sign into your Salesforce CRM environment.</span></span> 

    <span data-ttu-id="b43a6-352">e.</span><span class="sxs-lookup"><span data-stu-id="b43a6-352">e.</span></span> <span data-ttu-id="b43a6-353">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="b43a6-353">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b43a6-354">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b43a6-354">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    ![Écran d’opportunités Salesforce](images/salesforce/salesforce-casino-e.png)

    <span data-ttu-id="b43a6-356">f.</span><span class="sxs-lookup"><span data-stu-id="b43a6-356">f.</span></span> <span data-ttu-id="b43a6-357">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="b43a6-357">When you select a synchronized referral, the card view details are populated.</span></span>





## <a name="next-steps"></a><span data-ttu-id="b43a6-358">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="b43a6-358">Next steps</span></span>

- [<span data-ttu-id="b43a6-359">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="b43a6-359">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="b43a6-360">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="b43a6-360">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b43a6-361">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="b43a6-361">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b43a6-362">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="b43a6-362">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)