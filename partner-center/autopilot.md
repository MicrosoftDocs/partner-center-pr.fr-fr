---
title: Personnaliser l’expérience utilisateur prête à l’emploi d’un appareil avec les profils Windows AutoPilot | Espace partenaires
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment personnaliser ou préconfigurer une nouvelle expérience d’appareil prête à l’emploi avec des profils AutoPilot avant de livrer l’appareil au client.
author: LauraBrenner
ms.author: labrenne
keywords: Autopilot, Windows AutoPilot, Microsoft AutoPilot, déploiement Zero Touch, OOBE, écrans de connexion, prêts à l’emploi
ms.localizationpriority: medium
ms.openlocfilehash: 7fed49f9fd06be8765e3435862e3bee48b717ce7
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798607"
---
# <a name="customize-the-out-of-box-experience-for-a-device-with-windows-autopilot-profiles"></a>Personnaliser l’expérience out-of-Box pour un appareil avec des profils Windows AutoPilot

**S’applique à**

- Fournisseurs de services de chiffrement direct-partenaires, fournisseurs indirects et revendeurs indirects

**Rôles appropriés**

- Agent d’administration
- Administrateur général
- Agent commercial
- Administrateur de la gestion des utilisateurs

Si vous gérez des appareils clients, vous devrez peut-être personnaliser l’OOBE (out-of-Box Experience) pour les utilisateurs du client. Vous pouvez préconfigurer de nouveaux appareils avec des profils Windows AutoPilot avant de transmettre les appareils aux clients et appliquer de nouveaux profils aux appareils que les clients ont déjà achetés. 

Notez que les fabricants d’ordinateurs OEM ont commencé à inclure une étiquette d’expédition à l’extérieur de la zone de l’appareil AutoPilot qui affiche l' **ID de clé de produit (pkid)** de l’appareil.  Ce code-barres unidimensionnel et lisible offre aux partenaires en aval un moyen d’inscrire des appareils pour AutoPilot sans avoir à effectuer une unboxing sur le ou les appareils et à collecter l’ID de l’appareil par d’autres moyens.

Cet article explique comment créer et appliquer des profils AutoPilot à des appareils dans l’espace partenaires.

Si vous n’êtes pas déjà familiarisé avec AutoPilot, passez en revue les informations contenues dans les articles suivants :

