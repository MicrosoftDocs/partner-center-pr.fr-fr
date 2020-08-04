---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires à l’aide de votre Dynamics 365 CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 9cbdefb46691bf10ca1525190729a056f222ee90
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527575"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble

### <a name="appropriate-roles"></a>Rôles appropriés

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction et la date de clôture. Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente. Vous pouvez faire en sorte que toutes vos références fonctionnent dans le CRM de votre choix plutôt que dans l’espace partenaires. 

La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.

## <a name="before-you-install---pre-requisites"></a>Avant d’installer-conditions préalables

|**Rubriques**   |**Détails**   |**Liens**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Vous avez besoin d’un ID MPN valide|Pour rejoindre [MPN](https://partner.microsoft.com/)|
|Covente prête|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système|[Affecter des rôles dans Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Gestion de l’alimentation-automatiser le compte|Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM. Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)

1. Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit. Cette étape vous montrera les instances CRM disponibles.

2. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.

3. Sélectionnez **solutions** dans la barre de navigation de gauche.

4. Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.  

6. Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.

7. Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.  Acceptez les conditions générales.

8. Vous êtes ensuite dirigé vers la page **gérer vos solutions** .  Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page. **L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires. L’installation prendra 10-15 minutes. 

9. Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche. Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.

10. Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**. Les flux et entités Power automate suivants sont disponibles :

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRM disponibles":::

## <a name="best-practice-test-before-you-go-live"></a>Meilleure pratique : testez avant de passer en direct

Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.

- Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.
- Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.
- Testez la solution sur une instance intermédiaire/CRM. 
- En cas de réussite, importez en tant que solution gérée dans l’instance de production. 

## <a name="configure-the-solution"></a>Configuration de la solution

1. Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).

2. Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.

3. Vous devez créer des connexions qui associent les trois comptes d’utilisateur :

   - Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références

   - Événements de l’Espace partenaires

   - L’administrateur CRM avec les flux Power automate dans la solution.

      1. Sélectionnez **connexions** dans la barre de navigation de gauche et sélectionnez la solution « références de l’espace partenaires » dans la liste.

      2. Créez une connexion en cliquant sur **créer une connexion**.

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Créer une connexion":::

      3. Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.

      4. Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.

      5. Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.

      6. Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.

4. Pour associer les flux Power automate avec les connexions, modifiez chacun des flux Power automate pour vous connecter à Common Data Service et aux références de l’espace partenaires. Enregistrez les modifications.

5. **Activez** l’alimentation automatiser les flux.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utiliser les API webhook pour s’inscrire aux événements de changement de ressource

Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource. Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.

1. Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.

2. Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. Lorsque vous effectuez ces mises à jour, vous verrez

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Enregistrez vos modifications et sélectionnez **activer**.

   Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :

5. Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.

6. Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.

7. Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copier l’URL":::

8. Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.

9. Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.

10. Entrez les informations suivantes :

    1. **Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente

    2. **Événements à inscrire**: « création de références » et « référencement-mis à jour »

    3. **Remplacer les points de terminaison déclencheurs existants s'** ils sont présents : Oui (cette valeur remplace tous les points de terminaison existants).

11. Sélectionnez **exécuter** , puis sélectionnez **terminé.**

Le webhook peut maintenant écouter les événements de création et de mise à jour.

## <a name="customize-synchronization-steps"></a>Personnaliser les étapes de synchronisation

Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés ici.

Souvent, les systèmes CRM sont hautement personnalisés. Vous pouvez personnaliser les flux Power automate. Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans les étapes des flux d’automate Power.  Les centres partenaires Microsoft et les mappages CRM sont fournis, mais, en fonction de votre environnement CRM, vous pouvez choisir de personnaliser davantage les champs.

Plusieurs étapes de chacun des flux d’automate d’alimentation peuvent être personnalisées en fonction de vos besoins. Voici quelques exemples de personnalisations disponibles :

1. Pour personnaliser les champs pour les événements de création ou de mise à jour dans l’espace partenaires pour la synchronisation de références CRM : 

    a. Sélectionnez espace partenaires pour Dynamics 365 (version préliminaire d’Insider) ou espace partenaires pour Salesforce (version préliminaire d’Insider).

    b. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

    c. Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.

2. Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**. Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**. Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.

    d. Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».

    e. Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**. Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.  

    f. Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**

3. Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :

    a. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

    b. Sélectionnez **(étendue) synchroniser l’opportunité**.

    c. Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**. 

    d. Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.

   Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.

4. Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?

   a. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

   b. Sélectionnez **(étendue) synchronisation des références.**

   c. Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.

   Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout

Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.

### <a name="pre-requisites"></a>Conditions préalables

Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft. Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs personnalisés est disponible dans le cadre de l’entité **opportunité** . Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft

- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft

- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft

- **Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence

- **Produits**: liste des produits associés à cette opportunité

- **Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires

### <a name="scenarios"></a>SCÉNARIO

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :

   1. Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.

   2. Assurez-vous que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Opportunité":::

   3. Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :

      - **Synchroniser avec l’espace partenaires**: Oui

      - **Comment Microsoft peut-il vous aider ?**:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sélections d’aide":::

      - **Produits**: ID de solution du produit

   4. Une fois que l’opportunité est créée dans Dynamics 365 avec l’option **synchroniser avec l’espace partenaires** définie sur **Oui**, patientez 10 minutes, puis connectez-vous à votre compte espace partenaires. Vos références seront synchronisées avec Dynamics 365.

   5. De même, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.

   6. Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.

2. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :

   1. Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.

   2. Dans le menu de gauche, sélectionnez **références** .

   3. Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».

   4. Connectez-vous à votre environnement Dynamics 365 CRM.

   5. Accédez à **opportunités ouvertes**. La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.

   6. Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)

- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)

- [En savoir plus sur la plateforme Microsoft Power Automated ?](https://docs.microsoft.com/power-automate/)

- [Webhooks de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)