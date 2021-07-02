---
title: Connecteur de covente pour Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisez vos références dans l’espace partenaires avec votre CRM Salesforce. Les vendeurs peuvent ensuite se vendre avec Microsoft à partir de vos systèmes CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173672"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connecteur de covente pour Salesforce CRM - vue d’ensemble

**Rôles appropriés**: administration des références | Administrateur système ou personnalisateur de système sur le CRM

Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. À l’aide des connecteurs de covente, vous pouvez créer une référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction, et la date de clôture.  Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente. Vous pouvez faire en sorte que toutes vos références fonctionnent lorsque vous travaillez dans le CRM de votre choix plutôt que dans l’espace partenaires.

la solution est basée sur la solution Microsoft Power Automate et utilise des api de l’espace partenaires.

## <a name="before-you-install---pre-requisites"></a>Avant d’installer-conditions préalables

|**Rubriques**|**Détails**|**Liens**|
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Vous avez besoin d’un ID MPN valide|Pour rejoindre [MPN](https://partner.microsoft.com/)|
|Prêt pour la co-vente|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)|
|CRM Salesforce|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système|[Affecter des rôles dans Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|compte d’Flow Power Automate|Créez un nouvel environnement de production avec une base de données de test, intermédiaire et de production. Si vous disposez d’un environnement de production existant avec une base de données, vous pouvez le réutiliser. l’utilisateur qui va installer la solution connecteur doit disposer d’une licence Power Automate et d’un accès à cet environnement. vous pouvez surveiller la progression et obtenir plus d’informations dans [Power Automate](https://flow.microsoft.com/) en cas d’échec de l’installation. Sélectionnez **afficher l’historique** sous **solutions**.|[Créer ou gérer l’environnement](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installation du package Salesforce pour les champs personnalisés Microsoft

pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power Automate doit identifier clairement les champs de référence spécifiques à Microsoft. Cette délimitation fournit aux équipes de vendeur partenaires la possibilité de choisir les références qu’elles souhaitent partager avec Microsoft pour la covente.

1. Dans Salesforce, activez les **Notes** et ajoutez-les à la liste des opportunités associées. [Informations de référence](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Pour activer les **équipes d’opportunités** , procédez comme suit :
    - dans le programme d’installation, utilisez la zone de **recherche rapide** pour localiser l’équipe des opportunités Paramètres.
    - Définissez les paramètres selon vos besoins. [Informations de référence](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Dans Salesforce, installez des champs et des objets personnalisés à l’aide du [programme d’installation de package](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Utilisez ce programme d’installation pour installer le package dans n’importe quelle entreprise.

    >[!NOTE]
    >Si vous installez dans un bac à sable (sandbox), vous devez remplacer la partie initiale de l’URL par `http://test.salesforce.com` .

1. Dans Salesforce, ajoutez des solutions Microsoft à la liste des **opportunités** associées. Une fois ajouté, sélectionnez l’icône de **clé** et mettez à jour les propriétés

## <a name="best-practice-test-before-you-go-live"></a>Meilleure pratique : testez avant de passer en direct

avant d’installer, de configurer et de personnaliser la solution Power Automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.

- installez Microsoft Power Automate solution sur un environnement intermédiaire/une instance CRM.

- effectuez une copie de la solution et exécutez votre configuration et Power Automate les personnalisations de workflow sur l’environnement intermédiaire.

- Testez la solution sur une instance intermédiaire/CRM.

- En cas de réussite, importez en tant que solution gérée dans l’instance de production.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installer la synchronisation des références de l’espace partenaires pour Salesforce CRM

1. accédez à [Power Automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit. Les instances CRM disponibles s’affichent.

1. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.

1. Sélectionnez **solutions** dans la barre de navigation de gauche.

1. Sélectionnez le lien **ouvrir AppSource** dans le menu supérieur.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Ouvrez AppSource.":::

1. Recherchez les **connecteurs de références de l’espace partenaires pour Salesforce** dans l’écran contextuel.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Capture d’écran de l’offre maintenant.":::

1. Sélectionnez le bouton **Télécharger maintenant** , puis sélectionnez **Continuer**.

1. Dans la page suivante, sélectionnez l’environnement CRM Salesforce pour installer l’application. Acceptez les conditions générales.

1. Vous êtes ensuite dirigé vers la page **gérer vos solutions** .  Accédez à « références de l’espace partenaires » à l’aide des flèches en bas de la page. **L’installation planifiée** doit s’afficher en regard de solution de références de l’espace partenaires. L’installation prendra 10-15 minutes.

1. une fois l’installation terminée, revenez à [Power Automate](https://flow.microsoft.com) et sélectionnez **Solutions** dans la zone de navigation de gauche. Notez que la **synchronisation des références de l’espace partenaires pour Salesforce** est désormais disponible dans la liste des solutions.

1. Sélectionnez la **synchronisation des références de l’espace partenaires pour Salesforce**. les flux et entités de Power Automate suivantes sont disponibles :

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Les flux Salesforce.":::

## <a name="configure-the-solution"></a>Configurer la solution

1. Une fois que vous avez installé la solution dans votre instance CRM, revenez à [Power automate](https://flow.microsoft.com/).

1. dans la liste déroulante **environnements** dans l’angle supérieur droit, sélectionnez l’instance CRM dans laquelle vous avez installé la solution Power Automate.

1. Vous devez créer des connexions qui associent les trois comptes d’utilisateur :

   - Utilisateur de l’espace partenaires avec les informations d’identification d’administrateur de références
   - Événements de l’Espace partenaires
   - administration de CRM avec l’Power Automate flux dans la solution

   1. Sélectionnez **connexions** dans la barre de navigation de gauche, puis sélectionnez la solution références de l' **espace partenaires** dans la liste.

   1. Créez une connexion en sélectionnant **créer une connexion**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Capture d’écran montrant la création d’une connexion.":::

   1. Recherchez les **références de l’espace partenaires (version préliminaire)** dans la barre de recherche dans le coin supérieur droit.

   1. Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.

   1. Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.

   1. Créez une connexion pour Salesforce pour l’utilisateur administrateur CRM.
  
   1. Créez une connexion pour Microsoft Dataverse pour l’utilisateur administrateur CRM.

   1. Une fois que vous avez ajouté toutes les connexions, vous devez voir les connexions suivantes dans votre environnement :

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Capture d’écran montrant comment observer les connexions.":::

### <a name="edit-the-connections"></a>Modifier les connexions

1. Revenez à la page **solutions** et sélectionnez **solution par défaut**. Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Capture d’écran montrant la modification des connexions.":::

1. Modifiez chacune des connexions individuellement en sélectionnant l’icône représentant des points de suspension. Ajoutez les connexions appropriées.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="La capture d’écran ATHT montre comment modifier des connecteurs.":::

1. Activez les flux dans l’ordre suivant :
   - Inscription au webhook de l’espace partenaires (version préliminaire d’Insider)
   - Personnalisation Créer ou récupérer des détails à partir de Salesforce
   - Créer une Referral-Salesforce de covente à l’espace partenaires (version préliminaire d’Insider)
   - Espace partenaires Microsoft : mises à jour de la référence à Salesforce (version préliminaire d’Insider)  
   - Espace partenaires vers Salesforce (version préliminaire d’Insider)
   - Salesforce pour Partner Center (version préliminaire d’Insider)
   - Opportunité Salesforce pour Partner Center (version préliminaire d’Insider)
   - Solutions Microsoft Salesforce pour Partner Center (version préliminaire d’Insider)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Utiliser les API webhook pour s’inscrire aux événements de changement de ressource

Vous pouvez utiliser les API de webhook de l’espace partenaires pour vous inscrire aux événements de changement de ressource. Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.

1. Sélectionnez l' **espace partenaires pour Salesforce CRM (version préliminaire d’Insider)**.

1. Sélectionnez l' **icône modifier** et sélectionnez le **moment où une requête HTTP est reçue**.

1. Sélectionnez l’icône de **copie** pour copier l' **URL http postale** fournie.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Capture d’écran montrant comment copier l’URL.":::

1. sélectionnez l' **inscription du webhook de l’espace partenaires (version préliminaire d’insider Power Automate)** , puis sélectionnez **exécuter**.

1. Assurez-vous que la fenêtre **exécuter le déroulement** s’ouvre dans le volet droit, puis sélectionnez **Continuer**.

1. Entrez les informations suivantes :

   - **Point de terminaison du déclencheur http**: cette URL a été copiée à partir d’une étape précédente.
   - **Événements à inscrire**: sélectionnez tous les événements disponibles **(création de références**, **référence-mis à jour**, **référence-référence-créé** et associé-référence- **mis à jour**).
   - **Remplacer les points de terminaison déclencheurs existants s’ils sont présents ?**: Oui. Une seule URL peut être inscrite pour un événement webhook donné.

1. Sélectionnez **exécuter le workflow**, puis sélectionnez **terminé**.

Le webhook peut désormais écouter, créer et mettre à jour des événements.

## <a name="customize-synchronization-steps"></a>Personnaliser les étapes de synchronisation

les systèmes crm sont hautement personnalisés, et vous pouvez personnaliser la solution Power Automate en fonction de votre configuration de CRM. Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur l’ordinateur de l’espace partenaires sont répertoriés dans le [Guide de mappage de champs personnalisé](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications appropriées dans **[personnaliser] créer ou récupérer des détails à partir de Salesforce ou de variables d'** environnement. ne mettez pas à jour les autres flux de la solution Power Automate, car cela peut affecter les futures mises à niveau de solutions.

Les personnalisations suivantes sont disponibles :

- **Afficher la coche dans le nom de l’opportunité**: par défaut, une coche s’affiche en regard du nom de l’opportunité pour indiquer que la synchronisation entre l’espace partenaires et le CRM Salesforce s’est déroulée correctement. De même, une croix est affichée si la synchronisation échoue. Pour éviter d’ajouter une coche ou une croix dans le nom de l’opportunité, définissez la valeur actuelle de la **case à cocher Afficher dans la** variable d’environnement nom de l’opportunité sur non.

- **Nom** de la phase :

  - **Nom de l’étape active**: il s’agit de l’étape dans le pipeline des ventes d’une opportunité dans Salesforce.  Il représente une étape active et équivaut à une référence dans l’état accepté dans l’espace partenaires. Il peut s’agir de l’étape suivante du pipeline des ventes après l’étape de maintien. Le déplacement du niveau de vente de l’opportunité hors de la phase de mise en attente à l’étape active acceptera la référence dans l’espace partenaires et les modifications commenceront la synchronisation.

  - **Nom de l’étape de maintien**: nom de l’étape dans le pipeline des ventes d’une opportunité dans Salesforce. Il représente une étape de maintien. La nouvelle référence de covente partagée par Microsoft qui n’est pas encore acceptée sera définie à cette étape dans Salesforce. Toute modification apportée à une opportunité alors qu’elle est en attente n’est pas synchronisée avec l’espace partenaires. Le déplacement de la phase de vente de l’opportunité en dehors de cette phase de blocage acceptera la référence dans l’espace partenaires et les modifications commenceront la synchronisation.

- **Code du pays du compte client**: il est obligatoire de fournir un code de pays à deux lettres (ISO 3166) lorsque vous créez une nouvelle référence. Par défaut, l’indicatif du pays est synchronisé vers et à partir du champ **BillingCountry** du compte dans Salesforce. Si vous avez un champ différent dans Salesforce pour la synchronisation de l’indicatif du pays :

  - Dans le cas d’un champ indicatif de pays non-recherche dans le compte contenant un code à deux lettres :

    - Mettez à jour le nom du champ de **Code du pays du compte client** dans la variable d’environnement Salesforce avec le nom de champ de CRM. Assurez-vous de fournir le nom du champ, et non son nom d’affichage.

    - Modifiez **[personnaliser] créer ou obtenir des détails à partir de Salesforce**, puis accédez à l’action **créer ou obtenir un compte client dans CRM** pour affecter une valeur de **pays** au champ approprié dans le CRM. Supprimez également l’attribution de valeur de **pays** du **BillingCountry**.

  - Pour un champ Code de pays basé sur la recherche dans le compte :

    - Ajoutez un nouveau champ personnalisé dans le compte et remplissez-le automatiquement avec un code de pays à deux lettres (ISO 3166) en fonction de la valeur sélectionnée dans le champ basé sur la recherche et vice versa.

    - Suivez les étapes précédentes pour le champ Code pays non-Lookup pour synchroniser un nouveau champ personnalisé à partir du CRM vers et depuis l’espace partenaires.

- **Valeur** de la transaction : par défaut, la valeur de transaction de l’espace partenaires sera synchronisée à partir de et à partir de la **quantité** dans le CRM. Si vous avez un champ différent dans le CRM pour la valeur de transaction à synchroniser :

  - Mettez à jour le nom du champ de **valeur de transaction** dans la variable d’environnement Salesforce avec le nom de champ de CRM. Assurez-vous de fournir le nom du champ, et non son nom d’affichage.

  - Modifiez **[personnaliser] créez ou récupérez des détails à partir de Salesforce** et accédez à **créer ou mettre à jour une opportunité** dans CRM et mettez à jour les deux actions **créer une nouvelle opportunité** et **mettre à jour** l’opportunité existante pour affecter le **DealValue** au champ approprié dans Salesforce.

- **Code devise** de la valeur de transaction : nom du champ de code devise de la valeur de transaction dans Salesforce. Ce nom d’API de champ sera utilisé pour récupérer le code devise de la valeur de transaction de l’opportunité lors de la création ou de la mise à jour de la référence dans l’espace partenaires Microsoft. Si le champ Code devise de la valeur de la transaction est différent du champ par défaut **CurrencyISOCode**, mettez à jour la valeur actuelle de cette variable d’environnement.

  - Mettez à jour le nom du champ devise de la **valeur de transaction** dans la variable d’environnement Salesforce avec le nom de champ de CRM. Assurez-vous de fournir le nom du champ, et non son nom d’affichage.

  - Modifiez **[personnaliser] créez ou récupérez des détails à partir de Salesforce** et accédez à **créer ou mettre à jour une opportunité** dans CRM et mettez à jour les deux actions **créer une nouvelle opportunité** et **mettre à jour** l’opportunité existante pour affecter le **DealValueCurrency** au champ approprié dans Salesforce.

- **Opportunité de covente** de la synchronisation : si la valeur est **Oui**, seules les opportunités de covente et de partage de pipeline seront synchronisées entre l’espace partenaires et Salesforce. Si vous choisissez **non**, les prospects, les coventes et les opportunités de partage de pipeline seront synchronisés entre l’espace partenaires et Salesforce. Cette variable n’a aucun impact sur les opportunités synchronisées à partir de Salesforce à l’espace partenaires.

## <a name="update-environment-variable"></a>Mettre à jour la variable d’environnement

Pour mettre à jour une valeur de variable d’environnement :

1. Accédez à la page **solutions** , puis sélectionnez **solution par défaut**. Sélectionnez **variable d’environnement** en sélectionnant **tout**.

1. Sélectionnez la variable d’environnement pour la valeur qui doit être mise à jour, puis sélectionnez **modifier** à l’aide de l’icône de points de suspension.

1. Mettez à jour la **valeur actuelle** (ne mettez pas à jour la **valeur par défaut**) en utilisant l’option **nouvelle valeur** et en fournissant la valeur. La valeur doit correspondre au type de données de la variable. Par exemple, le type de données Yes ou no accepte la valeur Yes ou no.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Capture d’écran montrant les variables d’environnement de mise à jour.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout

une fois que vous avez installé, configuré et personnalisé la solution Power Automate, vous pouvez tester la synchronisation des références de covente entre Salesforce CRM et l’espace partenaires.

### <a name="pre-requisites"></a>Conditions préalables

pour synchroniser les références entre l’espace partenaires et le CRM Salesforce, la solution Power Automate doit clairement délimiter les champs de référence propres à Microsoft. Cette identification offre à vos équipes de vendeur la possibilité de décider quelles références elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs personnalisés est disponible dans le cadre de la synchronisation des références de l’espace partenaires pour l’entité **opportunité** de solution CRM Salesforce. Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires. Par défaut, la valeur de ce champ est non et doit être explicitement définie sur Oui par le vendeur pour partager une opportunité avec Microsoft. La valeur de ce champ est définie sur Oui pour les nouvelles références partagées entre l’espace partenaires et CRM.

- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft.

- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft.

- **Comment Microsoft aide peut**-il : aide requise de Microsoft pour la référence. Pour créer une référence de covente, sélectionnez l’aide appropriée requise de Microsoft. Un contact client doit être associé à la possibilité de créer une référence de covente. Pour créer une référence de non-vente, ne sélectionnez pas ce champ. Une référence de non-vente peut être convertie en référence de covente à tout moment en sélectionnant l’option d’aide appropriée.

- Visibilité de la référence de l' **espace partenaires Microsoft**: sélectionnez visibilité pour la référence de l’espace partenaires. En le rendant visible pour les vendeurs Microsoft, une référence à la non-vente peut être convertie en covente. Lorsque l’aide Microsoft est requise, la référence est visible par défaut pour les vendeurs Microsoft. Une fois ce champ marqué comme visible, il ne peut pas être rétabli.

- **identificateur de Microsoft CRM**: quand une référence de covente est créée et acceptée par microsoft, ce champ est renseigné avec l’identificateur microsoft CRM.

- **Solutions de l’espace partenaires Microsoft**: objet personnalisé pour associer des solutions prêtes pour la co-vente ou des solutions Microsoft avec l’opportunité. Une ou plusieurs solutions peuvent être ajoutées ou supprimées de l’opportunité. Il est obligatoire d’ajouter au moins une solution de co-vente prête ou Microsoft à l’opportunité avant de la partager avec Microsoft. Pour associer cet objet à l’opportunité, mettez à jour le formulaire d' **opportunité** dans le CRM.

- **Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires

### <a name="scenarios"></a>SCÉNARIO

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :

   1. Connectez-vous à votre environnement CRM Salesforce avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.

   1. Assurez-vous que la section **Microsoft Partner Center** est présente lorsque vous créez une **nouvelle opportunité** dans l’environnement CRM Salesforce.

   1. Les opportunités qui ont été correctement synchronisées avec l’espace partenaires sont identifiées avec l’icône ✔ dans Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Capture d’écran de l’environnement Salesforce.":::

   1. Pour synchroniser cette opportunité avec l’espace partenaires Microsoft, veillez à définir les champs suivants dans la vue de la carte :

      - **Comment Microsoft peut-il vous aider ?**: pour créer une référence de covente, sélectionnez une option d’aide appropriée.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Capture d’écran montrant comment obtenir les champs appropriés en mode carte.":::

      - **Synchroniser avec l’espace partenaires**: Oui
      - **Contact client**: pour créer une référence de covente, ajoutez un contact client à l’opportunité.
      - **Solutions Microsoft**: pour partager une référence avec Microsoft, ajoutez une solution de covente prête ou Microsoft à l’occasion.

   1. Une fois que vous avez défini l’option **synchroniser l’opportunité avec l’espace partenaires** sur **Oui**, patientez 10 minutes, connectez-vous à votre compte espace partenaires. Vos références seront synchronisées avec Salesforce CRM et le lien de référence sera rempli. En cas d’échec, le champ audit est rempli avec les informations d’erreur.

   1. De même, lorsque l’option **synchroniser avec l’espace partenaires** est définie sur **Oui**, si vous mettez à jour l’opportunité dans Salesforce CRM, les modifications sont synchronisées avec votre compte espace partenaires.

2. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement CRM Salesforce :

    1. Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.

    1. Dans le menu de gauche, sélectionnez **références** .

    1. Pour créer une nouvelle référence de covente à partir de l’espace partenaires, cliquez sur l’option « nouvelle offre ».

    1. Connectez-vous à votre environnement CRM Salesforce.

    1. Accédez à **opportunités ouvertes**. La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Salesforce CRM.

    1. Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Capture d’écran de la page d’opportunités Salesforce.":::

>[!NOTE]
>**Vous avez besoin d’aide pour le déploiement ?**
>Pour obtenir de l’aide pour le déploiement de votre connexion de covente, vous pouvez faire appel à un consultant technique partenaire. Ils peuvent fournir une assistance au déploiement et des méthodes recommandées pour une implémentation réussie.
>
>Pour plus d’informations, consultez [Comment soumettre une demande de services de déploiement et des préventes techniques](technical-benefits.md)

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)

- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)

- [Webhooks de l’Espace partenaires](/partner-center/develop/partner-center-webhooks)
