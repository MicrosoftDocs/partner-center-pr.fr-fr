---
title: Personnaliser les out-of-box d’un appareil avec des profils Windows Autopilot | L’espace partenaires
description: Préconfigurer expérience d’out-of-box d’un appareil avec des profils Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot windows, autopilot de microsoft, déploiement zero touch, oobe, écrans d’ouverture de session, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 46b8a74383585c630864079efa42b6e34412b91e
ms.sourcegitcommit: 80f3eb81f2e7605e77d19856827472f7830db419
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/22/2019
ms.locfileid: "9098826"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personnaliser les out-of-box d’un appareil avec des profils Windows Autopilot

**S'applique à:**

- Les partenaires de facture direct de fournisseur de solutions cloud, les fournisseurs indirects et les revendeurs indirects

Si vous gérez les appareils clients, vous devrez peut-être personnaliser l’expérience out-of-box (OOBE) pour les utilisateurs du client. Vous pouvez préconfigurer de nouveaux appareils avec des profils Windows Autopilot avant de distribuer les appareils à des clients et appliquer des profils à nouveau sur les appareils clients ont déjà acheté. Cet article explique comment créer et appliquer des profils Autopilot aux appareils dans l’espace partenaires.

Si vous n’êtes pas déjà familiarisé avec Autopilot, passez en revue les informations contenues dans les articles suivants:

