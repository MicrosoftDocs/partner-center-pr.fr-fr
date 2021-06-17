---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisez vos références dans l’espace partenaires avec votre CRM Salesforce. Les vendeurs peuvent ensuite se vendre avec Microsoft à partir de vos systèmes CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276975"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="ad58d-104">Connecteur de covente pour Salesforce CRM - vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="ad58d-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="ad58d-105">**Rôles appropriés**: administration des références | Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="ad58d-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="ad58d-106">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="ad58d-107">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="ad58d-108">À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.</span><span class="sxs-lookup"><span data-stu-id="ad58d-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="ad58d-109">Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="ad58d-110">Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="ad58d-111">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="ad58d-112">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="ad58d-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="ad58d-113">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="ad58d-113">**Topics**</span></span>   |<span data-ttu-id="ad58d-114">**Détails**</span><span class="sxs-lookup"><span data-stu-id="ad58d-114">**Details**</span></span>   |<span data-ttu-id="ad58d-115">**Liens**</span><span class="sxs-lookup"><span data-stu-id="ad58d-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="ad58d-116">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="ad58d-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="ad58d-117">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="ad58d-117">You need a valid MPN ID</span></span>|<span data-ttu-id="ad58d-118">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="ad58d-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="ad58d-119">Prêt pour la co-vente</span><span class="sxs-lookup"><span data-stu-id="ad58d-119">Co-sell ready</span></span>|<span data-ttu-id="ad58d-120">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="ad58d-121">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad58d-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="ad58d-122">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ad58d-122">Partner Center account</span></span>|<span data-ttu-id="ad58d-123">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="ad58d-124">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="ad58d-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="ad58d-125">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="ad58d-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ad58d-126">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ad58d-126">Partner Center user roles</span></span>|<span data-ttu-id="ad58d-127">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="ad58d-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="ad58d-128">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="ad58d-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="ad58d-129">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="ad58d-129">Salesforce CRM</span></span>|<span data-ttu-id="ad58d-130">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="ad58d-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="ad58d-131">Affecter des rôles dans Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ad58d-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="ad58d-132">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="ad58d-132">Power Automate Flow Account</span></span>|<span data-ttu-id="ad58d-133">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="ad58d-134">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="ad58d-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="ad58d-135">Installation du package Salesforce pour les champs personnalisés Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad58d-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="ad58d-136">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit identifier clairement les champs de référence spécifiques à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ad58d-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="ad58d-137">Cette délimitation fournit aux équipes de vendeur partenaires la possibilité de choisir les références qu’elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="ad58d-138">Dans Salesforce, activez les **Notes** et ajoutez-les à la liste des opportunités associées.</span><span class="sxs-lookup"><span data-stu-id="ad58d-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="ad58d-139">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="ad58d-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="ad58d-140">Pour activer les **équipes d’opportunités** , procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ad58d-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="ad58d-141">Dans le programme d’installation, utilisez la zone de **recherche rapide** pour localiser les paramètres de l’équipe des opportunités.</span><span class="sxs-lookup"><span data-stu-id="ad58d-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="ad58d-142">Définissez les paramètres selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ad58d-142">Define the settings as needed.</span></span>
[<span data-ttu-id="ad58d-143">Informations de référence</span><span class="sxs-lookup"><span data-stu-id="ad58d-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="ad58d-144">Dans Salesforce, installez des champs et des objets personnalisés à l’aide du [programme d’installation de package](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="ad58d-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="ad58d-145">À utiliser pour installer le package dans n’importe quelle entreprise.</span><span class="sxs-lookup"><span data-stu-id="ad58d-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="ad58d-146">Si vous installez dans un bac à sable (sandbox), vous devez remplacer la partie initiale de l’URL par http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="ad58d-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="ad58d-147">Dans Salesforce, ajoutez des solutions Microsoft à la liste des **opportunités** associées.</span><span class="sxs-lookup"><span data-stu-id="ad58d-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="ad58d-148">Une fois ajouté, sélectionnez l’icône de **clé** et mettez à jour les propriétés</span><span class="sxs-lookup"><span data-stu-id="ad58d-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="ad58d-149">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="ad58d-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="ad58d-150">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="ad58d-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="ad58d-151">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="ad58d-152">Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="ad58d-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="ad58d-153">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="ad58d-154">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="ad58d-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="ad58d-155">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ad58d-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="ad58d-156">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="ad58d-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="ad58d-157">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="ad58d-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="ad58d-158">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="ad58d-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="ad58d-159">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="ad58d-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="ad58d-160">Sélectionnez le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="ad58d-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrez AppSource.":::

5. <span data-ttu-id="ad58d-162">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="ad58d-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Équipes.":::

6. <span data-ttu-id="ad58d-164">Sélectionnez le bouton **Télécharger maintenant** , puis **continuez**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="ad58d-165">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="ad58d-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="ad58d-166">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="ad58d-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRM disponible.":::

8. <span data-ttu-id="ad58d-168">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="ad58d-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="ad58d-169">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="ad58d-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="ad58d-170">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="ad58d-171">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="ad58d-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="ad58d-172">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="ad58d-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="ad58d-173">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="ad58d-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="ad58d-174">Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="ad58d-175">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="ad58d-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Les flux Salesforce.":::



## <a name="configure-the-solution"></a><span data-ttu-id="ad58d-177">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="ad58d-177">Configure the solution</span></span>

1. <span data-ttu-id="ad58d-178">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ad58d-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="ad58d-179">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="ad58d-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="ad58d-180">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="ad58d-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="ad58d-181">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="ad58d-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="ad58d-182">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ad58d-182">Partner Center Events</span></span>
    - <span data-ttu-id="ad58d-183">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="ad58d-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="ad58d-184">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="ad58d-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="ad58d-185">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Créer une connexion.":::

- <span data-ttu-id="ad58d-187">Recherchez les références de l’espace partenaires (préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="ad58d-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="ad58d-188">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.</span><span class="sxs-lookup"><span data-stu-id="ad58d-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="ad58d-189">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.</span><span class="sxs-lookup"><span data-stu-id="ad58d-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="ad58d-190">Créez une connexion pour Salesforce pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="ad58d-191">Une fois que toutes les connexions ont été ajoutées, vous devez voir les connexions suivantes dans votre environnement :</span><span class="sxs-lookup"><span data-stu-id="ad58d-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observez les connexions.":::

### <a name="edit-the-connections"></a><span data-ttu-id="ad58d-193">Modifier les connexions</span><span class="sxs-lookup"><span data-stu-id="ad58d-193">Edit the connections</span></span>

1. <span data-ttu-id="ad58d-194">Revenez à la page solutions et sélectionnez **solution par défaut**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="ad58d-195">Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Commencez la modification du connecteur.":::

2. <span data-ttu-id="ad58d-197">Modifiez chaque connexion individuellement en sélectionnant l’icône en trois points.</span><span class="sxs-lookup"><span data-stu-id="ad58d-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="ad58d-198">Ajoutez les connexions appropriées.</span><span class="sxs-lookup"><span data-stu-id="ad58d-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modifiez les connecteurs.":::

3. <span data-ttu-id="ad58d-200">Activez les flux dans l’ordre suivant :</span><span class="sxs-lookup"><span data-stu-id="ad58d-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="ad58d-201">Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-202">Créer une référence de covente-Salesforce à l’espace partenaires (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-203">Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-204">Espace partenaires vers Salesforce (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-205">Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-206">Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ad58d-207">Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)</span><span class="sxs-lookup"><span data-stu-id="ad58d-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="ad58d-208">Utiliser les API webhook pour s’inscrire aux événements de changement de ressource</span><span class="sxs-lookup"><span data-stu-id="ad58d-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="ad58d-209">Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource.</span><span class="sxs-lookup"><span data-stu-id="ad58d-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="ad58d-210">Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.</span><span class="sxs-lookup"><span data-stu-id="ad58d-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="ad58d-211">Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.</span><span class="sxs-lookup"><span data-stu-id="ad58d-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="ad58d-212">Ajoutez des connexions pour (a.) utilisateur de l’espace partenaires avec les références d’administrateur (b.) des événements de l’espace partenaires comme indiqué ci-dessous</span><span class="sxs-lookup"><span data-stu-id="ad58d-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Stead.":::

3. <span data-ttu-id="ad58d-214">Lorsque vous effectuez ces mises à jour, vous verrez</span><span class="sxs-lookup"><span data-stu-id="ad58d-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="ad58d-216">Enregistrez vos modifications et sélectionnez **activer**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="ad58d-217">Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="ad58d-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="ad58d-218">Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="ad58d-219">Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="ad58d-220">Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.</span><span class="sxs-lookup"><span data-stu-id="ad58d-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copier l’URL.":::

8. <span data-ttu-id="ad58d-222">Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="ad58d-223">Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis sélectionnez **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="ad58d-224">Entrez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="ad58d-224">Enter the following details:</span></span>

    1. <span data-ttu-id="ad58d-225">**Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente</span><span class="sxs-lookup"><span data-stu-id="ad58d-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="ad58d-226">**Événements à inscrire**: « création de références » et « référencement-mis à jour »</span><span class="sxs-lookup"><span data-stu-id="ad58d-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="ad58d-227">**Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).</span><span class="sxs-lookup"><span data-stu-id="ad58d-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="ad58d-228">Sélectionnez **exécuter** , puis sélectionnez **terminé.**</span><span class="sxs-lookup"><span data-stu-id="ad58d-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="ad58d-229">Le webhook peut maintenant écouter les événements de création et de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="ad58d-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="ad58d-230">Personnaliser les étapes de synchronisation</span><span class="sxs-lookup"><span data-stu-id="ad58d-230">Customize synchronization steps</span></span>

<span data-ttu-id="ad58d-231">Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.</span><span class="sxs-lookup"><span data-stu-id="ad58d-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="ad58d-232">Souvent, les systèmes CRM sont hautement personnalisés.</span><span class="sxs-lookup"><span data-stu-id="ad58d-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="ad58d-233">Vous pouvez personnaliser les flux Power automate.</span><span class="sxs-lookup"><span data-stu-id="ad58d-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="ad58d-234">Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.</span><span class="sxs-lookup"><span data-stu-id="ad58d-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="ad58d-235">Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.</span><span class="sxs-lookup"><span data-stu-id="ad58d-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="ad58d-236">Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins.</span><span class="sxs-lookup"><span data-stu-id="ad58d-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="ad58d-237">Voici quelques exemples de personnalisations disponibles :</span><span class="sxs-lookup"><span data-stu-id="ad58d-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="ad58d-238">Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM :</span><span class="sxs-lookup"><span data-stu-id="ad58d-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="ad58d-239">Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).</span><span class="sxs-lookup"><span data-stu-id="ad58d-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="ad58d-240">Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="ad58d-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="ad58d-241">Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="ad58d-242">Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="ad58d-243">Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="ad58d-244">Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="ad58d-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="ad58d-245">Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, sélectionnez l’étape « (étendue) synchroniser le prospect ou l’opportunité ».</span><span class="sxs-lookup"><span data-stu-id="ad58d-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="ad58d-246">Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="ad58d-247">Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="ad58d-248">Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**</span><span class="sxs-lookup"><span data-stu-id="ad58d-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="ad58d-249">Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="ad58d-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="ad58d-250">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="ad58d-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ad58d-251">Sélectionnez **(étendue) synchroniser l’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="ad58d-252">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="ad58d-253">Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="ad58d-254">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="ad58d-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="ad58d-255">Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?</span><span class="sxs-lookup"><span data-stu-id="ad58d-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="ad58d-256">Sélectionnez **modifier**  pour modifier/personnaliser le Flow automatiser l’alimentation.</span><span class="sxs-lookup"><span data-stu-id="ad58d-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="ad58d-257">Sélectionnez **(étendue) synchronisation des références.**</span><span class="sxs-lookup"><span data-stu-id="ad58d-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="ad58d-258">Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="ad58d-259">Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.</span><span class="sxs-lookup"><span data-stu-id="ad58d-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="ad58d-260">Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout</span><span class="sxs-lookup"><span data-stu-id="ad58d-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="ad58d-261">Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="ad58d-262">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="ad58d-262">Pre-requisites</span></span>

<span data-ttu-id="ad58d-263">Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ad58d-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="ad58d-264">Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.</span><span class="sxs-lookup"><span data-stu-id="ad58d-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="ad58d-265">Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="ad58d-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="ad58d-266">Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .</span><span class="sxs-lookup"><span data-stu-id="ad58d-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="ad58d-267">Les champs personnalisés suivants doivent faire partie de la section CRM :</span><span class="sxs-lookup"><span data-stu-id="ad58d-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="ad58d-268">**Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad58d-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="ad58d-269">**Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad58d-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="ad58d-270">**Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft</span><span class="sxs-lookup"><span data-stu-id="ad58d-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="ad58d-271">**Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence</span><span class="sxs-lookup"><span data-stu-id="ad58d-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="ad58d-272">**Produits**: liste des produits associés à cette opportunité</span><span class="sxs-lookup"><span data-stu-id="ad58d-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="ad58d-273">**Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ad58d-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="ad58d-274">SCÉNARIO</span><span class="sxs-lookup"><span data-stu-id="ad58d-274">SCENARIOS:</span></span>

1. <span data-ttu-id="ad58d-275">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="ad58d-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="ad58d-276">Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="ad58d-277">Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="ad58d-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Environnement Salesforce.":::

   3. <span data-ttu-id="ad58d-279">Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :</span><span class="sxs-lookup"><span data-stu-id="ad58d-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="ad58d-280">« Synchroniser avec l’espace partenaires » : Oui</span><span class="sxs-lookup"><span data-stu-id="ad58d-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="ad58d-281">« Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="ad58d-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="ad58d-282">Produits : ID de solution du produit</span><span class="sxs-lookup"><span data-stu-id="ad58d-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="ad58d-283">Une fois que vous avez défini l’option  **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="ad58d-284">Vos références seront synchronisées avec Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="ad58d-285">Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="ad58d-286">Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="ad58d-287">Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :</span><span class="sxs-lookup"><span data-stu-id="ad58d-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="ad58d-288">Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="ad58d-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="ad58d-289">Dans le menu de gauche, sélectionnez **références** .</span><span class="sxs-lookup"><span data-stu-id="ad58d-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="ad58d-290">Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».</span><span class="sxs-lookup"><span data-stu-id="ad58d-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="ad58d-291">Connectez-vous à votre environnement CRM Salesforce.</span><span class="sxs-lookup"><span data-stu-id="ad58d-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="ad58d-292">Accédez à **opportunités ouvertes**.</span><span class="sxs-lookup"><span data-stu-id="ad58d-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="ad58d-293">La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="ad58d-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Écran d’opportunités Salesforce.":::

    6. <span data-ttu-id="ad58d-295">Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.</span><span class="sxs-lookup"><span data-stu-id="ad58d-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ad58d-296">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="ad58d-296">Next steps</span></span>

- [<span data-ttu-id="ad58d-297">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="ad58d-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="ad58d-298">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="ad58d-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="ad58d-299">Webhooks de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="ad58d-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
