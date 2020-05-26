---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisation du connecteur CRM Salesforce, recevoir des références de Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825696"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="c172a-103">Connecteur de co-vente pour Salesforce CRM-vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="c172a-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="c172a-104">Rôles appropriés</span><span class="sxs-lookup"><span data-stu-id="c172a-104">Appropriate roles</span></span>

- <span data-ttu-id="c172a-105">Administrateur des références</span><span class="sxs-lookup"><span data-stu-id="c172a-105">Referrals admin</span></span>
- <span data-ttu-id="c172a-106">Administrateur système ou personnalisateur de système sur le CRM</span><span class="sxs-lookup"><span data-stu-id="c172a-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="c172a-107">Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM.</span><span class="sxs-lookup"><span data-stu-id="c172a-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="c172a-108">Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente.</span><span class="sxs-lookup"><span data-stu-id="c172a-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="c172a-109">À l’aide des connecteurs de covente, vous serez en mesure de créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de transaction, telles que la valeur de la transaction, la date de clôture, etc., ainsi que recevoir les mises à jour des vendeurs Microsoft sur ces offres de covente</span><span class="sxs-lookup"><span data-stu-id="c172a-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="c172a-110">Vous pouvez effectuer toutes ces tâches tout en travaillant dans le CRM de votre choix plutôt que dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c172a-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="c172a-111">La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c172a-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="c172a-112">Avant d’installer-conditions préalables</span><span class="sxs-lookup"><span data-stu-id="c172a-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="c172a-113">**Rubriques**</span><span class="sxs-lookup"><span data-stu-id="c172a-113">**Topics**</span></span>   |<span data-ttu-id="c172a-114">**Détails**</span><span class="sxs-lookup"><span data-stu-id="c172a-114">**Details**</span></span>   |<span data-ttu-id="c172a-115">**Liens**</span><span class="sxs-lookup"><span data-stu-id="c172a-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="c172a-116">ID de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="c172a-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="c172a-117">Vous avez besoin d’un ID MPN valide</span><span class="sxs-lookup"><span data-stu-id="c172a-117">You need a valid MPN ID</span></span>|<span data-ttu-id="c172a-118">Pour rejoindre [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="c172a-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="c172a-119">Co-vente prête</span><span class="sxs-lookup"><span data-stu-id="c172a-119">Co-sell ready</span></span>|<span data-ttu-id="c172a-120">Votre solution IP/Services doit être prête à être covente.</span><span class="sxs-lookup"><span data-stu-id="c172a-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="c172a-121">Vendre avec Microsoft</span><span class="sxs-lookup"><span data-stu-id="c172a-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="c172a-122">Compte Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c172a-122">Partner Center account</span></span>|<span data-ttu-id="c172a-123">L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente.</span><span class="sxs-lookup"><span data-stu-id="c172a-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="c172a-124">Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.</span><span class="sxs-lookup"><span data-stu-id="c172a-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="c172a-125">Gérer votre compte</span><span class="sxs-lookup"><span data-stu-id="c172a-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c172a-126">Rôles d’utilisateur de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c172a-126">Partner Center user roles</span></span>|<span data-ttu-id="c172a-127">L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références</span><span class="sxs-lookup"><span data-stu-id="c172a-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="c172a-128">Affecter des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c172a-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="c172a-129">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="c172a-129">Salesforce CRM</span></span>|<span data-ttu-id="c172a-130">Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système</span><span class="sxs-lookup"><span data-stu-id="c172a-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="c172a-131">Affecter des rôles dans Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c172a-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="c172a-132">Gestion de l’alimentation-automatiser le compte</span><span class="sxs-lookup"><span data-stu-id="c172a-132">Power Automate Flow Account</span></span>|<span data-ttu-id="c172a-133">Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM.</span><span class="sxs-lookup"><span data-stu-id="c172a-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="c172a-134">Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.</span><span class="sxs-lookup"><span data-stu-id="c172a-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="c172a-135">Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="c172a-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="c172a-136">Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="c172a-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="c172a-137">Les instances CRM disponibles s’affichent.</span><span class="sxs-lookup"><span data-stu-id="c172a-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="c172a-138">Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="c172a-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="c172a-139">Sélectionnez **solutions** dans la barre de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="c172a-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="c172a-140">Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.</span><span class="sxs-lookup"><span data-stu-id="c172a-140">Click on the **Open AppSource** link on the top menu.</span></span>

![Ouvrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="c172a-142">Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.</span><span class="sxs-lookup"><span data-stu-id="c172a-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="c172a-143">Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.</span><span class="sxs-lookup"><span data-stu-id="c172a-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="c172a-144">Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.</span><span class="sxs-lookup"><span data-stu-id="c172a-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="c172a-145">Acceptez les conditions générales.</span><span class="sxs-lookup"><span data-stu-id="c172a-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="c172a-146">Vous êtes ensuite dirigé vers la page **gérer vos solutions** .</span><span class="sxs-lookup"><span data-stu-id="c172a-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="c172a-147">Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page.</span><span class="sxs-lookup"><span data-stu-id="c172a-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="c172a-148">**L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c172a-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="c172a-149">L’installation prendra 10-15 minutes.</span><span class="sxs-lookup"><span data-stu-id="c172a-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="c172a-150">Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche.</span><span class="sxs-lookup"><span data-stu-id="c172a-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="c172a-151">Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.</span><span class="sxs-lookup"><span data-stu-id="c172a-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="c172a-152">Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="c172a-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="c172a-153">Les flux et entités Power automate suivants sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="c172a-153">The following Power Automate flows and entities are available:</span></span>

![CRM disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="c172a-155">Meilleure pratique : testez avant de passer en direct</span><span class="sxs-lookup"><span data-stu-id="c172a-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="c172a-156">Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="c172a-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="c172a-157">Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.</span><span class="sxs-lookup"><span data-stu-id="c172a-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="c172a-158">Effectuez une copie de la solution et effectuez votre configuration et automatisez les personnalisations de flow sur l’environnement intermédiaire.</span><span class="sxs-lookup"><span data-stu-id="c172a-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="c172a-159">Testez la solution sur une instance intermédiaire/CRM.</span><span class="sxs-lookup"><span data-stu-id="c172a-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="c172a-160">En cas de réussite, importez en tant que solution gérée dans l’instance de production.</span><span class="sxs-lookup"><span data-stu-id="c172a-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="c172a-161">Configurer la solution</span><span class="sxs-lookup"><span data-stu-id="c172a-161">Configure the solution</span></span>

1. <span data-ttu-id="c172a-162">Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="c172a-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="c172a-163">Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.</span><span class="sxs-lookup"><span data-stu-id="c172a-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="c172a-164">Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="c172a-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="c172a-165">Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références</span><span class="sxs-lookup"><span data-stu-id="c172a-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="c172a-166">Événements de l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c172a-166">Partner Center Events</span></span>
- <span data-ttu-id="c172a-167">L’administrateur CRM avec les flux Power automate dans la solution.</span><span class="sxs-lookup"><span data-stu-id="c172a-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="c172a-168">a.</span><span class="sxs-lookup"><span data-stu-id="c172a-168">a.</span></span> <span data-ttu-id="c172a-169">Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.</span><span class="sxs-lookup"><span data-stu-id="c172a-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="c172a-170">b.</span><span class="sxs-lookup"><span data-stu-id="c172a-170">b.</span></span> <span data-ttu-id="c172a-171">Créez une connexion en cliquant sur **créer une connexion**.</span><span class="sxs-lookup"><span data-stu-id="c172a-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![Créer une connexion](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="c172a-173">c.</span><span class="sxs-lookup"><span data-stu-id="c172a-173">c.</span></span> <span data-ttu-id="c172a-174">Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.</span><span class="sxs-lookup"><span data-stu-id="c172a-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="c172a-175">d.</span><span class="sxs-lookup"><span data-stu-id="c172a-175">d.</span></span> <span data-ttu-id="c172a-176">Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références. Envoyer.</span><span class="sxs-lookup"><span data-stu-id="c172a-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="c172a-177">Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références. FA.</span><span class="sxs-lookup"><span data-stu-id="c172a-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="c172a-178">Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.</span><span class="sxs-lookup"><span data-stu-id="c172a-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="c172a-179">Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c172a-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="c172a-180">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="c172a-180">Save the changes.</span></span>

5. <span data-ttu-id="c172a-181">**Activez** les flux automate Power.</span><span class="sxs-lookup"><span data-stu-id="c172a-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c172a-182">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c172a-182">Next steps</span></span>

- [<span data-ttu-id="c172a-183">Utiliser des webhooks pour recevoir des événements de modification de ressource</span><span class="sxs-lookup"><span data-stu-id="c172a-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="c172a-184">En savoir plus sur la plateforme Microsoft Power Automated ?</span><span class="sxs-lookup"><span data-stu-id="c172a-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="c172a-185">Gérer les prospects</span><span class="sxs-lookup"><span data-stu-id="c172a-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="c172a-186">Gérer les opportunités de covente</span><span class="sxs-lookup"><span data-stu-id="c172a-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
