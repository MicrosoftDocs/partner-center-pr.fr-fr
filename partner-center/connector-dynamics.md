---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires à l’aide de votre Dynamics 365 CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 87b1d27fa2f42eeba3b0f8308648536c0686911e
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145133"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="a2141-103">Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="a2141-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="a2141-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="a2141-104">Appropriate roles</span></span>

- <span data-ttu-id="a2141-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="a2141-105">Referrals admin</span></span>
- <span data-ttu-id="a2141-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="a2141-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="a2141-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="a2141-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="a2141-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="a2141-109">Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="a2141-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="a2141-110">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="a2141-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="a2141-111">Vous pouvez faire en sorte que toutes vos références fonctionnent dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="a2141-112">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="a2141-113">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="a2141-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="a2141-114">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="a2141-114">**Topics**</span></span>   |<span data-ttu-id="a2141-115">**Détails**</span><span class="sxs-lookup"><span data-stu-id="a2141-115">**Details**</span></span>   |<span data-ttu-id="a2141-116">**Liens**</span><span class="sxs-lookup"><span data-stu-id="a2141-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="a2141-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="a2141-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="a2141-118">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="a2141-118">You need a valid MPN ID</span></span>|<span data-ttu-id="a2141-119">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="a2141-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="a2141-120">Covente prête</span><span class="sxs-lookup"><span data-stu-id="a2141-120">Cosell ready</span></span>|<span data-ttu-id="a2141-121">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="a2141-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="a2141-122">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2141-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="a2141-123">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2141-123">Partner Center account</span></span>|<span data-ttu-id="a2141-124">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="a2141-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="a2141-125">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="a2141-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="a2141-126">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="a2141-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="a2141-127">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2141-127">Partner Center user roles</span></span>|<span data-ttu-id="a2141-128">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="a2141-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="a2141-129">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a2141-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="a2141-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="a2141-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="a2141-131">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="a2141-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="a2141-132">Affecter des rôles dans Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2141-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="a2141-133">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="a2141-133">Power Automate Flow Account</span></span>|<span data-ttu-id="a2141-134">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="a2141-135">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="a2141-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="a2141-136">Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)</span><span class="sxs-lookup"><span data-stu-id="a2141-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="a2141-137">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2141-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="a2141-138">Cette étape vous montrera les instances CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="a2141-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="a2141-139">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2141-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="a2141-140">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="a2141-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="a2141-141">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="a2141-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Ouvrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="a2141-143">Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="a2141-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="a2141-144">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="a2141-144">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="a2141-145">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="a2141-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="a2141-146">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="a2141-146">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="a2141-147">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="a2141-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="a2141-148">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="a2141-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="a2141-149">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="a2141-150">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="a2141-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="a2141-151">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="a2141-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="a2141-152">Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="a2141-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="a2141-153">Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="a2141-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="a2141-154">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="a2141-154">The following Power Automate flows and entities are available:</span></span>

