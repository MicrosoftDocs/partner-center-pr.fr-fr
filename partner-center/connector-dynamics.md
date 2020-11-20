---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisez vos références dans l’espace partenaires à l’aide de votre connecteur de covente pour Dynamics 365 CRM. Les vendeurs peuvent ensuite se vendre avec Microsoft à partir de vos systèmes CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947735"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="1e3ae-104">Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="1e3ae-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1e3ae-105">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="1e3ae-105">Appropriate roles</span></span>

- <span data-ttu-id="1e3ae-106">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="1e3ae-106">Referrals admin</span></span>
- <span data-ttu-id="1e3ae-107">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="1e3ae-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1e3ae-108">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1e3ae-109">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1e3ae-110">Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="1e3ae-111">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1e3ae-112">Vous pouvez faire en sorte que toutes vos références fonctionnent dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1e3ae-113">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1e3ae-114">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="1e3ae-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1e3ae-115">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-115">**Topics**</span></span>   |<span data-ttu-id="1e3ae-116">**Détails**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-116">**Details**</span></span>   |<span data-ttu-id="1e3ae-117">**Liens**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1e3ae-118">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="1e3ae-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1e3ae-119">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="1e3ae-119">You need a valid MPN ID</span></span>|<span data-ttu-id="1e3ae-120">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1e3ae-121">Covente prête</span><span class="sxs-lookup"><span data-stu-id="1e3ae-121">Cosell ready</span></span>|<span data-ttu-id="1e3ae-122">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1e3ae-123">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e3ae-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1e3ae-124">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e3ae-124">Partner Center account</span></span>|<span data-ttu-id="1e3ae-125">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1e3ae-126">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="1e3ae-127">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="1e3ae-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1e3ae-128">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e3ae-128">Partner Center user roles</span></span>|<span data-ttu-id="1e3ae-129">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="1e3ae-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1e3ae-130">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1e3ae-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="1e3ae-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="1e3ae-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="1e3ae-132">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="1e3ae-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1e3ae-133">Affecter des rôles dans Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1e3ae-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1e3ae-134">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="1e3ae-134">Power Automate Flow Account</span></span>|<span data-ttu-id="1e3ae-135">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1e3ae-136">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="1e3ae-137">Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="1e3ae-138">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1e3ae-139">Cette étape vous montrera les instances CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1e3ae-140">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="1e3ae-141">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1e3ae-142">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. <span data-ttu-id="1e3ae-144">Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="1e3ae-145">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="1e3ae-146">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="1e3ae-147">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="1e3ae-148">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="1e3ae-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1e3ae-149">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1e3ae-150">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1e3ae-151">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="1e3ae-152">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1e3ae-153">Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1e3ae-154">Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="1e3ae-155">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRM disponibles":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1e3ae-157">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="1e3ae-157">Best practice: test before you go live</span></span>

<span data-ttu-id="1e3ae-158">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1e3ae-159">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="1e3ae-160">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="1e3ae-161">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="1e3ae-162">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="1e3ae-163">Configuration de la solution</span><span class="sxs-lookup"><span data-stu-id="1e3ae-163">Configure the solution</span></span>

1. <span data-ttu-id="1e3ae-164">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1e3ae-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="1e3ae-165">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1e3ae-166">Vous devez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="1e3ae-167">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="1e3ae-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="1e3ae-168">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e3ae-168">Partner Center Events</span></span>

   - <span data-ttu-id="1e3ae-169">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="1e3ae-170">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="1e3ae-171">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Créer une connexion":::

      3. <span data-ttu-id="1e3ae-173">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="1e3ae-174">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="1e3ae-175">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="1e3ae-176">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="1e3ae-177">Une fois que toutes les connexions ont été ajoutées, vous devez voir les connexions suivantes dans votre environnement :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Connexions":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="1e3ae-179">Modifier les connexions</span><span class="sxs-lookup"><span data-stu-id="1e3ae-179">Edit the connections</span></span>

1. <span data-ttu-id="1e3ae-180">Revenez à la page **solutions** et sélectionnez **solution par défaut**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="1e3ae-181">Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Connexion":::

2. <span data-ttu-id="1e3ae-183">Modifiez chacune des connexions une par une en sélectionnant l’icône à trois points.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="1e3ae-184">Ajoutez les connexions appropriées.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Connexions listées"::: 

