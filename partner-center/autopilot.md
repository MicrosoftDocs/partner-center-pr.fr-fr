---
title: Personnaliser l’expérience d’out-of-box d’un appareil avec des profils Windows Autopilot | Partenaires
description: Préconfigurer l’expérience d’out-of-box d’un appareil avec des profils Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot autopilot de windows, autopilot de microsoft, zero touch, oobe, écrans de connexion, de déploiement out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586912"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="8975f-104">Personnaliser l’expérience d’out-of-box d’un appareil avec des profils Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="8975f-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="8975f-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="8975f-105">**Applies to**</span></span>

- <span data-ttu-id="8975f-106">Les partenaires CSP direct-facture, les fournisseurs indirects et les revendeurs indirects</span><span class="sxs-lookup"><span data-stu-id="8975f-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="8975f-107">Si vous gérez des appareils clients, vous devrez peut-être personnaliser l’expérience out-of-box (OOBE) pour les utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="8975f-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="8975f-108">Vous pouvez préconfigurer les nouveaux appareils avec des profils Windows Autopilot avant de distribuer les appareils sur les clients et appliquer de nouveaux profils sur des appareils clients ont déjà acheté.</span><span class="sxs-lookup"><span data-stu-id="8975f-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="8975f-109">Cet article explique comment créer et appliquer des profils Autopilot sur les appareils de partenaires.</span><span class="sxs-lookup"><span data-stu-id="8975f-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="8975f-110">Si vous n’êtes pas déjà familiarisé avec Autopilot, passez en revue les informations contenues dans ces articles :</span><span class="sxs-lookup"><span data-stu-id="8975f-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="8975f-111">Vue d’ensemble de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="8975f-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="8975f-112">Guide de référence de déploiement AutoPilot</span><span class="sxs-lookup"><span data-stu-id="8975f-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="8975f-113">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="8975f-113">Overview</span></span>

