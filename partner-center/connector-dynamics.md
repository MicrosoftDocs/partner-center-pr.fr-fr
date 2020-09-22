---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires à l’aide de votre Dynamics 365 CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 39fbeb4e180b24dc19f73b5381af8b8b481045f3
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000493"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="a2e6b-103">Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="a2e6b-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="a2e6b-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="a2e6b-104">Appropriate roles</span></span>

- <span data-ttu-id="a2e6b-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="a2e6b-105">Referrals admin</span></span>
- <span data-ttu-id="a2e6b-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="a2e6b-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="a2e6b-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="a2e6b-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="a2e6b-109">Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="a2e6b-110">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="a2e6b-111">Vous pouvez faire en sorte que toutes vos références fonctionnent dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="a2e6b-112">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="a2e6b-113">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="a2e6b-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="a2e6b-114">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-114">**Topics**</span></span>   |<span data-ttu-id="a2e6b-115">**Détails**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-115">**Details**</span></span>   |<span data-ttu-id="a2e6b-116">**Liens**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="a2e6b-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="a2e6b-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="a2e6b-118">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="a2e6b-118">You need a valid MPN ID</span></span>|<span data-ttu-id="a2e6b-119">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="a2e6b-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="a2e6b-120">Covente prête</span><span class="sxs-lookup"><span data-stu-id="a2e6b-120">Cosell ready</span></span>|<span data-ttu-id="a2e6b-121">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="a2e6b-122">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2e6b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="a2e6b-123">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2e6b-123">Partner Center account</span></span>|<span data-ttu-id="a2e6b-124">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="a2e6b-125">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="a2e6b-126">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="a2e6b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="a2e6b-127">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2e6b-127">Partner Center user roles</span></span>|<span data-ttu-id="a2e6b-128">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="a2e6b-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="a2e6b-129">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a2e6b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="a2e6b-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="a2e6b-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="a2e6b-131">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="a2e6b-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="a2e6b-132">Affecter des rôles dans Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2e6b-132">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="a2e6b-133">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="a2e6b-133">Power Automate Flow Account</span></span>|<span data-ttu-id="a2e6b-134">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="a2e6b-135">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="a2e6b-136">Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)</span><span class="sxs-lookup"><span data-stu-id="a2e6b-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="a2e6b-137">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="a2e6b-138">Cette étape vous montrera les instances CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="a2e6b-139">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="a2e6b-140">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="a2e6b-141">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. <span data-ttu-id="a2e6b-143">Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="a2e6b-144">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="a2e6b-145">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="a2e6b-146">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="a2e6b-147">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="a2e6b-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="a2e6b-148">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="a2e6b-149">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="a2e6b-150">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="a2e6b-151">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="a2e6b-152">Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="a2e6b-153">Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="a2e6b-154">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRM disponibles":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="a2e6b-156">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="a2e6b-156">Best practice: test before you go live</span></span>

<span data-ttu-id="a2e6b-157">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="a2e6b-158">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="a2e6b-159">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="a2e6b-160">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="a2e6b-161">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="a2e6b-162">Configuration de la solution</span><span class="sxs-lookup"><span data-stu-id="a2e6b-162">Configure the solution</span></span>

1. <span data-ttu-id="a2e6b-163">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a2e6b-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="a2e6b-164">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="a2e6b-165">Vous devez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="a2e6b-166">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="a2e6b-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="a2e6b-167">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2e6b-167">Partner Center Events</span></span>

   - <span data-ttu-id="a2e6b-168">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="a2e6b-169">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="a2e6b-170">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Créer une connexion":::

      3. <span data-ttu-id="a2e6b-172">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="a2e6b-173">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="a2e6b-174">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="a2e6b-175">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="a2e6b-176">Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="a2e6b-177">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-177">Save the changes.</span></span>

5. <span data-ttu-id="a2e6b-178">**Activez** l’alimentation automatiser les flux.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="a2e6b-179">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="a2e6b-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="a2e6b-180">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="a2e6b-181">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="a2e6b-182">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="a2e6b-183">Ajoutez des connexions pour (a.) utilisateur de l’espace partenaires avec les références d’administrateur (b.) des événements de l’espace partenaires comme indiqué ci-dessous</span><span class="sxs-lookup"><span data-stu-id="a2e6b-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. <span data-ttu-id="a2e6b-185">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="a2e6b-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="a2e6b-187">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="a2e6b-188">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="a2e6b-189">Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="a2e6b-190">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="a2e6b-191">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copier l’URL":::

8. <span data-ttu-id="a2e6b-193">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="a2e6b-194">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="a2e6b-195">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-195">Enter the following details:</span></span>

    1. <span data-ttu-id="a2e6b-196">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="a2e6b-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="a2e6b-197">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="a2e6b-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="a2e6b-198">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="a2e6b-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="a2e6b-199">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="a2e6b-200">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="a2e6b-201">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="a2e6b-201">Customize synchronization steps</span></span>