3.  <span data-ttu-id="1e3ae-186">Activez les flux dans l’ordre suivant :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="1e3ae-187">Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-188">Créer une référence de covente – Dynamics 365 à l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-189">Espace partenaires Microsoft : mises à jour de référence de la co-vente à Dynamics 365 (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-190">Espace partenaires vers Dynamics 365 (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-191">Dynamics 365 pour l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-192">Opportunité Dynamics 365 pour l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1e3ae-193">Dynamics 365 solutions Microsoft pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1e3ae-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="1e3ae-194">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="1e3ae-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="1e3ae-195">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1e3ae-196">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="1e3ae-197">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1e3ae-198">Ajoutez des connexions pour (a.) utilisateur de l’espace partenaires avec les références d’administrateur (b.) des événements de l’espace partenaires comme indiqué ci-dessous</span><span class="sxs-lookup"><span data-stu-id="1e3ae-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. <span data-ttu-id="1e3ae-200">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="1e3ae-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1e3ae-202">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1e3ae-203">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="1e3ae-204">Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="1e3ae-205">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1e3ae-206">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copier l’URL":::

8. <span data-ttu-id="1e3ae-208">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1e3ae-209">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1e3ae-210">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-210">Enter the following details:</span></span>

    1. <span data-ttu-id="1e3ae-211">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="1e3ae-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1e3ae-212">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="1e3ae-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="1e3ae-213">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="1e3ae-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="1e3ae-214">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="1e3ae-215">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1e3ae-216">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="1e3ae-216">Customize synchronization steps</span></span>

<span data-ttu-id="1e3ae-217">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1e3ae-218">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1e3ae-219">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1e3ae-220">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1e3ae-221">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1e3ae-222">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1e3ae-223">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1e3ae-224">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="1e3ae-225">a.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-225">a.</span></span> <span data-ttu-id="1e3ae-226">Sélectionnez espace partenaires pour Dynamics 365 (version préliminaire d’Insider) ou espace partenaires pour Salesforce (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="1e3ae-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="1e3ae-227">b.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-227">b.</span></span> <span data-ttu-id="1e3ae-228">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1e3ae-229">c.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-229">c.</span></span> <span data-ttu-id="1e3ae-230">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1e3ae-231">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1e3ae-232">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1e3ae-233">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="1e3ae-234">d.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-234">d.</span></span> <span data-ttu-id="1e3ae-235">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="1e3ae-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="1e3ae-236">e.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-236">e.</span></span> <span data-ttu-id="1e3ae-237">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1e3ae-238">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="1e3ae-239">f.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-239">f.</span></span> <span data-ttu-id="1e3ae-240">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1e3ae-241">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="1e3ae-242">a.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-242">a.</span></span> <span data-ttu-id="1e3ae-243">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="1e3ae-244">b.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-244">b.</span></span> <span data-ttu-id="1e3ae-245">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="1e3ae-246">c.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-246">c.</span></span> <span data-ttu-id="1e3ae-247">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="1e3ae-248">d.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-248">d.</span></span> <span data-ttu-id="1e3ae-249">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1e3ae-250">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1e3ae-251">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="1e3ae-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="1e3ae-252">a.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-252">a.</span></span> <span data-ttu-id="1e3ae-253">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="1e3ae-254">b.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-254">b.</span></span> <span data-ttu-id="1e3ae-255">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="1e3ae-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="1e3ae-256">c.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-256">c.</span></span> <span data-ttu-id="1e3ae-257">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="1e3ae-258">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="1e3ae-259">Deux variables d’environnement sont créées :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-259">There are two environment variables created:</span></span>

- <span data-ttu-id="1e3ae-260">Coche : indique si vous avez besoin d’une icône de coche en plus des opportunités synchronisées de manière bidirectionnelle entre l’espace partenaires et Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="1e3ae-261">Opportunités de covente de la synchronisation uniquement : signifie que vous souhaitez synchroniser uniquement les opportunités de covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="1e3ae-262">Vous pouvez choisir de modifier la valeur par défaut pour les variables d’environnement.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Zone d’édition pour les valeurs par défaut":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1e3ae-264">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="1e3ae-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="1e3ae-265">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1e3ae-266">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="1e3ae-266">Pre-requisites</span></span>

<span data-ttu-id="1e3ae-267">Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="1e3ae-268">Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1e3ae-269">Un ensemble de champs personnalisés est disponible dans le cadre de l’entité **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="1e3ae-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="1e3ae-270">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="1e3ae-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1e3ae-271">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1e3ae-272">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e3ae-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1e3ae-273">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e3ae-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1e3ae-274">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1e3ae-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1e3ae-275">**Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="1e3ae-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1e3ae-276">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="1e3ae-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1e3ae-277">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e3ae-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="1e3ae-278">Mettez à jour le formulaire d’opportunité dans Dynamics 365 CRM pour inclure le champ solutions for Products.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulaire d’opportunité":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="1e3ae-281">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="1e3ae-281">SCENARIOS:</span></span>

1. <span data-ttu-id="1e3ae-282">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1e3ae-283">Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1e3ae-284">Assurez-vous que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="1e3ae-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Exemple de section d’opportunité présentant les informations de l’espace partenaires Microsoft dans Dynamics 365.":::

   3. <span data-ttu-id="1e3ae-286">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="1e3ae-287">**Synchroniser avec l’espace partenaires**: Oui</span><span class="sxs-lookup"><span data-stu-id="1e3ae-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="1e3ae-288">**Comment Microsoft peut-il vous aider ?**:</span><span class="sxs-lookup"><span data-stu-id="1e3ae-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Exemple de section d’opportunité dans Dynamics 365 qui affiche les options d’aide de l’espace partenaires Microsoft en regard d’un champ appelé comment peut-il aider Microsoft ?":::

      - <span data-ttu-id="1e3ae-290">**Produits**: ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="1e3ae-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1e3ae-291">Une fois que l’opportunité est créée dans Dynamics 365 avec l’option **synchroniser avec l’espace partenaires** définie sur **Oui**, patientez 10 minutes, puis connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="1e3ae-292">Vos références seront synchronisées avec Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="1e3ae-293">De même, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="1e3ae-294">Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="1e3ae-295">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :</span><span class="sxs-lookup"><span data-stu-id="1e3ae-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="1e3ae-296">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="1e3ae-297">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="1e3ae-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="1e3ae-298">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="1e3ae-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="1e3ae-299">Connectez-vous à votre environnement Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="1e3ae-300">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1e3ae-301">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="1e3ae-302">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="1e3ae-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1e3ae-303">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1e3ae-303">Next steps</span></span>

- [<span data-ttu-id="1e3ae-304">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="1e3ae-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1e3ae-305">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="1e3ae-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="1e3ae-306">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="1e3ae-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="1e3ae-307">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e3ae-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)