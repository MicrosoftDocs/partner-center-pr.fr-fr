---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
description: Synchronisez les références dans l’espace partenaires avec votre connecteur de co-vente pour Dynamics 365 CRM. Vous pouvez alors vendre en collaboration avec Microsoft à partir de votre système CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768769"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Vue d’ensemble de la co-vente du connecteur pour Dynamics 365 CRM

### <a name="appropriate-roles"></a>Rôles appropriés

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

Les connecteurs de covente de l’espace partenaires permettent à vos vendeurs de vendre en collaboration avec Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter ou refuser des références, et modifier les données de l’offre, telles que la valeur de l’offre et la date de clôture. Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente. Vous pouvez gérer toutes vos références dans le CRM de votre choix plutôt que dans l’espace partenaires.

La solution est basée sur Power automate et utilise les API de l’espace partenaires.

## <a name="prerequisites"></a>Prérequis

Avant d’installer la solution, assurez-vous de respecter les conditions préalables suivantes.

|**Rubriques**   |**Détails**   |**Liens**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network (MPN) |Vous avez besoin d’un ID MPN valide.|[Rejoindre le réseau partenaire](https://partner.microsoft.com/)|
|Prêt pour la co-vente|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références.|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système.|[Affecter des rôles dans Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Gestion de l’alimentation-automatiser le compte|Créez un nouvel environnement de production avec une base de données de test, intermédiaire et de production. Si vous disposez d’un environnement de production existant avec une base de données, vous pouvez le réutiliser. L’utilisateur qui va installer la solution connecteur doit disposer d’une licence Power automate et d’un accès à cet environnement. Vous pouvez surveiller la progression et obtenir des informations supplémentaires dans [Power automate](https://flow.microsoft.com/) en cas d’échec de l’installation. Sélectionnez **afficher l’historique** sous **solutions**.|[Créer ou gérer l’environnement](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)

1. Accédez à [Power automate](https://flow.microsoft.com), puis sélectionnez **environnements** dans l’angle supérieur droit. Cette étape vous montrera les instances CRM disponibles.

1. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.

1. Sélectionnez **solutions** sur la gauche.

1. Sélectionnez le lien **ouvrir AppSource** dans le menu supérieur.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Capture d’écran montrant les AppSource ouverts.":::

1. Recherchez Dynamics 365 dans l’écran contextuel pour rechercher les **connecteurs de référence de l’espace partenaires** .  

1. Sélectionnez le bouton **Télécharger maintenant** , puis sélectionnez **Continuer**.

1. Une page s’affiche, dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application. Acceptez les conditions générales.

1. Vous pouvez surveiller la progression et, en cas d’échec de l’installation, vous pouvez obtenir plus de détails dans Power automate en sélectionnant **afficher l’historique** sous **solutions**.

1. Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** sur la gauche. La **synchronisation des références de l’espace partenaires pour Dynamics 365** est désormais disponible dans la liste des **solutions** .

1. Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**. Les flux et entités Power automate suivants sont disponibles.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Capture d’écran montrant les CRM disponibles.":::

## <a name="test-before-you-go-live"></a>Testez avant de passer en temps réel

Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire. Vous devez effectuer les opérations suivantes :

- Installez la solution Power automate sur une instance CRM de l’environnement intermédiaire.
- Configurez et personnalisez la solution Power automate dans un environnement intermédiaire.
- Testez la solution sur une instance CRM intermédiaire.
- Après un test réussi, importez en tant que solution gérée dans l’instance de production.

## <a name="configure-the-solution"></a>Configuration de la solution

1. Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).

1. Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.

1. Vous devez créer des connexions qui associent les trois comptes d’utilisateur :

   - Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références
   - Événements de l’Espace partenaires
   - Administration CRM avec l’alimentation automatiser les flux de la solution

   1. Sélectionnez **connexions** sur la gauche, puis sélectionnez la solution références de l' **espace partenaires** dans la liste.

   1. Créez une connexion en sélectionnant **créer une connexion**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Capture d’écran montrant la création d’une connexion.":::

   1. Recherchez les **références de l’espace partenaires (version préliminaire)** dans la barre de recherche dans le coin supérieur droit.

   1. Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.

   1. Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références.

   1. Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.
     
   1. Une fois que vous avez ajouté toutes les connexions, vous devez voir les connexions suivantes dans votre environnement.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Capture d’écran montrant les connexions.":::

## <a name="edit-the-connections"></a>Modifier les connexions

1. Revenez à la page **solutions** et sélectionnez **solution par défaut**. Sélectionnez **référence de connexion (version préliminaire)** en sélectionnant **tout**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Capture d’écran montrant la modification des connexions.":::

1. Modifiez chacune des connexions une par une en cliquant sur l’icône de points de suspension. Ajoutez les connexions appropriées.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Capture d’écran montrant les connexions listées.":::

1.  Revenez à la page **solutions** , sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365** et activez le Flow en sélectionnant l’icône de points de suspension en regard de chaque Flow dans l’ordre suivant. Si vous rencontrez des problèmes lors de l’activation du Flow, consultez [étapes de personnalisation](connector-dynamics.md#customize-synchronization-steps) et [étapes de dépannage](connectors-troubleshoot.md).

Activez les flux dans l’ordre suivant :

- Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)
- Créer une référence de covente – Dynamics 365 à l’espace partenaires (version préliminaire d’Insider)
- Personnalisation Créer ou récupérer des détails à partir de Dynamics 365 Flow
- Espace partenaires vers Dynamics 365-Helper (version préliminaire d’Insider)
- Espace partenaires Microsoft : mises à jour de référence de la co-vente à Dynamics 365 (version préliminaire d’Insider)
- Espace partenaires vers Dynamics 365 (version préliminaire d’Insider)
- Dynamics 365 pour l’espace partenaires (version préliminaire d’Insider)
- Opportunité Dynamics 365 pour l’espace partenaires (version préliminaire d’Insider)
- Dynamics 365 solutions Microsoft pour Partner Center (version préliminaire d’Insider)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utiliser les API webhook pour s’inscrire aux événements de changement de ressource

Vous pouvez utiliser les API de webhook de l’espace partenaires pour vous inscrire aux événements de changement de ressource. Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.

1. Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.

1. Sélectionnez l’icône **modifier** , puis sélectionnez le **moment où une requête HTTP est reçue**.

1. Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.

   :::image type="content" source="images/webhook-video.gif" alt-text="Capture d’écran illustrant l’utilisation de webhooks pour enregistrer des modifications de ressources.":::

1. Sélectionnez l' **inscription du webhook de l’espace partenaires (version préliminaire)** Power automatiser Flow, puis sélectionnez **exécuter**.

1. Assurez-vous que la fenêtre **exécuter le déroulement** s’ouvre dans le volet droit, puis sélectionnez **Continuer**.

1. Entrez les informations suivantes :

   - **Point de terminaison du déclencheur http**: cette URL a été copiée à partir d’une étape précédente.
   - **Événements à inscrire**: sélectionnez tous les événements disponibles **(création de références**, **référence-mis à jour**, **référence-référence-créé** et associé-référence- **mis à jour**).
   - **Remplacer les points de terminaison déclencheurs existants s’ils sont présents ?**: Oui. Une seule URL peut être inscrite pour un événement webhook donné.

1. Sélectionnez **exécuter le workflow**, puis sélectionnez **terminé.**

Le webhook peut désormais écouter, créer et mettre à jour des événements.

## <a name="customize-synchronization-steps"></a>Personnaliser les étapes de synchronisation

Les systèmes CRM sont hautement personnalisés, et vous pouvez personnaliser la solution Power automate en fonction de votre configuration de CRM. Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur l’ordinateur de l’espace partenaires sont répertoriés dans le [Guide de mappage de champs personnalisé](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications nécessaires dans **[personnaliser] créer ou récupérer des détails à partir de variables d’environnement ou de fluide Dynamics 365** . Ne mettez pas à jour d’autres flux dans la solution Power automate, car cela peut affecter les futures mises à niveau de solutions.

Les personnalisations suivantes sont disponibles :

- **Afficher la coche dans le nom de l’opportunité**: par défaut, une coche s’affiche en regard du nom de l’opportunité pour indiquer que la synchronisation entre l’espace partenaires et Dynamics 365 CRM s’est déroulée correctement. De même, une croix est affichée si la synchronisation échoue. Pour éviter d’ajouter une coche ou une croix dans le nom de l’opportunité, définissez la valeur actuelle de la **case à cocher Afficher dans la** variable d’environnement nom de l’opportunité sur non.
- **Valeur** de la transaction : par défaut, la valeur de transaction de l’espace partenaires sera synchronisée vers et à partir de **ESTIMATEDVALUE** dans le CRM. Si vous avez un champ différent dans le CRM pour la valeur de transaction à partir de laquelle effectuer la synchronisation :

  - Mettez à jour le nom du champ de **valeur de transaction** dans la variable d’environnement Dynamics 365 avec le nom de champ de CRM. Assurez-vous de fournir le nom du champ, et non son nom d’affichage.
  - Modifiez **[personnaliser] créer ou obtenir des détails à partir de Dynamics 365 Flow**, puis accédez à **créer ou mettre à jour l’opportunité** dans CRM et à mettre à jour **créer une nouvelle opportunité** et **mettre à jour** les actions existantes pour affecter la valeur **DealValue** au champ approprié dans le CRM. En outre, supprimez l’affectation **DealValue** du champ **revenu estimé** .

- **Code du pays du compte client**: il est obligatoire de fournir un code de pays à deux lettres (ISO 3166) lorsque vous créez une nouvelle référence. Par défaut, l’indicatif du pays est synchronisé vers et à partir du champ **address1_country** du compte dans le CRM. Si vous avez un champ différent dans le CRM pour la synchronisation de l’indicatif du pays :

   - Dans le cas d’un champ indicatif de pays non-recherche dans le compte contenant un code à deux lettres :
     - Mettez à jour le nom du champ de **Code du pays du compte client** dans la variable d’environnement Dynamics 365 avec le nom de champ de CRM. Assurez-vous de fournir le nom du champ, et non son nom d’affichage.
     - Modifiez **[personnaliser] créer ou obtenir des détails à partir de Dynamics 365 Flow**, puis cliquez sur **créer ou obtenir un compte client** dans l’action CRM pour affecter une valeur de **pays** au champ approprié dans le CRM. Supprimez également l’attribution de valeur de **pays** dans le champ **adresse 1 : pays/région** .

   - Pour un champ Code de pays basé sur la recherche dans le compte :
     - Ajoutez un nouveau champ personnalisé dans le compte et remplissez-le automatiquement avec un code de pays à deux lettres (ISO 3166) en fonction de la valeur sélectionnée dans le champ basé sur la recherche et vice versa.
     - Suivez les étapes précédentes pour le champ Code pays non-Lookup pour synchroniser un nouveau champ personnalisé à partir du CRM vers et depuis l’espace partenaires.

- **Champs d’opportunité**: si des champs obligatoires doivent être renseignés dans l' **opportunité** , modifiez **[personnaliser] créer ou obtenir des détails à partir de Dynamics 365 Flow** et accédez à **créer ou mettre à jour une opportunité** dans le CRM et mettez à jour **créer une nouvelle action opportunité** pour affecter des valeurs aux champs obligatoires en fonction des besoins de votre entreprise.
- **Champs de prospect**: Si vous devez renseigner les champs obligatoires du **prospect** , modifiez **[personnaliser] créer ou obtenir des détails à partir de Dynamics 365 Flow** et accédez à **créer ou mettre à jour le prospect** dans le CRM et à mettre à jour **créer une action de prospect** pour affecter des valeurs aux champs obligatoires en fonction des besoins de votre entreprise.
- **Compte client**: quand une nouvelle référence est synchronisée de l’espace partenaires vers le CRM, la solution Power automate tente de rechercher un compte existant dans le CRM à l’aide du nom de la société client et du code postal. S’il n’en trouve pas, un nouveau compte client est créé dans le CRM. Pour mettre à jour les critères de recherche et les détails de la création du nouveau compte, modifiez **[personnaliser] créer ou afficher les détails à partir de Dynamics 365 Flow** et accédez à **créer ou recevoir un compte client** dans le CRM et à l' **action créer un compte** client.

## <a name="update-environment-variable"></a>Mettre à jour la variable d’environnement

Pour mettre à jour une valeur de variable d’environnement :

1. Accédez à la page **solutions** , puis sélectionnez **solution par défaut**. Sélectionnez **variable d’environnement** en sélectionnant **tout**.

1. Sélectionnez la variable d’environnement pour la valeur qui doit être mise à jour, puis sélectionnez **modifier** à l’aide de l’icône de points de suspension.

1. Mettez à jour la **valeur actuelle** (ne mettez pas à jour la **valeur par défaut**) en utilisant l’option **nouvelle valeur** et en fournissant la valeur. La valeur doit correspondre au type de données de la variable. Par exemple, le type de données Yes ou no accepte la valeur Yes ou no.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Capture d’écran montrant les variables d’environnement de mise à jour.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Synchronisation bidirectionnelle bidirectionnelle de la référence de la co-vente

Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.

### <a name="prerequisites"></a>Prérequis

Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft. Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs et d’objets personnalisés sera ajouté dans le cadre de l’installation de la solution. Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires. Par défaut, la valeur de ce champ est non et doit être explicitement définie sur Oui par le vendeur pour partager une opportunité avec Microsoft. La valeur de ce champ est définie sur Oui pour les nouvelles références partagées entre l’espace partenaires et CRM.
- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires.
- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires.
- **Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence. Pour créer une référence de covente, sélectionnez l’aide appropriée requise de Microsoft. Un contact client doit être associé à la possibilité de créer une référence de covente. Pour créer une référence de non-vente, ne sélectionnez pas ce champ. Une référence de non-vente peut être convertie en référence de covente à tout moment en sélectionnant l’option d’aide appropriée.
- Visibilité de la référence de l' **espace partenaires Microsoft**: sélectionnez visibilité pour la référence de l’espace partenaires. En le rendant visible pour les vendeurs Microsoft, une référence à la non-vente peut être convertie en covente. Lorsque l’aide Microsoft est requise, la référence est visible par défaut pour les vendeurs Microsoft. Une fois ce champ marqué comme visible, il ne peut pas être rétabli.
- **Identificateur Microsoft CRM**: quand une référence de covente est créée et acceptée par Microsoft, ce champ est renseigné avec l’identificateur Microsoft CRM.
- **Produits : obsolète**: n’utilisez pas ce champ ou ajoutez-le à la section CRM. Elle est disponible uniquement à des fins de compatibilité descendante. Utilisez à la place des solutions de l’espace partenaires.
- **Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires.
- **Solutions de l’espace partenaires Microsoft**: objet personnalisé pour associer des solutions prêtes pour la co-vente ou des solutions Microsoft avec l’opportunité. Une ou plusieurs solutions peuvent être ajoutées ou supprimées de l’opportunité. Il est obligatoire d’ajouter au moins une solution de co-vente prête ou Microsoft à l’opportunité avant de la partager avec Microsoft. Pour associer cet objet à l’opportunité, mettez à jour le formulaire d' **opportunité** dans le CRM.

  Sélectionnez l’onglet approprié dans le formulaire d' **opportunité** , puis ajoutez une sous-grille comme indiqué ici.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Capture d’écran montrant le formulaire d’opportunité.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Capture d’écran montrant les solutions Microsoft.":::

- Une fois que vous avez ajouté des solutions Microsoft, vous pouvez préremplir les détails de la solution de covente pour que vos vendeurs n’aient pas à les ajouter. Pour ajouter un nouveau détail de solution, accédez à l’objet détails de la solution Microsoft dans le CRM et sélectionnez **Ajouter un enregistrement** pour ajouter une entrée ou utiliser le **Téléchargement Excel** pour ajouter plusieurs entrées.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Capture d’écran montrant les nouveaux détails de la solution Microsoft.":::

### <a name="scenarios"></a>Scénarios

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans le CRM et synchronisée dans l’espace partenaires :

   1. Connectez-vous à votre environnement CRM Dynamics 365 avec l’utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.

   1. Assurez-vous que la section **Microsoft Partner Center** est présente lorsque vous créez une nouvelle opportunité dans l’environnement Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Capture d’écran montrant une nouvelle opportunité.":::

   1. Pour synchroniser cette opportunité avec l’espace partenaires, veillez à définir les champs suivants dans la vue de la carte :

      - **Comment Microsoft peut-il vous aider ?**: pour créer une référence de covente, sélectionnez une option d’aide appropriée.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Capture d’écran montrant comment obtenir les champs appropriés en mode carte.":::

      - **Contact client**: pour créer une référence de covente, ajoutez un contact client à l’opportunité.
      - **Synchroniser avec l’espace partenaires**: Oui.
      - **Solutions Microsoft**: pour partager une référence avec Microsoft, ajoutez une solution de covente prête ou Microsoft à l’occasion.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Capture d’écran montrant l’ID de la solution.":::

   1. Une fois l’opportunité créée dans Dynamics 365 avec l’option **synchroniser avec le Centre des partenaires** définie sur Oui, patientez 10 minutes. Ensuite, connectez-vous à votre compte espace partenaires. Vos références seront synchronisées avec Dynamics 365 et l' **identificateur de référence**. Le **lien de référence** sera rempli. En cas d’échec, le champ **audit** est rempli avec les informations d’erreur.
     
    1. De même, pour une opportunité dans laquelle l’option **synchroniser avec l’espace partenaires** est définie sur Oui, si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.

    1. Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires et synchronisée dans l’environnement Dynamics 365 :

   1. Connectez-vous au tableau de [bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.

   1. Dans le menu de gauche, sélectionnez **références** .

   1. Pour créer une nouvelle référence de covente à partir de l’espace partenaires, sélectionnez l’option **nouveau contrat** .

   1. Connectez-vous à votre environnement Dynamics 365 CRM.

   1. Accédez à **ouvrir opportunités**. La référence créée dans l’espace partenaires est maintenant synchronisée dans Dynamics 365 CRM.

   1. Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)
- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)
- [En savoir plus sur la plateforme Microsoft Power automatiser](/power-automate/)
- [Webhooks de l’Espace partenaires](/partner-center/develop/partner-center-webhooks)
