---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniser vos références dans l’espace partenaires avec votre CRM Salesforce
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 0a22587f5b555281cae6f557acfc2695ba92727e
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302376"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connecteur de covente pour Salesforce CRM - vue d’ensemble

### <a name="appropriate-roles"></a>Rôles appropriés

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.  Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente. Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires. 

La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.

## <a name="before-you-install---pre-requisites"></a>Avant d’installer-conditions préalables

|**Explique**   |**Détails**   |**Liens**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Vous avez besoin d’un ID MPN valide|Pour rejoindre [MPN](https://partner.microsoft.com/)|
|Co-vente prête|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)|
|CRM Salesforce|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système|[Affecter des rôles dans Salesforce CRM](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Gestion de l’alimentation-automatiser le compte|Un compte Active [Power automate](https://flow.microsoft.com) actif pour l’administrateur système ou le personnalisateur système CRM. Cet utilisateur doit se connecter à [Power automate](https://flow.microsoft.com) au moins une fois avant l’installation.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM

1. Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit. Les instances CRM disponibles s’affichent.

2. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.

3. Sélectionnez **solutions** dans la barre de navigation de gauche.

4. Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.

7. Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM Salesforce pour installer l’application.  Acceptez les conditions générales.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRM disponibles":::

8. Vous êtes ensuite dirigé vers la page **gérer vos solutions** .  Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page. **L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires. L’installation prendra 10-15 minutes.

9. Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche. Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est disponible dans la liste des solutions.

10. Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**. Les flux et entités Power automate suivants sont disponibles :

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Flux Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a>Meilleure pratique : testez avant de passer en direct

Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.

- Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.

- Effectuez une copie de la solution et exécutez votre configuration et l’alimentation automatiser les personnalisations de flow sur l’environnement intermédiaire.

- Testez la solution sur une instance intermédiaire/CRM.

- En cas de réussite, importez en tant que solution gérée dans l’instance de production.

## <a name="configure-the-solution"></a>Configuration de la solution

1. Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).

2. Dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power automate.

3. Vous devrez créer des connexions qui associent les trois comptes d’utilisateur :

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

5. **Activez** les flux automate Power.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utiliser les API webhook pour s’inscrire aux événements de changement de ressource

Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource. Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.

1. Pour inscrire votre URL, sélectionnez **inscription du webhook de l’espace partenaires (version préliminaire)** alimentation automatiser le Flow.

2. Ajouter des connexions pour (a.) Utilisateur de l’espace partenaires avec des références d’administrateur d’administration (b.) Événements de l’espace partenaires mis en surbrillance ci-dessous

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Déclencheur":::

3. Lorsque vous effectuez ces mises à jour, vous verrez

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Enregistrez vos modifications et sélectionnez **activer**.

   Pour activer les webhooks de l’espace partenaires afin d’écouter les modifications des événements, procédez comme suit :

5. Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.

6. Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.

7. Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copier l’URL":::

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

   1. Sélectionnez l’espace partenaires pour Salesforce CRM (version préliminaire d’Insider).

   2. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

   3. Sélectionnez **(étendue) synchroniser le prospect ou l’opportunité**.

2. Pour personnaliser les mappages de champs CRM pour les événements de création, sélectionnez **s’il s’agit d’une nouvelle opportunité partagée, puis**. Sélectionnez la sous-étape **si oui** , puis développez **création d’une nouvelle opportunité dans le CRM**. Vous pouvez modifier les mappages dans cette section à l’aide du Guide de mappage de champs.

   1. Pour personnaliser les mappages de champs CRM pour les événements de mise à jour, cliquez sur l’étape « (étendue) synchroniser le prospect ou l’opportunité ».

   2. Sélectionnez **s’il s’agit d’une mise à jour d’une opportunité, puis**. Sélectionnez la sous-étape **si oui** , puis développez **si la différence entre les objets d’opportunité dans l’espace partenaires et CRM est déplacée**.  

   3. Sélectionner **si oui** suivi de **mettre à jour l’opportunité existante**

3. Pour personnaliser les champs pour la synchronisation des références de CRM à PC pour les événements de mise à jour :

   1. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

   2. Sélectionnez **(étendue) synchroniser l’opportunité**.

   3. Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour les événements de mise à jour, sélectionnez **s’il existe une différence entre les objets de Prospect dans l’espace partenaires et CRM, puis**.

   4. Sélectionnez la sous-étape **si oui** , puis développez l’étape **mettre à jour une référence avec les données d’opportunité**.

   Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.

4. Pour personnaliser les champs de la synchronisation de référence de CRM à PC pour les événements de création ?

   1. Sélectionnez **modifier** pour modifier/personnaliser le Flow automatiser l’alimentation.

   2. Sélectionnez **(étendue) synchronisation des références.**

   3. Pour personnaliser les mappages de champs CRM (en fonction du Guide des mappages de champs) pour créer des événements, sélectionnez **créer une référence Microsoft**.

Vous pouvez modifier les mappages dans cette section en fonction du Guide de mappage de champs.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Créer une section distincte dans la disposition des opportunités CRM Salesforce

Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft. Cela permet à vos équipes de vendeur de décider quelles références elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** CRM Salesforce. Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .
L’utilisateur administrateur CRM Salesforce devra créer une section CRM distincte.

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft

- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft

- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft

- **Comment Microsoft peut-il vous aider ?** Aide requise de Microsoft pour la référence

- **Produits**: liste des produits associés à cette opportunité

- **Audit**: piste d’audit en lecture seule pour la synchronisation avec la référence de l’espace partenaires Microsoft

### <a name="set-up-fields-and-relationships"></a>Définir des champs et des relations

1. Connectez-vous à votre compte Salesforce et accédez à **opportunité**.

2. Cliquez sur les options **d’installation** et de **modification d’objet** pour ajouter les champs nécessaires.

3. Sélectionner les **champs & les relations** dans le volet de navigation gauche

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. Ajoutez les champs suivants dans la table **fields & Relationship** :

   |**Étiquette du champ**   |**Nom du champ**|**Type de données**|**Indexée**|
   |---------------------|:-------------------|:--------------|:----------------|
   |Audit| Audit__c|Longue zone de texte (100000) (ligne visible 4)||
   |Comment Microsoft peut-il vous aider ?|How_can_Microsoft_help_c|Liste déroulante|
   |Products|Products_c|texte (255)||
   |Referral | Referral_Identfier_c|Texte (100) (ID externe)|Oui|
   |Lien de référence| Referral_Link_c_|URL (255)||
   |Synchroniser avec l’espace partenaires|sync_with_partner_center_c|Case à cocher (désactivé par défaut)||

   * Valeurs de liste déroulante :

   - Proposition de valeur spécifique à la charge de travail
   - Architecture technique du client
   - Preuve de concept ou démonstration
   - Devis ou licences
   - Succès du client après la vente
   - Général ou autre

5. Les champs sont créés sous les **champs & les relations**

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Champs créés":::

6. Dans la disposition opportunité, créez une section distincte avec les champs comme indiqué ci-dessus.

   - Cette section doit être disponible pour les vendeurs dans la disposition opportunité.

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Disposition des champs de l’espace partenaires":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout

Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.

### <a name="pre-requisites"></a>Conditions préalables

Pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power automate doit clairement délimiter les champs de référence propres à Microsoft. Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce. Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft

- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft

- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft

- **Comment Microsoft peut**-il vous aider : aide requise de Microsoft pour la référence

- **Produits**: liste des produits associés à cette opportunité

- **Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires

### <a name="scenarios"></a>SCÉNARIO

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :

   1. Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.

   2. Vérifiez que la section suivante est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement CRM Salesforce

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Environnement Salesforce":::

   3. Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :

       - « Synchroniser avec l’espace partenaires » : Oui
       - « Comment Microsoft peut-il m’aider ? » : sélectionnez l’une des options suivantes :
       - Produits : ID de solution du produit

   4. Une fois que vous avez défini l’option **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires. Vos références seront synchronisées avec Salesforce CRM.

   5. Lorsque l’option « synchroniser avec l’espace partenaires » est définie sur « Oui », si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.

   6. Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.

2. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :

    1. Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.

    2. Dans le menu de gauche, sélectionnez **références** .

    3. Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».

    4. Connectez-vous à votre environnement CRM Salesforce.

    5. Accédez à **opportunités ouvertes**. La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Écran d’opportunités Salesforce":::

    6. Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.

## <a name="next-steps"></a>Étapes suivantes

- [En savoir plus sur la plateforme Microsoft Power Automated ?](https://docs.microsoft.com/-automate/)

- [Gérer les prospects](manage-leads.md)

- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)

- [Webhooks de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)