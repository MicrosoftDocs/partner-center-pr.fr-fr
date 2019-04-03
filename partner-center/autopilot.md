---
title: Personnaliser l’expérience d’out-of-box d’un appareil avec des profils Windows Autopilot | Partenaires
description: Préconfigurer l’expérience d’out-of-box d’un appareil avec des profils Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot autopilot de windows, autopilot de microsoft, zero touch, oobe, écrans de connexion, de déploiement out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162219"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personnaliser l’expérience d’out-of-box d’un appareil avec des profils Windows Autopilot

**S’applique à**

- Les partenaires CSP direct-facture, les fournisseurs indirects et les revendeurs indirects

Si vous gérez des appareils clients, vous devrez peut-être personnaliser l’expérience out-of-box (OOBE) pour les utilisateurs du client. Vous pouvez préconfigurer les nouveaux appareils avec des profils Windows Autopilot avant de distribuer les appareils sur les clients et appliquer de nouveaux profils sur des appareils clients ont déjà acheté. Cet article explique comment créer et appliquer des profils Autopilot sur les appareils de partenaires.

Si vous n’êtes pas déjà familiarisé avec Autopilot, passez en revue les informations contenues dans ces articles :

- [Vue d’ensemble de Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guide de référence de déploiement AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Vue d'ensemble

Avec la fonctionnalité Windows Autopilot dans Partner Center, vous pouvez créer des profils personnalisés à appliquer à des appareils clients. Les paramètres de profil suivants étaient disponibles au moment de la que publication de cet article :

- Ignorer les paramètres de confidentialité. Ce paramètre de profil Autopilot facultatif permet aux organisations de plus de paramètres de confidentialité pendant le processus OOBE.

- Désactiver la création du compte administrateur local sur l’appareil. Les organisations peuvent décider si l’utilisateur de la configuration de l’appareil doit avoir un accès administrateur une fois que le processus est terminé.

- Configurer automatiquement des appareils pour les professionnels ou scolaires. Tous les appareils inscrits avec Autopilot seront automatiquement considérée comme Professionnel ou scolaire d’appareils, donc cette question ne sera pas invitée au cours du processus OOBE.

- Ignorer les pages de configuration de l’inscription Cortana, OneDrive et OEM. Tous les appareils inscrits avec Autopilot ignorera automatiquement ces pages au cours du processus d’out-of-box experience (OOBE).

- Ignorer le contrat de licence utilisateur final (CLUF). À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page CLUF présentée au cours du processus OOBE. Consultez [licenciement de Windows Autopilot CLUF](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF pendant Windows le programme d’installation.

Les autorisations de gestion de profil et le périphérique et les limitations suivantes s’appliquent :

- Les partenaires CSP peuvent continuer à gérer des profils Autopilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé des privilèges d’administration déléguée du partenaire.

- Vous pouvez gérer des appareils existants à vos clients que vous avez ajoutés.

- Vous ne pouvez pas gérer les appareils de que votre client a téléchargé vers le Microsoft Store pour entreprises ou Microsoft Intune Portal.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Créer et gérer des profils Autopilot dans Partner Center

Dans Partner Center, vous pouvez créer des profils de déploiement Windows Autopilot et les appliquer aux appareils.

>[!NOTE]
>Seuls les agents d’administration peuvent créer et appliquer les profils.

### <a name="create-a-new-autopilot-profile"></a>Créer un nouveau profil Autopilot

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client que vous créez le profil Autopilot pour.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **profils Windows Autopilot** sélectionnez **Ajouter nouveau profil**.

4. Entrez le nom et la description du profil, puis configurez les paramètres OOBE. Choisissez parmi :  

   - Ignorer les paramètres de confidentialité dans le programme d’installation

   - Désactiver le compte d’administrateur local dans l'installation
  
   - Ignorer automatiquement des pages dans l'installation<br>
        (Inclut *sélectionner automatiquement le programme d’installation pour les professionnels ou scolaires* et *les pages de configuration de l’inscription Skip Cortana, OneDrive et OEM*)
  
   - Ignorer le contrat de licence utilisateur final (CLUF)<br> 
       >[!IMPORTANT] 
       >Consultez [licenciement de Windows Autopilot CLUF](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF pendant Windows le programme d’installation.

5. Sélectionnez **Envoyer** une fois terminé.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Appliquer un profil Autopilot à des appareils clients

>[!NOTE]
>Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client pour les partenaires et que vous pouvez accéder à leur liste des appareils. Si vous n’avez pas déjà ajouté les appareils du client, suivez les instructions de [ajouter des appareils à un compte client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.

Après avoir créé un profil Autopilot pour un client, vous pouvez l’appliquer aux appareils du client.

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client vous avez créé le profil Autopilot pour.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer les profils aux appareils** sélectionnez les périphériques ou les groupes de périphériques que vous souhaitez ajouter des profils à, puis sélectionnez **appliquer le profil**. Le profil que vous venez d’appliquer s’affiche dans le **profil** colonne.

4. Suivez les étapes ci-dessous pour vérifier que le profil est appliqué correctement à l’appareil.

    a.  Connecter un appareil au réseau et mettez-le sous tension.

    b.  Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.

    c.  Lorsque le processus OOBE s’arrête, réinitialiser l’appareil ses paramètres d’usine par défaut afin de le préparer pour un nouvel utilisateur.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Supprimer un profil Autopilot à partir de l’appareil d’un client

1. Sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client vous avez créé le profil Autopilot pour.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer les profils aux appareils** sélectionner les appareils que vous souhaitez supprimer le profil à partir de, puis sélectionnez **supprimer le profil**.

   >[!NOTE]
   >Suppression d’un profil à partir d’un appareil ne supprime pas le profil de votre liste. Si vous souhaitez supprimer un profil, suivez les instructions de [mise à jour ou supprimer un profil Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Mettre à jour ou supprimer un profil Autopilot

Si un client souhaite modifier l’expérience out-of-box après avoir expédié les appareils pour les, vous pouvez modifier le profil dans le centre de partenaires.

Lorsque l’appareil de client se connecte à internet, elle télécharge la dernière version de profil au cours du processus OOBE. Également, lorsqu’un client restaure un appareil ses paramètres d’usine par défaut, l’appareil sera à nouveau télécharger la dernière version de profil au cours du processus OOBE.

1. Sélectionnez **clients** dans le menu espace partenaires puis sélectionnez le client qui souhaite vous permettent de modifier un profil Autopilot.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **profils Windows Autopilot** sélectionnez le profil que vous devez mettre à jour. Apportez les modifications requises, puis sélectionnez **envoyer**.

Pour supprimer ce profil, sélectionnez **supprimer le profil** à partir de l’angle supérieur droit de la page.

### <a name="add-devices-to-a-customers-account"></a>Ajouter des appareils à un compte client

>[!NOTE]
>Les agents client et administrateur peut ajouter des appareils sur un compte client.

Avant de pouvoir appliquer des profils Autopilot personnalisés pour des appareils clients, vous devez être en mesure d’accéder à la liste des appareils du client.

Si vous envisagez d’utiliser le nom OEM, le numéro de série et la combinaison de modèle, tenez compte des limitations suivantes :

- Ce tuple s’applique uniquement aux appareils récents (4 k hachages, par exemple) et n’est pas prise en charge des hachages de 128 b (RS2 et périphériques préalables).

- L’inscription de tuple respecte la casse, donc les données dans le fichier doivent correspondre aux noms de modèle et le fabricant ***exactement*** tel que fourni par le fournisseur OEM (fournisseur de matériel).

Suivez les instructions ci-dessous pour ajouter des appareils à un compte client dans le centre de partenaires.

1. Sélectionnez **clients** dans le menu espace partenaires puis sélectionnez le client dont vous souhaitez gérer les appareils.

2. Sur la page de détails du client, sélectionnez **appareils**.

3. Sous **appliquer les profils aux appareils** sélectionnez **ajouter des appareils**.

4. Entrez un nom pour la liste des appareils, puis sélectionnez **Parcourir** pour charger la liste du client (au format de fichier .csv) pour les partenaires.

    >[!NOTE]
    >Vous devez avoir reçu ce fichier .csv avec l’achat de votre appareil. Si vous n’avez pas reçu d’un fichier .csv, vous pouvez créer un vous-même en suivant les étapes décrites dans [Ajout de périphériques pour Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Téléchargez le fichier .csv, puis sélectionnez **enregistrer**.

Si vous obtenez un message d’erreur lorsqu’il tente de charger le fichier .csv, vérifiez le format du fichier. Vous pouvez utiliser le hachage matériel uniquement, ou le nom du fabricant OEM, numéro de série et model (dans cet ordre de colonne) ou l’ID de produit de Windows. Vous pouvez également utiliser l’exemple de fichier .csv fourni à partir du lien suivant pour **ajouter des appareils** pour créer une liste des appareils.

## <a name="windows-autopilot-eula-dismissal"></a>Licenciement de Windows Autopilot CLUF

### <a name="important-information"></a>INFORMATIONS IMPORTANTES

Windows Autopilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients. Si l’autorisation par le client, vous pouvez supprimer ou masquer certains écrans de configuration qui sont normalement présentées aux utilisateurs lorsque vous configurez Windows, y compris l’écran de l’acceptation du CLUF (contrat de licence utilisateur final).

À l’aide de cette fonction, vous acceptez de supprimer ou masquer tous les écrans sont conçus pour fournir aux utilisateurs avec notification ou l’acceptation de moyens de termes que vous avez obtenu suffisamment consentement et autorisation à partir de votre client pour masquer les termes du contrat et que vous, de la part de votre client (si une organisation ou un utilisateur individuel, le cas peut être), donner son consentement pour des notifications et accepter les termes qui sont applicables à votre client. Cela inclut votre acceptation des termes et conditions de la licence ou de l'avis qui serait présenté à l'utilisateur si vous ne l'aviez pas supprimé(e) ni masqué(e) à l'aide de cet outil. Votre client ne peut pas utiliser le logiciel Windows sur ces appareils s'il n'a pas légitimement acquis une licence pour le logiciel auprès de Microsoft ou de ses revendeurs.