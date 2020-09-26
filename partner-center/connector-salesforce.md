---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires avec votre CRM Salesforce
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 1b658f04b1348eb48f694fac069518a7a7fc6a70
ms.sourcegitcommit: 505c38436780a31692f5f5694830fcfe01502977
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91372824"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="1bcd3-103">Connecteur de covente pour Salesforce CRM - vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="1bcd3-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1bcd3-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="1bcd3-104">Appropriate roles</span></span>

- <span data-ttu-id="1bcd3-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="1bcd3-105">Referrals admin</span></span>
- <span data-ttu-id="1bcd3-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="1bcd3-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1bcd3-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1bcd3-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1bcd3-109">À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="1bcd3-110">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1bcd3-111">Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1bcd3-112">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1bcd3-113">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="1bcd3-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1bcd3-114">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-114">**Topics**</span></span>   |<span data-ttu-id="1bcd3-115">**Détails**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-115">**Details**</span></span>   |<span data-ttu-id="1bcd3-116">**Liens**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1bcd3-117">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="1bcd3-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1bcd3-118">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="1bcd3-118">You need a valid MPN ID</span></span>|<span data-ttu-id="1bcd3-119">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1bcd3-120">Prêt pour la co-vente</span><span class="sxs-lookup"><span data-stu-id="1bcd3-120">Co-sell ready</span></span>|<span data-ttu-id="1bcd3-121">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1bcd3-122">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="1bcd3-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1bcd3-123">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-123">Partner Center account</span></span>|<span data-ttu-id="1bcd3-124">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1bcd3-125">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="1bcd3-126">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="1bcd3-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1bcd3-127">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-127">Partner Center user roles</span></span>|<span data-ttu-id="1bcd3-128">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="1bcd3-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1bcd3-129">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1bcd3-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1bcd3-130">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="1bcd3-130">Salesforce CRM</span></span>|<span data-ttu-id="1bcd3-131">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="1bcd3-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1bcd3-132">Affecter des rôles dans Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1bcd3-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1bcd3-133">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="1bcd3-133">Power Automate Flow Account</span></span>|<span data-ttu-id="1bcd3-134">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1bcd3-135">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="1bcd3-136">Installation du package Salesforce pour les champs personnalisés Microsoft</span><span class="sxs-lookup"><span data-stu-id="1bcd3-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="1bcd3-137">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit identifier clairement les champs de référence spécifiques à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="1bcd3-138">Cette délimitation fournit aux équipes de vendeur partenaires la possibilité de choisir les références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="1bcd3-139">Dans Salesforce, activez les **Notes** et ajoutez-les à la liste des opportunités associées.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="1bcd3-140">Référence</span><span class="sxs-lookup"><span data-stu-id="1bcd3-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="1bcd3-141">Pour activer les **équipes d’opportunités** , procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="1bcd3-142">Dans le programme d’installation, utilisez la zone de **recherche rapide** pour localiser les paramètres de l’équipe des opportunités.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="1bcd3-143">Définissez les paramètres selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-143">Define the settings as needed.</span></span>
[<span data-ttu-id="1bcd3-144">Référence</span><span class="sxs-lookup"><span data-stu-id="1bcd3-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="1bcd3-145">Dans Salesforce, installez les champs et les objets personnalisés à l’aide du programme d’installation de package ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="1bcd3-146">Cliquez [ici](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) pour installer le package dans une société :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="1bcd3-147">Remarque : Si vous installez dans un bac à sable (sandbox), vous devez remplacer la partie initiale de l’URL par http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="1bcd3-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="1bcd3-148">Dans Salesforce, ajoutez des solutions Microsoft à la liste des **opportunités** associées.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="1bcd3-149">Une fois que vous avez ajouté, cliquez sur l’icône de **clé** et mettez à jour les propriétés</span><span class="sxs-lookup"><span data-stu-id="1bcd3-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1bcd3-150">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="1bcd3-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="1bcd3-151">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1bcd3-152">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="1bcd3-153">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="1bcd3-154">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="1bcd3-155">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="1bcd3-156">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1bcd3-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="1bcd3-157">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1bcd3-158">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1bcd3-159">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="1bcd3-160">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1bcd3-161">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. <span data-ttu-id="1bcd3-163">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="1bcd3-165">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="1bcd3-166">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="1bcd3-167">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRM disponibles":::

8. <span data-ttu-id="1bcd3-169">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="1bcd3-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1bcd3-170">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1bcd3-171">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1bcd3-172">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="1bcd3-173">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1bcd3-174">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1bcd3-175">Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="1bcd3-176">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flux Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="1bcd3-178">Configuration de la solution</span><span class="sxs-lookup"><span data-stu-id="1bcd3-178">Configure the solution</span></span>

1. <span data-ttu-id="1bcd3-179">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1bcd3-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="1bcd3-180">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="1bcd3-181">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="1bcd3-182">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="1bcd3-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="1bcd3-183">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-183">Partner Center Events</span></span>
    - <span data-ttu-id="1bcd3-184">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="1bcd3-185">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="1bcd3-186">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Créer une connexion":::

- <span data-ttu-id="1bcd3-188">Recherchez les références de l’espace partenaires (préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="1bcd3-189">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="1bcd3-190">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="1bcd3-191">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="1bcd3-192">Une fois que toutes les connexions ont été ajoutées, vous devez voir les connexions suivantes dans votre environnement :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observer les connexions":::

### <a name="edit-the-connections"></a><span data-ttu-id="1bcd3-194">Modifier les connexions</span><span class="sxs-lookup"><span data-stu-id="1bcd3-194">Edit the connections</span></span>

1. <span data-ttu-id="1bcd3-195">Revenez à la page solutions et sélectionnez **solution par défaut**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="1bcd3-196">Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Commencer la modification du connecteur":::

2. <span data-ttu-id="1bcd3-198">Modifiez chacune des connexions une par une en sélectionnant l’icône à trois points.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="1bcd3-199">Ajoutez les connexions appropriées.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modifier les connecteurs":::

3. <span data-ttu-id="1bcd3-201">Activez les flux dans l’ordre suivant :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="1bcd3-202">Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-203">Créer une référence de covente-Salesforce à l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-204">Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-205">Espace partenaires vers Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-206">Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-207">Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1bcd3-208">Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="1bcd3-209">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="1bcd3-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="1bcd3-210">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1bcd3-211">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="1bcd3-212">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1bcd3-213">Ajoutez des connexions pour (a.) utilisateur de l’espace partenaires avec les références d’administrateur (b.) des événements de l’espace partenaires comme indiqué ci-dessous</span><span class="sxs-lookup"><span data-stu-id="1bcd3-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. <span data-ttu-id="1bcd3-215">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="1bcd3-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1bcd3-217">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1bcd3-218">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="1bcd3-219">Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="1bcd3-220">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1bcd3-221">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copier l’URL":::

8. <span data-ttu-id="1bcd3-223">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1bcd3-224">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1bcd3-225">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-225">Enter the following details:</span></span>

    1. <span data-ttu-id="1bcd3-226">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="1bcd3-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1bcd3-227">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="1bcd3-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="1bcd3-228">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="1bcd3-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="1bcd3-229">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="1bcd3-230">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1bcd3-231">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="1bcd3-231">Customize synchronization steps</span></span>

<span data-ttu-id="1bcd3-232">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1bcd3-233">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1bcd3-234">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1bcd3-235">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1bcd3-236">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1bcd3-237">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1bcd3-238">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1bcd3-239">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="1bcd3-240">Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="1bcd3-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="1bcd3-241">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="1bcd3-242">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1bcd3-243">Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1bcd3-244">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1bcd3-245">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="1bcd3-246">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="1bcd3-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="1bcd3-247">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1bcd3-248">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="1bcd3-249">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1bcd3-250">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="1bcd3-251">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1bcd3-252">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="1bcd3-253">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="1bcd3-254">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1bcd3-255">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1bcd3-256">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="1bcd3-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="1bcd3-257">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1bcd3-258">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="1bcd3-259">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="1bcd3-260">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="1bcd3-261">Définir des champs et des relations</span><span class="sxs-lookup"><span data-stu-id="1bcd3-261">Set up fields and relationships</span></span>

1. <span data-ttu-id="1bcd3-262">Connectez-vous à votre compte Salesforce et accédez à **opportunité**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-262">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="1bcd3-263">Cliquez sur les options **d’installation** et de **modification d’objet** pour ajouter les champs nécessaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-263">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="1bcd3-264">Sélectionner les **champs & les relations** dans le volet de navigation gauche</span><span class="sxs-lookup"><span data-stu-id="1bcd3-264">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="1bcd3-266">Ajoutez les champs suivants dans la table **fields & Relationship** :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-266">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="1bcd3-267">**Étiquette du champ**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-267">**Field label**</span></span>   |<span data-ttu-id="1bcd3-268">**Nom du champ**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-268">**Field name**</span></span>|<span data-ttu-id="1bcd3-269">**Type de données**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-269">**Data type**</span></span>|<span data-ttu-id="1bcd3-270">**Indexée**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-270">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="1bcd3-271">Audit</span><span class="sxs-lookup"><span data-stu-id="1bcd3-271">Audit</span></span>| <span data-ttu-id="1bcd3-272">Audit__c</span><span class="sxs-lookup"><span data-stu-id="1bcd3-272">Audit__c</span></span>|<span data-ttu-id="1bcd3-273">Longue zone de texte (100000) (ligne visible 4)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-273">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="1bcd3-274">Comment Microsoft peut-il vous aider ?</span><span class="sxs-lookup"><span data-stu-id="1bcd3-274">How can Microsoft help?</span></span>|<span data-ttu-id="1bcd3-275">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="1bcd3-275">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="1bcd3-276">Liste déroulante</span><span class="sxs-lookup"><span data-stu-id="1bcd3-276">Picklist\*</span></span>|
   |<span data-ttu-id="1bcd3-277">Produits</span><span class="sxs-lookup"><span data-stu-id="1bcd3-277">Products</span></span>|<span data-ttu-id="1bcd3-278">Products_c</span><span class="sxs-lookup"><span data-stu-id="1bcd3-278">Products_c</span></span>|<span data-ttu-id="1bcd3-279">texte (255)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-279">text (255)</span></span>||
   |<span data-ttu-id="1bcd3-280">Referral</span><span class="sxs-lookup"><span data-stu-id="1bcd3-280">Referral</span></span> | <span data-ttu-id="1bcd3-281">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="1bcd3-281">Referral_Identfier_c</span></span>|<span data-ttu-id="1bcd3-282">Texte (100) (ID externe)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-282">Text(100)(External ID)</span></span>|<span data-ttu-id="1bcd3-283">Oui</span><span class="sxs-lookup"><span data-stu-id="1bcd3-283">yes</span></span>|
   |<span data-ttu-id="1bcd3-284">Lien de référence</span><span class="sxs-lookup"><span data-stu-id="1bcd3-284">Referral Link</span></span>| <span data-ttu-id="1bcd3-285">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="1bcd3-285">Referral_Link_c_</span></span>|<span data-ttu-id="1bcd3-286">URL (255)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-286">URL(255)</span></span>||
   |<span data-ttu-id="1bcd3-287">Synchroniser avec l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-287">Sync with Partner Center</span></span>|<span data-ttu-id="1bcd3-288">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="1bcd3-288">sync_with_partner_center_c</span></span>|<span data-ttu-id="1bcd3-289">Case à cocher (désactivé par défaut)</span><span class="sxs-lookup"><span data-stu-id="1bcd3-289">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="1bcd3-290">\* Valeurs de liste déroulante :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-290">\*Picklist values:</span></span>

   - <span data-ttu-id="1bcd3-291">Proposition de valeur spécifique à la charge de travail</span><span class="sxs-lookup"><span data-stu-id="1bcd3-291">Workload specific value proposition</span></span>
   - <span data-ttu-id="1bcd3-292">Architecture technique du client</span><span class="sxs-lookup"><span data-stu-id="1bcd3-292">Customer technical architecture</span></span>
   - <span data-ttu-id="1bcd3-293">Preuve de concept ou démonstration</span><span class="sxs-lookup"><span data-stu-id="1bcd3-293">Proof of concept or demo</span></span>
   - <span data-ttu-id="1bcd3-294">Devis ou licences</span><span class="sxs-lookup"><span data-stu-id="1bcd3-294">Quotes or licensing</span></span>
   - <span data-ttu-id="1bcd3-295">Succès du client après la vente</span><span class="sxs-lookup"><span data-stu-id="1bcd3-295">Post sales customer success</span></span>
   - <span data-ttu-id="1bcd3-296">Général ou autre</span><span class="sxs-lookup"><span data-stu-id="1bcd3-296">General or other</span></span>

5. <span data-ttu-id="1bcd3-297">Les champs sont créés sous les **champs & les relations**</span><span class="sxs-lookup"><span data-stu-id="1bcd3-297">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Champs créés":::

6. <span data-ttu-id="1bcd3-299">Dans la disposition opportunité, créez une section distincte avec les champs comme indiqué ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-299">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="1bcd3-300">Cette section doit être disponible pour les vendeurs dans la disposition opportunité.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-300">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Disposition des champs de l’espace partenaires":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1bcd3-302">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="1bcd3-302">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="1bcd3-303">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-303">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1bcd3-304">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="1bcd3-304">Pre-requisites</span></span>

<span data-ttu-id="1bcd3-305">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-305">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="1bcd3-306">Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-306">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1bcd3-307">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-307">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="1bcd3-308">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="1bcd3-308">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1bcd3-309">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-309">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1bcd3-310">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1bcd3-310">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1bcd3-311">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1bcd3-311">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1bcd3-312">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="1bcd3-312">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1bcd3-313">**Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="1bcd3-313">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1bcd3-314">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="1bcd3-314">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1bcd3-315">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-315">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="1bcd3-316">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="1bcd3-316">SCENARIOS:</span></span>

1. <span data-ttu-id="1bcd3-317">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-317">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1bcd3-318">Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-318">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1bcd3-319">Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="1bcd3-319">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Environnement Salesforce":::

   3. <span data-ttu-id="1bcd3-321">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-321">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="1bcd3-322">« Synchroniser avec l’espace partenaires » : Oui</span><span class="sxs-lookup"><span data-stu-id="1bcd3-322">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="1bcd3-323">« Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-323">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="1bcd3-324">Produits : ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="1bcd3-324">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1bcd3-325">Une fois que vous avez défini l’option  **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-325">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="1bcd3-326">Vos références seront synchronisées avec Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-326">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="1bcd3-327">Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-327">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="1bcd3-328">Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-328">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="1bcd3-329">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :</span><span class="sxs-lookup"><span data-stu-id="1bcd3-329">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="1bcd3-330">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-330">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="1bcd3-331">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="1bcd3-331">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="1bcd3-332">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="1bcd3-332">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="1bcd3-333">Connectez-vous à votre environnement CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-333">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="1bcd3-334">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-334">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1bcd3-335">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-335">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Écran d’opportunités Salesforce":::

    6. <span data-ttu-id="1bcd3-337">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="1bcd3-337">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1bcd3-338">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1bcd3-338">Next steps</span></span>

- [<span data-ttu-id="1bcd3-339">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="1bcd3-339">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1bcd3-340">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="1bcd3-340">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="1bcd3-341">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1bcd3-341">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)