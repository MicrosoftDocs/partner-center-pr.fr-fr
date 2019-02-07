---
title: Personnaliser les out-of-box d’un appareil avec des profils Windows Autopilot | L’espace partenaires
description: Préconfigurer expérience d’out-of-box d’un appareil avec des profils Autopilot.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot windows, autopilot de microsoft, déploiement zero touch, oobe, écrans d’ouverture de session, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062277"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="d96dc-104">Personnaliser les out-of-box d’un appareil avec des profils Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="d96dc-105">S’applique à</span><span class="sxs-lookup"><span data-stu-id="d96dc-105">Applies to</span></span>**

- <span data-ttu-id="d96dc-106">Les partenaires de facture direct de fournisseur de solutions cloud, les fournisseurs indirects et les revendeurs indirects</span><span class="sxs-lookup"><span data-stu-id="d96dc-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="d96dc-107">Si vous gérez les appareils clients, vous devrez peut-être personnaliser l’expérience out-of-box (OOBE) pour les utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="d96dc-108">Vous pouvez préconfigurer de nouveaux appareils avec des profils Windows Autopilot avant de distribuer les appareils à des clients et appliquer des profils à nouveau sur les appareils clients ont déjà acheté.</span><span class="sxs-lookup"><span data-stu-id="d96dc-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="d96dc-109">Cet article explique comment créer et appliquer des profils Autopilot aux appareils dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d96dc-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="d96dc-110">Si vous n’êtes pas déjà familiarisé avec Autopilot, passez en revue les informations contenues dans les articles suivants:</span><span class="sxs-lookup"><span data-stu-id="d96dc-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="d96dc-111">Vue d’ensemble de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="d96dc-112">Guide de référence de déploiement AutoPilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="d96dc-113">Vue d'ensemble</span><span class="sxs-lookup"><span data-stu-id="d96dc-113">Overview</span></span>

