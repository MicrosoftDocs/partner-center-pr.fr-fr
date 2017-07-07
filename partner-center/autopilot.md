---
title: "Simplifier l’installation des appareils avec WindowsAutoPilot | Espace partenaires"
description: "Ajouter un profil de déploiement WindowsAutoPilot dans l’Espace partenaires pour simplifier l’installation d’appareils avec WindowsAutoPilot"
author: KPacquer
keywords: "autopilot, windows autopilot, microsoft autopilot, déploiement zero touch, oobe, écrans d’ouverture de session"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: aa650ee5f2848694fe44d4751d52f8014e0d22a8
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Simplifier l’installation d’appareils avec WindowsAutoPilot 

WindowsAutoPilot simplifie et sécurise l’installation de nouveaux appareils Windows10Professionnel dès le premier démarrage, en quelques étapes seulement. Pour plus d’informations, voir [Présentation de WindowsAutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Fonctionnalités

*  **Désactiver les autorisations d’administrateur local** pour les utilisateurs finaux qui configurent des appareils
*  **Afficher la page de connexion d’une organisation**. L’organisation peut prédéfinir une page de connexion qui ajoute l’appareil en tant qu’appareil professionnel et le joint à Azure ActiveDirectory.
*  **Inscrire l’appareil dans un gestionnaire de périphériques mobiles (GPM)** tel que MicrosoftIntune, une fois la phaseOOBE terminée.
*  **Simplifier la phaseOOBE (Out-Of-Box Experience)** pour utiliser uniquement les étapes et les décisions nécessaires, à l’aide d’un profil de déploiement WindowsAutoPilot. 

## <a name="requirements"></a>Exigences

*  Appareils préinstallés avec Windows10 Professionnel Creators Update (1703 ou version ultérieure)
*  Identificateur d'appareil appelé code de hachage matériel (128 HWH ou 4k HWH), généralement fourni par un fabricant d'ordinateurs OEM. Vous utiliserez des identificateurs pour affecter des profils d’organisation dans l’Espace partenaires. À compter d’août2017, le code de hachage matériel ne sera plus nécessaire. 
*  Les appareils doivent avoir accès à Internet. Lorsque l'appareil ne peut pas se connecter, il affiche les écrans Windows OOBE (Out-Of-Box Experience) par défaut.
*  L’inscription de l’appareil dans une solution GPM nécessite Azure ActiveDirectory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Ajouter des pages de connexion à la phase OOBE

Pour ajouter des pages spécifiques de l’organisation, ajoutez les appareils dans l’[annuaire AzureAD](https://go.microsoft.com/fwlink/?linkid=848958) de votre organisation et créez des pages de connexion.


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Supprimer des pages Windows de la phaseOOBE à l’aide d’un profil de déploiement WindowsAutoPilot

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a>Exemples de paramètres dans un profil de déploiement WindowsAutoPilot
*  Ignorer les paramètres de confidentialité dans l’installation
*  Désactiver le compte d’administrateur local dans l'installation
*  Ignorer automatiquement des pages dans l'installation
   *  Sélectionner automatiquement le programme d’installation professionnel ou scolaire
   *  Ignorer les pages de configuration de Cortana, de OneDrive et d'inscription OEM

### <a name="add-devices-and-apply-a-profile"></a>Ajouter des appareils et appliquer un profil

Dans l’Espace partenaires, vous pouvez créer un profil de déploiement WindowsAutoPilot et l’appliquer à une liste d’appareils.

Pour configurer des appareils, téléchargez une liste d’appareils dans l’Espace partenaires, créez un profil qui s’applique à ces appareils, puis appliquez-le.

1.  Ajoutez la liste d'appareils dans l’Espace partenaires. (Les agents commerciaux et administrateurs disposent d'un accès pour ajouter la liste des appareils dans l’Espace partenaires.)

    a.  Créez un fichier.csv à l’aide du script PowerShell de la rubrique: [Présentation de WindowsAutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). Ce fichier.csv contient des informations sur l’appareil, notamment le numéro de série, le nom OEM, le nom de modèle, l’ID produit et l’identificateur d’appareil. 

    b.  À partir du tableau de bord de l'Espace partenaires, accédez à **Clients** > sélectionnez le client destinataire des appareils > **Appareils > Ajouter des appareils**.

    c.  Nom du lot d’appareils, par exemple, «Ordinateurs du service des ventes de Contoso – commande d'avril2017.» 

    d.  Cliquez sur **Parcourir** > sélectionnez le fichier d’informations sur les appareils > **Valider**.

    **Remarque:** si vous obtenez un message d’erreur lorsque vous essayez de télécharger le fichier.csv, vérifiez le format du fichier. À compter du mois d’août, vous pouvez utiliser le code de hachage matériel uniquement, ou le nom OEM, le numéro de série et le modèle, dans cet ordre de colonnes, ou l’ID produit Windows. Vous pouvez également utiliser l’exemple de fichier.csv fourni à partir du lien en regard de **Ajouter des appareils**.

2.  Créez un profil que vous pouvez appliquer aux appareils. (Seuls les agents administrateurs disposent d'un accès pour créer et appliquer des profils dans l’Espace partenaires.)

    a.  Dans **Appareils**, cliquez sur **Ajouter un nouveau profil**.

    b.  Nommez le profil, par exemple, «Profil Bureau Contoso – Ignorer toutes les phases OOBE».

    c.  Configurez les paramètres de la phase OOBE. Par exemple, cochez **Ignorer la configuration rapide dans l'installation**.

    d.  Cliquez sur **Envoyer**.

3.  Appliquez le profil.

    a.  Dans **Appareils**, dans le volet **Affecter et supprimer des appareils**, sélectionnez les appareils à configurer. Pour sélectionner un lot entier, cliquez sur la case à cocher en regard du nom de lot (par exemple, «Ordinateurs du service des ventes de Contoso – commande de mars2017»).

    b.  Cliquez sur **Appliquer un profil** et sélectionnez le profil (par exemple, «Profil Bureau Contoso – Ignorer toutes les phases OOBE»). Les appareils affichent le profil dans la colonne Profil.

4.  Facultatif: testez pour vérifier que votre profil fonctionne.

    a.  Connectez un appareil au réseau et mettez-le sous tension.

    b.  Vérifiez que les écrans OOBE appropriés (le cas échéant) s’affichent.

    c.  Pour préparer l'appareil à un nouvel utilisateur, effectuez la phase OOBE, puis rétablissez les paramètres par défaut de l’appareil.


## <a name="to-update-or-delete-a-profile"></a>Pour mettre à jour ou supprimer un profil 

Une fois que vous avez affecté à un profil à un appareil, vous pouvez le mettre à jour, même si vous avez déjà donné l'appareil à votre client. Lorsque l’appareil se connecte à Internet, il télécharge la dernière version de votre profil lors du processus OOBE. Si votre client rétablit les paramètres par défaut de l'appareil, celui-ci télécharge à nouveau les dernières mises à jour de votre profil. 

###<a name="you-can-remove-a-profile-from-a-device"></a>Vous pouvez supprimer un profil à partir d’un appareil
1. Sélectionnez l'appareil (ou un lot d'appareils) dont vous voulez supprimer le profil. 

2. Dans le volet **Affecter et supprimer des appareils**, sélectionnez **Supprimer un profil**.

3. Accédez au profil à supprimer et supprimez-le. Le profil sera supprimé de l'ensemble des appareils.

Dans **Appareils**, sélectionnez le profil. À ce stade, vous pouvez modifier les paramètres existants.