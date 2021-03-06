---
title: Annonces d’avril 2021
description: Annonces du mois d’avril 2021 pour l’Espace partenaires Microsoft, avec notamment les nouvelles fonctionnalités, les promotions, les offres, les marchés ou les changements apportés aux offres existantes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150129"
---
# <a name="april-2021-announcements"></a>Annonces d’avril 2021

Cette page contient les annonces de l’Espace partenaires Microsoft d’avril 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Préparation : Mise à jour de l’API de validation des adresses client CSP en juin - Fonctionnalité de test disponible dès maintenant

### <a name="categories"></a>Catégories

- Date : 30/04/2021
- Préparation

### <a name="summary"></a>Résumé

Pour aider nos partenaires et nos clients à gérer leur entreprise en toute confiance, nous les invitons à tester les modifications qui ont été apportées à l’API de validation des adresses, disponible pour le monde entier.

### <a name="impacted-audience"></a>Public concerné

Les partenaires à facturation directe CSP et les fournisseurs indirects qui créent ou mettent à jour l’adresse de clients existants

### <a name="details"></a>Détails

Chez Microsoft, la confiance est notre priorité. Nous nous engageons à fournir une méthode de validation des adresses clients qui soit conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme Fournisseur de solutions Cloud (CSP). Depuis le 31 mars 2021, nous avons apporté des modifications à l’API de validation des adresses. Nous invitons les partenaires à tester l’API avant sa mise en ligne à la fin du mois de juin 2021. 

Notez que ces modifications affectent uniquement l’API de validation des adresses. Les API de création de client et de mise à jour du profil de facturation ne sont pas affectées. Même s’il n’est pas obligatoire d’utiliser l’adresse suggérée avec l’API de création de client, il est vivement recommandé de le faire.

La réponse renverra l’un des messages d’état suivants :

| Statut     | Description |    Nombre d’adresses suggérées retournées |
|-------|---------------|-------------------|
|Verified shippable (Valide pour l’expédition) | L’adresse est vérifiée, et valide en tant qu’adresse d’expédition. | Unique |
|Verified | L’adresse est vérifiée. | Unique |
|Interaction required (Interaction nécessaire) | L’adresse suggérée est très différente de la précédente et nécessite une confirmation de l’utilisateur. | Unique |
|Street partial (Informations sur la voie incomplètes) | La rue donnée dans l’adresse est partielle et nécessite davantage d’informations. | Multiple (maximum trois) |
|Premises partial (Informations sur le bâtiment incomplètes) | Les informations fournies sur le bâtiment (numéro de bâtiment, numéro de suite, etc.) sont incomplètes. | Multiple (maximum trois) |
|Multiple | Plusieurs champs sont incomplets dans l’adresse (notamment ceux concernant la voie et le bâtiment). | Multiple (maximum trois) |
|Aucun | L’adresse est incorrecte. | Aucun |
|Non validée | L’adresse n’a pas pu être envoyée au processus de validation. | Aucun |

Les codes postaux des États-Unis retournent quatre chiffres supplémentaires + un trait d’union, par exemple 12345-6789.

### <a name="next-steps"></a>Étapes suivantes

- Pour obtenir des instructions plus détaillées, consultez la documentation technique et les questions fréquemment posées dans le [groupe de partenaires dédié](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).
- Préparez l’intégration des modifications à l’aide de l’API Espace partenaires et de l’expérience utilisateur web. 
- Partagez votre ID de locataire sandbox avec l’expert technique (Ali Khaki) afin de l’inclure dans la série de tests et de pouvoir commencer à préparer la mise à jour. 
- Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.

### <a name="questions"></a>Des questions ?

