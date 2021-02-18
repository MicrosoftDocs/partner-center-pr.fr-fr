---
title: Connecteur de la co-vente pour Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchronisez les références dans l’espace partenaires avec votre connecteur de co-vente pour Dynamics 365 CRM. Les vendeurs peuvent ensuite se vendre avec Microsoft à partir de vos systèmes CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645705"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Connecteur de co-vente pour Dynamics 365 CRM-vue d’ensemble

### <a name="appropriate-roles"></a>Rôles appropriés

- Administrateur des références
- Administrateur système ou personnalisateur de système sur le CRM

Le connecteur de co-vente de l’espace partenaires permet à vos vendeurs de vendre leurs produits auprès de Microsoft à partir de vos systèmes CRM. Ils n’ont pas besoin d’être formés pour utiliser l’espace partenaires pour gérer les ventes de covente. Utilisez les connecteurs de covente pour créer une nouvelle référence de covente pour contacter un vendeur Microsoft, recevoir des références de la part du vendeur Microsoft, accepter/refuser des références, modifier les données de l’offre, telles que la valeur de la transaction et la date de clôture. Vous pouvez également recevoir toutes les mises à jour des vendeurs Microsoft sur ces offres de covente. Vous pouvez gérer toutes vos références dans le CRM de votre choix plutôt que dans l’espace partenaires. 

La solution est basée sur Microsoft Power Automated solution et utilise les API de l’espace partenaires.

## <a name="before-you-install---pre-requisites"></a>Avant d’installer-conditions préalables