- [Vue d’ensemble de Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guide de référence du déploiement AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Vue d’ensemble

Avec la fonctionnalité Windows AutoPilot de l’espace partenaires, vous pouvez créer des profils personnalisés à appliquer aux appareils clients. Les paramètres de profil suivants étaient disponibles au moment de la publication de cet article :

- Ignorer les paramètres de confidentialité. Ce paramètre de profil AutoPilot facultatif permet aux organisations de ne pas poser de questions sur les paramètres de confidentialité pendant le processus OOBE.

- Désactivez la création de compte administrateur local sur l’appareil. Les organisations peuvent décider si l’utilisateur qui configure l’appareil doit disposer d’un accès administrateur une fois le processus terminé.

- Configurer automatiquement l’appareil pour l’entreprise ou l’école. Tous les appareils inscrits avec AutoPilot seront automatiquement considérés comme des appareils professionnels ou scolaires. cette question ne sera donc pas demandée pendant le processus OOBE.

- Ignorez les pages de configuration d’inscription Cortana, OneDrive et OEM. Tous les appareils inscrits avec AutoPilot ignorent automatiquement ces pages pendant le processus OOBE (out-of-Box Experience).

- Ignorer le contrat de licence utilisateur final (CLUF). À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page du CLUF présentée pendant le processus OOBE. Pour obtenir des informations importantes sur l’ignorance de la page du CLUF lors de l’installation de Windows, consultez [CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) ci-dessous.

Les autorisations et limitations de gestion des périphériques et des profils suivantes s’appliquent :

- Les partenaires CSP peuvent continuer à gérer les profils AutoPilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé les privilèges d’administration déléguée du partenaire.

- Vous pouvez gérer les appareils existants pour vos clients que vous avez ajoutés.

- Vous ne pouvez pas gérer les appareils que votre client a téléchargés vers Microsoft Store for Business ou le portail Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Créer et gérer des profils AutoPilot dans l’espace partenaires

Dans l’espace partenaires, vous pouvez créer des profils de déploiement Windows AutoPilot et les appliquer aux appareils.

>[!NOTE]
>Seuls les agents d’administration peuvent créer et appliquer des profils.

### <a name="create-a-new-autopilot-profile"></a>Créer un nouveau profil AutoPilot

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous créez le profil AutoPilot.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **profils Windows AutoPilot** , sélectionnez **Ajouter un nouveau profil**.

4. Entrez le nom et la description du profil, puis configurez les paramètres OOBE. Choisissez parmi :  

   - Ignorer les paramètres de confidentialité dans le programme d’installation

   - Désactiver le compte administrateur local dans le programme d’installation
  
   - Ignorer automatiquement les pages dans le programme d’installation<br>
        (Comprend la *sélection automatique de la configuration pour le travail ou l’école* et *l’omission des pages de configuration d’inscription Cortana, OneDrive et OEM*)
  
   - Ignorer le contrat de licence utilisateur final (CLUF)<br> 
       >[!IMPORTANT] 
       >Pour obtenir des informations importantes sur l’ignorance de la page du CLUF lors de l’installation de Windows, consultez [CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) ci-dessous.

5. Sélectionnez **Envoyer** lorsque vous avez terminé.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Appliquer un profil AutoPilot à des appareils clients

>[!NOTE]
>Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client à l’espace partenaires et que vous pouvez accéder à leur liste d’appareils. Si vous n’avez pas encore ajouté les appareils du client, suivez les instructions de la section [Ajouter des appareils au compte d’un client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.

Une fois que vous avez créé un profil AutoPilot pour un client, vous pouvez l’appliquer aux appareils du client.

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous avez créé le profil AutoPilot.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer des profils aux appareils** , sélectionnez les appareils ou les groupes d’appareils auxquels vous souhaitez ajouter des profils, puis sélectionnez **appliquer le profil**. Le profil que vous venez d’appliquer apparaît dans la colonne **Profil** .

4. Suivez les étapes ci-dessous pour vérifier que le profil sera appliqué correctement à l’appareil.

    a.  Connectez un appareil au réseau et activez-le.

    b.  Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.

    c.  Lorsque le processus OOBE s’arrête, rétablissez les paramètres d’usine de l’appareil pour le préparer pour un nouvel utilisateur.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Supprimer un profil AutoPilot de l’appareil d’un client

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client pour lequel vous avez créé le profil AutoPilot.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer les profils aux appareils** , sélectionnez les appareils à partir desquels vous souhaitez supprimer le profil, puis sélectionnez **supprimer le profil**.

   >[!NOTE]
   >La suppression d’un profil d’un appareil ne supprime pas le profil de votre liste. Si vous souhaitez supprimer un profil, suivez les instructions de la procédure de [mise à jour ou de suppression d’un profil AutoPilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Mettre à jour ou supprimer un profil AutoPilot

Si un client souhaite modifier l’expérience sans assistance après l’envoi des appareils à ces derniers, vous pouvez modifier le profil dans l’espace partenaires.

Lorsque l’appareil du client se connecte à Internet, il télécharge la dernière version de profil pendant le processus OOBE. En outre, chaque fois qu’un client restaure les paramètres d’usine d’un appareil, celui-ci télécharge à nouveau la dernière version de profil pendant le processus OOBE.

1. Sélectionnez **clients** dans le menu de l’espace partenaires, puis sélectionnez le client qui veut que vous modifiiez un profil AutoPilot.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **profils Windows AutoPilot** , sélectionnez le profil que vous devez mettre à jour. Apportez les modifications requises, puis sélectionnez **Envoyer**.

Pour supprimer ce profil, sélectionnez **supprimer le profil** dans l’angle supérieur droit de la page.

### <a name="add-devices-to-a-customers-account"></a>Ajouter des appareils au compte d’un client

>[!NOTE]
>Les agents commerciaux et les agents d’administration peuvent ajouter des appareils au compte d’un client.

Avant de pouvoir appliquer des profils AutoPilot personnalisés à des appareils clients, vous devez être en mesure d’accéder à la liste des appareils du client.

Si vous envisagez d’utiliser le nom OEM, le numéro de série et la combinaison de modèles, tenez compte des limitations suivantes :

- Ce tuple fonctionne uniquement pour les appareils plus récents (par exemple, les hachages de 4 Ko) et n’est pas pris en charge pour les hachages 128b (RS2 et les appareils précédents).

- L’inscription de tuple est sensible à la casse, donc les données du fichier doivent correspondre aux noms de modèle et de fabricant ***exactement*** tels qu’ils sont fournis par le fournisseur OEM (fournisseur de matériel).

Suivez les instructions ci-dessous pour ajouter des appareils au compte d’un client dans l’espace partenaires.

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les appareils.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer des profils aux appareils** , sélectionnez **Ajouter des appareils**.

4. Entrez un nom pour la liste des appareils, puis sélectionnez **Parcourir** pour télécharger la liste du client (au format de fichier. csv) vers l’espace partenaires.

    >[!NOTE]
    >Vous devez avoir reçu ce fichier. csv avec votre achat d’appareil. Si vous n’avez pas reçu de fichier. csv, vous pouvez en créer un vous-même en suivant les étapes décrites dans [Ajout d’appareils à Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Téléchargez le fichier. csv, puis sélectionnez **Enregistrer**.

Si vous recevez un message d’erreur lors de la tentative de téléchargement du fichier. csv, vérifiez le format du fichier. Vous pouvez utiliser le hachage matériel uniquement ou le nom OEM, le numéro de série et le modèle (dans cet ordre de colonne) ou l’ID de produit Windows. Vous pouvez également utiliser le fichier Sample. csv fourni à partir du lien situé en regard de **Ajouter des appareils** pour créer une liste d’appareils.

Votre fichier. csv devrait ressembler à ceci :

> **Numéro de série de l’appareil, ID de produit Windows, hachage matériel, nom de fabricant, modèle d’appareil**

> **{serialNumber},,, Microsoft Corporation, portable surface**

Notez que « nom du fabricant » et « modèle d’appareil » respectent la casse.

Si vous ne savez pas quelle valeur placer pour le nom du fabricant et le modèle de l’appareil, vous pouvez l’exécuter sur l’appareil pour recueillir les valeurs correctes :

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>CLUF de Windows AutoPilot

### <a name="important-information"></a>INFORMATIONS IMPORTANTES

Windows AutoPilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients. Si le client vous y autorise, vous pouvez supprimer ou masquer certains écrans de configuration qui sont normalement présentés aux utilisateurs lors de la configuration de Windows, y compris l’écran d’acceptation du contrat de licence utilisateur final (CLUF).

À l’aide de cette fonction, vous acceptez que la suppression ou le masquage de tous les écrans destinés à fournir des avis ou à l’acceptation des conditions d’utilisation signifie que vous avez obtenu un consentement et une autorisation suffisants de la part de votre client pour masquer les conditions et que, pour le compte de votre client (qu’il s’agisse d’une organisation ou d’un utilisateur individuel), acceptez les avis et acceptez les termes applicables Cela comprend l’accord aux termes et conditions de la licence ou à la notification qui est présentée à l’utilisateur si vous ne l’avez pas supprimé ou masqué à l’aide de cet outil. Votre client peut ne pas utiliser le logiciel Windows sur ces appareils si le client n’a pas acquis une licence pour le logiciel auprès de Microsoft ou de ses distributeurs sous licence.