![CRM disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="a2141-156">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="a2141-156">Best practice: test before you go live</span></span>

<span data-ttu-id="a2141-157">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="a2141-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="a2141-158">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="a2141-159">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="a2141-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="a2141-160">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="a2141-161">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="a2141-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="a2141-162">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="a2141-162">Configure the solution</span></span>

1. <span data-ttu-id="a2141-163">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a2141-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="a2141-164">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="a2141-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="a2141-165">Vous devez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="a2141-165">You'll need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="a2141-166">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="a2141-166">Partner Center user with referrals admin credentials</span></span> 

- <span data-ttu-id="a2141-167">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2141-167">Partner Center Events</span></span>

- <span data-ttu-id="a2141-168">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="a2141-168">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="a2141-169">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-169">a.</span></span> <span data-ttu-id="a2141-170">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a2141-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="a2141-171">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-171">b.</span></span> <span data-ttu-id="a2141-172">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="a2141-172">Create a connection by clicking **Create a connection**.</span></span>

    ![Créer une connexion](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="a2141-174">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-174">c.</span></span> <span data-ttu-id="a2141-175">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2141-175">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

    <span data-ttu-id="a2141-176">d.</span><span class="sxs-lookup"><span data-stu-id="a2141-176">d.</span></span> <span data-ttu-id="a2141-177">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="a2141-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="a2141-178">e.</span><span class="sxs-lookup"><span data-stu-id="a2141-178">e.</span></span> <span data-ttu-id="a2141-179">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="a2141-179">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

    <span data-ttu-id="a2141-180">f.</span><span class="sxs-lookup"><span data-stu-id="a2141-180">f.</span></span> <span data-ttu-id="a2141-181">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-181">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="a2141-182">Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-182">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="a2141-183">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="a2141-183">Save the changes.</span></span>

5. <span data-ttu-id="a2141-184">**Activez** l’alimentation automatiser les flux.</span><span class="sxs-lookup"><span data-stu-id="a2141-184">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="a2141-185">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="a2141-185">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="a2141-186">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="a2141-186">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="a2141-187">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="a2141-187">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="a2141-188">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="a2141-188">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="a2141-189">Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous</span><span class="sxs-lookup"><span data-stu-id="a2141-189">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Déclencheur](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="a2141-191">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="a2141-191">When you make these updates, you'll see</span></span>

![Webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="a2141-193">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="a2141-193">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="a2141-194">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a2141-194">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="a2141-195">Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="a2141-195">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="a2141-196">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="a2141-196">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="a2141-197">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="a2141-197">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copier l’URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="a2141-199">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="a2141-199">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="a2141-200">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="a2141-200">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="a2141-201">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="a2141-201">Enter the following details:</span></span> 

    <span data-ttu-id="a2141-202">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-202">a.</span></span> <span data-ttu-id="a2141-203">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="a2141-203">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="a2141-204">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-204">b.</span></span> <span data-ttu-id="a2141-205">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="a2141-205">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="a2141-206">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-206">c.</span></span> <span data-ttu-id="a2141-207">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="a2141-207">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="a2141-208">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="a2141-208">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="a2141-209">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="a2141-209">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="a2141-210">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="a2141-210">Customize synchronization steps</span></span>

<span data-ttu-id="a2141-211">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="a2141-211">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="a2141-212">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="a2141-212">Often CRM systems are highly customized.</span></span> <span data-ttu-id="a2141-213">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="a2141-213">You can customize the Power Automate flows.</span></span> <span data-ttu-id="a2141-214">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="a2141-214">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="a2141-215">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="a2141-215">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="a2141-216">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="a2141-216">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="a2141-217">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="a2141-217">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="a2141-218">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="a2141-218">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="a2141-219">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-219">a.</span></span> <span data-ttu-id="a2141-220">Sélectionnez espace partenaires pour Dynamics 365 (version préliminaire d’Insider) ou espace partenaires pour Salesforce (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="a2141-220">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="a2141-221">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-221">b.</span></span> <span data-ttu-id="a2141-222">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2141-222">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2141-223">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-223">c.</span></span> <span data-ttu-id="a2141-224">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2141-224">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="a2141-225">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2141-225">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="a2141-226">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="a2141-226">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="a2141-227">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2141-227">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="a2141-228">d.</span><span class="sxs-lookup"><span data-stu-id="a2141-228">d.</span></span> <span data-ttu-id="a2141-229">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="a2141-229">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="a2141-230">e.</span><span class="sxs-lookup"><span data-stu-id="a2141-230">e.</span></span> <span data-ttu-id="a2141-231">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2141-231">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="a2141-232">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="a2141-232">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="a2141-233">f.</span><span class="sxs-lookup"><span data-stu-id="a2141-233">f.</span></span> <span data-ttu-id="a2141-234">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="a2141-234">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="a2141-235">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="a2141-235">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="a2141-236">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-236">a.</span></span> <span data-ttu-id="a2141-237">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2141-237">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2141-238">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-238">b.</span></span> <span data-ttu-id="a2141-239">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2141-239">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="a2141-240">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-240">c.</span></span> <span data-ttu-id="a2141-241">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2141-241">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="a2141-242">d.</span><span class="sxs-lookup"><span data-stu-id="a2141-242">d.</span></span> <span data-ttu-id="a2141-243">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2141-243">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="a2141-244">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2141-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="a2141-245">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="a2141-245">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="a2141-246">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-246">a.</span></span> <span data-ttu-id="a2141-247">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2141-247">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="a2141-248">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-248">b.</span></span> <span data-ttu-id="a2141-249">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="a2141-249">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="a2141-250">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-250">c.</span></span> <span data-ttu-id="a2141-251">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="a2141-251">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="a2141-252">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2141-252">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="a2141-253">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="a2141-253">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="a2141-254">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-254">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="a2141-255">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="a2141-255">Pre-requisites</span></span>

<span data-ttu-id="a2141-256">Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a2141-256">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="a2141-257">Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="a2141-257">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="a2141-258">Un ensemble de champs personnalisés est disponible dans le cadre de l’entité **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="a2141-258">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="a2141-259">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="a2141-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="a2141-260">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="a2141-260">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="a2141-261">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2141-261">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="a2141-262">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2141-262">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="a2141-263">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2141-263">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="a2141-264">**Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="a2141-264">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="a2141-265">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="a2141-265">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="a2141-266">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2141-266">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="a2141-267">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="a2141-267">SCENARIOS:</span></span>

1. <span data-ttu-id="a2141-268">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="a2141-268">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="a2141-269">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-269">a.</span></span> <span data-ttu-id="a2141-270">Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-270">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="a2141-271">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-271">b.</span></span> <span data-ttu-id="a2141-272">Assurez-vous que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2141-272">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Opportunité](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="a2141-274">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-274">c.</span></span> <span data-ttu-id="a2141-275">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="a2141-275">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="a2141-276">**Synchroniser avec l’espace partenaires**: Oui</span><span class="sxs-lookup"><span data-stu-id="a2141-276">**Sync with Partner Center**: Yes</span></span>

    - <span data-ttu-id="a2141-277">**Comment Microsoft peut-il vous aider ?**:</span><span class="sxs-lookup"><span data-stu-id="a2141-277">**How can Microsoft help?**: Select from the following:</span></span>

    ![Sélections d’aide](images/cosellconnectors/help.png)

    - <span data-ttu-id="a2141-279">**Produits**: ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="a2141-279">**Products**: Solution IDs of the product</span></span>

    <span data-ttu-id="a2141-280">d.</span><span class="sxs-lookup"><span data-stu-id="a2141-280">d.</span></span> <span data-ttu-id="a2141-281">Une fois que l’opportunité est créée dans Dynamics 365 avec l’option **synchroniser avec l’espace partenaires** définie sur **Oui**, patientez 10 minutes, puis connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-281">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="a2141-282">Vos références seront synchronisées avec Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2141-282">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="a2141-283">e.</span><span class="sxs-lookup"><span data-stu-id="a2141-283">e.</span></span> <span data-ttu-id="a2141-284">De même, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-284">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="a2141-285">f.</span><span class="sxs-lookup"><span data-stu-id="a2141-285">f.</span></span> <span data-ttu-id="a2141-286">Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2141-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="a2141-287">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :</span><span class="sxs-lookup"><span data-stu-id="a2141-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

    <span data-ttu-id="a2141-288">a.</span><span class="sxs-lookup"><span data-stu-id="a2141-288">a.</span></span> <span data-ttu-id="a2141-289">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2141-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="a2141-290">b.</span><span class="sxs-lookup"><span data-stu-id="a2141-290">b.</span></span> <span data-ttu-id="a2141-291">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="a2141-291">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="a2141-292">c.</span><span class="sxs-lookup"><span data-stu-id="a2141-292">c.</span></span> <span data-ttu-id="a2141-293">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="a2141-293">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="a2141-294">d.</span><span class="sxs-lookup"><span data-stu-id="a2141-294">d.</span></span> <span data-ttu-id="a2141-295">Connectez-vous à votre environnement Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-295">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="a2141-296">e.</span><span class="sxs-lookup"><span data-stu-id="a2141-296">e.</span></span> <span data-ttu-id="a2141-297">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="a2141-297">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="a2141-298">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2141-298">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="a2141-299">f.</span><span class="sxs-lookup"><span data-stu-id="a2141-299">f.</span></span> <span data-ttu-id="a2141-300">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="a2141-300">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2141-301">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a2141-301">Next steps</span></span>

- [<span data-ttu-id="a2141-302">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="a2141-302">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="a2141-303">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="a2141-303">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="a2141-304">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="a2141-304">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="a2141-305">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2141-305">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)