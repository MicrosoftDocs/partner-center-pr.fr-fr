---
title: Personnaliser l’expérience utilisateur prête à l’emploi d’un appareil
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Avant de diffuser le nouvel appareil d’un client, vous pouvez utiliser les profils Windows AutoPilot pour personnaliser ou préconfigurer l’expérience OOBE (out-of-Box Experience) de l’appareil.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a59b0c25b8f5203942e73b549d5ffb9d65d90c36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527655"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="23401-103">Utiliser les profils Windows AutoPilot sur de nouveaux appareils pour personnaliser l’expérience out-of-Box d’un client</span><span class="sxs-lookup"><span data-stu-id="23401-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="23401-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="23401-104">**Applies to**</span></span>

- <span data-ttu-id="23401-105">Fournisseurs de services de chiffrement direct-partenaires, fournisseurs indirects et revendeurs indirects</span><span class="sxs-lookup"><span data-stu-id="23401-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="23401-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="23401-106">**Appropriate roles**</span></span>

- <span data-ttu-id="23401-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="23401-107">Admin agent</span></span>
- <span data-ttu-id="23401-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="23401-108">Global admin</span></span>
- <span data-ttu-id="23401-109">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="23401-109">Sales agent</span></span>
- <span data-ttu-id="23401-110">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="23401-110">User management admin</span></span>

<span data-ttu-id="23401-111">Si vous gérez des appareils clients, vous devrez peut-être personnaliser l’OOBE (out-of-Box Experience) pour les utilisateurs du client.</span><span class="sxs-lookup"><span data-stu-id="23401-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="23401-112">Vous pouvez préconfigurer de nouveaux appareils avec des profils Windows AutoPilot avant de transmettre les appareils aux clients et appliquer de nouveaux profils aux appareils que les clients ont déjà achetés.</span><span class="sxs-lookup"><span data-stu-id="23401-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="23401-113">Notez que les fabricants d’ordinateurs OEM ont commencé à inclure une étiquette d’expédition à l’extérieur de la zone de l’appareil AutoPilot qui affiche l' **ID de clé de produit (pkid)** de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="23401-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="23401-114">Ce code-barres unidimensionnel et lisible offre aux partenaires en aval un moyen d’inscrire des appareils pour AutoPilot sans avoir à effectuer une unboxing sur le ou les appareils et à collecter l’ID de l’appareil par d’autres moyens.</span><span class="sxs-lookup"><span data-stu-id="23401-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="23401-115">Cet article explique comment créer et appliquer des profils AutoPilot à des appareils dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="23401-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="23401-116">Si vous n’êtes pas déjà familiarisé avec AutoPilot, passez en revue les informations contenues dans les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="23401-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="23401-117">Vue d’ensemble de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="23401-117">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="23401-118">Guide de référence du déploiement AutoPilot</span><span class="sxs-lookup"><span data-stu-id="23401-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="23401-119">Vue d’ensemble</span><span class="sxs-lookup"><span data-stu-id="23401-119">Overview</span></span>