- [Vue d’ensemble de Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guide de référence de déploiement AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Vue d'ensemble

Avec la fonctionnalité Windows Autopilot dans l’espace partenaires, vous pouvez créer des profils personnalisés à appliquer aux appareils du client. Les paramètres de profil suivants étaient disponibles lors de la publication de cet article:

- Ignorer les paramètres de confidentialité. Ce paramètre de profil Autopilot facultatif permet aux organisations de ne demander pas sur les paramètres de confidentialité au cours du processus OOBE.

- Désactiver la création du compte administrateur local sur l’appareil. Les organisations peuvent décider si l’utilisateur de configurer l’appareil doit avoir un accès administrateur une fois que le processus est terminé.

- Configurer automatiquement l’appareil professionnel ou scolaire. Tous les appareils enregistrés avec Autopilot seront automatiquement être considérée comme professionnelle ou à l’établissement d’appareils, afin que cette question ne sera pas demandée au cours du processus OOBE.

- Ignorez les pages de paramètres d’inscription Cortana, OneDrive et OEM. Tous les appareils enregistrés avec Autopilot ignore automatiquement ces pages au cours du processus d’out-of-box experience (OOBE).

- Ignorer le contrat de licence utilisateur final (CLUF). À compter de Windows 10 version 1709, les organisations peuvent décider d’ignorer la page CLUF présentée au cours du processus OOBE. Voir [abandon du CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF lors de l’installation de Windows.

Les autorisations de gestion de profil et le périphérique et les limitations suivantes s’appliquent:

- Les partenaires fournisseurs de solutions cloud peuvent continuer à gérer les profils Autopilot pour les clients existants avec lesquels ils ont des relations de revendeur, même si les clients ont supprimé les privilèges d’administration déléguées du partenaire.

- Vous pouvez gérer des appareils existants pour vos clients qui ont été ajoutés par vous ou par un autre partenaire fournisseur de solutions cloud.

- Vous ne pouvez pas gérer les appareils que votre client a téléchargés à Microsoft Store pour entreprises ou Microsoft Intune Portal.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Créer et gérer les profils Autopilot dans l’espace partenaires

Dans l’espace partenaires, vous pouvez créer des profils Windows Autopilot deployment et les appliquer aux appareils.

>[!NOTE]
>Seuls les agents peuvent créer et appliquer des profils.

### <a name="create-a-new-autopilot-profile"></a>Créez un nouveau profil Autopilot

1. Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous créez le profil Autopilot pour.

2. Sur la page des détails du client, sélectionnez **les appareils**.

3. Sous **profils Windows Autopilot** sélectionnez **Ajouter un nouveau profil**.

4. Entrez le nom et une description du profil, puis configurez les paramètres de la phase OOBE. Choisir parmi:  

   - Ignorer les paramètres de confidentialité dans le programme d’installation

   - Désactiver le compte d’administrateur local dans l'installation
  
   - Ignorer automatiquement des pages dans l'installation<br>
        (Inclut *Ignorer Cortana, OneDrive et OEM pages de paramètres d’inscription*et de *Sélectionner automatiquement le programme d’installation Professionnel ou scolaire* )
  
   - Ignorer le contrat de licence utilisateur final (CLUF)<br> 
       >[!IMPORTANT] 
       >Voir [abandon du CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) ci-dessous pour obtenir des informations importantes à prendre en compte sur le fait d’ignorer la page CLUF lors de l’installation de Windows.

5. Sélectionnez **Envoyer** une fois terminé.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Appliquer un profil Autopilot aux appareils du client

>[!NOTE]
>Les instructions ci-dessous supposent que vous avez déjà ajouté les appareils du client vers l’espace partenaires et que vous pouvez accéder à leur liste d’appareils. Si vous n’avez pas déjà ajouté les appareils du client, suivez les instructions de [périphériques d’ajouter à un compte client](#add-devices-to-a-customers-account) , puis suivez les étapes ci-dessous.

Après avoir créé un profil Autopilot pour un client, vous pouvez l’appliquer aux appareils du client.

1. Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous avez créé le profil Autopilot pour.

2. Sur la page des détails du client, sélectionnez **les appareils**.

3. Sous **profils appliquer aux appareils** sélectionner les périphériques ou les groupes de périphériques que vous souhaitez ajouter des profils, puis sélectionnez **Appliquer profil**. Le profil que vous venez d’appliquer s’affiche dans la colonne **profil** .

4. Suivez les étapes ci-dessous pour vérifier que le profil est appliqué correctement à l’appareil.

    a.  Connectez un appareil au réseau et mettez-le sous tension.

    b.  Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.

    c.  Lorsque le processus OOBE s’arrête, réinitialiser l’appareil ses paramètres d’usine par défaut pour préparer à un nouvel utilisateur.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Supprimer un profil Autopilot à partir de l’appareil d’un client

1. Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client que vous avez créé le profil Autopilot pour.

2. Sur la page des détails du client, sélectionnez **les appareils**.

3. Sous **profils appliquer aux appareils** sélectionnez les périphériques que vous souhaitez supprimer le profil, puis sélectionnez **Supprimer le profil**.

   >[!NOTE]
   >Supprimer un profil à partir d’un appareil ne supprime pas le profil de votre liste. Si vous souhaitez supprimer un profil, suivez les instructions de [mise à jour ou supprimer un profil Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Mettre à jour ou supprimer un profil Autopilot

Si un client souhaite modifier l’expérience out-of-box après avoir expédié les appareils sur ces derniers, vous pouvez modifier le profil dans l’espace partenaires.

Lorsque l’appareil du client se connecte à internet, il télécharge la dernière version de profil au cours du processus OOBE. En outre, n’importe quel moment qu'un client rétablit un appareil ses paramètres d’usine par défaut, l’appareil télécharge à nouveau la dernière version de profil au cours du processus OOBE.

1. Sélectionnez **clients** à partir du menu de l’espace partenaires, puis sélectionnez le client qui souhaite vous permettent de modifier un profil Autopilot.

2. Sur la page des détails du client, sélectionnez **les appareils**.

3. Sous **profils Windows Autopilot** , sélectionnez le profil, que vous devez mettre à jour. Apportez les modifications requises, puis sélectionnez **Envoyer**.

Pour supprimer ce profil, sélectionnez **Supprimer le profil** à partir de l’angle supérieur droit de la page.

### <a name="add-devices-to-a-customers-account"></a>Ajouter des appareils au compte d’un client

>[!NOTE]
>Les agents commerciaux et administrateurs peuvent ajouter des appareils au compte d’un client.

Avant d’appliquer des profils Autopilot personnalisés pour les appareils clients, vous devez être en mesure d’accéder à la liste d’appareil du client.

Si vous prévoyez d’utiliser le nom OEM, le numéro de série et combinaison de modèle, n’oubliez pas de ces limitations:

- Cela convient tuple uniquement pour les appareils plus récents (4 k hachages, par exemple) et n’est pas prise en charge des hachages de 128 b (RS2 et périphériques préalables).

- L’inscription tuple respecte la casse, afin que les données dans le fichier doivent correspondre le modèle et le fabricant noms ***exactement*** comme fournie par le fournisseur OEM (fournisseur matériel).

Suivez les instructions ci-dessous pour ajouter des appareils au compte d’un client dans l’espace partenaires.

1. Sélectionnez des **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les appareils.

2. Sur la page des détails du client, sélectionnez **les appareils**.

3. Sous **profils appliquer aux appareils** sélectionnez **Ajouter les appareils**.

4. Entrez un nom pour la liste des périphériques, puis **accédez** à charger la liste du client (au format de fichier .csv) dans l’espace partenaires.

    >[!NOTE]
    >Vous devez avoir reçu ce fichier .csv avec votre achat d’appareil. Si vous n’avez pas recevoir un fichier .csv, vous pouvez créer une vous-même en suivant les étapes décrites dans les [périphériques d’ajout de Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Télécharger le fichier .csv, puis sélectionnez **Enregistrer**.

Si vous obtenez un message d’erreur en essayant de charger le fichier .csv, vérifiez le format du fichier. Vous pouvez utiliser le code de hachage matériel uniquement, ou le nom OEM, le numéro de série et modèle (dans cet ordre de colonnes) ou l’ID de produit Windows. Vous pouvez également utiliser l’exemple de fichier .csv fourni à partir du lien en regard de **périphériques ajouter** pour créer une liste d’appareils.

## <a name="windows-autopilot-eula-dismissal"></a>Abandon du CLUF de Windows Autopilot

### <a name="important-information"></a>INFORMATIONS IMPORTANTES

Windows Autopilot vous permet de configurer des installations personnalisées de Windows sur les appareils que vous gérez pour vos clients. Si vous êtes autorisé à le faire par le client, vous pouvez supprimer ou de masquer certains écrans d’installation qui sont normalement présentés aux utilisateurs lors de la configuration de Windows, y compris l’écran d’acceptation du CLUF (contrat de licence utilisateur final).

À l’aide de cette fonction, vous convenez qu’en supprimant ou en masquant les écrans sont conçus pour fournir aux utilisateurs des avis ou l’acceptation des moyens de termes que vous avez obtenu les consentement suffisant et autorisation à partir de votre client pour masquer les termes du contrat et que vous avez, pour le compte de votre client (indique si une organisation ou un utilisateur individuel en tant que celle-ci peut être), consentez à n’importe quel avis et acceptez les conditions applicables à votre client. Cela inclut votre acceptation des termes et conditions de la licence ou de l'avis qui serait présenté à l'utilisateur si vous ne l'aviez pas supprimé(e) ni masqué(e) à l'aide de cet outil. Votre client ne peut pas utiliser le logiciel Windows sur ces appareils s'il n'a pas légitimement acquis une licence pour le logiciel auprès de Microsoft ou de ses revendeurs.