<span data-ttu-id="a2e6b-202">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="a2e6b-203">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="a2e6b-204">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="a2e6b-205">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="a2e6b-206">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="a2e6b-207">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="a2e6b-208">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="a2e6b-209">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="a2e6b-210">a.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-210">a.</span></span> <span data-ttu-id="a2e6b-211">Sélectionnez espace partenaires pour Dynamics 365 (version préliminaire d’Insider) ou espace partenaires pour Salesforce (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="a2e6b-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="a2e6b-212">b.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-212">b.</span></span> <span data-ttu-id="a2e6b-213">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2e6b-214">c.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-214">c.</span></span> <span data-ttu-id="a2e6b-215">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="a2e6b-216">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="a2e6b-217">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="a2e6b-218">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="a2e6b-219">d.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-219">d.</span></span> <span data-ttu-id="a2e6b-220">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="a2e6b-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="a2e6b-221">e.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-221">e.</span></span> <span data-ttu-id="a2e6b-222">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="a2e6b-223">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="a2e6b-224">f.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-224">f.</span></span> <span data-ttu-id="a2e6b-225">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="a2e6b-226">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="a2e6b-227">a.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-227">a.</span></span> <span data-ttu-id="a2e6b-228">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2e6b-229">b.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-229">b.</span></span> <span data-ttu-id="a2e6b-230">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="a2e6b-231">c.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-231">c.</span></span> <span data-ttu-id="a2e6b-232">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="a2e6b-233">d.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-233">d.</span></span> <span data-ttu-id="a2e6b-234">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="a2e6b-235">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="a2e6b-236">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="a2e6b-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="a2e6b-237">a.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-237">a.</span></span> <span data-ttu-id="a2e6b-238">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="a2e6b-239">b.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-239">b.</span></span> <span data-ttu-id="a2e6b-240">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="a2e6b-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="a2e6b-241">c.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-241">c.</span></span> <span data-ttu-id="a2e6b-242">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="a2e6b-243">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="a2e6b-244">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="a2e6b-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="a2e6b-245">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="a2e6b-246">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="a2e6b-246">Pre-requisites</span></span>

<span data-ttu-id="a2e6b-247">Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="a2e6b-248">Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="a2e6b-249">Un ensemble de champs personnalisés est disponible dans le cadre de l’entité **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="a2e6b-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="a2e6b-250">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="a2e6b-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="a2e6b-251">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="a2e6b-252">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2e6b-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="a2e6b-253">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2e6b-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="a2e6b-254">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2e6b-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="a2e6b-255">**Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="a2e6b-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="a2e6b-256">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="a2e6b-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="a2e6b-257">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2e6b-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="a2e6b-258">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="a2e6b-258">SCENARIOS:</span></span>

1. <span data-ttu-id="a2e6b-259">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="a2e6b-260">Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="a2e6b-261">Assurez-vous que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2e6b-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Exemple de section d’opportunité présentant les informations de l’espace partenaires Microsoft dans Dynamics 365.":::

   3. <span data-ttu-id="a2e6b-263">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="a2e6b-264">**Synchroniser avec l’espace partenaires**: Oui</span><span class="sxs-lookup"><span data-stu-id="a2e6b-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="a2e6b-265">**Comment Microsoft peut-il vous aider ?**:</span><span class="sxs-lookup"><span data-stu-id="a2e6b-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Exemple de section d’opportunité dans Dynamics 365 qui affiche les options d’aide de l’espace partenaires Microsoft en regard d’un champ appelé comment peut-il aider Microsoft ?":::

      - <span data-ttu-id="a2e6b-267">**Produits**: ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="a2e6b-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="a2e6b-268">Une fois que l’opportunité est créée dans Dynamics 365 avec l’option **synchroniser avec l’espace partenaires** définie sur **Oui**, patientez 10 minutes, puis connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="a2e6b-269">Vos références seront synchronisées avec Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="a2e6b-270">De même, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="a2e6b-271">Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="a2e6b-272">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :</span><span class="sxs-lookup"><span data-stu-id="a2e6b-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="a2e6b-273">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="a2e6b-274">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="a2e6b-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="a2e6b-275">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="a2e6b-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="a2e6b-276">Connectez-vous à votre environnement Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="a2e6b-277">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="a2e6b-278">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="a2e6b-279">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="a2e6b-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2e6b-280">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a2e6b-280">Next steps</span></span>

- [<span data-ttu-id="a2e6b-281">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="a2e6b-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="a2e6b-282">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="a2e6b-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="a2e6b-283">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="a2e6b-283">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="a2e6b-284">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a2e6b-284">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)