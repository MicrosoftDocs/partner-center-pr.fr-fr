---
title: Migrer à partir de Partner vente Connect (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires Microsoft peuvent migrer de Partner Sales Connect (PSC) vers l’espace partenaires et créer ou gérer des transactions envoyées par les vendeurs Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999343"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guide de la co-vente dans l’espace partenaires (PC) pour les partenaires qui migrent à partir de Partner vente Connect (PSC)

**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Administrateur des comptes
- Administrateur des références
- Vendeur Partner Sales Connect (PSC)
- Administrateur Partner Sales Connect (PSC)
- Responsable des ventes Partner Sales Connect (PSC)

Comme vous le savez, votre entreprise perdra l’accès au PSC après le 31 décembre 2020. Toutefois, vous trouverez tout ce que vous souhaitez faire pour créer des ventes de covente, gérer vos demandes et agir sur les transactions envoyées par les vendeurs Microsoft à vous dans l’espace partenaires. Toutefois, il y aura des différences, et les conseils suivants vous aideront à rendre votre transition vers l’espace partenaires plus lisse et directe.

>[!Important]
> Si vous êtes ici, car vous avez vu une bannière dans PSC sur la migration, vous êtes au bon endroit. Ce guide n’est pas applicable à l’évaluation de la solution (SA) et aux partenaires de l’IOT OEM qui gèrent leurs affaires dans PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Avant de vous déplacer, vous devez connaître les points suivants

### <a name="if-you-are-psc-admin"></a>Si vous êtes administrateur PSC

- Vous avez besoin d’un e-mail professionnel pour vous connecter à l' [espace partenaires](https://partner.microsoft.com/).
- Configurez votre compte avec l’aide de l' [administrateur de compte](permissions-overview.md)de l’espace partenaires.
- Découvrez comment vendre en collaboration dans l’espace partenaires en lisant ce document.
- Configurez des comptes d’utilisateur dans l’espace partenaires pour tous les utilisateurs de votre PSC (rôles Admin, Deal Manager et seller) et attribuez-leur des [rôles d’administrateur de référence](permissions-overview.md).

>[!Important]
> Assurez-vous que l’ID MPN affiché dans la bannière du PSC est disponible dans la liste des emplacements MPN dans l’espace partenaires. Vous pouvez vérifier que dans l’espace partenaires, accédez à « paramètres du compte » et à « emplacements » sous cet[emplacement](manage-locations.md)pour trouver la liste de tous les MPNs associés au compte de l’espace partenaires.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Image représentant la bannière du PSC dans laquelle les partenaires peuvent trouver l’ID MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Si vous êtes responsable des transactions de PSC ou du vendeur

- Vous avez besoin d’un e-mail professionnel pour vous connecter à l' [espace partenaires](https://partner.microsoft.com/).
- Si vous utilisez un compte non professionnel dans PSC ou si votre adresse de messagerie professionnelle est destinée à une société différente de celle de l’entreprise partenaire, contactez votre administrateur PSC pour obtenir de l’aide sur l’installation du compte.
- Vérifiez auprès de votre administrateur PSC si la configuration de votre compte espace partenaires est terminée, quel que soit le compte que vous utilisez pour vous connecter à PSC.
- Vérifiez si vous avez accès à l’espace partenaires et à la section Références.
- Lisez ce document pour comprendre les flux de travail et les modifications apportées à l’espace partenaires.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>En tant qu’administrateur dans PSC, Voici les étapes suivantes

Si vous ne voyez pas l’onglet Références :

- L' [administrateur général](permissions-overview.md) de votre entreprise peut vous accorder l’accès à l’onglet Références. Pour trouver votre administrateur général, accédez à paramètres du partenaire à partir de l’icône d’engrenage en haut à droite de l’espace partenaires. Sélectionnez la page gestion des utilisateurs dans le deuxième niveau de la barre de navigation de gauche. Cliquez sur la liste déroulante qui affiche « tous les utilisateurs » en haut à droite de la page, puis choisissez « administrateurs généraux ». La page affiche ensuite tous les administrateurs globaux avec leurs ID d’adresse de messagerie respectifs. Contactez-le pour obtenir un accès « administrateur de référence » pour votre compte professionnel.

>[!Important]
> Si votre rôle gère uniquement les utilisateurs dans le PSC, vous pouvez vous procurer le rôle d' [administrateur de compte](permissions-overview.md#manage-mpn-membership-and-your-company) dans l’espace partenaires. Si votre rôle comprend également la gestion des opportunités de covente, vous devez disposer d’un rôle d' [administrateur de références](permissions-overview.md#manage-referrals) . En outre, désignez un seul Prospect de gestion des modifications parmi les administrateurs du PSC pour travailler avec l’administrateur de compte de l’espace partenaires au lieu de tous les administrateurs PSC qui accèdent aux administrateurs de compte sur le PC individuellement.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Image représentant les administrateurs de comptes dans la page de gestion des utilisateurs paramètres du partenaire.":::

- Accédez à l’onglet références dans le volet de navigation gauche et vérifiez si vous pouvez accéder aux pages.

>[!Note]
> Vous devrez peut-être vous déconnecter de l’espace partenaires et vous reconnecter pour actualiser vos informations d’identification afin d’accéder aux pages de références.

Une fois votre compte configuré dans l’espace partenaires,

- Invitez tous les utilisateurs qui ont un rôle « gestionnaire des ventes » ou « vendeur » dans PSC à l’espace partenaires à l’étape suivante.
- L' [administrateur de compte](permissions-overview.md#manage-mpn-membership-and-your-company) qui vous a aidé avec l’accès aux références peut inviter tous les utilisateurs.
- Lors de l’invitation des utilisateurs, demandez à l’administrateur de compte de lui affecter le rôle d' [administrateur de référence](permissions-overview.md#manage-referrals) .
- Certains de vos utilisateurs de PSC peuvent utiliser un compte non professionnel ou un compte d’un domaine différent de celui que vous utilisez dans l’espace partenaires. Tous ces utilisateurs doivent se connecter à l’espace partenaires à l’aide de leur compte professionnel associé à votre locataire Azure AD. Votre [administrateur général](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) peut vous aider. Pour trouver votre administrateur général, accédez à paramètres du partenaire à partir de l’icône d’engrenage en haut à droite de l’espace partenaires. Cliquez sur la page gestion des utilisateurs dans le deuxième niveau de la barre de navigation de gauche. Cliquez sur la liste déroulante qui affiche « tous les utilisateurs » en haut à droite de la page, puis choisissez « administrateurs généraux ».
- L’administrateur général peut créer un nouveau compte d’utilisateur dans votre client Azure AD ou attribuer à un utilisateur invité l’accès aux autres utilisateurs du compte de domaine.
- Une fois les comptes configurés pour tous les responsables et les utilisateurs du PSC, ils doivent se connecter à l’espace partenaires, accéder à l’onglet de référence dans le volet de navigation gauche et vérifier s’assurer qu’ils peuvent voir la page références.

Si votre entreprise dispose d’un système PDM, lorsque votre compte espace partenaires est configuré et que vos utilisateurs sont déplacés et disposent de rôles et d’autorisations, vous pouvez déplacer vos activités de covente vers l’espace partenaires. Informez le système PDM d’effectuer le commutateur au lieu de patienter jusqu’à la fin de l’échéance de la migration, ce qui permettra à tous vos nouveaux contrats d’être transmis à l’espace partenaires.
>[!Note]
>Une fois ce commutateur effectué, vous ne pourrez agir que sur les transactions actives existantes dans le PSC. Vous ne pouvez pas créer de nouvelles demandes ni recevoir de transactions de la part de vendeurs Microsoft dans PSC.

Si votre entreprise n’a pas de PDM, assurez-vous que tous les comptes d’utilisateur sont configurés et vérifiés par tous les utilisateurs. Vous recevrez une notification par courrier électronique et une bannière dans le PSC indiquant la date exacte à laquelle vous pouvez commencer à vendre des produits dans l’espace partenaires. N’oubliez pas que vous devrez toujours gérer les transactions actives existantes dans le PSC.

>[!Important]
>Les contrats actifs ne seront pas migrés vers le PC. Vous avez jusqu’au 31 décembre 2020 pour fermer et enregistrer les demandes.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Étapes suivantes pour les administrateurs PSC, les responsables des affaires PSC et les vendeurs de PSC

Découvrez comment vendre des produits dans l’espace partenaires.
Il s’agit d’une étape importante, qui vous aidera à préparer la covente dans l’espace partenaires. Découvrez les flux de travail et les modifications dans l’espace partenaires pour vous permettre de vendre en toute covente dès le premier jour. Commencez par lire ce document entièrement. Une bonne série de ressources est également disponible dans la [Galerie d’expérience de la co-vente](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principales différences entre les flux de travail des PSC et des PC

|**Scénario**|**Vente des partenaires**|**Espace partenaires**|
|-----|:-----|:-----|
|Rôles d’utilisateur|PSC a des rôles d’administrateur, de responsable des transactions et de vendeur.|PC dispose uniquement d’un rôle d' [administrateur de référence](permissions-overview.md#manage-referrals) qui donne des autorisations en lecture et en écriture pour toutes les transactions.|
|Invitation à Microsoft sur un contrat de covente|Initié par Microsoft seller, il n’y a pas de demande explicite de partenaire.|Le partenaire devra faire une [demande explicite](manage-co-sell-opportunities.md#add-solutions) si une aide du vendeur Microsoft est nécessaire pour une affaire. Le vendeur Microsoft dispose d’une option pour refuser la demande.|
|Expiry|Il n’existe aucun concept d’expiration de la transaction.|Les contrats de contrats entrants du partenaire expirent dans 14 jours s’ils ne sont pas acceptés par le partenaire. Il en est de même pour les contrats de partenariat sortants où ils peuvent passer à l’État expiré si le vendeur Microsoft n’agit pas sur ceux-ci dans un délai de 14 jours.|
|Détails du vendeur Microsoft|Visible dès qu’une transaction est créée.|Les détails du vendeur Microsoft sont partagés avec le partenaire uniquement si le vendeur accepte expressément l’invitation pour la co-vendre du partenaire.|
|[Pipeline privé](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Non disponible.|Les partenaires peuvent partager leur pipeline sans donner de visibilité aux vendeurs Microsoft.|
|Solutions|Les solutions appartenant à une seule liste de prix peuvent être ajoutées à un contrat.|Le partenaire peut ajouter des [solutions](manage-co-sell-opportunities.md#add-solutions) qui appartiennent aux listes suivantes. a) leurs propres solutions b) à partir du catalogue Microsoft First Party (semblable au rôle transaction de transaction dans PSC) et c) coventent les solutions d’autres partenaires tiers (semblable au rôle Dealer ISV dans PSC).|
|Attribution des transactions|Seul le vendeur affecté peut afficher et agir sur les transactions.|Les membres de l’équipe peuvent être ajoutés à un contrat pour spécifier les personnes qui travaillent sur une transaction, il n’y a aucun blocage d’autres administrateurs de la référence pour afficher ou agir sur ces transactions.|
|Organisation cliente|Entrée de texte de forme libre.|Vous pouvez effectuer une recherche dans l' [organisation cliente](manage-co-sell-opportunities.md#select-your-customer) par rapport à la [base de données D&B](https://www.dnb.com/) en tapant simplement quelques caractères. Le nom et l’adresse légaux sont renseignés automatiquement en fonction du choix.|
|Contact client|Non obligatoire.|Non obligatoire pour le partage de pipeline privé. Obligatoire si Microsoft seller est invité à participer à une demande de covente.|
|API publique|Non disponible.|[API publique](/partner/develop/referrals) permettant de gérer par programmation les références de l’espace partenaires.|

## <a name="psc-and-partner-center-field-mapping"></a>Mise en correspondance des champs PSC et espace partenaires

Cette section présente le mappage exact des attributs entre PSC et l’espace partenaires. Chaque écran du PSC est comparé à la vue appropriée dans la section opportunités de co-vente de l’espace partenaires. 

>[!Note]
>Suivez les chiffres sur les bulles jaunes dans les captures d’écran du PSC pour trouver l’attribut équivalent dans l’espace partenaires. Les bulles rouges indiquent que le champ n’est pas disponible dans l’espace partenaires.

**Page d’hébergement du PSC et vue par défaut des opportunités de covente dans l’espace partenaires**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Image qui montre les mappages de champs entre la page d’hébergement de Partner Sales Connect et l’affichage par défaut des opportunités de covente dans l’espace partenaires.":::

**Affichage de grille du PSC et vue des transactions de l’espace partenaires**

- Il n’existe aucun affichage de liste dans l’espace partenaires comme celui de PSC.  Toutes les transactions sont répertoriées en fonction de la date de réception ou de la date de création la plus récente avec les informations sur le client et le type de la transaction. La première affaire de la vue est sélectionnée par défaut. La plupart des valeurs affichées au format de table PSC sont disponibles dans l’affichage détaillé de la transaction sur le PC.
- Le rôle de la transaction n’est pas un champ obligatoire dans PC. Il n’est ni affiché, ni capturé dans aucun des flux de travail. Elle est automatiquement dérivée du côté du vendeur Microsoft en fonction des solutions ajoutées à la transaction.
- La date de dernière modification n’est pas affichée sur la page Détails de la référence du PC. Les partenaires peuvent utiliser la fonctionnalité de tri pour trier les transactions en fonction de la date de la dernière mise à jour.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Image présentant les mappages de champs entre l’affichage de la grille PSC et l’affichage des ventes de l’espace partenaires.":::

**Vue des détails de la transaction dans PSC et l’espace partenaires**

- Les partenaires peuvent modifier une transaction en cliquant sur le bouton modifier de la vue Détails de l’offre de partenaire (6). Une fois que vous avez cliqué sur le bouton modifier, tous les champs deviennent modifiables avec l’option permettant d’enregistrer ou d’annuler les modifications apportées à la transaction.
- Il n’est pas possible de fermer la transaction en tant que doublon dans l’espace partenaires.
- Le résultat du client n’est pas disponible dans l’espace partenaires. Tous les détails relatifs aux interactions avec les clients peuvent être mis à jour dans la section Notes de PC.
- La date de fermeture de la solution estimée est disponible uniquement pour les contrats IOT OEM dans l’espace partenaires. Elle n’est pas affichée pour d’autres types de transactions.
- Le programme de licence n’est pas requis sur PC. Elle est déduite automatiquement en fonction des solutions sélectionnées dans le contrat.

>[!Note]
>Toute transaction marquée comme conclue ou perdue ne peut pas être modifiée. Faites preuve de prudence lors du déplacement d’un contrat vers l’un de ces États de terminal.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Image présentant les mappages de champs entre l’affichage des détails du contrat PSC et l’affichage Détails de la transaction de l’espace partenaires.":::

**Vue « ajouter des produits » du PSC et vue de l’espace partenaires « ajouter des solutions »**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Image présentant les mappages de champs entre l’affichage de l’ajout de produits Partner Sales Connect (PSC) et la vue ajouter des solutions de l’espace partenaires.":::

**Gestion des utilisateurs dans PSC et l’espace partenaires**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Image présentant les mappages de champs entre la page d’administration de l’utilisateur Partner Sales Connect (PSC) et la gestion des utilisateurs de l’espace partenaires dans la vue des paramètres du compte.":::

**Attribution de rôle d’utilisateur dans PSC et l’espace partenaires**

- Le rôle équivalent pour l’administrateur PSC est le rôle d’administrateur de compte dans l’espace partenaires.
- Il n’existe qu’un seul rôle dans l’espace partenaires pour la gestion des ventes de covente, qui est le rôle d’administrateur de référence.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Image présentant les mappages de champs entre l’affichage de l’attribution de rôle PSC (Partner Sales Connect) et l’affichage de l’attribution de rôle de l’espace partenaires.":::

**Notifications dans PSC et l’espace partenaires**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Image qui montre le mappage entre les notifications Partner Sales Connect (PSC) et l’affichage des notifications de l’espace partenaires.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passage de PSC à l’espace partenaires-Forum aux questions

**1er. Que dois-je faire si je n’ai pas accès à l’espace partenaires ?**

Vous pouvez contacter vos administrateurs listés sur la page « aucun accès » pour que les rôles soient attribués. Vous devez disposer du rôle «[administrateur de référence](permissions-overview.md#manage-referrals)» pour l’autorisation d’accès en lecture et en écriture dans la section Références. Si vous gérez uniquement des profils d’entreprise, vous aurez besoin du rôle « administrateur du profil d’entreprise » dans l’espace partenaires.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Image présentant l’expérience sans accès dans l’espace partenaires.":::

**Q2. Qui peut me donner accès à la section Références de l’espace partenaires ?**

L' [administrateur](permissions-overview.md#manage-mpn-membership-and-your-company) de votre compte peut vous accorder l’accès à l’onglet Références. Pour trouver votre administrateur de compte, accédez à paramètres de partenaire à partir de l’icône d’engrenage en haut à droite de l’espace partenaires. Cliquez sur la page gestion des utilisateurs dans le deuxième niveau de la barre de navigation de gauche. Cliquez sur la liste déroulante qui affiche « tous les utilisateurs » en haut à droite de la page, puis choisissez « Admins du compte ». La page affiche ensuite tous les administrateurs de comptes avec leurs ID d’adresse de messagerie respectifs. Contactez-le pour obtenir un accès « administrateur de référence » pour votre compte professionnel.

**Q3. Le bouton + nouveau contrat est grisé pour notre compte. Que dois-je faire pour commencer à créer des transactions ?**

Cela se produit uniquement s’il n’existe aucune solution de covente prête associée à l’organisation MPN que vous utilisez dans l’espace partenaires. Contactez votre PDM pour obtenir l’ID MPN de vos solutions corrigées ou créez un ticket de support mentionnant le problème « le bouton nouveau contrat a été grisé après la migration du PSC ».

**4ème. Puis-je attribuer des transactions à une personne spécifique de notre organisation, comme PSC ?**

Vous pouvez assigner des membres d’équipe à une transaction spécifique. Il n’empêche pas les autres administrateurs de référence d’afficher ou d’agir sur ces transactions. 

**Q5. Existe-t-il une vue de toutes les transactions qui me sont attribuées ?**

Vous pouvez utiliser la fonctionnalité favoris, qui est un onglet de niveau utilisateur. Vous pouvez marquer toutes les transactions qui vous sont attribuées en tant que favoris pour accéder rapidement aux transactions.

**Q6. Existe-t-il une vue en lecture seule des transactions ?**

Non, il n’existe pas d’affichage en lecture seule des transactions dans la section Références. Tous les administrateurs de référence disposent d’un accès complet en lecture et en écriture à toutes les demandes.

**Q7. Comment puis-je inscrire un contrat après l’avoir gagné ?**

Si la transaction répond aux critères ci-dessous, nous allons afficher une fenêtre contextuelle pour commencer [l’enregistrement des transactions](./register-deals.md).

- Une solution d’incentives incitative est jointe à la transaction.
- Le vendeur de Microsoft est invité à participer au contrat ou il vous a invité à le faire.
- La carte Microsoft est dans l’état accepté ou gagné dans l’espace partenaires.

**Q8. J’obtiens un message d’erreur lorsque je clique sur le bouton « + nouvel enregistrement de la transaction » dans la section d’enregistrement des transactions. Comment puis-je inscrire mes demandes ?**

Le « + nouvel enregistrement de la transaction » doit être utilisé uniquement par les partenaires inscrits au programme ISV Connect pour l’enregistrement d’un contrat sans opportunité de covente correspondante dans l’espace partenaires. Pour l’enregistrement des transactions avec une opportunité de covente, une fenêtre contextuelle s’affiche lorsque la transaction est marquée comme conclue et si elle répond aux critères d’enregistrement des transactions.

**Q9. L’ajout d’une organisation client est-il obligatoire ?**

Oui, l’ajout d’une [organisation client](./manage-co-sell-opportunities.md#select-your-customer) est obligatoire dans l’espace partenaires. Commencez par Rechercher l’emplacement où se trouve le client. En fonction des détails que vous avez ; vous pouvez être spécifique, y compris le nom de build exact, ou simplement fournir les détails de la ville. La recherche d’organisation récupère toutes les entités juridiques correspondant au nom que vous entrez afin que vous n’ayez pas à entrer les détails de l’adresse. Tous les détails sont renseignés automatiquement en fonction de l’organisation sélectionnée.

**Q10. Les coordonnées du client sont-elles obligatoires ?**

Dépend du [type de transaction](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que vous créez. Si vous partagez simplement votre pipeline et que vous n’avez pas besoin d’aide de la part de l’Organisation des ventes Microsoft, vous pouvez choisir de ne pas fournir les coordonnées du client. Si vous êtes en train de vendre à l’endroit où vous recherchez activement de l’aide auprès de Microsoft seller, vous devrez fournir les coordonnées du client. Vous devez obtenir un consentement explicite du client avant de créer une demande de covente dans l’espace partenaires.

**Q11. Combien de solutions puis-je ajouter à un contrat ?**

Vous pouvez ajouter jusqu’à 50 solutions (similaires à « Products » dans PSC) à un contrat. Contrairement à PSC, vous pouvez mélanger des solutions à partir de vos propres solutions de covente éligible, des SKU Microsoft First Party et d’autres solutions éligibles tierces de covente. Il n’existe aucun rôle de contrat qui doit être sélectionné ou disponible dans l’espace partenaires. Pour les références SKU Microsoft, vous pouvez éventuellement ajouter des quantités et des prix pour chaque référence ajoutée à la transaction.

**Q12. Quand dois-je connaître les détails du vendeur Microsoft après avoir créé un contrat ?**

Les vendeurs Microsoft sont affectés uniquement après avoir adapté la spécification d’aide exacte indiquée lors de la création du contrat avec le personnage du vendeur du côté Microsoft. Même après l’attribution, les vendeurs Microsoft auront la possibilité d’accepter ou de refuser l’invitation de covente. Si une invitation de covente est acceptée par un vendeur, la vente sera mise à jour avec les coordonnées du vendeur Microsoft. L’accord de niveau de service pour les vendeurs Microsoft sur la transaction est de 14 jours. Il s’agit du même contrat de niveau de service que les partenaires doivent faire face à la transaction avant qu’elle ne passe à l’État expiré.

**Q13. Où puis-je trouver l’ID d’opportunité ?**

L’ID d’opportunité dans PSC est le même que l’ID de contrat dans PC. Vous pouvez trouver l’ID de contrat en regard du nom de la transaction lorsque vous ouvrez une transaction.

**Q14. Comment mon PDM peut-il accéder à un PC ?**

L’espace partenaires n’est pas accessible directement à votre prestations contrairement à PSC. Il existe plusieurs options pour activer cette fonctionnalité, comme indiqué ci-dessous.

- Informations sur l’OCP-si les prestations affichent simplement les contrats & progression qui leur sont associés, ils peuvent utiliser le portail OCP Insights pour obtenir une vue d’ensemble de votre organisation. Il s’agit d’un outil interne qui est uniquement disponible pour prestations. Notez que les Insights OCP ne sont pas disponibles pour les utilisateurs de votre entreprise.
- Utilisateur invité dans l’espace partenaires : vous pouvez ajouter votre @microsoft.com compte PDM en tant qu’utilisateur invité dans l’espace partenaires et lui affecter un rôle d’administrateur de référence afin qu’il puisse afficher et agir sur les références.
- Création d’un [utilisateur](./create-user-accounts-and-set-permissions.md#add-a-new-user) dans votre client : vous pouvez créer un nouvel utilisateur dans votre propre locataire et partager ces informations avec le PDM afin qu’il puisse afficher et agir sur des références similaires à d’autres utilisateurs de référence dans votre compte.

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

## <a name="additional-resources"></a>Ressources supplémentaires

- [Vente des partenaires se connecter au](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) classeur de l’espace partenaires-classeur pour aligner les processus et les rôles des ventes des partenaires avec les nouveaux processus de vente via l’espace partenaires et les ventes de partenaires.
- [Guide d’utilisation de la co-vente de l’espace partenaires](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -aide pour identifier un modèle d’exploitation via l’espace partenaires pour gérer les prospects, vendre des opportunités et enregistrer des transactions.
- Guide de [gestion des références](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : instructions pas à pas pour gérer les prospects et les opportunités de covente via l’espace partenaires.
- [Publication et gestion dans le Marketplace commercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : instructions pas à pas pour créer, gérer et publier des offres via l’espace partenaires dans la place de marché commerciale.
