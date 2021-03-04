---
title: Migrer à partir de Partner vente Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires Microsoft peuvent migrer de Partner Sales Connect (PSC) vers l’espace partenaires et créer ou gérer des transactions envoyées par les vendeurs Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 84863e96278ba17ecc9922ff9589abc504ff1fe0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756176"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guide de la co-vente dans l’espace partenaires (PC) pour les partenaires qui migrent à partir de Partner vente Connect (PSC)

**Rôles appropriés**

- Administrateur des comptes
- Administrateur des références
- Vendeur Partner Sales Connect (PSC)
- Administrateur Partner Sales Connect (PSC)
- Responsable des ventes Partner Sales Connect (PSC)

Cet article fournit des conseils pour les partenaires qui effectuent des migrations de Partner Sales Connect vers l’espace partenaires afin qu’ils puissent continuer à créer et à gérer les ventes de covente dans l’espace partenaires.

>[!Note]
> Si vous êtes ici, car vous avez vu une bannière dans PSC sur la migration, vous êtes au bon endroit. Ce guide n’est pas applicable pour les partenaires commerciaux d’évaluation de la solution (SA) et de licence OEM qui gèrent leurs demandes dans PSC.

>[!Important]
> À partir du 1er mai, 2021 votre entreprise ne sera pas en mesure de créer ou de modifier des transactions dans le PSC. **Vous serez toujours en mesure de télécharger les données de transactions existantes à l’aide de la fonctionnalité d’exportation en bloc dans PSC. Vous pouvez également [migrer les transactions ouvertes](psc-to-pc.md#psc-deals-migration) de PSC vers l’espace partenaires après cette date.** <br><br> Si vous travaillez activement avec des demandes qui contiennent des solutions éligibles pour la co-vente IP, vous avez deux options : <br><br> 1. Marquez le contrat comme conclu et terminez l’enregistrement du contrat dans le PSC avant le 30 avril 2021. <br> 2. [migrez les demandes](psc-to-pc.md#psc-deals-migration) d’accès à l’espace partenaires pour obtenir plus de temps pour travailler sur le contrat et pour commencer à enregistrer votre contrat.

Comme vous le savez, **l’entreprise perdra l’accès au PSC après le 31 mai, 2021**. Toutefois, vous trouverez tout ce que vous souhaitez faire dans l’espace partenaires, par exemple créer des offres de covente, gérer vos demandes et agir sur les transactions que les vendeurs Microsoft vous ont envoyées.

Toutefois, il y aura des différences. Les conseils suivants peuvent vous aider à rendre votre transition vers l’espace partenaires plus lisse et plus simple.

## <a name="before-you-move-things-you-need-to-know"></a>Avant de vous déplacer, vous devez connaître les points suivants

### <a name="if-you-are-a-psc-admin"></a>Si vous êtes un administrateur PSC

- Vous avez besoin d’un e-mail professionnel pour vous connecter à l' [espace partenaires](https://partner.microsoft.com/).
- Configurez votre compte à l’aide de l' [administrateur de compte](permissions-overview.md)de l’espace partenaires.
- Découvrez comment vendre en collaboration dans l’espace partenaires en lisant ce document.
- Configurez des comptes d’utilisateur dans l’espace partenaires pour tous les utilisateurs du PSC (rôles administrateur, gestionnaire des affaires et vendeur) et attribuez-leur des [rôles d’administrateur de référence](permissions-overview.md).

>[!IMPORTANT]
> Assurez-vous que l’ID MPN affiché dans la bannière du PSC est disponible dans la liste des emplacements MPN dans l’espace partenaires.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Image représentant la bannière du PSC dans laquelle les partenaires peuvent trouver l’ID MPN.":::

 Pour vérifier que l’ID MPN apparaît en tant qu’emplacement MPN de l’espace partenaires, connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires, puis sélectionnez **paramètres** (l’icône d’engrenage) en haut à droite de l’écran, suivi des **paramètres de compte**. Dans le menu de navigation de gauche et de deuxième niveau, sélectionnez **Locations (emplacements** ) pour afficher la liste de tous les ID et emplacements MPN associés au compte de l’espace partenaires.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Si vous êtes un responsable des ventes ou un vendeur PSC

- Vous avez besoin d’un e-mail professionnel pour vous connecter au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.
- Si vous utilisez un compte non professionnel dans PSC ou si votre adresse de messagerie professionnelle est destinée à une société différente de celle de l’entreprise partenaire, contactez votre administrateur PSC pour obtenir de l’aide sur l’installation du compte.
- Vérifiez auprès de votre administrateur PSC si la configuration de votre compte espace partenaires est terminée, quel que soit le compte que vous utilisez pour vous connecter à PSC.
- Vérifiez si vous avez accès à l’espace partenaires et à la section Références.
- Lisez ce document pour comprendre les flux de travail et les modifications apportées à l’espace partenaires.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>En tant qu’administrateur dans PSC, Voici les étapes suivantes

Dans le menu de navigation de gauche de l’espace partenaires, sélectionnez l’option **références** . Confirmez que vous pouvez accéder aux pages de références.

  >[!Note]
  > Vous devrez peut-être vous déconnecter de l’espace partenaires et vous reconnecter pour actualiser vos informations d’identification afin d’accéder aux pages de références.

Si vous ne voyez pas l’option **références** dans le menu de l’espace partenaires ou les pages liées aux références, contactez l' [administrateur du compte](permissions-overview.md) de votre entreprise et demandez-lui de vous permettre d’accéder à l’option **références** et à la zone associée.

Pour trouver l’administrateur de compte de votre société :

1. Sélectionnez **paramètres du compte** à partir de l’icône d’engrenage en haut à droite du tableau de bord de l’espace partenaires.

1. Sélectionnez **gestion des utilisateurs** dans le menu de navigation de second niveau de gauche.

1. En haut de la liste des utilisateurs, sélectionnez le menu déroulant **filtre** . Remplacez l’option par **admin de compte**.

   La page affiche tous les administrateurs de comptes avec leurs adresses e-mail respectives. Envoyez un e-mail à l’un d’eux et demandez-lui d’attribuer le rôle d’administrateur de références pour votre compte professionnel.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Image représentant les administrateurs de comptes dans la page de gestion des utilisateurs paramètres du partenaire.":::

>[!Important]
>- Si votre rôle implique uniquement la gestion des utilisateurs dans PSC, demandez à l’administrateur de compte de votre entreprise de vous attribuer le rôle d' [administrateur de compte](permissions-overview.md#manage-mpn-membership-and-your-company) dans l’espace partenaires. 
>- Si votre rôle comprend également la gestion des opportunités de covente, demandez à être affecté au rôle d' [administrateur de références](permissions-overview.md#manage-referrals) .
> - Il est judicieux de nommer également un chef de gestion des modifications parmi les administrateurs PSC. Cela empêchera tous les administrateurs du PSC d’avoir à accéder individuellement aux administrateurs de compte de l’espace partenaires. Au lieu de cela, le responsable de la gestion des modifications peut être la principale personne travaillant avec l’administrateur de compte de l’espace partenaires.

## <a name="user-migration"></a>Migration utilisateur

Une fois votre compte configuré dans l’espace partenaires, utilisez l’Assistant Migration des utilisateurs de la page opportunités de covente pour affecter automatiquement des rôles de l’espace partenaires aux employés de votre entreprise.

>[!Note]
> La migration des utilisateurs ne peut être effectuée que par les [administrateurs de compte](permissions-overview.md#manage-mpn-membership-and-your-company) de votre entreprise. Si vous n’avez pas le rôle d’administrateur de compte, recherchez un administrateur de compte qui peut vous aider à configurer les comptes d’utilisateur à l’aide de l’Assistant Migration des utilisateurs.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Image représentant l’Assistant Migration des utilisateurs.":::

Les administrateurs de comptes verront un lien de l’Assistant Migration des utilisateurs PSC dans la page opportunités de covente à côté du Guide de références. Ils peuvent lancer la migration des utilisateurs en sélectionnant le lien. Pour initier la migration de l’utilisateur, les administrateurs peuvent sélectionner le lien. Ils peuvent effectuer cette étape de migration utilisateur plusieurs fois jusqu’à ce que tous les utilisateurs aient des rôles appropriés dans l’espace partenaires.

La table de migration utilisateur contient les informations suivantes :

- Compte d’utilisateur : ID d’E-mail de l’employé
- Compte de partenaire PSC : compte auquel l’employé est associé dans PSC
- Rôle d’utilisateur PSC : l’un des trois rôles affectés à dans le PSC.
- Emplacement MPN du PC : emplacement pour lequel l’utilisateur recevra des rôles d’ordinateur pertinents. Le compte MPN de partenaire PSC est utilisé pour trouver l’emplacement MPN équivalent dans l’espace partenaires pour affecter des autorisations. L’ensemble de l’organisation indique l’ID MPN vOrg.
- Rôle d’utilisateur PC : les employés se voient attribuer des rôles en fonction de leurs rôles d’utilisateur PSC. L’administrateur du PSC se verra attribuer des rôles d’administrateur de références dans PC. Le rôle d’utilisateur de références sera attribué au vendeur dans PC. En savoir plus sur les rôles de PC et les utilisateurs avec ces rôles peuvent effectuer cette opération dans l’espace partenaires [ici](permissions-overview.md#manage-referrals)
- Client AAD de PC : locataire auquel les utilisateurs sont attribués dans l’espace partenaires
- État : il existe trois États possibles pour l’état de la migration.
    - **Non migré** -l’utilisateur n’a pas de rôle de références de PC affecté
    - **Migration** effectuée-l’utilisateur a été migré avec le rôle approprié affecté comme indiqué dans le tableau
    - **Erreur** : impossible de terminer la migration en raison d’une erreur

Parfois, la migration peut échouer et provoquer des erreurs. Voici quelques raisons pour lesquelles une migration peut provoquer une erreur et certaines des façons de résoudre le problème :

1. Les utilisateurs du PSC utilisent peut-être un compte non professionnel.

2. L’utilisateur PSC peut utiliser un compte d’un domaine différent de celui que vous utilisez dans l’espace partenaires.

   Pour résoudre les erreurs liées aux scénarios 1 et 2, demandez à l’utilisateur de se connecter à l’espace partenaires à l’aide de son compte professionnel associé à votre locataire Azure AD. Votre [administrateur général](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) peut vous aider.
   
   Pour trouver votre administrateur général : 
   - Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’espace partenaires et sélectionnez les **paramètres de compte** à partir de l’icône d’engrenage en haut à droite.
   - Sélectionnez **gestion des utilisateurs** dans la barre de navigation gauche de second niveau.
   - En haut de la liste des utilisateurs, sélectionnez le menu déroulant **filtre** et remplacez l’option par **administrateur général**. La page affiche ensuite tous les administrateurs globaux avec leurs adresses e-mail respectives. Demandez à l’un d’eux d’attribuer le rôle d’administrateur de référence pour votre compte professionnel.
   
      L’administrateur général peut créer un nouveau compte d’utilisateur dans votre client Azure AD ou attribuer à un utilisateur invité l’accès aux autres utilisateurs du compte de domaine. Une fois les comptes configurés pour tous les responsables et les utilisateurs du PSC, ils doivent se connecter à l’espace partenaires, sélectionner des **références** dans le menu de navigation de gauche et confirmer qu’ils peuvent voir la page références.

3. Un rôle de référence est déjà attribué à l’utilisateur dans l’espace partenaires.
    - Vous pouvez vérifier le rôle existant de l’utilisateur. Dans l’angle supérieur droit de l’espace partenaires, sélectionnez **paramètres** (l’icône d’engrenage), puis **paramètres de compte**. Quand vous voyez un deuxième menu de navigation à gauche, sélectionnez **gestion des utilisateurs** et recherchez l’utilisateur.

## <a name="psc-deals-migration"></a>Migration des contrats PSC

Une fois que vous avez terminé la migration des utilisateurs, utilisez l’Assistant Migration des offres dans la page opportunités de covente pour mettre toutes les transactions ouvertes éligibles de PSC à PC. **Le lien de migration de contrats sera visible uniquement les administrateurs de référence avec une étendue d’organisation entière dans l’espace partenaires.** Un lien nommé **« migration des affaires PSC »** s’affiche en haut à droite de la page opportunités de covente, qui ouvre l’Assistant Migration des transactions.

Lisez cette section avant de commencer la migration de la transaction.

**Éligible pour la migration**

Seules certaines affaires sont éligibles pour la migration de PSC vers PC. Cet Assistant de migration est conçu pour aider les partenaires à apporter leurs offres à l’espace partenaires dans lequel ils travaillent toujours activement avec leurs clients pour conclure le contrat. **Seules les demandes qui sont à l’état ouvert créées à partir du 1er janvier 2020 avec des détails de compte de partenaire valides (ID MPN valide) et qui ne sont pas en cours d’inscription sont éligibles pour la migration.**

**Non éligible pour la migration**

- Les contrats d’évaluation de solution ne sont pas éligibles pour la migration des contrats
- Les contrats de licence OEM ne sont pas éligibles pour la migration des contrats
- Toute transaction marquée comme conclue dans le PSC n’est pas éligible pour la migration. L’enregistrement de la transaction s’il est éligible pour les transactions marquées comme conclues doit être effectué dans le PSC.

## <a name="pre-requisites-for-deal-migration"></a>Conditions préalables à la migration des transactions

Avant de commencer la migration des contrats à partir du PC, suivez les instructions ci-dessous pour configurer les transactions dans le PSC en vue d’une migration réussie.

1. Tous les membres de l’équipe des ventes de votre entreprise qui travaillent sur les contrats ouverts sont informés de cette migration.
2. Les membres de l’équipe des ventes sont formés pour utiliser l’espace partenaires pour la gestion des transactions.
3. Le traite de toutes les informations requises, comme décrit ci-dessous.
    - Détails de la société client, y compris le nom et l’adresse
    - Coordonnées du client s’il s’agit d’une vente de covente
    - Au moins une solution
    - Au moins un membre de l’équipe avec tous les détails (prénom, nom, ID de courrier électronique et numéro de téléphone).
    - Valeur de la transaction
    - Date de fermeture de la transaction estimée
    - Notes du partenaire

Vous pouvez utiliser les fonctionnalités de téléchargement et de chargement en bloc dans PSC pour ajouter tous les détails manquants dans le contrat pour toutes les transactions éligibles.

>[!Note]
> La migration de la transaction échouera même si les conditions préalables ci-dessus ne sont pas remplies. Toutefois, vous ne pouvez pas modifier l’état de la transaction si l’un des champs requis mentionnés ci-dessus dans l’espace partenaires n’est pas disponible. Vous devrez ensuite entrer toutes les informations requises manquantes dans les offres de l’espace partenaires pour commencer à travailler dessus. **Il est vivement recommandé de nettoyer les demandes éligibles du PSC avant de les migrer vers l’espace partenaires.**

La migration des transactions dans l’espace partenaires s’appuie sur une expérience unique. Il vous suffit de cliquer sur le bouton **« migrer les offres »** une fois que votre entreprise est prête à migrer les demandes éligibles. **Vous ne pouvez pas choisir les contrats que vous souhaitez migrer à partir de PSC. Si vous ne souhaitez pas migrer des transactions vers l’espace partenaires, déplacez-les à l’état fermé dans le PSC avant de commencer la migration.**

>[!Note]
> Après l’initialisation de la migration, **la migration des demandes peut prendre jusqu’à 24 heures**.

Une fois la migration terminée, l’état du message de la bannière est changé pour se terminer avec un lien vers le rapport de migration. Téléchargez le rapport pour afficher les détails des transactions qui ont été migrées de PSC à PC.

Le rapport contient les détails ci-dessous.

1. **ID d’engagement de l’espace partenaires** : identificateur unique dans l’espace partenaires pour toutes les transactions d’un engagement. Il existe deux contrats : un pour le partenaire et un pour Microsoft dans un engagement de covente dans l’espace partenaires.
2. **ID de référence de l’espace partenaires** : identificateur unique dans l’espace partenaires pour la transaction appartenant au partenaire.
3. **Nom** de la transaction : identificateur donné au contrat du COPS.
4. **ID de contrat PSC** : identificateur unique dans le PSC pour le contrat.
5. **Erreurs** : pour indiquer s’il y a une erreur lors de la migration d’une transaction spécifique.

Toutes les transactions qui ont été migrées avec succès ne seront pas visibles dans le PSC. Vous pouvez continuer à travailler sur les contrats migrés sur PC, y compris pour terminer l’inscription des transactions sur PC. Aucune modification n’est apportée aux interactions avec les vendeurs Microsoft pour les ventes de covente.

Les offres migrées à partir de PSC seront disponibles dans les onglets entrant et sortant en fonction de la source de la transaction. Toutes les transactions partagées par votre entreprise sont disponibles sous l’onglet sortant et les offres engagées par Microsoft sont disponibles dans l’onglet entrant de l’espace partenaires. Il y aura deux types de transactions qui seront créées après la migration.

1. **Ventes de covente** : les demandes qui sont marquées comme covente dans PSC sont créées en tant que ventes de covente dans l’espace partenaires.
2. Transactions **dirigées** par un partenaire : les demandes qui ne sont pas marquées comme covente sont créées en tant que contrats dirigés par un partenaire dans l’espace partenaires. Les offres dirigées par un partenaire sont visibles par les vendeurs Microsoft et peuvent être mises à niveau pour vendre leurs offres avant d’atteindre l’état des terminaux (gagnés, perdus). En outre, les contrats menés par un partenaire sont éligibles à l’enregistrement de la transaction s’il existe une solution incitative dans le contrat.

>[!Important]
> Si des erreurs se sont produites en raison de l’impossibilité de migrer certaines affaires, **vous pouvez relancer la migration de la transaction en cliquant sur le bouton « migrer les contrats »**. Il sera activé uniquement s’il existe des transactions éligibles à migrer. Cela sera également utile si vous êtes dans la phase de transition où de nouvelles transactions sont créées dans le PSC après le lancement de la migration de la transaction.

Une fois que toutes les transactions ont été migrées avec succès, il y a une bannière qui indique **« aucune opération de migration »** avec le bouton **« migrer les transactions »** **désactivé**.

Après avoir effectué la migration des utilisateurs et/ou la migration des transactions, suivez les instructions ci-dessous pour déterminer la stratégie de migration :

Si votre entreprise dispose d’un responsable de développement partenaire (PDM) : lorsque votre compte de l’espace partenaires est configuré et que vos utilisateurs ont passé des rôles et des autorisations, vous pouvez déplacer vos activités de covente vers l’espace partenaires. Informez le système PDM d’effectuer le commutateur au lieu de patienter jusqu’à la fin de l’échéance de la migration, ce qui permettra à tous vos nouveaux contrats d’être transmis à l’espace partenaires.

>[!Note]
>Une fois ce commutateur effectué, vous ne pourrez agir que sur les transactions actives existantes dans le PSC. Vous ne pouvez pas créer de nouvelles demandes ni recevoir de transactions de la part de vendeurs Microsoft dans PSC.

Si votre entreprise n’a pas de PDM, assurez-vous que tous les comptes d’utilisateur sont configurés et vérifiés par tous les utilisateurs. Vous recevrez une notification par courrier électronique et une bannière dans le PSC indiquant la date exacte à laquelle vous pouvez commencer à vendre des produits dans l’espace partenaires. N’oubliez pas que vous devrez toujours gérer les transactions actives existantes dans le PSC.

>[!Important]
> Vous avez jusqu’au 30 avril 2021 pour inscrire les demandes qui sont marquées comme conclues.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Étapes suivantes pour les administrateurs PSC, les responsables des affaires PSC et les vendeurs de PSC

Découvrez comment vendre des produits dans l’espace partenaires.
Il s’agit d’une étape importante, qui vous aidera à préparer la covente dans l’espace partenaires. Comprenez les flux de travail et les modifications apportées à l’espace partenaires pour que vous puissiez effectivement covendre immédiatement. Commencez par lire ce document entièrement. Un bon ensemble de ressources est également disponible dans la [Galerie d’expérience de la co-vente](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principales différences entre les flux de travail des PSC et des PC

|**Scénario**|**Vente des partenaires**|**Espace partenaires**|
|-----|:-----|:-----|
|Rôles d'utilisateur|PSC a des rôles d’administrateur, de responsable des transactions et de vendeur.|PC dispose uniquement d’un rôle d' [administrateur de référence](permissions-overview.md#manage-referrals) qui donne des autorisations en lecture et en écriture pour toutes les transactions.|
|Invitation à Microsoft sur un contrat de covente|Initié par Microsoft seller, il n’y a pas de demande explicite de partenaire.|Le partenaire devra faire une [demande explicite](manage-co-sell-opportunities.md#add-solutions) si une aide du vendeur Microsoft est nécessaire pour une affaire. Le vendeur Microsoft dispose d’une option pour refuser la demande.|
|Expiry|Il n’existe aucun concept d’expiration de la transaction.|Les contrats de contrats entrants du partenaire expirent dans 14 jours s’ils ne sont pas acceptés par le partenaire. Il en est de même pour les contrats de partenariat sortants où ils peuvent passer à l’État expiré si le vendeur Microsoft n’agit pas sur ceux-ci dans un délai de 14 jours.|
|Détails du vendeur Microsoft|Visible dès qu’une transaction est créée.|Les détails du vendeur Microsoft sont partagés avec le partenaire uniquement si le vendeur accepte expressément l’invitation pour la co-vendre du partenaire.|
|[Pipeline privé](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Non disponible.|Les partenaires peuvent partager leur pipeline sans donner de visibilité aux vendeurs Microsoft.|
|Solutions|Les solutions appartenant à une seule liste de prix peuvent être ajoutées à un contrat.|Le partenaire peut ajouter des [solutions](manage-co-sell-opportunities.md#add-solutions) qui appartiennent aux listes suivantes. a) leurs propres solutions b) à partir du catalogue Microsoft First Party (semblable au rôle transaction de transaction dans PSC) et c) coventent les solutions d’autres partenaires tiers (semblable au rôle Dealer ISV dans PSC).|
|Attribution des transactions|Seul le vendeur affecté peut afficher et agir sur les transactions.|Les membres de l’équipe peuvent être ajoutés à un contrat pour spécifier les personnes qui travaillent sur une transaction, il n’y a aucun blocage d’autres administrateurs de la référence pour afficher ou agir sur ces transactions.|
|Organisation cliente|Entrée de texte de forme libre.|Vous pouvez effectuer une recherche dans l' [organisation cliente](manage-co-sell-opportunities.md#select-your-customer) par rapport à la [base de données D&B](https://www.dnb.com/) en tapant simplement quelques caractères. Le nom et l’adresse légaux sont renseignés automatiquement en fonction du choix.|
|Contact client|Non obligatoire.|Non obligatoire pour le partage de pipeline privé. Obligatoire si Microsoft seller est invité à participer à une demande de covente.|
|API publique|Non disponible.|[API publique](/partner/develop/referrals) permettant de gérer par programmation les références de l’espace partenaires.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapper les champs dans le PSC aux champs correspondants dans l’espace partenaires

Cette section compare (ou « mappe ») les captures d’écran sélectionnées indiquées pour le PSC à la vue correspondante dans la section opportunités de co-vente de l’espace partenaires.

Vous verrez des cercles numérotés, jaunes ou rouges sur chaque paire de captures d’écran :

- **Signification des cercles jaunes** Numérotées, les cercles jaunes apparaissent en premier sur chaque capture d’écran du PSC. Vous trouverez ensuite une capture d’écran de l’espace partenaires en dessous avec un grand nombre des mêmes chiffres.

   Pour voir comment chaque champ ou attribut du PSC est mappé à son équivalent dans l’espace partenaires, associez les cercles numérotés dans les deux captures d’écran associées. Par exemple, faites correspondre le chiffre, jaune « 1 » dans la première capture d’écran du PSC, au numéro « 1 » jaune dans la seconde, la capture d’écran de l’espace partenaires ci-dessous.

- **Signification d’un cercle rouge** Si vous voyez un cercle rouge dans une capture d’écran, cela indique que le champ PSC n’est pas disponible dans l’espace partenaires.

Les mappages de champs du centre PSC à partenaire sont affichés pour les domaines suivants :

1. Page d’hébergement du PSC mappée à l’affichage par défaut opportunités de co-vente de l’espace partenaires
1. Vue de grille du PSC mappée à l’affichage des transactions de l’espace partenaires
1. Vue Détails de la transaction PSC mappée à la vue Détails de la transaction de l’espace partenaires
1. Vue PSC ajouter des produits mappée à l’affichage de l’espace partenaires ajouter des solutions
1. Vue de gestion des utilisateurs du PSC mappée à la vue de gestion des utilisateurs de l’espace partenaires
1. Vue d’attribution de rôle d’utilisateur PSC mappée à l’affichage de l’attribution de rôle de l’espace partenaires
1. Affichage des notifications du PSC mappé à l’affichage des notifications de l’espace partenaires

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-page d’hébergement du PSC mappée à l’affichage par défaut opportunités de co-vente de l’espace partenaires

Comparez les cercles correspondants numérotés entre la capture d’écran principale du PSC et la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe aucun champ de l’espace partenaires correspondant.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Image qui montre les mappages de champs entre la page d’hébergement de Partner Sales Connect et l’affichage par défaut des opportunités de covente dans l’espace partenaires." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-affichage de grille du PSC mappé à la vue des transactions de l’espace partenaires

Comparez les cercles correspondants numérotés entre la capture d’écran principale du PSC et la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe aucun champ de l’espace partenaires correspondant.  

> [!NOTE]
> D’autres considérations apparaissent sous les captures d’écran.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Image présentant les mappages de champs entre l’affichage de la grille PSC et l’affichage des ventes de l’espace partenaires." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considérations spéciales :**

- Il n’existe aucun affichage de liste dans l’espace partenaires comme celui de PSC.  Toutes les transactions sont répertoriées en fonction de la date de réception ou de la date de création la plus récente avec les informations sur le client et le type de la transaction. La première affaire de la vue est sélectionnée par défaut. La plupart des valeurs affichées au format de table PSC sont disponibles dans l’affichage détaillé de la transaction sur le PC.
- Le rôle de la transaction n’est pas un champ obligatoire dans PC. Elle n’est pas affichée ou capturée dans les flux de travail. Elle est automatiquement dérivée du côté du vendeur Microsoft en fonction des solutions ajoutées à la transaction.
- La date de dernière modification n’est pas affichée sur la page Détails de la référence du PC. Les partenaires peuvent utiliser la fonctionnalité de tri pour trier les transactions en fonction de la date de la dernière mise à jour.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-Affichage des détails de la transaction du PSC mappé à l’espace partenaires

Comparez les cercles correspondants sur la capture d’écran du haut (PSC) à la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe pas de champ ou de zone correspondant dans l’espace partenaires.

> [!NOTE]
> D’autres considérations apparaissent sous les captures d’écran.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Image présentant les mappages de champs entre l’affichage des détails du contrat PSC et l’affichage Détails de la transaction de l’espace partenaires." lightbox="images/pscmigration/deal-details-expanded.png":::

**Considérations spéciales :**

- Les partenaires peuvent modifier une transaction en sélectionnant le bouton modifier dans l’affichage Détails de l’offre de partenaire (6). Une fois le bouton modifier sélectionné, tous les champs sont modifiables. Vous avez ensuite la possibilité d’enregistrer ou d’annuler les modifications apportées à la transaction.
- Il n’est pas possible de fermer la transaction en tant que doublon dans l’espace partenaires.
- Le résultat du client n’est pas disponible dans l’espace partenaires. Tous les détails relatifs aux interactions avec les clients peuvent être mis à jour dans la section Notes de PC.
- La date de fermeture de la solution estimée est disponible uniquement pour les contrats IOT OEM dans l’espace partenaires. Ces informations ne sont pas affichées pour d’autres types de transactions.
- Le programme de licence n’est pas requis sur PC. Ces informations sont déduites automatiquement en fonction des solutions sélectionnées dans le contrat.

>[!Note]
>Toute transaction marquée comme conclue ou perdue ne peut pas être modifiée par la suite. Faites preuve de prudence lors du déplacement d’un contrat dans l’un de ces États de terminal.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-la vue « ajouter des produits » est mappée à l’affichage de l’espace partenaires « ajouter des solutions »

Comparez les cercles correspondants sur la capture d’écran du haut (PSC) à la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe pas de champ ou de zone correspondant dans l’espace partenaires.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Image présentant les mappages de champs entre l’affichage de l’ajout de produits Partner Sales Connect (PSC) et la vue ajouter des solutions de l’espace partenaires." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-gestion des utilisateurs dans le PSC et l’espace partenaires

Comparez les cercles correspondants sur la capture d’écran du haut (PSC) à la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe pas de champ ou de zone correspondant dans l’espace partenaires.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Image présentant les mappages de champs entre la page d’administration de l’utilisateur Partner Sales Connect (PSC) et l’affichage de la page de gestion des utilisateurs de l’espace partenaires dans la zone Paramètres du compte."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-attribution de rôle d’utilisateur dans PSC et espace partenaires

Comparez les cercles correspondants sur la capture d’écran du haut (PSC) à la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe pas de champ ou de zone correspondant dans l’espace partenaires.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Image présentant les mappages de champs entre l’affichage de l’attribution de rôle PSC (Partner Sales Connect) et l’affichage de l’attribution de rôle de l’espace partenaires." lightbox="images/pscmigration/roles-expanded.png":::

**Considérations spéciales :**

- Le rôle équivalent pour l’administrateur PSC est le rôle d’administrateur de compte dans l’espace partenaires.
- Il n’existe qu’un seul rôle dans l’espace partenaires pour la gestion des ventes de covente. Ce rôle est le rôle d’administrateur de référence.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-notifications dans le PSC et l’espace partenaires

Comparez les cercles correspondants sur la capture d’écran du haut (PSC) à la capture d’écran de l’espace partenaires ci-dessous. Les numéros correspondants indiquent où se trouve la fonctionnalité ou l’attribut associé au PSC dans l’espace partenaires. Les cercles rouges indiquent qu’il n’existe pas de champ ou de zone correspondant dans l’espace partenaires.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Image qui montre le mappage entre les notifications Partner Sales Connect (PSC) et l’affichage des notifications de l’espace partenaires."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passage de PSC à l’espace partenaires-Forum aux questions

Les sections suivantes répondent à des questions fréquentes sur la migration.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-que dois-je faire si je n’ai pas accès à l’espace partenaires ?

Vous pouvez contacter vos administrateurs listés sur la page « aucun accès » pour que les rôles soient attribués. Vous aurez besoin du rôle d' [administrateur de référence](permissions-overview.md#manage-referrals) pour l’autorisation d’accès en lecture et en écriture dans la section Références. Si vous gérez uniquement des profils d’entreprise, vous aurez besoin du rôle d’administrateur du profil d’entreprise dans l’espace partenaires.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Image présentant l’expérience sans accès dans l’espace partenaires.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-qui peut me donner accès à la section Références de l’espace partenaires ?

L' [administrateur](permissions-overview.md#manage-mpn-membership-and-your-company) de votre compte peut vous accorder l’accès à l’onglet Références. Pour trouver votre administrateur de compte, sélectionnez **paramètres de compte** à partir de l’icône d’engrenage en haut à droite du tableau de [bord](https://partner.microsoft.com/dashboard)de l’espace partenaires. Ensuite, sélectionnez **gestion des utilisateurs** dans la barre de navigation gauche de second niveau. En haut de la liste des utilisateurs, sélectionnez le menu déroulant **filtre** et remplacez l’option par **administrateur de compte**. La page affiche tous les administrateurs de comptes avec leurs adresses e-mail respectives. Demandez à l’un d’eux d’attribuer le rôle d’administrateur de référence pour votre compte professionnel.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-le bouton + nouveau contrat est grisé pour notre compte. Que dois-je faire pour commencer à créer des transactions ?

Cela se produit uniquement s’il n’existe aucune solution de covente prête associée à l’organisation MPN que vous utilisez dans l’espace partenaires. Contactez votre PDM pour obtenir l’ID MPN de vos solutions corrigées ou créez un ticket de support mentionnant le problème, « le bouton nouveau contrat est grisé après la migration du PSC ».

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-puis-je attribuer des transactions à une personne spécifique de notre organisation, comme PSC ?

Vous pouvez assigner des membres d’équipe à une transaction spécifique. Il n’empêche pas les autres administrateurs de référence d’afficher ou d’agir sur ces transactions.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-existe-t-il une vue de toutes les transactions qui me sont attribuées ?

Vous pouvez utiliser la fonctionnalité favoris, qui est un onglet de niveau utilisateur. Vous pouvez marquer toutes les transactions qui vous sont attribuées en tant que favoris pour accéder rapidement aux transactions.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-existe-t-il une vue en lecture seule des transactions ?

Non, il n’existe pas d’affichage en lecture seule des transactions dans la section Références. Tous les administrateurs de référence disposent d’un accès complet en lecture et en écriture à toutes les demandes.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-Comment puis-je inscrire une transaction après l’avoir marquée comme conclue ?

Si la transaction répond aux critères ci-dessous, nous allons afficher une fenêtre contextuelle pour commencer [l’enregistrement des transactions](./register-deals.md).

- Une solution d’incentives incitative est jointe à la transaction.
- Le vendeur de Microsoft est invité à participer au contrat ou il vous a invité à le faire.
- La carte Microsoft est dans l’état accepté ou gagné dans l’espace partenaires.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-J’obtiens un message d’erreur lorsque je sélectionne le bouton « + New transaction Registration » dans la section d’enregistrement des transactions. Comment puis-je inscrire mes demandes ?

Le bouton **+ nouvel enregistrement** de la transaction ne doit être utilisé que par les partenaires inscrits dans le programme ISV Connect pour l’inscription d’un contrat sans opportunité de covente correspondante dans l’espace partenaires. Pour l’enregistrement des transactions avec une opportunité de covente, une fenêtre contextuelle s’affiche lorsque la transaction est marquée comme conclue et si elle répond aux critères d’enregistrement des transactions.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-l’ajout d’une organisation client est-il obligatoire ?

Oui, l’ajout d’une [organisation client](./manage-co-sell-opportunities.md#select-your-customer) est obligatoire dans l’espace partenaires. Commencez par Rechercher l’emplacement où se trouve le client. En fonction des détails que vous avez ; vous pouvez être spécifique, y compris le nom de build exact, ou simplement fournir les détails de la ville. La recherche d’organisation récupère toutes les entités juridiques correspondant au nom que vous entrez afin que vous n’ayez pas à entrer les détails de l’adresse. Tous les détails sont renseignés automatiquement en fonction de l’organisation sélectionnée.

### <a name="10---are-customer-contact-details-mandatory"></a>10-les coordonnées du client sont-elles obligatoires ?

Dépend du [type de transaction](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que vous créez. Si vous partagez simplement votre pipeline et que vous n’avez pas besoin d’aide de la part de l’Organisation des ventes Microsoft, vous pouvez choisir de ne pas fournir les coordonnées du client. Si vous êtes en train de vendre à l’endroit où vous recherchez activement de l’aide auprès de Microsoft seller, vous devrez fournir les coordonnées du client. Vous devez obtenir un consentement explicite du client avant de créer une demande de covente dans l’espace partenaires.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-combien de solutions puis-je ajouter à un contrat ?

Vous pouvez ajouter jusqu’à 50 solutions (similaires à « Products » dans PSC) à un contrat. Contrairement à PSC, vous pouvez mélanger des solutions à partir de vos propres solutions de covente éligible, des SKU Microsoft First Party et d’autres solutions éligibles tierces de covente. Il n’existe aucun rôle de contrat qui doit être sélectionné ou disponible dans l’espace partenaires. Pour les références SKU Microsoft, vous pouvez éventuellement ajouter des quantités et des prix pour chaque référence ajoutée à la transaction.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-Quand dois-je connaître les détails du vendeur Microsoft après avoir créé un contrat ?

Les vendeurs Microsoft sont affectés uniquement après avoir adapté la spécification d’aide exacte indiquée lors de la création du contrat avec le personnage du vendeur du côté Microsoft. Même après l’attribution, les vendeurs Microsoft auront la possibilité d’accepter ou de refuser l’invitation de covente. Si une invitation de covente est acceptée par un vendeur, la vente sera mise à jour avec les coordonnées du vendeur Microsoft. L’accord de niveau de service pour les vendeurs Microsoft sur la transaction est de 14 jours. Il s’agit du même contrat de niveau de service que les partenaires doivent faire face à la transaction avant qu’elle ne passe à l’État expiré.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-où puis-je trouver l’ID d’opportunité ?

L’ID d’opportunité dans PSC est le même que l’ID de contrat dans PC. Vous pouvez trouver l’ID de contrat en regard du nom de la transaction lorsque vous ouvrez une transaction.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-Comment mon PDM peut-il accéder à un PC ?

L’espace partenaires n’est pas accessible directement à votre prestations contrairement à PSC. Il existe plusieurs options pour activer cette fonctionnalité, comme indiqué ci-dessous.

- Informations OCP : si les prestations affichent simplement les contrats et la progression associés, ils peuvent utiliser le portail OCP Insights pour obtenir une vue d’ensemble de votre organisation. Il s’agit d’un outil interne qui est uniquement disponible pour prestations. Notez que les Insights OCP ne sont pas disponibles pour les utilisateurs de votre entreprise.
- Utilisateur invité dans l’espace partenaires : vous pouvez ajouter votre @microsoft.com compte PDM en tant qu’utilisateur invité dans l’espace partenaires et lui affecter un rôle d’administrateur de référence afin qu’il puisse afficher et agir sur les références.
- Création d’un [utilisateur](./create-user-accounts-and-set-permissions.md#add-a-new-user) dans votre client : vous pouvez créer un nouvel utilisateur dans votre propre locataire et partager ces informations avec le PDM afin qu’il puisse afficher et agir sur des références similaires à d’autres utilisateurs de référence dans votre compte.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Recherche de l’ID MPN approprié si votre compte dans PSC n’est pas associé à un MPN valide

Si vous êtes ici, parce que vous avez vu une bannière dans le PSC mentionnant « problème d’association d’ID MPN non valide », vous êtes au bon endroit. Votre compte a peut-être été lié à un ID MPN non valide pour les raisons suivantes

- Votre entreprise ne dispose pas d’un compte de l’espace partenaires.
- Votre récupération PDM a commis une erreur lors de la saisie de l’ID MPN de votre compte dans les systèmes internes qui lient votre compte PSC à votre compte espace partenaires (MPNID).
- Votre entreprise n’a pas terminé la migration du centre d’appartenance (PMC) partenaire vers le PC.

Tout d’abord, recherchez l’ID MPN correct en suivant les étapes ci-dessous.

- Connectez-vous à votre compte espace partenaires
- Utilisez les instructions fournies dans la [documentation des paramètres de compte](./partner-center-account-setup.md#locate-your-mpn-id) pour localiser l’ID MPN.

Vous trouverez ci-dessous une capture d’écran montrant l’emplacement exact où vous pouvez trouver votre ID MPN de l’espace partenaires.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Image représentant les paramètres de compte où le partenaire peut trouver son ID MPN."  lightbox="images/pscmigration/findingMPNID.png":::

Ensuite,

- Si vous disposez d’un système PDM, demandez-lui d’obtenir votre ID MPN corrigé avec l’ID MPN correct à partir de votre compte espace partenaires.
- Si vous n’avez pas de PDM, envoyez un e-mail à l’adresse indiquée dans la bannière du PSC avec les informations du compte PSC figurant dans la bannière du PSC et l’ID MPN correct de votre compte espace partenaires.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Ressources pour vous aider à créer et gérer vos offres dans l’espace partenaires

Si vous n’avez pas encore lu les rubriques d’aide de la co-vente, les ressources suivantes vous aideront à gérer les transactions dans l’espace partenaires.

|**Pour ce faire**   |**Lisez cela**   |
|-----------------------|:-----------------------|
|Compréhension des onglets et de la navigation dans la page opportunités de co-vente|[Navigation dans la section de covente](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Sélection d’une organisation cliente dans la liste D&B |[Sélectionnez votre client](./manage-co-sell-opportunities.md#select-your-customer)|
|Modification des champs dans la section Détails de la transaction|[Détails de la transaction](./manage-co-sell-opportunities.md#deal-details)|
|Ajout des membres de votre équipe à une équipe de gestion|[Ajoutez vos employés](./manage-co-sell-opportunities.md#add-team-members)|
|Réponse à une transaction de covente|[Gérer les offres de covente](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Inscrire les demandes que vous avez remportées dans l’espace partenaires |[Enregistrer une nouvelle transaction](./register-deals.md)
|Obtenir des informations de référence et découvrir le fonctionnement de vos références |[Insights de référence](./referral-insights.md)
|Création et gestion d’un profil d’entreprise|[Gérer un profil professionnel](./create-a-marketing-profile.md)
|Gérer les responsables pour votre profil d’entreprise |[Gérer les prospects](./manage-leads.md)|

## <a name="next-steps"></a>Étapes suivantes


- [Vente des partenaires se connecter au](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) classeur de l’espace partenaires-classeur pour aligner les processus et les rôles des ventes des partenaires avec les nouveaux processus de vente via l’espace partenaires et les ventes de partenaires.
- [Guide d’utilisation de la co-vente de l’espace partenaires](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -aide pour identifier un modèle d’exploitation via l’espace partenaires pour gérer les prospects, vendre des opportunités et enregistrer des transactions.
- Guide de [gestion des références](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : instructions pas à pas pour gérer les prospects et les opportunités de covente via l’espace partenaires.
- [Publication et gestion dans le Marketplace commercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : instructions pas à pas pour créer, gérer et publier des offres via l’espace partenaires dans la place de marché commerciale.