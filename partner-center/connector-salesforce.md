---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisez vos références dans l’espace partenaires avec votre CRM Salesforce. Les vendeurs peuvent ensuite se vendre avec Microsoft à partir de vos systèmes CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b3817dafbd05edf0c50b062b52ac4814c767d04
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031462"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="6ff13-104">Connecteur de covente pour Salesforce CRM - vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="6ff13-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="6ff13-105">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="6ff13-105">Appropriate roles</span></span>

- <span data-ttu-id="6ff13-106">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="6ff13-106">Referrals admin</span></span>
- <span data-ttu-id="6ff13-107">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="6ff13-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="6ff13-108">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="6ff13-109">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="6ff13-110">À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="6ff13-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="6ff13-111">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="6ff13-112">Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="6ff13-113">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="6ff13-114">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="6ff13-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="6ff13-115">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="6ff13-115">**Topics**</span></span>   |<span data-ttu-id="6ff13-116">**Détails**</span><span class="sxs-lookup"><span data-stu-id="6ff13-116">**Details**</span></span>   |<span data-ttu-id="6ff13-117">**Liens**</span><span class="sxs-lookup"><span data-stu-id="6ff13-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="6ff13-118">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="6ff13-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="6ff13-119">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="6ff13-119">You need a valid MPN ID</span></span>|<span data-ttu-id="6ff13-120">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="6ff13-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="6ff13-121">Prêt pour la co-vente</span><span class="sxs-lookup"><span data-stu-id="6ff13-121">Co-sell ready</span></span>|<span data-ttu-id="6ff13-122">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="6ff13-123">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="6ff13-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="6ff13-124">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ff13-124">Partner Center account</span></span>|<span data-ttu-id="6ff13-125">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="6ff13-126">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="6ff13-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="6ff13-127">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="6ff13-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="6ff13-128">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ff13-128">Partner Center user roles</span></span>|<span data-ttu-id="6ff13-129">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="6ff13-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="6ff13-130">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="6ff13-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="6ff13-131">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="6ff13-131">Salesforce CRM</span></span>|<span data-ttu-id="6ff13-132">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="6ff13-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="6ff13-133">Affecter des rôles dans Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="6ff13-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="6ff13-134">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="6ff13-134">Power Automate Flow Account</span></span>|<span data-ttu-id="6ff13-135">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="6ff13-136">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="6ff13-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="6ff13-137">Installation du package Salesforce pour les champs personnalisés Microsoft</span><span class="sxs-lookup"><span data-stu-id="6ff13-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="6ff13-138">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit identifier clairement les champs de référence spécifiques à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6ff13-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="6ff13-139">Cette délimitation fournit aux équipes de vendeur partenaires la possibilité de choisir les références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="6ff13-140">Dans Salesforce, activez les **Notes** et ajoutez-les à la liste des opportunités associées.</span><span class="sxs-lookup"><span data-stu-id="6ff13-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="6ff13-141">Référence</span><span class="sxs-lookup"><span data-stu-id="6ff13-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="6ff13-142">Pour activer les **équipes d’opportunités** , procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6ff13-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="6ff13-143">Dans le programme d’installation, utilisez la zone de **recherche rapide** pour localiser les paramètres de l’équipe des opportunités.</span><span class="sxs-lookup"><span data-stu-id="6ff13-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="6ff13-144">Définissez les paramètres selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="6ff13-144">Define the settings as needed.</span></span>
[<span data-ttu-id="6ff13-145">Référence</span><span class="sxs-lookup"><span data-stu-id="6ff13-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="6ff13-146">Dans Salesforce, installez les champs et les objets personnalisés à l’aide du programme d’installation de package ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="6ff13-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="6ff13-147">Cliquez [ici](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) pour installer le package dans une société :</span><span class="sxs-lookup"><span data-stu-id="6ff13-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="6ff13-148">Remarque : Si vous installez dans un bac à sable (sandbox), vous devez remplacer la partie initiale de l’URL par http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="6ff13-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="6ff13-149">Dans Salesforce, ajoutez des solutions Microsoft à la liste des **opportunités** associées.</span><span class="sxs-lookup"><span data-stu-id="6ff13-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="6ff13-150">Une fois que vous avez ajouté, cliquez sur l’icône de **clé** et mettez à jour les propriétés</span><span class="sxs-lookup"><span data-stu-id="6ff13-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="6ff13-151">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="6ff13-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="6ff13-152">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="6ff13-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="6ff13-153">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="6ff13-154">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="6ff13-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="6ff13-155">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="6ff13-156">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="6ff13-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="6ff13-157">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="6ff13-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="6ff13-158">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="6ff13-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="6ff13-159">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="6ff13-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="6ff13-160">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="6ff13-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="6ff13-161">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="6ff13-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="6ff13-162">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="6ff13-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. <span data-ttu-id="6ff13-164">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="6ff13-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Ouvrir AppSource":::

6. <span data-ttu-id="6ff13-166">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="6ff13-167">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="6ff13-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="6ff13-168">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="6ff13-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Ouvrir AppSource":::

8. <span data-ttu-id="6ff13-170">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="6ff13-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="6ff13-171">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="6ff13-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="6ff13-172">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="6ff13-173">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="6ff13-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="6ff13-174">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="6ff13-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="6ff13-175">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="6ff13-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="6ff13-176">Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="6ff13-177">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="6ff13-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Ouvrir AppSource":::



## <a name="configure-the-solution"></a><span data-ttu-id="6ff13-179">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="6ff13-179">Configure the solution</span></span>

1. <span data-ttu-id="6ff13-180">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="6ff13-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="6ff13-181">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="6ff13-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="6ff13-182">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="6ff13-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="6ff13-183">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="6ff13-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="6ff13-184">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ff13-184">Partner Center Events</span></span>
    - <span data-ttu-id="6ff13-185">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="6ff13-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="6ff13-186">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="6ff13-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="6ff13-187">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Ouvrir AppSource":::

- <span data-ttu-id="6ff13-189">Recherchez les références de l’espace partenaires (préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="6ff13-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="6ff13-190">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="6ff13-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="6ff13-191">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="6ff13-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="6ff13-192">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-192">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="6ff13-193">Une fois que toutes les connexions ont été ajoutées, vous devez voir les connexions suivantes dans votre environnement :</span><span class="sxs-lookup"><span data-stu-id="6ff13-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Ouvrir AppSource":::

### <a name="edit-the-connections"></a><span data-ttu-id="6ff13-195">Modifier les connexions</span><span class="sxs-lookup"><span data-stu-id="6ff13-195">Edit the connections</span></span>

1. <span data-ttu-id="6ff13-196">Revenez à la page solutions et sélectionnez **solution par défaut**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="6ff13-197">Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Ouvrir AppSource":::

2. <span data-ttu-id="6ff13-199">Modifiez chacune des connexions une par une en sélectionnant l’icône à trois points.</span><span class="sxs-lookup"><span data-stu-id="6ff13-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="6ff13-200">Ajoutez les connexions appropriées.</span><span class="sxs-lookup"><span data-stu-id="6ff13-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Ouvrir AppSource":::

3. <span data-ttu-id="6ff13-202">Activez les flux dans l’ordre suivant :</span><span class="sxs-lookup"><span data-stu-id="6ff13-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="6ff13-203">Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-204">Créer une référence de covente-Salesforce à l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-205">Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-206">Espace partenaires vers Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-207">Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-208">Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="6ff13-209">Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="6ff13-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="6ff13-210">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="6ff13-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="6ff13-211">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="6ff13-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="6ff13-212">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="6ff13-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="6ff13-213">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="6ff13-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="6ff13-214">Ajoutez des connexions pour (a.) utilisateur de l’espace partenaires avec les références d’administrateur (b.) des événements de l’espace partenaires comme indiqué ci-dessous</span><span class="sxs-lookup"><span data-stu-id="6ff13-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Ouvrir AppSource":::

3. <span data-ttu-id="6ff13-216">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="6ff13-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Ouvrir AppSource":::

4. <span data-ttu-id="6ff13-218">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="6ff13-219">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6ff13-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="6ff13-220">Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="6ff13-221">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="6ff13-222">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="6ff13-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Ouvrir AppSource":::

8. <span data-ttu-id="6ff13-224">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="6ff13-225">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="6ff13-226">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ff13-226">Enter the following details:</span></span>

    1. <span data-ttu-id="6ff13-227">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="6ff13-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="6ff13-228">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="6ff13-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="6ff13-229">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="6ff13-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="6ff13-230">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="6ff13-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="6ff13-231">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="6ff13-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="6ff13-232">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="6ff13-232">Customize synchronization steps</span></span>

<span data-ttu-id="6ff13-233">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="6ff13-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="6ff13-234">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="6ff13-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="6ff13-235">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="6ff13-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="6ff13-236">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="6ff13-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="6ff13-237">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="6ff13-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="6ff13-238">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="6ff13-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="6ff13-239">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="6ff13-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="6ff13-240">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="6ff13-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="6ff13-241">Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="6ff13-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="6ff13-242">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="6ff13-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="6ff13-243">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="6ff13-244">Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="6ff13-245">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="6ff13-246">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="6ff13-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="6ff13-247">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="6ff13-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="6ff13-248">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="6ff13-249">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="6ff13-250">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="6ff13-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="6ff13-251">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="6ff13-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="6ff13-252">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="6ff13-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="6ff13-253">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="6ff13-254">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="6ff13-255">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="6ff13-256">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="6ff13-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="6ff13-257">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="6ff13-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="6ff13-258">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="6ff13-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="6ff13-259">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="6ff13-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="6ff13-260">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="6ff13-261">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="6ff13-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="6ff13-262">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="6ff13-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="6ff13-263">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="6ff13-264">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="6ff13-264">Pre-requisites</span></span>

<span data-ttu-id="6ff13-265">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6ff13-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="6ff13-266">Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="6ff13-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="6ff13-267">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="6ff13-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="6ff13-268">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="6ff13-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="6ff13-269">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="6ff13-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="6ff13-270">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="6ff13-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="6ff13-271">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="6ff13-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="6ff13-272">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="6ff13-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="6ff13-273">**Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="6ff13-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="6ff13-274">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="6ff13-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="6ff13-275">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ff13-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="6ff13-276">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="6ff13-276">SCENARIOS:</span></span>

1. <span data-ttu-id="6ff13-277">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="6ff13-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="6ff13-278">Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="6ff13-279">Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="6ff13-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ouvrir AppSource":::

   3. <span data-ttu-id="6ff13-281">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="6ff13-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="6ff13-282">« Synchroniser avec l’espace partenaires » : Oui</span><span class="sxs-lookup"><span data-stu-id="6ff13-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="6ff13-283">« Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ff13-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="6ff13-284">Produits : ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="6ff13-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="6ff13-285">Une fois que vous avez défini l’option  **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="6ff13-286">Vos références seront synchronisées avec Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="6ff13-287">Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="6ff13-288">Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="6ff13-289">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :</span><span class="sxs-lookup"><span data-stu-id="6ff13-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="6ff13-290">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="6ff13-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="6ff13-291">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="6ff13-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="6ff13-292">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="6ff13-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="6ff13-293">Connectez-vous à votre environnement CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="6ff13-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="6ff13-294">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="6ff13-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="6ff13-295">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="6ff13-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Ouvrir AppSource":::

    6. <span data-ttu-id="6ff13-297">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="6ff13-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ff13-298">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="6ff13-298">Next steps</span></span>

- [<span data-ttu-id="6ff13-299">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="6ff13-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="6ff13-300">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="6ff13-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="6ff13-301">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="6ff13-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)