<span data-ttu-id="23401-120">Avec la fonctionnalité Windows AutoPilot de l’espace partenaires, vous pouvez créer des profils personnalisés à appliquer aux appareils clients.</span><span class="sxs-lookup"><span data-stu-id="23401-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="23401-121">Les paramètres de profil suivants étaient disponibles au moment de la publication de cet article :</span><span class="sxs-lookup"><span data-stu-id="23401-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="23401-122">Ignorer les paramètres de confidentialité.</span><span class="sxs-lookup"><span data-stu-id="23401-122">Skip privacy settings.</span></span> <span data-ttu-id="23401-123">Ce paramètre de profil AutoPilot facultatif permet aux organisations de ne pas poser de questions sur les paramètres de confidentialité pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="23401-124">Désactivez la création de compte administrateur local sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="23401-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="23401-125">Les organisations peuvent décider si l’utilisateur qui configure l’appareil doit disposer d’un accès administrateur une fois le processus terminé.</span><span class="sxs-lookup"><span data-stu-id="23401-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="23401-126">Configurer automatiquement l’appareil pour l’entreprise ou l’école.</span><span class="sxs-lookup"><span data-stu-id="23401-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="23401-127">Tous les appareils inscrits avec AutoPilot seront automatiquement considérés comme des appareils professionnels ou scolaires. cette question ne sera donc pas demandée pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="23401-128">Ignorez les pages de configuration d’inscription Cortana, OneDrive et OEM.</span><span class="sxs-lookup"><span data-stu-id="23401-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="23401-129">Tous les appareils inscrits avec AutoPilot ignorent automatiquement ces pages pendant le processus OOBE (out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="23401-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="23401-130">Ignorer le contrat de licence utilisateur final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="23401-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="23401-131">À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page du CLUF présentée pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="23401-132">Pour obtenir des informations importantes sur l’ignorance de la page du CLUF lors de l’installation de Windows, consultez [CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="23401-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="23401-133">Les autorisations et limitations de gestion des périphériques et des profils suivantes s’appliquent :</span><span class="sxs-lookup"><span data-stu-id="23401-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="23401-134">Les partenaires CSP peuvent continuer à gérer les profils AutoPilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé les privilèges d’administration déléguée du partenaire.</span><span class="sxs-lookup"><span data-stu-id="23401-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="23401-135">Vous pouvez gérer les appareils existants pour vos clients que vous avez ajoutés.</span><span class="sxs-lookup"><span data-stu-id="23401-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="23401-136">Vous ne pouvez pas gérer les appareils que votre client a téléchargés vers Microsoft Store for Business ou le portail Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="23401-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="23401-137">Créer et gérer des profils AutoPilot dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="23401-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="23401-138">Dans l’espace partenaires, vous pouvez créer des profils de déploiement Windows AutoPilot et les appliquer aux appareils.</span><span class="sxs-lookup"><span data-stu-id="23401-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="23401-139">Seuls les agents d’administration peuvent créer et appliquer des profils.</span><span class="sxs-lookup"><span data-stu-id="23401-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="23401-140">Créer un nouveau profil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="23401-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="23401-141">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous créez le profil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="23401-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="23401-142">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-142">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="23401-143">Sous **profils Windows AutoPilot** , sélectionnez **Ajouter un nouveau profil**.</span><span class="sxs-lookup"><span data-stu-id="23401-143">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="23401-144">Entrez le nom et la description du profil, puis configurez les paramètres OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="23401-145">Choisissez parmi :</span><span class="sxs-lookup"><span data-stu-id="23401-145">Choose from:</span></span>  

   - <span data-ttu-id="23401-146">Ignorer les paramètres de confidentialité dans le programme d’installation</span><span class="sxs-lookup"><span data-stu-id="23401-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="23401-147">Désactiver le compte administrateur local dans le programme d’installation</span><span class="sxs-lookup"><span data-stu-id="23401-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="23401-148">Ignorer automatiquement les pages dans le programme d’installation</span><span class="sxs-lookup"><span data-stu-id="23401-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="23401-149">(Comprend la *sélection automatique de la configuration pour le travail ou l’école* et *l’omission des pages de configuration d’inscription Cortana, OneDrive et OEM*)</span><span class="sxs-lookup"><span data-stu-id="23401-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="23401-150">Ignorer le contrat de licence utilisateur final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="23401-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="23401-151">Pour obtenir des informations importantes sur l’ignorance de la page du CLUF lors de l’installation de Windows, consultez [CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="23401-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="23401-152">Sélectionnez **Envoyer** lorsque vous avez terminé.</span><span class="sxs-lookup"><span data-stu-id="23401-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="23401-153">Appliquer un profil AutoPilot à des appareils clients</span><span class="sxs-lookup"><span data-stu-id="23401-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="23401-154">Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client à l’espace partenaires et que vous pouvez accéder à leur liste d’appareils.</span><span class="sxs-lookup"><span data-stu-id="23401-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="23401-155">Si vous n’avez pas encore ajouté les appareils du client, suivez les instructions de la section [Ajouter des appareils au compte d’un client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="23401-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="23401-156">Une fois que vous avez créé un profil AutoPilot pour un client, vous pouvez l’appliquer aux appareils du client.</span><span class="sxs-lookup"><span data-stu-id="23401-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="23401-157">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous avez créé le profil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="23401-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="23401-158">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-158">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="23401-159">Sous **appliquer des profils aux appareils** , sélectionnez les appareils ou les groupes d’appareils auxquels vous souhaitez ajouter des profils, puis sélectionnez **appliquer le profil**.</span><span class="sxs-lookup"><span data-stu-id="23401-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="23401-160">Le profil que vous venez d’appliquer apparaît dans la colonne **Profil** .</span><span class="sxs-lookup"><span data-stu-id="23401-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="23401-161">Suivez les étapes ci-dessous pour vérifier que le profil sera appliqué correctement à l’appareil.</span><span class="sxs-lookup"><span data-stu-id="23401-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="23401-162">a.</span><span class="sxs-lookup"><span data-stu-id="23401-162">a.</span></span>  <span data-ttu-id="23401-163">Connectez un appareil au réseau et activez-le.</span><span class="sxs-lookup"><span data-stu-id="23401-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="23401-164">b.</span><span class="sxs-lookup"><span data-stu-id="23401-164">b.</span></span>  <span data-ttu-id="23401-165">Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.</span><span class="sxs-lookup"><span data-stu-id="23401-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="23401-166">c.</span><span class="sxs-lookup"><span data-stu-id="23401-166">c.</span></span>  <span data-ttu-id="23401-167">Lorsque le processus OOBE s’arrête, rétablissez les paramètres d’usine de l’appareil pour le préparer pour un nouvel utilisateur.</span><span class="sxs-lookup"><span data-stu-id="23401-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="23401-168">Supprimer un profil AutoPilot de l’appareil d’un client</span><span class="sxs-lookup"><span data-stu-id="23401-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="23401-169">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous avez créé le profil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="23401-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="23401-170">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-170">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="23401-171">Sous **appliquer les profils aux appareils** , sélectionnez les appareils à partir desquels vous souhaitez supprimer le profil, puis sélectionnez **supprimer le profil**.</span><span class="sxs-lookup"><span data-stu-id="23401-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="23401-172">La suppression d’un profil d’un appareil ne supprime pas le profil de votre liste.</span><span class="sxs-lookup"><span data-stu-id="23401-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="23401-173">Si vous souhaitez supprimer un profil, suivez les instructions de la procédure de [mise à jour ou de suppression d’un profil AutoPilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="23401-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="23401-174">Mettre à jour ou supprimer un profil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="23401-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="23401-175">Si un client souhaite modifier l’expérience sans assistance après l’envoi des appareils à ces derniers, vous pouvez modifier le profil dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="23401-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="23401-176">Lorsque l’appareil du client se connecte à Internet, il télécharge la dernière version de profil pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="23401-177">En outre, chaque fois qu’un client restaure les paramètres d’usine d’un appareil, celui-ci télécharge à nouveau la dernière version de profil pendant le processus OOBE.</span><span class="sxs-lookup"><span data-stu-id="23401-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="23401-178">Sélectionnez **clients** dans le menu de l’espace partenaires, puis sélectionnez le client qui veut que vous modifiiez un profil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="23401-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="23401-179">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-179">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="23401-180">Sous **profils Windows AutoPilot** , sélectionnez le profil que vous devez mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="23401-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="23401-181">Apportez les modifications requises, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="23401-181">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="23401-182">Pour supprimer ce profil, sélectionnez **supprimer le profil** dans l’angle supérieur droit de la page.</span><span class="sxs-lookup"><span data-stu-id="23401-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="23401-183">Ajouter des appareils au compte d’un client</span><span class="sxs-lookup"><span data-stu-id="23401-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="23401-184">Les agents commerciaux et les agents d’administration peuvent ajouter des appareils au compte d’un client.</span><span class="sxs-lookup"><span data-stu-id="23401-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="23401-185">Avant de pouvoir appliquer des profils AutoPilot personnalisés à des appareils clients, vous devez être en mesure d’accéder à la liste des appareils du client.</span><span class="sxs-lookup"><span data-stu-id="23401-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="23401-186">Si vous envisagez d’utiliser le nom OEM, le numéro de série et la combinaison de modèles, tenez compte des limitations suivantes :</span><span class="sxs-lookup"><span data-stu-id="23401-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="23401-187">Ce tuple fonctionne uniquement pour les appareils plus récents (par exemple, les hachages de 4 Ko) et n’est pas pris en charge pour les hachages 128b (RS2 et les appareils précédents).</span><span class="sxs-lookup"><span data-stu-id="23401-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="23401-188">L’inscription de tuple est sensible à la casse, donc les données du fichier doivent correspondre aux noms de modèle et de fabricant ***exactement*** tels qu’ils sont fournis par le fournisseur OEM (fournisseur de matériel).</span><span class="sxs-lookup"><span data-stu-id="23401-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="23401-189">Suivez les instructions ci-dessous pour ajouter des appareils au compte d’un client dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="23401-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="23401-190">Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les appareils.</span><span class="sxs-lookup"><span data-stu-id="23401-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="23401-191">Sur la page de détails du client, sélectionnez **appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-191">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="23401-192">Sous **appliquer des profils aux appareils** , sélectionnez **Ajouter des appareils**.</span><span class="sxs-lookup"><span data-stu-id="23401-192">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="23401-193">Entrez un nom pour la liste des appareils, puis sélectionnez **Parcourir** pour télécharger la liste du client (au format de fichier. csv) vers l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="23401-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="23401-194">Vous devez avoir reçu ce fichier. csv avec votre achat d’appareil.</span><span class="sxs-lookup"><span data-stu-id="23401-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="23401-195">Si vous n’avez pas reçu de fichier. csv, vous pouvez en créer un vous-même en suivant les étapes décrites dans [Ajout d’appareils à Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="23401-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="23401-196">Téléchargez le fichier. csv, puis sélectionnez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="23401-196">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="23401-197">Si vous recevez un message d’erreur lors de la tentative de téléchargement du fichier. csv, vérifiez le format du fichier.</span><span class="sxs-lookup"><span data-stu-id="23401-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="23401-198">Vous pouvez utiliser le hachage matériel uniquement ou le nom OEM, le numéro de série et le modèle (dans cet ordre de colonne) ou l’ID de produit Windows.</span><span class="sxs-lookup"><span data-stu-id="23401-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="23401-199">Vous pouvez également utiliser le fichier Sample. csv fourni à partir du lien situé en regard de **Ajouter des appareils** pour créer une liste d’appareils.</span><span class="sxs-lookup"><span data-stu-id="23401-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="23401-200">Votre fichier. csv devrait ressembler à ceci :</span><span class="sxs-lookup"><span data-stu-id="23401-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="23401-201">**Numéro de série de l’appareil, ID de produit Windows, hachage matériel, nom de fabricant, modèle d’appareil**</span><span class="sxs-lookup"><span data-stu-id="23401-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="23401-202">**{serialNumber},,, Microsoft Corporation, portable surface**</span><span class="sxs-lookup"><span data-stu-id="23401-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="23401-203">« Manufacturer Name » et « Device Model » respectent la casse.</span><span class="sxs-lookup"><span data-stu-id="23401-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="23401-204">Si vous ne savez pas quelle valeur placer pour le nom du fabricant et le modèle de l’appareil, vous pouvez l’exécuter sur l’appareil pour recueillir les valeurs correctes :</span><span class="sxs-lookup"><span data-stu-id="23401-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="23401-205">CLUF de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="23401-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="23401-206">INFORMATIONS IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="23401-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="23401-207">Windows AutoPilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients.</span><span class="sxs-lookup"><span data-stu-id="23401-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="23401-208">Si le client vous y autorise, vous pouvez supprimer ou masquer certains écrans de configuration qui sont normalement présentés aux utilisateurs lors de la configuration de Windows, y compris l’écran d’acceptation du contrat de licence utilisateur final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="23401-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="23401-209">À l’aide de cette fonction, vous acceptez que la suppression ou le masquage de tous les écrans destinés à fournir des avis ou à l’acceptation des conditions d’utilisation signifie que vous avez obtenu un consentement et une autorisation suffisants de la part de votre client pour masquer les conditions et que, pour le compte de votre client (qu’il s’agisse d’une organisation ou d’un utilisateur individuel), acceptez les avis et acceptez les termes applicables</span><span class="sxs-lookup"><span data-stu-id="23401-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="23401-210">Cela comprend l’accord aux termes et conditions de la licence ou à la notification qui est présentée à l’utilisateur si vous ne l’avez pas supprimé ou masqué à l’aide de cet outil.</span><span class="sxs-lookup"><span data-stu-id="23401-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="23401-211">Votre client peut ne pas utiliser le logiciel Windows sur ces appareils si le client n’a pas acquis une licence pour le logiciel auprès de Microsoft ou de ses distributeurs sous licence.</span><span class="sxs-lookup"><span data-stu-id="23401-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