Si vous avez besoin d’aide pour vos opérations Microsoft, contactez le groupe Yammer de votre support partenaire ou [faites une demande de service](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nouvel emplacement pour la documentation Swagger de l’API de l’Espace partenaires

### <a name="categories"></a>Catégories

- Date : 26/04/2021
- Fonctions

### <a name="summary"></a>Résumé

Les documents Swagger de l’API Espace partenaires ont été déplacés de l’[ancien site de documentation Swagger](https://apidocs.microsoft.com/services/partnercenter) vers le [nouveau site de documentation Swagger](/rest/api/partner-center-rest/).

### <a name="impacted-audience"></a>Public concerné

Les partenaires à facturation directe et les fournisseurs indirects participant au programme CSP qui utilisent les API de l’Espace partenaires.

### <a name="details"></a>Détails

À compter du 26 avril 2021, la documentation Swagger de l’API Espace partenaires, y compris le contenu de l’API REST, se trouve sur un [nouveau site](/rest/api/partner-center-rest/). L’ancien site deviendra inaccessible dans les semaines qui suivront.

### <a name="benefits"></a>Avantages

La documentation Swagger de l’API Espace partenaires fournit une **fonction d’essai**. Pour utiliser cette fonction, vous devez disposer d’un jeton du porteur, que vous pouvez générer en suivant les étapes indiquées dans [Authentification auprès de l’Espace partenaires](/partner-center/develop/partner-center-authentication#app--user-authentication).

### <a name="next-steps"></a>Étapes suivantes

Partagez ces informations dans votre organisation pour permettre à l’équipe compétente de passer en revue et de mettre à jour ses processus.

### <a name="questions"></a>Vous avez des questions ?

Si vous avez des questions sur ces offres, consultez les communautés Yammer appropriées.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Politique de période de retour des logiciels de fournisseur de solutions Cloud (CSP) et avis d’expiration du lien de téléchargement

### <a name="categories"></a>Catégories

- Date : 21/04/2021
- Fonctions

### <a name="summary"></a>Résumé

Des modifications ont été apportées à la politique concernant la période de retour des logiciels CSP et l’expiration du lien de téléchargement.

### <a name="impacted-audience"></a>Public concerné

Partenaires proposant des offres d’abonnement à des logiciels avec licence perpétuelle ou non dans le programme CSP

### <a name="details"></a>Détails

Tenez compte des notifications importantes qui suivent concernant les achats d’abonnement à des logiciels avec licence perpétuelle ou non, via l’Espace partenaires :

#### <a name="software-return-period-policy"></a>Politique relative à la période de retour des logiciels

Comme le stipule le Contrat Partenaire Microsoft (MPA), à partir du 1er juin 2021, la période de retour pour les offres logicielles dans le cadre du programme CSP passe de 60 jours à 30 jours à compter de la date de la commande.

Une fois qu’une commande a été effectuée pour une offre logicielle, les partenaires auront 30 jours à compter de la date de commande pour envoyer les révisions suivantes :

- Toute licence perpétuelle de logiciel retournée pendant la période de retour de 30 jours fera l’objet d’un remboursement intégral du prix d’achat.

- Tout abonnement à un produit logiciel retourné pendant la période de retour de 30 jours fera l’objet d’un remboursement calculé au prorata du prix d’achat.

Ce message fait suite aux e-mails que nous avons envoyés en décembre 2020 et en avril 2021 à tous les partenaires CSP, au sujet de la période de retour et d’autres informations sur le contrat MPA. Reportez-vous à ces e-mails pour obtenir des informations complètes sur les modifications qui affectent le contrat MPA.

#### <a name="software-download-link-expiry"></a>Expiration du lien de téléchargement de logiciel

À compter du 3 juin 2021, les liens de téléchargement pour les abonnements à des logiciels avec licence perpétuelle ou non via l’Espace partenaires expireront au bout de cinq jours à compter du premier téléchargement. La période d’expiration s’appliquera à tous les achats effectués avant le 3 juin 2021, ainsi que le 3 juin 2021 et après cette date.

### <a name="next-steps"></a>Étapes suivantes

Lisez les [Questions fréquentes relatives à la période de retour et à l’expiration du lien de téléchargement dans le programme CSP](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), et informez toutes les équipes concernées de votre organisation de ces modifications :

### <a name="questions"></a>Vous avez des questions ?

Si vous avez des questions sur ces offres, consultez les communautés Yammer appropriées.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Programme Open License : transition des revendeurs vers le programme Fournisseur de solutions Cloud (CSP)

### <a name="categories"></a>Catégories

- Date : 19/04/2021
- Développer votre activité

### <a name="summary"></a>Résumé

Cette communication explique en détail comment se préparer aux changements qui seront bientôt apportés au programme Open License.

### <a name="impacted-audience"></a>Public concerné

Partenaires CSP et Open License

### <a name="details"></a>Détails

En 2020, Microsoft a [annoncé](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) la diffusion prochaine de licences logicielles perpétuelles aux partenaires et clients par le biais du programme Fournisseur de solutions Cloud (CSP). La première étape a été franchie en janvier 2021 avec la mise à disposition d’offres commerciales de logiciels perpétuels. La prochaine étape clé aura lieu en juillet 2021, lorsque les offres du [secteur public](https://aka.ms/openlicensepublicsector) seront disponibles. Nous avons également [communiqué](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) qu’à compter du 1er janvier 2022, aucun nouvel achat de licence logicielle ou renouvellement de Software Assurance ou de services en ligne ne pourra être effectué dans le cadre du programme Open License.

La transition des logiciels perpétuels vers le programme CSP dans la nouvelle expérience commerciale aidera les partenaires à offrir des solutions diversifiées et des services managés dans davantage de scénarios. Cela accélèrera également la transition des clients vers le cloud.  Pour garantir une transition fluide à la fois pour nos partenaires et nos clients, nous avons effectué des ajustements et créé des documents visant à accélérer la transformation numérique :

#### <a name="april-2021"></a>Avril 2021

[Disponible immédiatement](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) : documents de transition Open License vers CSP pour les revendeurs

#### <a name="july-2021"></a>Juillet 2021

##### <a name="csp"></a>CSP

- 1er juillet : Licences logicielles perpétuelles disponibles pour les clients du secteur public

- 7 juillet : Licences logicielles perpétuelles Visual Studio Pro et Get Genuine Windows Agreement disponibles pour tous les segments

##### <a name="open-value"></a>Open Value

- 1er juillet : Références SKU supplémentaires disponibles dans le programme Open Value pour l’éducation et les associations, avec des offres similaires à celles du programme Open License

##### <a name="open-license"></a>Open License

- 1er juillet : Microsoft ne lancera plus de nouvelles offres dans le cadre du programme Open License.

#### <a name="january-2022"></a>Janvier 2022

- 1er janvier : Aucun nouvel achat ou renouvellement ne pourra être effectué par le biais du programme Open License.

### <a name="next-steps"></a>Étapes suivantes

#### <a name="csp-indirect-providers"></a>Fournisseurs indirects CSP

Profitez des mois à venir pour aider les revendeurs Open License à s’orienter vers le programme CSP en participant à des événements organisés par la communauté des partenaires et en utilisant les documents de transition Open License vers CSP pour les revendeurs :

- [Documents de transition Open License vers CSP pour les revendeurs](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/) : présentation personnalisable, modèle d’e-mail, guide d’intégration des revendeurs indirects CSP, etc. pour encourager vos revendeurs à adopter le programme à grande échelle.

- [Événements de la communauté des partenaires CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) organisés par Microsoft Business organisée.  Rejoignez les différentes sessions proposées pour apprendre les principes de base du programme CSP ou vous tenir à jour, et posez des questions sur les logiciels dans CSP (sessions de questions et réponses).

- (Bientôt disponible) Session de formation destinée aux revendeurs indirects CSP organisée par Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Revendeurs Open License

- Si votre organisation n’est pas actuellement inscrite au programme CSP, contactez votre distributeur pour savoir par où commencer. Cliquez [ici](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider) pour contacter un fournisseur indirect.

- Si votre organisation est déjà inscrite au programme CSP, cliquez [ici](https://partner.microsoft.com/resources/collection/software-in-csp) pour en savoir plus sur les logiciels perpétuels dans CSP.

### <a name="questions"></a>Vous avez des questions ?

Si vous avez d’autres questions sur ces offres, consultez vos communautés Yammer pertinentes.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Maintenant disponible : Guide de préparation des promotions mondiales

### <a name="categories"></a>Catégories

- Date : 16/04/2021
- Fonctions

### <a name="summary"></a>Résumé

Launch Readiness a publié un nouveau [guide de préparation des promotions mondiales](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) dans la galerie de ressources Operations Readiness. Ce guide offre une vue consolidée de toutes les [promotions actives à l’échelle mondiale](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires VL (licence en volume), DPL (liste de prix Dynamics) et CSP (Fournisseur de solutions Cloud)

### <a name="details"></a>Détails

Les partenaires Microsoft nous ont fait part de la nécessité de disposer d’un guide regroupant toutes les promotions mondiales avec les détails de chaque offre. Le but de ce guide est de regrouper toutes les informations disponibles dans un emplacement central et facilement accessible pour aider les partenaires à utiliser les promotions.

À compter d’avril 2021, Microsoft mettra à jour ce guide tous les mois et le publiera dans une collection de guides de préparation des promotions mondiales. Celle collection dédiée sera disponible dans la galerie de ressources Operations Readiness.

Des liens vers ce guide seront également inclus dans les collections suivantes :

- La [collection de calendriers de lancement](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), qui fournit une vue centralisée des changements et des lancements à venir.

- Les [collections de la communauté](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), qui contiennent des documents de support pour nos appels mensuels aux partenaires et qui soulignent les changements à venir et les sujets d’actualité présentant un intérêt opérationnel.

- Les [bulletins d’informations pour les partenaires](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), notamment les mises à jour apportées chaque mois au programme CSP.

En guise de rappel, nous publierons également chaque mois une annonce dans l’Espace partenaires pour signaler la parution du nouveau numéro du guide de préparation des promotions mondiales.

### <a name="next-steps"></a>Étapes suivantes

Au début de chaque mois, vous trouverez le dernier [guide de préparation des promotions mondiales](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) dans la [galerie des ressources Operations Readiness](https://partner.microsoft.com/resources).

Partagez ces informations avec les personnes concernées dans vos organisations et donnez-nous votre avis sur le guide en utilisant le bouton « Cette page vous a-t-elle été utile ? » à la fin de chaque page.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Mise à jour et rappels de la communauté pour les fournisseurs de solutions cloud (CSP) - Avril

### <a name="categories"></a>Catégories

- Date : 16/04/2021
- Communauté | Invitations et rappels

### <a name="summary"></a>Résumé

Les ressources de la communauté CSP sont disponibles à la demande et mises à jour chaque mois pour vous tenir informé des changements apportés au programme CSP.

### <a name="impacted-audience"></a>Public concerné

Partenaires à facturation directe et fournisseurs indirects inscrits à CSP

### <a name="details"></a>Détails

Ce mois-ci, les ressources incluent les sujets clés suivants :

- [Mise à jour de l’évolution du programme CSP et changements du programme Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Changements des conditions d’intégration des clients CSP dans certaines régions](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nouveau format de la nouvelle facture PDF commerciale dans le programme CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

Dans la [collection de la communauté CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), vous trouverez :

- Le [bulletin des mises à jour mensuelles du programme CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), qui regroupe les annonces récentes, mises à jour, événements et rappels en rapport avec le programme CSP dans un document convivial.

- Le [calendrier des annonces CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), qui liste chronologiquement les changements à venir affectant le programme.

- Le nouveau [calendrier de lancement de produit](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), dans lequel vous pouvez voir les lancements et les offres de produits à venir.

- Les [ressources liées aux mises à jour apportées au programme CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/), avec du contenu facile à utiliser sur les changements opérationnels clés.

- [Des sessions de recyclage et des rappels](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sur les principes clés du programme CSP suscitant de l’intérêt et des demandes.

#### <a name="csp-community-call-qas"></a>Appel de la communauté CSP - Questions et réponses

Les questions et réponses des appels de la communauté sont disponibles pour vous aider à répondre à vos interrogations sur les changements à venir. Inscrivez-vous dès à présent aux sessions de questions et réponses lors des appels de la communauté CSP qui auront lieu en avril, mai et juin. Ces appels porteront sur les derniers lancements et fourniront des sessions de recyclage et des rappels importants.

[Inscrivez-vous ici](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources de la communauté et inscrivez-vous aux questions et réponses des appels de la communauté.

Pour tirer le meilleur parti des questions et réponses des appels de la communauté, passez en revue le contenu de la communauté à la demande et envoyez vos questions 48 heures au maximum avant l’appel.

### <a name="questions"></a>Des questions ?

La session mensuelle de questions et réponses lors de l’appel de la communauté CSP est le meilleur endroit pour poser des questions sur les changements affectant le programme CSP. Chaque mois, passez en revue les documents et envoyez vos questions à l’avance afin que nous puissions orienter la session sur les sujets qui vous intéressent le plus.

Pour plus d’informations, contactez le [support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Dernier rappel : Dépréciation de la qualification GET le 6 mai 2021

### <a name="categories"></a>Catégories

- Date : 04/05/2021

- Fonctions

### <a name="impacted-audience"></a>Public concerné

Partenaires proposant des offres Éducation, Sans but lucratif et Cloud de la communauté du secteur public par le biais du programme Fournisseur de solutions Cloud avec l’API Espace partenaires

### <a name="details"></a>Détails

Cette annonce est faite à la suite des [améliorations de l’Espace partenaires publiées en décembre](./2020-december.md#1). Dans le cadre de cette version, de nouvelles API pour les qualifications GET et POST ont été déployées et, par conséquent, **la qualification GET existante sera mise hors service le 6 mai 2021**. D’ici là, vous devrez passer aux nouvelles API POST de l’Espace partenaires. Les nouvelles API POST vous permettront d’acheter des offres Éducation, et les nouvelles API GET des offres préqualifiées Sans but lucratif et Cloud de la communauté du secteur public.

### <a name="next-steps"></a>Étapes suivantes

- Pour garantir une transition réussie et dans les temps, **faites la mise à jour vers les nouvelles API**.

- **Passez en revue les nouveaux changements de l’API Espace partenaires et le guide correspondant** dans les ressources de préparation opérationnelle : [Améliorations du processus de validation des clients Éducation dans l’Espace partenaires](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Partagez ces informations avec les équipes appropriées au sein de votre organisation et avec vos revendeurs pour les aider à anticiper ces changements.

### <a name="questions"></a>Des questions ?

Pour toute question relative à cette notification, contactez le [support technique de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Journal des modifications

- 4 mai 2021 : Dernier rappel de la dépréciation à venir de la qualification GET

- 9 avril 2021 : Rappel de la dépréciation à venir de la qualification GET 

- Février : Plannings mis à jour pour la dépréciation des qualifications GET et PUT

- Janvier : Rappel des dépréciations à venir des qualifications GET et PUT

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nouveau format pour la nouvelle facture PDF commerciale dans CSP

### <a name="categories"></a>Catégories

- Date : 05/04/2021
- Fonctions

### <a name="summary"></a>Résumé

Microsoft introduit un nouveau format pour les factures PDF commerciales dans le programme CSP (Cloud Solution Provider) afin d’afficher les détails de facturation par détail du produit au lieu de la description de la référence SKU.

### <a name="impacted-audience"></a>Public concerné

Partenaires effectuant des transactions via le programme CSP

### <a name="details"></a>Détails

À compter du mois de mai 2021, Microsoft présente un nouveau format pour les factures PDF commerciales dans le programme CSP afin d’afficher les détails de facturation par détail du produit au lieu de la description de la référence SKU. Avec cette nouvelle mise à jour, nous allons regrouper les éléments de ligne par type de produit tout en affichant chaque produit sur une ligne individuelle.

Les partenaires remarqueront l’entrée en vigueur de ce changement dans leur facture du mois de mai pour la période de facturation comprise entre le 1er avril 2021 et le 30 avril 2021. Les offres affectées sont Microsoft Azure Reserved Instance, les abonnements Azure (plan Azure) et la Place de marché.

Toutes les demandes de crédit-refacturation effectuées après la mise à jour du format de facture seront générées au nouveau format.

#### <a name="partner-benefits"></a>Avantages pour les partenaires

Cette mise à jour améliore l’expérience de facturation pour les partenaires des manières suivantes :

- Réduction de la taille des factures tout en conservant les données critiques

- Alignement du format sur les normes du secteur pour des factures compactes et conviviales 

Les éléments suivants ne seront pas affectés :

- Page de résumé de facturation sur le fichier PDF de facture

- API de facturation existantes

- Fichiers de rapprochement (les fichiers de rapprochement peuvent être utilisés pour récupérer des données précises.) 

- Factures de frais d’utilisation et basés sur les licences

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les informations relatives à ce sujet dans la [galerie des ressources Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) sur le site web des partenaires Microsoft. Pour plus d’informations sur la facturation et les taxes, notamment les ressources de facturation, les factures, la facturation des fournisseurs CSP et les taxes, consultez la [section Facturation](../billing.md) dans l’Espace partenaires.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Changements dans les conditions d’intégration des clients CSP (Cloud Solution Provider)

### <a name="categories"></a>Catégories

- Date : 02/04/2021
- Offres/marchés

### <a name="summary"></a>Résumé

Dans le cadre de notre engagement à aider les partenaires et les clients à exercer leur activité en toute confiance, nous demanderons des informations supplémentaires sur les clients à compter du 25 mars 2021.

### <a name="impacted-audience"></a>Public concerné

Fournisseurs indirects et partenaires à facturation directe CSP qui ont des clients nouveaux ou existants dans les pays listés dans la section suivante

### <a name="details"></a>Détails

Chez Microsoft, la confiance est notre priorité. Nous nous engageons à fournir une méthode de validation des clients conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme Fournisseur de solutions Cloud. Le 25 mars 2021, nous présenterons des améliorations de l’interface utilisateur et de l’API de l’Espace partenaires qui affecteront les partenaires répondant aux deux critères suivants :

- Le partenaire a une relation de facturation directe avec Microsoft (ce qui signifie que le partenaire est un partenaire à facturation directe ou un fournisseur indirect).

- Le partenaire fait affaire avec des clients nouveaux ou déjà existants dans les pays suivants :

    - Thaïlande
    - Vietnam
    - Turquie
    - Pologne
    - Afrique du Sud
    - Inde
    - Brésil
    - Irak
    - Myanmar
    - Soudan du Sud
    - Arabie saoudite
    - Émirats arabes unis
    - Venezuela

Les partenaires qui satisfont aux critères devront soumettre l’ID d’inscription d’entreprise d’un client (également connu sous le nom de code INN d’organisation) et le numéro de téléphone d’un client lors de la prochaine mise à jour ou création d’un abonnement pour ce client. Ces partenaires peuvent également entrer un deuxième prénom facultatif pour le client.

Notez que lorsque vous ajoutez votre ID d’inscription d’entreprise, vous devez utiliser votre ID de taxe professionnelle et non l’ID personnel du client.

Les partenaires qui travaillent avec des clients nouveaux ou existants dans les pays suivants ont déjà été intégrés à une version précédente en novembre 2020.

- Arménie
- Azerbaïdjan
- Bélarus
- Hongrie
- Kazakhstan
- Kirghizistan
- Moldova
- Russie
- Tadjikistan
- Ukraine
- Ouzbékistan

Les partenaires ayant des clients dans le reste du monde auront la possibilité à la fin du mois de mars 2021 d’entrer l’ID d’inscription d’entreprise, le numéro de téléphone et le deuxième prénom pour les clients, au titre d’informations facultatives.

### <a name="next-steps"></a>Étapes suivantes

- Pour obtenir des instructions plus détaillées, consultez la documentation technique et les questions fréquemment posées dans le [groupe de partenaires](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dédiée.
- Préparez l’intégration des modifications à l’aide de l’API Espace partenaires et de l’expérience utilisateur web. L’API et les SDK seront disponibles à des fins de test.
- Veillez à soumettre les données supplémentaires lors de l’intégration de nouveaux clients ou de la modification des détails de clients existants.
- Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.

### <a name="questions"></a>Des questions ?

Si vous avez des questions liées à l’ID d’inscription d’entreprise (également appelé code INN ou TIN), contactez votre conseiller fiscal ou le service des impôts local. Microsoft ne peut pas fournir d’aide sur les questions fiscales.

Si vous avez besoin de support pour vos opérations avec Microsoft, [ouvrez une demande de service](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Voir les lancements de produit et les offres du mois

### <a name="categories"></a>Catégories

- Date : 01/04/2021
- Fonctions
 
### <a name="summary"></a>Résumé

Le calendrier de lancement de produit d’avril 2021 a été publié.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

Le [calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) d’avril 2021 est maintenant disponible dans la galerie des ressources Operations readiness. Vous pouvez y voir les lancements de produits et les offres à venir.

### <a name="next-steps"></a>Étapes suivantes

Passez en revue le [calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) et partagez les informations avec les parties prenantes appropriées de votre organisation.  

### <a name="questions"></a>Vous avez des questions ?

Si vous avez d’autres questions sur ces offres, consultez vos communautés Yammer appropriées.