<span data-ttu-id="d96dc-114">Avec la fonctionnalité Windows Autopilot dans l’espace partenaires, vous pouvez créer des profils personnalisés à appliquer aux appareils du client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="d96dc-115">Les paramètres de profil suivants étaient disponibles lors de la publication de cet article:</span><span class="sxs-lookup"><span data-stu-id="d96dc-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="d96dc-116">Ignorer les paramètres de confidentialité.</span><span class="sxs-lookup"><span data-stu-id="d96dc-116">Skip privacy settings.</span></span> <span data-ttu-id="d96dc-117">Ce paramètre de profil Autopilot facultatif permet aux organisations de ne demander pas sur les paramètres de confidentialité au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="d96dc-118">Désactiver la création du compte administrateur local sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="d96dc-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="d96dc-119">Les organisations peuvent décider si l’utilisateur de configurer l’appareil doit avoir un accès administrateur une fois que le processus est terminé.</span><span class="sxs-lookup"><span data-stu-id="d96dc-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="d96dc-120">Configurer automatiquement l’appareil professionnel ou scolaire.</span><span class="sxs-lookup"><span data-stu-id="d96dc-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="d96dc-121">Tous les appareils enregistrés avec Autopilot seront automatiquement être considérée comme professionnelle ou à l’établissement d’appareils, afin que cette question ne sera pas demandée au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="d96dc-122">Ignorez les pages de paramètres d’inscription Cortana, OneDrive et OEM.</span><span class="sxs-lookup"><span data-stu-id="d96dc-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="d96dc-123">Tous les appareils enregistrés avec Autopilot ignore automatiquement ces pages au cours du processus d’out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="d96dc-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="d96dc-124">Ignorer le contrat de licence utilisateur final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="d96dc-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="d96dc-125">À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page CLUF présentée au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="d96dc-126">Voir [abandon du CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF lors de l’installation de Windows.</span><span class="sxs-lookup"><span data-stu-id="d96dc-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="d96dc-127">Les autorisations de gestion de profil et le périphérique et les limitations suivantes s’appliquent:</span><span class="sxs-lookup"><span data-stu-id="d96dc-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="d96dc-128">Les partenaires fournisseurs de solutions cloud peuvent continuer à gérer les profils Autopilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé les privilèges d’administration déléguées du partenaire.</span><span class="sxs-lookup"><span data-stu-id="d96dc-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="d96dc-129">Vous pouvez gérer des appareils existants pour vos clients qui ont été ajoutés par vous ou par un autre partenaire fournisseur de solutions cloud.</span><span class="sxs-lookup"><span data-stu-id="d96dc-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="d96dc-130">Vous ne pouvez pas gérer les appareils que votre client a téléchargés à Microsoft Store pour entreprises ou Microsoft Intune Portal.</span><span class="sxs-lookup"><span data-stu-id="d96dc-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="d96dc-131">Créer et gérer les profils Autopilot dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d96dc-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="d96dc-132">Dans l’espace partenaires, vous pouvez créer des profils Windows Autopilot deployment et les appliquer aux appareils.</span><span class="sxs-lookup"><span data-stu-id="d96dc-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="d96dc-133">Seuls les agents peuvent créer et appliquer des profils.</span><span class="sxs-lookup"><span data-stu-id="d96dc-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="d96dc-134">Créez un nouveau profil Autopilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="d96dc-135">Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous créez le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="d96dc-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="d96dc-136">Sur la page des détails du client, sélectionnez **les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d96dc-137">Sous **profils Windows Autopilot** sélectionnez **Ajouter un nouveau profil**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="d96dc-138">Entrez le nom et une description du profil, puis configurez les paramètres de la phase OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="d96dc-139">Choisir parmi:</span><span class="sxs-lookup"><span data-stu-id="d96dc-139">Choose from:</span></span>  

   - <span data-ttu-id="d96dc-140">Ignorer les paramètres de confidentialité dans le programme d’installation</span><span class="sxs-lookup"><span data-stu-id="d96dc-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="d96dc-141">Désactiver le compte d’administrateur local dans l'installation</span><span class="sxs-lookup"><span data-stu-id="d96dc-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="d96dc-142">Ignorer automatiquement des pages dans l'installation</span><span class="sxs-lookup"><span data-stu-id="d96dc-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="d96dc-143">(Inclut *Ignorer Cortana, OneDrive et OEM pages de paramètres d’inscription*et de *Sélectionner automatiquement le programme d’installation Professionnel ou scolaire* )</span><span class="sxs-lookup"><span data-stu-id="d96dc-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="d96dc-144">Ignorer le contrat de licence utilisateur final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="d96dc-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="d96dc-145">Voir [abandon du CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF lors de l’installation de Windows.</span><span class="sxs-lookup"><span data-stu-id="d96dc-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="d96dc-146">Sélectionnez **Envoyer** une fois terminé.</span><span class="sxs-lookup"><span data-stu-id="d96dc-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="d96dc-147">Appliquer un profil Autopilot aux appareils du client</span><span class="sxs-lookup"><span data-stu-id="d96dc-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="d96dc-148">Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client vers l’espace partenaires et que vous pouvez accéder à leur liste d’appareils.</span><span class="sxs-lookup"><span data-stu-id="d96dc-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="d96dc-149">Si vous n’avez pas déjà ajouté les appareils du client, suivez les instructions de [périphériques d’ajouter à un compte client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="d96dc-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="d96dc-150">Après avoir créé un profil Autopilot pour un client, vous pouvez l’appliquer aux appareils du client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="d96dc-151">Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous avez créé le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="d96dc-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d96dc-152">Sur la page des détails du client, sélectionnez **les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d96dc-153">Sous **profils appliquer aux appareils** sélectionner les périphériques ou les groupes de périphériques que vous souhaitez ajouter des profils, puis sélectionnez **Appliquer profil**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="d96dc-154">Le profil que vous venez d’appliquer s’affiche dans la colonne **profil** .</span><span class="sxs-lookup"><span data-stu-id="d96dc-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="d96dc-155">Suivez les étapes ci-dessous pour vérifier que le profil est appliqué correctement à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="d96dc-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="d96dc-156">a.</span><span class="sxs-lookup"><span data-stu-id="d96dc-156">a.</span></span>  <span data-ttu-id="d96dc-157">Connectez un appareil au réseau et mettez-le sous tension.</span><span class="sxs-lookup"><span data-stu-id="d96dc-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="d96dc-158">b.</span><span class="sxs-lookup"><span data-stu-id="d96dc-158">b.</span></span>  <span data-ttu-id="d96dc-159">Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.</span><span class="sxs-lookup"><span data-stu-id="d96dc-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="d96dc-160">c.</span><span class="sxs-lookup"><span data-stu-id="d96dc-160">c.</span></span>  <span data-ttu-id="d96dc-161">Lorsque le processus OOBE s’arrête, réinitialiser l’appareil ses paramètres d’usine par défaut pour préparer à un nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d96dc-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="d96dc-162">Supprimer un profil Autopilot à partir de l’appareil d’un client</span><span class="sxs-lookup"><span data-stu-id="d96dc-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="d96dc-163">Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous avez créé le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="d96dc-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d96dc-164">Sur la page des détails du client, sélectionnez **les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d96dc-165">Sous **profils appliquer aux appareils** sélectionnez les périphériques que vous souhaitez supprimer le profil, puis sélectionnez **Supprimer le profil**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="d96dc-166">Supprimer un profil à partir d’un appareil ne supprime pas le profil de votre liste.</span><span class="sxs-lookup"><span data-stu-id="d96dc-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="d96dc-167">Si vous souhaitez supprimer un profil, suivez les instructions de [mise à jour ou supprimer un profil Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="d96dc-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="d96dc-168">Mettre à jour ou supprimer un profil Autopilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="d96dc-169">Si un client souhaite modifier l’expérience out-of-box après avoir expédié les appareils sur ces derniers, vous pouvez modifier le profil dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d96dc-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="d96dc-170">Lorsque l’appareil du client se connecte à internet, il télécharge la dernière version de profil au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="d96dc-171">En outre, n’importe quel moment qu'un client rétablit un appareil ses paramètres d’usine par défaut, l’appareil télécharge à nouveau la dernière version de profil au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="d96dc-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="d96dc-172">Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client qui souhaite vous permettent de modifier un profil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="d96dc-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="d96dc-173">Sur la page des détails du client, sélectionnez **les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d96dc-174">Sous **profils Windows Autopilot** , sélectionnez le profil, que vous devez mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="d96dc-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="d96dc-175">Apportez les modifications requises, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="d96dc-176">Pour supprimer ce profil, sélectionnez **Supprimer le profil** à partir de l’angle supérieur droit de la page.</span><span class="sxs-lookup"><span data-stu-id="d96dc-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="d96dc-177">Ajouter des appareils au compte d’un client</span><span class="sxs-lookup"><span data-stu-id="d96dc-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="d96dc-178">Les agents commerciaux et administrateurs peuvent ajouter des appareils au compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="d96dc-179">Avant d’appliquer des profils Autopilot personnalisés pour les appareils clients, vous devez être en mesure d’accéder à la liste d’appareil du client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="d96dc-180">Si vous prévoyez d’utiliser le nom OEM, le numéro de série et combinaison de modèle, n’oubliez pas de ces limitations:</span><span class="sxs-lookup"><span data-stu-id="d96dc-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="d96dc-181">Cela convient tuple uniquement pour les appareils plus récents (4 k hachages, par exemple) et n’est pas prise en charge des hachages de 128 b (RS2 et périphériques préalables).</span><span class="sxs-lookup"><span data-stu-id="d96dc-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="d96dc-182">L’inscription tuple respecte la casse, afin que les données dans le fichier doivent correspondre le modèle et le fabricant noms ***exactement*** comme fournie par le fournisseur OEM (fournisseur matériel).</span><span class="sxs-lookup"><span data-stu-id="d96dc-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="d96dc-183">Suivez les instructions ci-dessous pour ajouter des appareils au compte d’un client dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d96dc-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="d96dc-184">Sélectionnez des **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les appareils.</span><span class="sxs-lookup"><span data-stu-id="d96dc-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="d96dc-185">Sur la page des détails du client, sélectionnez **les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d96dc-186">Sous **profils appliquer aux appareils** sélectionnez **Ajouter les appareils**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="d96dc-187">Entrez un nom pour la liste des périphériques, puis **accédez** à charger la liste du client (au format de fichier .csv) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d96dc-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d96dc-188">Vous devez avoir reçu ce fichier .csv avec votre achat d’appareil.</span><span class="sxs-lookup"><span data-stu-id="d96dc-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="d96dc-189">Si vous n’avez pas recevoir un fichier .csv, vous pouvez créer une vous-même en suivant les étapes décrites dans les [périphériques d’ajout de Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="d96dc-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="d96dc-190">Télécharger le fichier .csv, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="d96dc-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="d96dc-191">Si vous obtenez un message d’erreur en essayant de charger le fichier .csv, vérifiez le format du fichier.</span><span class="sxs-lookup"><span data-stu-id="d96dc-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="d96dc-192">Vous pouvez utiliser le code de hachage matériel uniquement, ou le nom OEM, le numéro de série et modèle (dans cet ordre de colonnes) ou l’ID de produit Windows.</span><span class="sxs-lookup"><span data-stu-id="d96dc-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="d96dc-193">Vous pouvez également utiliser l’exemple de fichier .csv fourni à partir du lien en regard de **périphériques ajouter** pour créer une liste d’appareils.</span><span class="sxs-lookup"><span data-stu-id="d96dc-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="d96dc-194">Abandon du CLUF de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="d96dc-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="d96dc-195">INFORMATIONS IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="d96dc-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="d96dc-196">Windows Autopilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients.</span><span class="sxs-lookup"><span data-stu-id="d96dc-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="d96dc-197">Si vous êtes autorisé à le faire par le client, vous pouvez supprimer ou de masquer certains écrans d’installation qui sont normalement présentés aux utilisateurs lors de la configuration de Windows, y compris l’écran d’acceptation du CLUF (contrat de licence utilisateur final).</span><span class="sxs-lookup"><span data-stu-id="d96dc-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="d96dc-198">À l’aide de cette fonction, vous convenez qu’en supprimant ou en masquant les écrans sont conçus pour fournir aux utilisateurs des avis ou l’acceptation des moyens de termes que vous avez obtenu les consentement suffisant et autorisation à partir de votre client pour masquer les termes du contrat et que vous avez, pour le compte de votre client (indique si une organisation ou un utilisateur individuel en tant que celle-ci peut être), consentez à n’importe quel avis et acceptez les conditions applicables à votre client.</span><span class="sxs-lookup"><span data-stu-id="d96dc-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="d96dc-199">Cela inclut votre acceptation des termes et conditions de la licence ou de l'avis qui serait présenté à l'utilisateur si vous ne l'aviez pas supprimé(e) ni masqué(e) à l'aide de cet outil.</span><span class="sxs-lookup"><span data-stu-id="d96dc-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="d96dc-200">Votre client ne peut pas utiliser le logiciel Windows sur ces appareils s'il n'a pas légitimement acquis une licence pour le logiciel auprès de Microsoft ou de ses revendeurs.</span><span class="sxs-lookup"><span data-stu-id="d96dc-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>