<span data-ttu-id="8975f-114">Avec la fonctionnalité Windows Autopilot dans Partner Center, vous pouvez créer des profils personnalisés à appliquer à des appareils clients.</span><span class="sxs-lookup"><span data-stu-id="8975f-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="8975f-115">Les paramètres de profil suivants étaient disponibles au moment de la que publication de cet article :</span><span class="sxs-lookup"><span data-stu-id="8975f-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="8975f-116">Ignorer les paramètres de confidentialité.</span><span class="sxs-lookup"><span data-stu-id="8975f-116">Skip privacy settings.</span></span> <span data-ttu-id="8975f-117">Ce paramètre de profil Autopilot facultatif permet aux organisations de plus de paramètres de confidentialité pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="8975f-118">Désactiver la création du compte administrateur local sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="8975f-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="8975f-119">Les organisations peuvent décider si l’utilisateur de la configuration de l’appareil doit avoir un accès administrateur une fois que le processus est terminé.</span><span class="sxs-lookup"><span data-stu-id="8975f-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="8975f-120">Configurer automatiquement des appareils pour les professionnels ou scolaires.</span><span class="sxs-lookup"><span data-stu-id="8975f-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="8975f-121">Tous les appareils inscrits avec Autopilot seront automatiquement considérée comme Professionnel ou scolaire d’appareils, donc cette question ne sera pas invitée au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="8975f-122">Ignorer les pages de configuration de l’inscription Cortana, OneDrive et OEM.</span><span class="sxs-lookup"><span data-stu-id="8975f-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="8975f-123">Tous les appareils inscrits avec Autopilot ignorera automatiquement ces pages au cours du processus d’out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="8975f-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="8975f-124">Ignorer le contrat de licence utilisateur final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="8975f-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="8975f-125">À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page CLUF présentée au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="8975f-126">Consultez [licenciement de Windows Autopilot CLUF](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF pendant Windows le programme d’installation.</span><span class="sxs-lookup"><span data-stu-id="8975f-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="8975f-127">Les autorisations de gestion de profil et le périphérique et les limitations suivantes s’appliquent :</span><span class="sxs-lookup"><span data-stu-id="8975f-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="8975f-128">Les partenaires CSP peuvent continuer à gérer des profils Autopilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé des privilèges d’administration déléguée du partenaire.</span><span class="sxs-lookup"><span data-stu-id="8975f-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="8975f-129">Vous pouvez gérer des appareils existants pour vos clients qui ont été ajoutés par vous ou par un autre partenaire CSP.</span><span class="sxs-lookup"><span data-stu-id="8975f-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="8975f-130">Vous ne pouvez pas gérer les appareils de que votre client a téléchargé vers le Microsoft Store pour entreprises ou Microsoft Intune Portal.</span><span class="sxs-lookup"><span data-stu-id="8975f-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="8975f-131">Créer et gérer des profils Autopilot dans Partner Center</span><span class="sxs-lookup"><span data-stu-id="8975f-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="8975f-132">Dans Partner Center, vous pouvez créer des profils de déploiement Windows Autopilot et les appliquer aux appareils.</span><span class="sxs-lookup"><span data-stu-id="8975f-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="8975f-133">Seuls les agents d’administration peuvent créer et appliquer les profils.</span><span class="sxs-lookup"><span data-stu-id="8975f-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="8975f-134">Créer un nouveau profil Autopilot</span><span class="sxs-lookup"><span data-stu-id="8975f-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="8975f-135">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client que vous créez le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="8975f-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="8975f-136">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8975f-137">Sous **profils Windows Autopilot** sélectionnez **Ajouter nouveau profil**.</span><span class="sxs-lookup"><span data-stu-id="8975f-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="8975f-138">Entrez le nom et la description du profil, puis configurez les paramètres OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="8975f-139">Choisissez parmi :</span><span class="sxs-lookup"><span data-stu-id="8975f-139">Choose from:</span></span>  

   - <span data-ttu-id="8975f-140">Ignorer les paramètres de confidentialité dans le programme d’installation</span><span class="sxs-lookup"><span data-stu-id="8975f-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="8975f-141">Désactiver le compte d’administrateur local dans l'installation</span><span class="sxs-lookup"><span data-stu-id="8975f-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="8975f-142">Ignorer automatiquement des pages dans l'installation</span><span class="sxs-lookup"><span data-stu-id="8975f-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="8975f-143">(Inclut *sélectionner automatiquement le programme d’installation pour les professionnels ou scolaires* et *les pages de configuration de l’inscription Skip Cortana, OneDrive et OEM*)</span><span class="sxs-lookup"><span data-stu-id="8975f-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="8975f-144">Ignorer le contrat de licence utilisateur final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="8975f-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="8975f-145">Consultez [licenciement de Windows Autopilot CLUF](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF pendant Windows le programme d’installation.</span><span class="sxs-lookup"><span data-stu-id="8975f-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="8975f-146">Sélectionnez **Envoyer** une fois terminé.</span><span class="sxs-lookup"><span data-stu-id="8975f-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="8975f-147">Appliquer un profil Autopilot à des appareils clients</span><span class="sxs-lookup"><span data-stu-id="8975f-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="8975f-148">Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client pour les partenaires et que vous pouvez accéder à leur liste des appareils.</span><span class="sxs-lookup"><span data-stu-id="8975f-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="8975f-149">Si vous n’avez pas déjà ajouté les appareils du client, suivez les instructions de [ajouter des appareils à un compte client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8975f-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="8975f-150">Après avoir créé un profil Autopilot pour un client, vous pouvez l’appliquer aux appareils du client.</span><span class="sxs-lookup"><span data-stu-id="8975f-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="8975f-151">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client vous avez créé le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="8975f-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8975f-152">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8975f-153">Sous **appliquer les profils aux appareils** sélectionnez les périphériques ou les groupes de périphériques que vous souhaitez ajouter des profils à, puis sélectionnez **appliquer le profil**.</span><span class="sxs-lookup"><span data-stu-id="8975f-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="8975f-154">Le profil que vous venez d’appliquer s’affiche dans le **profil** colonne.</span><span class="sxs-lookup"><span data-stu-id="8975f-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="8975f-155">Suivez les étapes ci-dessous pour vérifier que le profil est appliqué correctement à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="8975f-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="8975f-156">a.</span><span class="sxs-lookup"><span data-stu-id="8975f-156">a.</span></span>  <span data-ttu-id="8975f-157">Connecter un appareil au réseau et mettez-le sous tension.</span><span class="sxs-lookup"><span data-stu-id="8975f-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="8975f-158">b.</span><span class="sxs-lookup"><span data-stu-id="8975f-158">b.</span></span>  <span data-ttu-id="8975f-159">Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.</span><span class="sxs-lookup"><span data-stu-id="8975f-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="8975f-160">c.</span><span class="sxs-lookup"><span data-stu-id="8975f-160">c.</span></span>  <span data-ttu-id="8975f-161">Lorsque le processus OOBE s’arrête, réinitialiser l’appareil ses paramètres d’usine par défaut afin de le préparer pour un nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8975f-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="8975f-162">Supprimer un profil Autopilot à partir de l’appareil d’un client</span><span class="sxs-lookup"><span data-stu-id="8975f-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="8975f-163">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client vous avez créé le profil Autopilot pour.</span><span class="sxs-lookup"><span data-stu-id="8975f-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8975f-164">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8975f-165">Sous **appliquer les profils aux appareils** sélectionner les appareils que vous souhaitez supprimer le profil à partir de, puis sélectionnez **supprimer le profil**.</span><span class="sxs-lookup"><span data-stu-id="8975f-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="8975f-166">Suppression d’un profil à partir d’un appareil ne supprime pas le profil de votre liste.</span><span class="sxs-lookup"><span data-stu-id="8975f-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="8975f-167">Si vous souhaitez supprimer un profil, suivez les instructions de [mise à jour ou supprimer un profil Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="8975f-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="8975f-168">Mettre à jour ou supprimer un profil Autopilot</span><span class="sxs-lookup"><span data-stu-id="8975f-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="8975f-169">Si un client souhaite modifier l’expérience out-of-box après avoir expédié les appareils pour les, vous pouvez modifier le profil dans le centre de partenaires.</span><span class="sxs-lookup"><span data-stu-id="8975f-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="8975f-170">Lorsque l’appareil de client se connecte à internet, elle télécharge la dernière version de profil au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="8975f-171">Également, lorsqu’un client restaure un appareil ses paramètres d’usine par défaut, l’appareil sera à nouveau télécharger la dernière version de profil au cours du processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="8975f-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="8975f-172">Sélectionnez **clients** dans le menu espace partenaires puis sélectionnez le client qui souhaite vous permettent de modifier un profil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="8975f-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="8975f-173">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8975f-174">Sous **profils Windows Autopilot** sélectionnez le profil que vous devez mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="8975f-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="8975f-175">Apportez les modifications requises, puis sélectionnez **envoyer**.</span><span class="sxs-lookup"><span data-stu-id="8975f-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="8975f-176">Pour supprimer ce profil, sélectionnez **supprimer le profil** à partir de l’angle supérieur droit de la page.</span><span class="sxs-lookup"><span data-stu-id="8975f-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="8975f-177">Ajouter des appareils à un compte client</span><span class="sxs-lookup"><span data-stu-id="8975f-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="8975f-178">Les agents client et administrateur peut ajouter des appareils sur un compte client.</span><span class="sxs-lookup"><span data-stu-id="8975f-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="8975f-179">Avant de pouvoir appliquer des profils Autopilot personnalisés pour des appareils clients, vous devez être en mesure d’accéder à la liste des appareils du client.</span><span class="sxs-lookup"><span data-stu-id="8975f-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="8975f-180">Si vous envisagez d’utiliser le nom OEM, le numéro de série et la combinaison de modèle, tenez compte des limitations suivantes :</span><span class="sxs-lookup"><span data-stu-id="8975f-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="8975f-181">Ce tuple s’applique uniquement aux appareils récents (4 k hachages, par exemple) et n’est pas prise en charge des hachages de 128 b (RS2 et périphériques préalables).</span><span class="sxs-lookup"><span data-stu-id="8975f-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="8975f-182">L’inscription de tuple respecte la casse, donc les données dans le fichier doivent correspondre aux noms de modèle et le fabricant ***exactement*** tel que fourni par le fournisseur OEM (fournisseur de matériel).</span><span class="sxs-lookup"><span data-stu-id="8975f-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="8975f-183">Suivez les instructions ci-dessous pour ajouter des appareils à un compte client dans le centre de partenaires.</span><span class="sxs-lookup"><span data-stu-id="8975f-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="8975f-184">Sélectionnez **clients** dans le menu espace partenaires puis sélectionnez le client dont vous souhaitez gérer les appareils.</span><span class="sxs-lookup"><span data-stu-id="8975f-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="8975f-185">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8975f-186">Sous **appliquer les profils aux appareils** sélectionnez **ajouter des appareils**.</span><span class="sxs-lookup"><span data-stu-id="8975f-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="8975f-187">Entrez un nom pour la liste des appareils, puis sélectionnez **Parcourir** pour charger la liste du client (au format de fichier .csv) pour les partenaires.</span><span class="sxs-lookup"><span data-stu-id="8975f-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8975f-188">Vous devez avoir reçu ce fichier .csv avec l’achat de votre appareil.</span><span class="sxs-lookup"><span data-stu-id="8975f-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="8975f-189">Si vous n’avez pas reçu d’un fichier .csv, vous pouvez créer un vous-même en suivant les étapes décrites dans [Ajout de périphériques pour Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="8975f-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="8975f-190">Téléchargez le fichier .csv, puis sélectionnez **enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="8975f-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="8975f-191">Si vous obtenez un message d’erreur lorsqu’il tente de charger le fichier .csv, vérifiez le format du fichier.</span><span class="sxs-lookup"><span data-stu-id="8975f-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="8975f-192">Vous pouvez utiliser le hachage matériel uniquement, ou le nom du fabricant OEM, numéro de série et model (dans cet ordre de colonne) ou l’ID de produit de Windows.</span><span class="sxs-lookup"><span data-stu-id="8975f-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="8975f-193">Vous pouvez également utiliser l’exemple de fichier .csv fourni à partir du lien suivant pour **ajouter des appareils** pour créer une liste des appareils.</span><span class="sxs-lookup"><span data-stu-id="8975f-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="8975f-194">Licenciement de Windows Autopilot CLUF</span><span class="sxs-lookup"><span data-stu-id="8975f-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="8975f-195">INFORMATIONS IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="8975f-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="8975f-196">Windows Autopilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients.</span><span class="sxs-lookup"><span data-stu-id="8975f-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="8975f-197">Si l’autorisation par le client, vous pouvez supprimer ou masquer certains écrans de configuration qui sont normalement présentées aux utilisateurs lorsque vous configurez Windows, y compris l’écran de l’acceptation du CLUF (contrat de licence utilisateur final).</span><span class="sxs-lookup"><span data-stu-id="8975f-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="8975f-198">À l’aide de cette fonction, vous acceptez de supprimer ou masquer tous les écrans sont conçus pour fournir aux utilisateurs avec notification ou l’acceptation de moyens de termes que vous avez obtenu suffisamment consentement et autorisation à partir de votre client pour masquer les termes du contrat et que vous, de la part de votre client (si une organisation ou un utilisateur individuel, le cas peut être), donner son consentement pour des notifications et accepter les termes qui sont applicables à votre client.</span><span class="sxs-lookup"><span data-stu-id="8975f-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="8975f-199">Cela inclut votre acceptation des termes et conditions de la licence ou de l'avis qui serait présenté à l'utilisateur si vous ne l'aviez pas supprimé(e) ni masqué(e) à l'aide de cet outil.</span><span class="sxs-lookup"><span data-stu-id="8975f-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="8975f-200">Votre client ne peut pas utiliser le logiciel Windows sur ces appareils s'il n'a pas légitimement acquis une licence pour le logiciel auprès de Microsoft ou de ses revendeurs.</span><span class="sxs-lookup"><span data-stu-id="8975f-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>