|**Rubriques**   |**Détails**   |**Liens**   |
|--------------|--------------------|------|
|ID de Microsoft Partner Network |Vous avez besoin d’un ID MPN valide|Pour rejoindre [MPN](https://partner.microsoft.com/)|
|Covente prête|Votre solution IP/Services doit être prête à être covente.|[Vendre avec Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Compte Espace partenaires|L’ID MPN associé au locataire de l’espace partenaires doit être identique à l’ID MPN associé à votre solution de covente. Vérifiez que vous pouvez voir vos références de covente dans le portail espace partenaires avant de déployer les connecteurs.|[Gérer votre compte](create-user-accounts-and-set-permissions.md)|
|Rôles d’utilisateur de l’Espace partenaires|L’employé qui va installer et utiliser les connecteurs doit être un administrateur de références|[Affecter des rôles et des autorisations aux utilisateurs](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Le rôle d’utilisateur CRM est administrateur système ou personnalisateur système|[Affecter des rôles dans Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Gestion de l’alimentation-automatiser le compte|Créez un environnement de production avec une base de données pour le test, la mise en lots et la production. Si vous disposez déjà d’un environnement de production avec une base de données, vous pouvez le réutiliser. L’utilisateur qui va installer la solution connecteur doit avoir une licence Power automate et un accès à cet environnement. Vous pouvez surveiller la progression et obtenir plus de détails en cas d’échec de l’installation dans [Power automate](https://flow.microsoft.com/) en cliquant sur Afficher l’historique sous solutions.|[Créer ou gérer l’environnement](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installer la synchronisation des références de l’espace partenaires pour Dynamics 365 (solution Power automate)

1. Accédez à [Power automate](https://flow.microsoft.com) et sélectionnez **environnements** dans le coin supérieur droit. Cette étape vous montrera les instances CRM disponibles.

2. Sélectionnez l’instance CRM appropriée dans la liste déroulante dans le coin supérieur droit.

3. Sélectionnez **solutions** dans la barre de navigation de gauche.

4. Cliquez sur le lien **ouvrir AppSource** dans le menu supérieur.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Ouvrir AppSource":::

5. Recherchez les **connecteurs de références de l’espace partenaires pour Dynamics365** dans l’écran contextuel.  

6. Cliquez sur le bouton **Télécharger maintenant** , puis sur **Continuer**.

7. Cela ouvre la page dans laquelle vous pouvez sélectionner l’environnement CRM (Dynamics 365) pour installer l’application.  Acceptez les conditions générales.

8. Vous pouvez surveiller la progression et obtenir plus de détails en cas d’échec de l’installation dans Power automate en cliquant sur **afficher l’historique** sous **solutions**.
 

9. Une fois l’installation terminée, revenez à [Power automate](https://flow.microsoft.com) et sélectionnez **solutions** dans la zone de navigation de gauche. Notez que la **synchronisation des références de l’espace partenaires pour Dynamics 365** est disponible dans la liste des solutions.

10. Sélectionnez la **synchronisation des références de l’espace partenaires pour Dynamics 365**. Les flux et entités Power automate suivants sont disponibles :

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRM disponibles":::

## <a name="best-practice-test-before-you-go-live"></a>Meilleure pratique : testez avant de passer en direct

Avant d’installer, de configurer et de personnaliser la solution Power automate sur l’environnement de production, veillez à tester la solution sur une instance CRM intermédiaire.

- Installez Microsoft Power Automated solution sur un environnement intermédiaire/une instance CRM.
- Configurez et personnalisez la solution Microsoft Power Automated dans un environnement intermédiaire.
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

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Créer une connexion":::

      3. Recherchez les **références de l’espace partenaires (** préversion) dans la barre de recherche dans le coin supérieur droit.

      4. Créez une connexion pour votre utilisateur de l’espace partenaires avec le rôle informations d’identification de l’administrateur de références.

      5. Ensuite, créez une connexion des événements de l’espace partenaires pour votre utilisateur de l’espace partenaires avec les informations d’identification de l’administrateur des références.

      6. Créez une connexion pour Common Data Service (environnement actuel) pour l’utilisateur administrateur CRM.
     
      7. Une fois que toutes les connexions ont été ajoutées, vous devez voir les connexions suivantes dans votre environnement :

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Connexions":::
   
## <a name="edit-the-connections"></a>Modifier les connexions

1. Revenez à la page **solutions** et sélectionnez **solution par défaut**. Sélectionnez **référence de connexion (version préliminaire)** en cliquant sur **tout**.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Connexion":::

2. Modifiez chacune des connexions une par une en sélectionnant l’icône à trois points. Ajoutez les connexions appropriées.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Connexions listées"::: 

3.  Revenez à la page solutions, sélectionnez la synchronisation des références de l’espace partenaires pour Dynamics 365 et activez le Flow en cliquant sur l’icône à trois points en regard de chaque Flow dans l’ordre suivant. Si vous rencontrez des problèmes lors de l’activation du workflow, reportez-vous aux [étapes de personnalisation](connector-dynamics.md#customize-synchronization-steps) et aux [étapes de dépannage](connectors-troubleshoot.md). 

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

Les API de webhook de l’espace partenaires vous permettent de vous inscrire aux événements de changement de ressource. Ces événements de modification sont envoyés à votre URL en tant que messages HTTP.

1. Sélectionnez **espace partenaires sur Dynamics 365 (Insider Preview)**.

2. Sélectionnez l’icône **modifier** et sélectionnez le **moment où une requête HTTP est reçue**.

3. Sélectionnez l’icône de **copie** pour copier l’URL http postale fournie.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copier l’URL":::

4. Maintenant, sélectionnez l’option inscription à un webhook de l’espace partenaires (version préliminaire d’Insider) et sélectionnez **exécuter**.

5. Vérifiez que la fenêtre « exécuter le workflow » s’affiche dans le volet de droite, puis cliquez sur **Continuer**.

6. Entrez les informations suivantes :

   - **Point de terminaison du déclencheur http**: URL copiée à partir de l’étape précédente

   - **Événements à inscrire**: sélectionnez tous les événements disponibles (« créé avec la référence », « référence-mis à jour », « associé-référence-créé », « relation-référence-mis à jour »)

   -**Remplacer les points de terminaison déclencheurs existants, le cas échéant**: Oui il est important de noter qu’une seule URL peut être inscrite pour un événement webhook donné. Il est important de noter qu’une seule URL peut être inscrite pour un événement webhook donné. 

7. Sélectionnez **exécuter** , puis sélectionnez **terminé.**

Le webhook peut maintenant écouter les événements de création et de mise à jour.

## <a name="customize-synchronization-steps"></a>Personnaliser les étapes de synchronisation

Les systèmes CRM sont hautement personnalisés, et vous pouvez personnaliser la solution Power automate en fonction de votre configuration de CRM.  Lorsque les références de covente sont synchronisées entre l’espace partenaires et votre système CRM, les champs qui sont synchronisés sur le PC de l’espace partenaires sont répertoriés dans le [Guide de mappage de champs personnalisé](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Suivez le Guide de mappage de champs et, si nécessaire, apportez les modifications nécessaires dans **[personnaliser] créer ou récupérer des détails à partir de variables d’environnement ou de fluide Dynamics 365**  . Il est recommandé de ne pas mettre à jour d’autres flux dans Power Automated solution, car cela peut avoir un impact sur les futures mises à niveau de solutions. 

Les personnalisations disponibles sont les suivantes :

- Coche dans nom de l’opportunité : par défaut, une coche s’affiche en regard du nom de l’opportunité pour indiquer que la synchronisation entre le Centre des partenaires et Dynamics 365 CRM s’est déroulée correctement. De même, une croix est affichée si la synchronisation échoue. Pour éviter l’ajout de la vérification ou de la Croix dans le nom de l’opportunité, définissez la valeur actuelle de l’option Afficher la coche dans la variable d’environnement nom de l’opportunité sur non.

- Valeur de la transaction : par défaut, la valeur de transaction de l’espace partenaires sera synchronisée vers et à partir de **estimatedvalue** dans CRM. Si vous avez un champ différent dans CRM pour la synchronisation de la valeur de transaction :

    a.    Mettez à jour le nom du champ de valeur de contrat dans la variable d’environnement Dynamics 365 avec le nom de champ de CRM. Notez que vous devez fournir le nom du champ comme nom d’affichage.

    b.    Modifiez **[personnaliser] créer ou obtenir des détails à partir de Dynamics 365 Flow**  et accédez à **créer ou mettre à jour** une opportunité dans CRM et à mettre à jour **créer une nouvelle opportunité** et mettre à jour des actions d' **opportunité existantes** pour affecter la valeur **DealValue** au champ approprié dans CRM. En outre, supprimez l' **affectation DealValue** du champ **revenu estimé** .

- Code du pays du compte client : il est obligatoire de fournir un code de pays à deux lettres (ISO 3166) lors de la création d’une nouvelle référence. Par défaut, l’indicatif du pays sera synchronisé à partir du champ address1_country du compte dans CRM. Si vous avez un champ différent dans CRM pour le code de pays à synchroniser :

   a.    Pour un champ de code de pays non-recherche dans le compte qui contient le code à deux lettres :

   - Mettez à jour le nom du champ de code du pays du compte client dans la variable d’environnement Dynamics 365 avec le nom de champ de CRM. Notez que vous devez fournir le nom du champ comme nom d’affichage.

   - Modifiez **[personnaliser] créez ou récupérez des détails à partir de Dynamics 365 Flow**  , puis accédez à créer ou à accéder à un compte client dans une action CRM pour affecter la valeur de pays au champ approprié dans CRM. En outre, supprimez l’affectation de valeur de pays du champ adresse 1 : pays/région.

   b.    Pour un champ Code de pays basé sur la recherche dans compte :

   - Ajoutez un nouveau champ personnalisé dans compte et remplissez-le automatiquement avec un code de pays à deux lettres (ISO 3166) en fonction de la valeur sélectionnée dans champ de recherche et vice versa.

   - Suivez les étapes ci-dessus pour le champ Code pays de non-recherche pour synchroniser le nouveau champ personnalisé de CRM vers et depuis l’espace partenaires.

- Champs d’opportunité : si les champs obligatoires de l’opportunité doivent être remplis, modifiez **[personnaliser] créer ou obtenir des détails à partir du Flow Dynamics 365**  , puis accédez à **créer ou mettre à jour l’opportunité** dans CRM et à mettre à jour **créer une nouvelle action d’opportunité** pour affecter des valeurs aux champs obligatoires en fonction des besoins de votre entreprise.

- Champs de Prospect : si les champs obligatoires du prospect doivent être remplis, modifiez **[personnaliser] créer ou obtenir des détails à partir du Flow Dynamics 365**  , puis accédez à **créer ou mettre à jour le prospect** dans CRM et à mettre à jour **créer une action Prospect** pour affecter des valeurs aux champs obligatoires en fonction des besoins de votre entreprise.

- Compte client : quand une nouvelle référence est synchronisée de l’espace partenaires vers CRM, la solution Power automate tente de rechercher un compte existant dans CRM à l’aide du nom de la société client et du code postal. S’il n’en trouve pas, un nouveau compte client est créé dans CRM. Pour mettre à jour les critères de recherche et les nouveaux détails de création de compte, modifiez **[personnaliser] créer ou extraire des détails à partir de Dynamics 365 Flow** , puis accédez à **créer ou à accéder au compte client** dans CRM et à **créer une action de compte client**.

## <a name="update-environment-variable"></a>Mettre à jour la variable d’environnement

Pour mettre à jour une valeur de variable d’environnement :

1. Accédez à la page **solutions** et sélectionnez **solution par défaut**. Sélectionnez **variable d’environnement** en cliquant sur tout.

2. Sélectionnez la variable d’environnement correspondant à la valeur qui doit être mise à jour, puis cliquez sur le bouton **modifier** à l’aide de trois points.

3. Mettez à jour la **valeur actuelle** (ne pas mettre à jour la valeur par défaut) à l’aide de l’option **nouvelle valeur** et fournissez la valeur. La valeur doit correspondre au type de données de la variable pour, par exemple, le type de données yes/no accepte la valeur Yes ou no.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Zone d’édition pour les valeurs par défaut":::

- Synchronisation bidirectionnelle de la direction de la co-vente de bout en bout

Une fois que vous avez installé, configuré et personnalisé la solution Power automate, vous pouvez tester la synchronisation des références de covente entre Dynamics 365 et l’espace partenaires.

### <a name="pre-requisites"></a>Conditions préalables

Pour synchroniser les références entre l’espace partenaires et Dynamics 365 CRM, la solution Power automate délimite clairement les champs de référence propres à Microsoft. Cette identification permet aux équipes de vendeur de décider des références qu’elles souhaitent partager avec Microsoft pour la covente.

Un ensemble de champs et d’objets personnalisés sera ajouté dans le cadre de l’installation de la solution. Un utilisateur administrateur CRM devra créer une section CRM distincte avec les champs personnalisés d' **opportunité** .

Les champs personnalisés suivants doivent faire partie de la section CRM :

- **Synchroniser avec l’espace partenaires**: s’il faut synchroniser l’opportunité avec l’espace partenaires Microsoft. Par défaut, la valeur de ce champ est non et doit être explicitement définie sur Oui par le vendeur pour partager une opportunité avec Microsoft. La valeur de ce champ est définie sur Oui pour les nouvelles références partagées entre l’espace partenaires et CRM.

- **Identificateur de référence**: champ d’identificateur en lecture seule pour la référence de l’espace partenaires Microsoft

- **Lien de référence**: lien en lecture seule vers la référence dans l’espace partenaires Microsoft
- **Comment Microsoft peut**-il vous aider ?: aide requise de Microsoft pour la référence. Pour créer une référence de covente, sélectionnez l’aide appropriée requise de Microsoft. Un contact client doit être associé à la possibilité de créer une référence de covente. Pour créer une référence de non-vente, laissez ce champ non sélectionné. Une référence de non-vente peut être convertie en référence de covente à tout moment en sélectionnant l’option aide appropriée requise.

- Visibilité de la référence de l' **espace partenaires Microsoft**: sélectionnez visibilité pour la référence de l’espace partenaires Microsoft. En le rendant visible pour les vendeurs Microsoft, une référence de non-vente peut être convertie en covente. Lorsque l’aide Microsoft est requise, la référence est visible par défaut pour les vendeurs Microsoft. Une fois marqué comme visible, ce champ ne peut pas être rétabli.

- **Identificateur Microsoft CRM**: quand une référence de covente est créée et acceptée par Microsoft, ce champ est renseigné avec l’identificateur Microsoft CRM.

- **Produits : obsolètes** : n’utilisez pas ce champ ou ajoutez-le à la section CRM. il est disponible uniquement à des fins de compatibilité descendante. Utilisez les solutions de l’espace partenaires Microsoft à la place.

- **Audit**: piste d’audit en lecture seule pour la synchronisation avec les références de l’espace partenaires

- **Solutions de l’espace partenaires Microsoft**: objet personnalisé pour associer des solutions prêtes pour la co-vente ou des solutions Microsoft avec l’opportunité. Une ou plusieurs solutions peuvent être ajoutées et/ou supprimées de l’opportunité. Il est obligatoire d’ajouter au moins une solution de covente prête ou Microsoft à l’occasion avant de la partager avec Microsoft. Pour associer cet objet à l’opportunité, mettez à jour le formulaire d’opportunité dans CRM :

  Sélectionnez l’onglet approprié dans formulaire d’opportunité et ajoutez une sous-grille comme indiqué ci-dessous :

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Formulaire d’opportunité":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Après avoir ajouté des solutions Microsoft, vous pouvez préremplir les détails des solutions de covente pour que vos vendeurs n’aient pas à les ajouter. Pour ajouter un nouveau détail de solution, accédez à l’objet détails de la solution Microsoft dans CRM, puis cliquez sur **Ajouter un enregistrement** pour ajouter une entrée ou utiliser le **Téléchargement Excel** pour ajouter plusieurs entrées.

:::image type="content" source="images/dynamic-1a.png" alt-text="Détails de la solution":::

### <a name="scenarios"></a>SCÉNARIO

1. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans CRM et synchronisée dans l’espace partenaires :

   1. Connectez-vous à votre environnement Dynamics 365 CRM avec un utilisateur qui dispose de la visibilité dans la section **opportunité** de CRM.

   2. Vérifiez que la section Microsoft Partner Center est présente lorsque vous créez une « nouvelle opportunité » dans l’environnement Dynamics 365

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nouvelle opportunité"::: 

   3. Pour synchroniser cette opportunité avec l’espace partenaires, veillez à définir les champs suivants dans la vue de la carte :

      - **Comment Microsoft peut-il vous aider ?**: pour créer une référence de covente, sélectionnez une option d’aide appropriée.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Comment obtenir les champs appropriés dans la vue carte":::

      - **Contact client**: pour créer une référence de covente, ajoutez un contact client à l’opportunité.
      - **Synchroniser avec l’espace partenaires**: Oui

      - Solutions Microsoft : pour partager une référence avec Microsoft, ajoutez une solution de covente prête ou Microsoft à vos opportunités.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="ID de solution":::

   4. Une fois que l’opportunité est créée dans Dynamics 365 avec l’option synchroniser avec l’espace partenaires définie sur Oui, patientez 10 minutes, puis connectez-vous à votre compte espace partenaires. Vos références seront synchronisées avec Dynamics 365 et l’identificateur de référence. Le lien de référence sera rempli. En cas de défaillance, le champ audit est rempli avec les informations d’erreur.
     
    5. De même, pour une opportunité avec l’option « synchroniser avec l’espace partenaires » définie sur « Oui », si vous mettez à jour l’opportunité dans Dynamics 365 CRM, les modifications sont synchronisées dans votre compte espace partenaires.

    6. Les opportunités qui sont synchronisées avec succès avec l’espace partenaires sont identifiées avec l’icône ✔ dans Dynamics 365.

2. Synchronisation de la référence lorsque la référence est créée ou mise à jour dans l’espace partenaires Microsoft et synchronisée dans l’environnement Dynamics 365 :

   1. Connectez-vous à votre [tableau de bord](https://partner.microsoft.com/dashboard/home)de l’espace partenaires.

   2. Dans le menu de gauche, sélectionnez **références** .

   3. Pour créer une nouvelle référence de covente à partir de l’espace partenaires, sélectionnez l’option  **nouveau contrat** .

   4. Connectez-vous à votre environnement Dynamics 365 CRM.

   5. Accédez à **opportunités ouvertes**. La référence créée dans l’espace partenaires Microsoft est maintenant synchronisée dans Dynamics 365 CRM.

   6. Lorsque vous sélectionnez une référence synchronisée, les détails de l’affichage de la carte sont remplis.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)

- [Gérer les opportunités de covente](manage-co-sell-opportunities.md)

- [En savoir plus sur la plateforme Microsoft Power Automated ?](/power-automate/)

- [Webhooks de l’Espace partenaires](/partner-center/develop/partner-center-webhooks)