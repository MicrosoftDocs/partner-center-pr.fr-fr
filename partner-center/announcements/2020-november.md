---
title: Annonces de novembre 2020
description: Annonces du mois de novembre 2020 pour l’Espace partenaires Microsoft, telles que les nouvelles fonctionnalités, les promotions, les offres, les marchés ou les changements apportés aux offres existantes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691297"
---
# <a name="november-2020-announcements"></a>Annonces de novembre 2020

Cette page détaille les annonces de l’Espace partenaires Microsoft pour novembre 2020.

Annonces 2020 : [Avril](2020-april.md) | [Mai](2020-may.md) | [Juin](2020-june.md) | [Juillet](2020-july.md) | [Août](2020-august.md) | [Septembre](2020-september.md) | [Octobre](2020-October.md) | Novembre

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>Changement de la devise de facturation des partenaires pour les nouvelles offres commerciales en UE/AELE.  

### <a name="categories"></a>Catégories
- Date : 17/11/2020
- Fonctionnalités

### <a name="impacted-audience"></a>Public concerné  

Les partenaires effectuant des transactions commerciales via le programme Fournisseur de solutions cloud (CSP) dans la région EU/AELE 

### <a name="summary"></a>Résumé 

Dans la région UE/AELE (Union européenne/Association Européenne de Libre-Échange), toutes les nouvelles offres commerciales du programme Fournisseur de solutions cloud utiliseront l’emplacement de facturation du partenaire au lieu de l’emplacement de facturation du client. Cela signifie que les partenaires seront facturés par Microsoft en fonction de la devise de leur emplacement géographique plutôt que de celui de leur client. Cela s’effectuera en deux phases : 

- **Phase 1 : Nouveaux clients achetant une nouvelle offre commerciale dans CSP**

À compter de janvier 2021, les partenaires dont les nouveaux clients achètent de nouvelles offres commerciales seront facturés pour ces achats dans la devise de l’emplacement du partenaire. Les partenaires ayant des clients existants qui ont déjà acheté de nouvelles offres commerciales dans CSP continueront à être facturés dans la devise de l’emplacement de facturation du client au cours de cette phase. 

 

- **Phase 2 : Clients existants qui ont acheté une nouvelle offre commerciale dans CSP avant janvier 2021** 

Suite à la phase 1 et au cours de l’année civile 2021, Microsoft fera passer la facturation des nouvelles offres commerciales pour les partenaires ayant des clients existants qui ont acheté une nouvelle offre commerciale dans CSP avant janvier 2021 de la devise de l’emplacement du client à la devise de l’emplacement du partenaire. Les partenaires seront avertis à l’avance avant que ce changement soit implémenté.  

>[Remarque] Ce changement n’affecte que la devise de facturation du partenaire, et non les tarifs des nouvelles offres commerciales dans CSP. 

Les nouvelles offres commerciales concernées par ce changement sont les suivantes : Abonnements Azure qui font partie d’un plan Azure, de réservations Azure, d’abonnements de serveur, de logiciels perpétuels et d’achats de la Place de marché commerciale Microsoft sont achetés le programme Fournisseur de solutions Cloud.

### <a name="partner-benefits"></a>Avantages pour les partenaires  

- Cette mise à jour réduira la complexité et la surcharge liées à la facturation multidevise dans la région UE/AELE pour la nouvelle expérience commerciale.  

- Les partenaires recevront une facture consolidée dans une devise unique, et ne recevront plus de facture pour chaque devise d’emplacement des clients. 

- Les paiements d’incentives seront effectués dans la même devise que la devise de facturation du partenaire.

- Les partenaires remarqueront une réduction de la complexité due à la facturation multidevise, libérant ainsi le temps et les ressources actuellement associés au rapprochement des comptes. 

- Pour les partenaires qui n’ont pas encore adopté de nouvelles offres commerciales, ce changement s’aligne sur le modèle de facturation de partenaire précédent, ce qui permet aux partenaires de basculer plus facilement vers la nouvelle expérience commerciale dans CSP. 

### <a name="resources"></a>Ressources 

Passez en revue les informations relatives à cette rubrique dans [Galerie d’opérations] (https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ sur le site web des partenaires Microsoft.  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>Limitation des API aux partenaires appelant les API de l’Espace partenaires

### <a name="categories"></a>Catégories

- Date : 17/11/2020
- Fonctions

### <a name="summary"></a>Résumé

Microsoft introduit une limitation d’API aux partenaires qui appellent des API de l’Espace partenaires, afin de bénéficier d’une meilleure cohérence des performances dans un laps de temps donné.

### <a name="impacted-audience"></a>Public concerné

Les partenaires effectuant des transactions commerciales via le programme Fournisseur de solutions cloud (CSP)

### <a name="details"></a>Détails

Microsoft implémente la limitation des API au 1er trimestre 2021 afin de bénéficier d’une meilleure cohérence des performances dans un laps de temps donné pour les partenaires appelant les API de l’Espace partenaires. La limitation restreint le nombre de requêtes envoyées à un service dans un intervalle de temps donné, afin d’empêcher l’utilisation excessive des ressources. Lorsqu’un seuil de limitation est dépassé, l’Espace partenaires limite les requêtes ultérieures de ce client pendant un certain temps.  

### <a name="partner-benefits"></a>Avantages pour les partenaires 

L’Espace partenaires est conçu pour gérer un volume élevé de requêtes, mais si un nombre excessif de requêtes est effectué par quelques partenaires, la limitation permet de maintenir des performances et une fiabilité optimales pour tous les partenaires. Cela garantit un temps d’arrêt minimal. En réduisant le volume élevé de requêtes, nous pouvons garantir des performances cohérentes pour tous les partenaires. 


### <a name="apis-to-be-throttled"></a>API devant être limitées

|**opération**|**Documentation sur Espace partenaires**|
|-------------------------|----------------------------------|
|{baseURL}/v1/customers/{customer_id}/subscriptions|[Obtenir tous les abonnements d’un client](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[Obtenir un abonnement par ID](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/customers/{customer_id}/orders||[Obtenir toutes les commandes d’un client](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}|[Obtenir une commande par ID](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus|[Obtenir l’état de provisionnement d’un abonnement](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[Gérer les commandes et gérer un abonnement](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons|[Obtenir la liste des extensions d’un abonnement](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements|[Obtenir la liste des droits Azure d’un abonnement](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus|[Obtenir l’état d’inscription d’un abonnement](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/customers/{customer-tenant-id}/transfers|[Obtenir tous les transferts d’un client](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{upgrade-id}/status|[Obtenir l’état de mise à niveau du produit](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions|[Obtenir la liste des offres de conversion d’essai](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

Cette annonce a pour but de fournir aux partenaires une connaissance anticipée des changements à venir, afin de leur permettre de se préparer. Nous recommandons vivement aux partenaires de se familiariser avec ces API et de réfléchir à l’utilisation de l’API du journal d’activité afin d’optimiser l’efficacité et d’éviter toute limitation. Pour plus d’informations sur cette fonctionnalité, reportez-vous aux détails fournis dans [Aide sur la limitation des API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance). 

### <a name="next-steps"></a>Étapes suivantes

Passez en revue l’[Aide sur la limitation des API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance) et prenez les mesures nécessaires. 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>Erreurs 409 dues à des requêtes MCA en double

### <a name="categories"></a>Catégories

- Date : 16/11/2020
- Fonctionnalités

### <a name="context"></a>Context

- En février de cette année, les partenaires ont été invités à signer le Contrat client Microsoft (MCuA). Il s’agissait d’une migration à partir du contrat Microsoft Cloud (MCA). 
- Dans le cadre de ce changement, il a été demandé aux partenaires d’inclure le paramètre Type d'accord comme indiqué [ici](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement).

### <a name="what-happened-next"></a>Que s’est-il passé ensuite ?

- Tous les partenaires n’ont pas inclus la demande de paramètre dans leur implémentation. Microsoft a retourné le MCA à ces partenaires.
- Le partenaire devait alors renvoyer la demande de signature au client, et renvoyer le MCA à Microsoft. 
- La duplication a affecté la capacité de Microsoft à fournir un service aux partenaires.
- En septembre 2020, nous avons envoyé une notification aux partenaires, par le biais de Yammer dans plusieurs forums, leur demandant de corriger le paramètre. Microsoft ne pouvait plus accepter les doublons et les partenaires recevraient des erreurs 409.

>[Remarque] Il ne s’agissait PAS d’un nouveau contrat/changement d’API pour les partenaires.

- En octobre, nous avons travaillé en étroite collaboration avec les partenaires qui avaient le plus de demandes en double en vue de résoudre le problème.
- Actuellement, nous envoyons des rappels aux partenaires ainsi que des e-mails personnels aux 10 principaux partenaires en infraction les invitant à examiner leurs demandes et à nous contacter afin que nous puissions les aider à tester et à résoudre le problème.
- Le 10 novembre 2020, nous avons cessé d’accepter les doublons, et les partenaires qui n’avaient pas corrigé les paramètres ont rencontré des erreurs 409.
- Nous avons depuis annulé cette décision de ne pas accepter les doublons. 
- Toutefois, le 14 janvier 2021, nous recommencerons à ne plus accepter les doublons. Les partenaires disposent ainsi de davantage de temps pour effectuer des ajustements de leur côté. Nous avons déjà reçu une notification de la part d’un partenaire indiquant qu’il prévoit de déployer une mise à jour le 16/11, sur laquelle nous travaillerons en étroite collaboration avec lui.
- Nous demandons aux partenaires de nous contacter afin que nous puissions les aider à effectuer des tests en ajoutant leurs locataires à une version d’évaluation avec les changements, de sorte qu’ils puissent garantir que la mise à jour de leur solution fonctionne comme prévu.



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>Tests disponibles : mises à jour des API de l’Espace partenaires et améliorations de l’interface utilisateur pour le processus de validation des clients Éducation

### <a name="categories"></a>Catégories

- Date : 10/11/2020
- Fonctionnalités | Améliorer l’efficacité et mettre l’échelle

### <a name="impacted-audience"></a>Public concerné

Partenaires proposant des offres Éducation dans le cadre du programme Fournisseur de solutions Cloud (CSP).

### <a name="summary"></a>Résumé

Des tests sont désormais disponibles pour les mises à jour des API de l’Espace partenaires et les améliorations de l’interface utilisateur concernant le processus de validation des clients Éducation.

### <a name="details"></a>Détails

Chez Microsoft, la confiance est notre priorité. Nous nous engageons à fournir une méthode de validation des clients conforme, sûre et sécurisée pour les transactions d’offres Éducation dans le programme Fournisseur de solutions Cloud. Dans le cadre de cet engagement, nous allons introduire des améliorations de l’interface utilisateur et des API de l’Espace partenaires au cours du deuxième trimestre de notre exercice (T2 de l’exercice 2021). Ces améliorations renforceront la clarté et la visibilité du processus de validation des clients, et permettront la saisie de données plus précises en vue d’améliorer cette validation.

**Améliorations de l’Espace partenaires**

- Nouvelles API de qualification GET et POST pour prendre en charge la saisie de données précises et améliorer le processus de validation des clients Éducation par Microsoft.

- Améliorations de l’interface utilisateur pour prendre en charge la saisie de données précises et perfectionner le processus de validation des clients Éducation par Microsoft.

Test

Pour mieux comprendre les API et les données nécessaires à la réussite de la validation des clients, les partenaires pourront tester ces améliorations à compter d’octobre 2020. Nous vous fournirons bientôt plus de détails sur la date exacte de cette opportunité et sur la façon d’y participer. Les API existantes de l’Espace partenaires seront mises hors service avant la fin du deuxième trimestre de l’exercice 2021. À ce moment-là, vous devrez être passé aux nouvelles API de l’Espace partenaires.

   - Tests disponibles. Les dates de test des partenaires s’étendent du 2 octobre au 2 décembre 2020. Les partenaires qui souhaitent participer doivent télécharger le Guide de test des clients Éducation de l’Espace partenaires pour savoir comment se préparer, comment s’inscrire et à quoi s’attendre pendant la phase de test.

**Clients des bibliothèques et musées**

En plus de ces améliorations, nous sommes ravis d’annoncer la mise en place au cours du deuxième trimestre de l’exercice 2021 d’offres à prix Éducation pour les clients des bibliothèques et musées, élargissant ainsi le nombre de clients Éducation auxquels vous pouvez proposer des offres Fournisseur de solutions Cloud.

Microsoft se réserve le droit d’examiner le status d’un client ou d’un client proposé pour déterminer s’il répond aux critères d’un utilisateur Éducation. Pour plus de détails, reportez-vous aux [conditions que doit remplir un utilisateur pour bénéficier des offres Éducation](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7).

## <a name="next-steps"></a>Étapes suivantes

Passer en revue les nouveaux changements apportés à l’interface utilisateur et aux API de l’Espace partenaires, ainsi que le Guide de test disponible dans la [collection de contenus sur les améliorations du processus de validation des clients Éducation dans l’Espace partenaires](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

• Inscrivez-vous pour participer aux tests. (Pour plus d’informations, consultez le [Guide de test](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf).) 

• Vérifiez que les [conditions que doit remplir un utilisateur pour bénéficier des offres Éducation](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7) sont connues dans votre organisation. 

• Partagez ces informations avec les équipes appropriées au sein de votre organisation, ainsi qu’avec vos revendeurs pour les aider à anticiper ces changements.



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>Expansion du contenu partenaire des licences commerciales dans la Galerie de préparation à l’exploitation

### <a name="categories"></a>Catégories

- Date : 5-11-2020
- Fonctions

### <a name="summary"></a>Résumé

À compter du 5 novembre 2020, le contenu partenaire des licences commerciales de l’Université partenaire sera également disponible dans la Galerie de préparation à l’exploitation.

### <a name="impacted-audience"></a>Public concerné

Partenaires commerciaux

### <a name="details"></a>Détails

À compter du 5 novembre 2020, le contenu partenaire des licences commerciales de l’Université partenaire sera également disponible dans la Galerie de préparation à l’exploitation. Cela regroupe le contenu de lancement partenaire des licences commerciales et opérationnel existant dans la Galerie de préparation à l’exploitation avec notre contenu partenaire permanent de licences commerciales de l’Université partenaire. Les partenaires bénéficieront ainsi d’une expérience de préparation ininterrompue. Les regroupements suivants ont été ajoutés à la Galerie de préparation à l’exploitation :

- [Microsoft Azure - Offres et licences](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [Licences commerciales - Appel mis en lumière du programme CSP](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [Licence commerciale - Appel des mises à jour des licences](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>Étapes suivantes

Communiquez ces informations à tous les contacts concernés de votre organisation.

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5">Lancement de la référence SKU Premium pour Salles Microsoft Teams</a>

### <a name="categories"></a>Catégories

- Date : 3-11-2020
- Offres/marchés

### <a name="summary"></a>Résumé

La référence SKU Salles Microsoft Teams Premium pour Microsoft Teams par le biais du programme Fournisseur de solutions Cloud (CSP) est désormais disponible.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

La nouvelle référence SKU Salles Microsoft Teams Premium pour Salles Microsoft Teams est maintenant disponible pour vos clients qui achètent auprès d’un CSP en passant par vous, au prix de 50 USD par appareil et par mois. La référence SKU Salles Microsoft Teams Premium est une alternative à la référence SKU Salles Microsoft Teams Standard (anciennement appelée « Licence Salle de réunion »). Cette référence SKU comprend tous les éléments de l’offre standard, comme les licences nécessaires pour Microsoft Teams, Skype Entreprise Online et la gestion Intune. L’offre permet également d’utiliser le Système téléphonique, nécessaire à l’intégration du réseau téléphonique commuté, et l’Audioconférence, le cas échéant. 

Avec l’offre Premium, les clients ont accès aux nouveaux services managés de Salles Microsoft Teams, où des experts s’occupent de la gestion et de l’exploitation des salles de réunion pour le compte du client. Ce service de gestion et de supervision informatique cloud assure la mise à jour et la sécurité des appareils de Salles Microsoft Teams et de leurs périphériques. Ils sont également supervisés et gérés de manière proactive, en maintenant un environnement optimisé pour une expérience optimale dans les salles.

#### <a name="released-at-launch"></a>Publiées dès le lancement

   |****|**Salles Microsoft Teams Standard - 15 USD par appareil et par mois**|**Salles Microsoft Teams Premium - 50 USD par appareil et par mois**|
   |-------------------|:------|:------|
   |Skype Entreprise|Oui| |
   |Microsoft Teams|Oui|Oui|
   |Système téléphonique|Oui|Oui|
   |Audioconférence|Oui|Oui|
   |Microsoft Intune|Oui|Oui|
   | |Salles Microsoft Teams Standard - 15 USD par appareil et par mois|Salles Microsoft Teams Premium - 50 USD par appareil et par mois|
   |Services managés de Salles Microsoft Teams| |Oui|
   |Disponibilité mondiale|Oui|Sur certains marchés|

#### <a name="microsoft-teams-rooms-managed-services"></a>Services managés de Salles Microsoft Teams

- Gestion proactive : Gestion 24x7x365 de vos systèmes de salle, y compris la mise à jour corrective, la gestion de la configuration, etc.
•   Supervision en temps réel et analyse des causes racines : Supervision et détection, avec une réponse de la gestion orchestrée des incidents par Microsoft en coordination avec le client, quand c’est nécessaire. L’application mobile vous permet de rester alerté quand vous êtes en déplacement.
- Mises à jour managées : Gestion et distribution des mises à jour des applications, de la Base de connaissances Windows et des microprogrammes.
- Protection contre les menaces de sécurité : Protection contre les menaces de sécurité par le biais de la protection avancée contre les menaces Microsoft Defender.
- Support technique : Support par tickets 24x7x365 via notre centre d’opérations des services dédié avec remédiation assistée des incidents pour les cas non automatisés. Contrôle précis de l’accès en fonction du rôle.
- Insights et recommandations : Des insights agrégés entre les clients et les rapports sur l’intégrité des salles, l’inventaire, l’utilisation, les réunions en ligne et les tendances des incidents.

#### <a name="offer-details"></a>Détails de l'offre

   |**Nom de l'offre**|**ID de l’offre**|**ID de contenu**|
   |-------------------|:------|:------|
   |Salles Teams Premium|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Salles Teams Premium (États-Unis et Canada)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Salles Teams Premium pour les universités|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>Étapes suivantes

- Pour vous familiariser avec la nouvelle offre et sa disponibilité géographique, consultez les [questions fréquentes (FAQ)]().
- Familiarisez-vous avec la nouvelle offre et sa disponibilité géographique. 
- Découvrez plus d’informations sur Salles Microsoft et les offres associées dans [Salles Microsoft Teams](https://rooms.microsoft.com/).
- Utilisez le [Guide du partenaire Teams](https://aka.ms/teamscallingmeetingsguide) pour développer votre pratique des salles de réunion Teams et créer une offre prête pour la co-vente.
- Pour en savoir plus sur la solution et les services du produit, passez en revue les [Questions fréquentes (FAQ) sur Salles Microsoft Teams](https://aka.ms/PartnerMTRFAQ). 
- Partagez ces informations avec tous les contacts concernés de votre organisation, et découvrez les opportunités de ventes incitatives et de ventes croisées.

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>Nouvelles références SKU Microsoft Teams Advanced Communications pour le Cloud de la communauté du secteur public bientôt disponibles

### <a name="categories"></a>Catégories

- Date : 2020-11-2
- Offres/marchés

### <a name="summary"></a>Résumé

La nouvelle référence SKU du module complémentaire Advanced Communications pour Microsoft Teams dans le Cloud de la communauté du secteur public sera disponible le 1er décembre 2020.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

Le nouveau module complémentaire Advanced Communications pour Microsoft Teams dans le Cloud de la communauté du secteur public est disponible au prix de 12 USD par utilisateur et par mois. Les références SKU du module complémentaire peuvent être achetées en plus de toute autre suite Microsoft 365 comprenant Microsoft Teams. Advanced Communications offre un nouvel ensemble de fonctionnalités pour les grandes réunions, les stratégies de communication et les intégrations, ainsi que des outils avancés de gestion informatique. 

#### <a name="offer-details"></a>Détails de l'offre

   |**Nom de l'offre**|**ID de l’offre**|**ID de contenu**|
   |-------------------|:------|:------|
   |Advanced Communications pour le Cloud de la communauté du secteur public|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>Forum aux questions 

**Présentation d’Advanced Communications** Ce nouveau module complémentaire Microsoft Teams permet aux clients d’améliorer leur expérience de communication. Il peut être acheté en plus de n’importe quelle référence SKU Microsoft 365 à laquelle les clients sont abonnés.

**Combien ça coûte ?** Le prix de revente estimé est de 12 USD par utilisateur et par mois.

**Quels types de clients peuvent acheter le module complémentaire ?** Les clients du Cloud de la communauté du secteur public peuvent acheter le module complémentaire.

**Comment acheter ?** Le module complémentaire peut être acheté par le biais des programmes Contrat Entreprise, Contrat Souscription Entreprise, Inscription aux solutions d’éducation, Fournisseur de solutions Cloud ou Web Direct.

**Où vendre ?** Il peut être vendu sur le marché américain.

**Quels sont les prérequis ?** N’importe quelle suite Microsoft 365 ou Office 365 qui comprend Microsoft Teams peut bénéficier de ce module complémentaire.

### <a name="next-steps"></a>Étapes suivantes

Fournissez ces informations aux personnes concernées de votre organisation et découvrez les opportunités de ventes incitatives et de ventes croisées. Consultez la section Ressources du [Guide des partenaires Teams](https://aka.ms/teamscallingmeetingsguide).

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365 : Lancements récents et à venir de nouveaux produits et offres

### <a name="categories"></a>Catégories

- Date : 2020-11-2
- Offres/marchés

### <a name="impacted-audience"></a>Public concerné

Fournisseurs directs, fournisseurs indirects et revendeurs indirects.

### <a name="details"></a>Détails

#### <a name="new-offers"></a>Nouvelles offres

Le 1er novembre 2020, Microsoft a publié des offres Dynamics 365 Project Operations et a supprimé Dynamics 365 Project Service Automation (PSA) pour les clients commerciaux. Cette communication fournit des informations supplémentaires sur le mappage des droits d’utilisation double à l’occasion de ce lancement et de nouvelles offres incorporées d’éditeurs de logiciels indépendants (ISV).

#### <a name="project-operations-isv-embed-offers"></a>Offres ISV Embed pour Project Operations

Le 1er novembre 2020, Microsoft a publié trois autres offres ISV Embed de 36 mois pour Dynamics 365 for Project Operations à l’attention des clients du programme Fournisseur de solutions Cloud (CSP). Pour obtenir des détails sur les références SKU, consultez l’onglet Project Operations dans le [document Excel Dynamics CSP Offers-November 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls).

#### <a name="project-operations-dual-use-rights-mapping"></a>Mappage des droits d’utilisation double pour Project Operations

Vous trouverez des informations sur le mappage au niveau local des droits d’utilisation double de Dynamics 365 pour les offres Project Operations dans le tableau suivant :

   |**Offre D365 Operations**|**Mappage des droits d’utilisation double au niveau local de D365**|
   |-------------------|:------|
   |Offre D365 Operations|Mappage des droits d’utilisation double au niveau local de D365|
   |D365 Project Operations|D365 for Operations, en local (serveur AX) utilisant la référence SKU Dyn365 Project Operations (109108477)|
   |D365 Project Operations Attach|D365 for Operations, en local (serveur AX) utilisant la référence SKU Dyn365 Project Operations (109108477)|
   |D365 Finance avec Project Operations|D365 for Operations, en local (serveur AX) utilisant la référence SKU Dyn365 Project Operations (109108477)|
   |D365 Finance Attach avec Project Operations|D365 for Operations, en local (serveur AX) utilisant la référence SKU Dyn365 Project Operations (109108477)|
   |D365 Unified Operations – Activity avec Project Operations|D365 for Operations, en local (serveur AX) utilisant la référence SKU Dyn365 Project Operations (109108477)|

#### <a name="previously-announced"></a>Annonces précédentes

Le 1er novembre 2020, Microsoft a publié les offres et produits Dynamics 365 et Power Platform suivants, comprenant des nouveautés et des mises à jour, pour CSP :

- Dynamics 365 Customer Voice USL 

Pour obtenir des détails sur les ID des offres, passez en revue l’onglet Project Operations dans le [document Excel Dynamics CSP Offers-November 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls).

Vous trouverez d’autres ressources dans la page d’accueil de Microsoft Dynamics 365 Customer Voice.

### <a name="next-steps"></a>Étapes suivantes

Partagez ces informations avec les personnes concernées dans votre organisation.

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>Présentation de Microsoft 365 Business Voice pour les organisations à but non lucratif

### <a name="categories"></a>Catégories

- Date : 2020-11-2
- Offres/marchés

### <a name="summary"></a>Résumé

Le 1er novembre 2020, Microsoft a introduit de nouvelles références SKU pour Microsoft 365 Business Voice pour les organisations à but non lucratif.

### <a name="impacted-audience"></a>Public concerné

Fournisseurs directs, fournisseurs indirects et revendeurs indirects.

### <a name="details"></a>Détails

Le 1er novembre 2020, Microsoft a introduit de nouvelles références SKU pour Business Voice. La suite complète est disponible au Canada, au Royaume-Uni et aux États-Unis. Business Voice (sans forfait d’appels) est disponible dans tous les autres marchés. 

Microsoft 365 Business Voice est un système téléphonique basé sur le cloud destiné aux petites et moyennes entreprises et intégré à Office 365. L’ajout de Business Voice à l’abonnement Office 365 d’un client offre une solution de communication et de collaboration tout-en-un avec appel, conversation et réunions dans une application unique, Microsoft Teams.

Pour plus d’informations sur les tarifs, consultez la liste des prix.

Microsoft 365 Business Voice peut être ajouté aux abonnements suivants pour un maximum de 300 utilisateurs :

- Office 365 : Business Essentials, Business Premium, A1, E1, A3 et E3
- Microsoft 365 : Business, A3 et E3


### <a name="next-steps"></a>Étapes suivantes

- Familiarisez-vous avec les tarifs préliminaires et partagez ces informations avec tous les contacts appropriés dans votre organisation. 
- Passez en revue tous les éléments de préparation de la galerie de ressources des mises à jour du programme Fournisseur de solutions Microsoft Cloud : [Présentation de Microsoft 365 Business Voice pour les petites et moyennes entreprises](https://partner.microsoft.com/resources/collection/m365-voice-smb#/). 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>Promotion Fournisseur de solutions Cloud (CSP) pour Microsoft 365 Business Voice désormais disponible

### <a name="categories"></a>Catégories

- Date : 2020-11-2
- Offres/marchés

### <a name="summary"></a>Résumé

Tarifs réduits disponibles pour les nouveaux abonnements et les renouvellements d’abonnement à Microsoft 365 Business Voice avec forfait d’appels et Microsoft 365 Business Voice sans forfait d’appels.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions via le programme CSP

### <a name="details"></a>Détails

Du 1er novembre 2020 au 30 avril 2021, les nouveaux abonnements et les renouvellements d’abonnement à Microsoft 365 Business Voice avec forfait d’appels et Microsoft 365 Business Voice sans forfait d’appels bénéficient de tarifs réduits. Microsoft 365 Business Voice avec forfait d’appels bénéficie d’une remise de 25 % pendant 12 mois, et Microsoft 365 Business Voice sans forfait d’appels d’une remise de 33 % pendant 12 mois. 

#### <a name="offer-details"></a>Détails de l'offre

   |**Nom de l'offre**|**ID de l’offre**|**ID de contenu**|
   |-------------------|:------|:------|
   |Promotion pour l’adoption de Microsoft 365 Business Voice|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Promotion pour l’adoption de Microsoft 365 Business Voice|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Promotion pour l’adoption de Microsoft 365 Business Voice (US)|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Promotion pour l’adoption de Microsoft 365 Business Voice (sans forfait d’appels)|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Promotion pour l’adoption de Microsoft 365 Business Voice (sans forfait d’appels)|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Promotion pour l’adoption de Microsoft 365 Business Voice (sans forfait d’appels)|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |Promotion pour l’adoption de Microsoft 365 Business Voice (sans forfait d’appels) pour les États-Unis|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

Ces promotions affectent les clients suivants :

- Nouveaux locataires client
- Locataires de clients existants qui n’ont pas d’abonnement actif ou récemment annulé (au cours des 30 derniers jours) sur une licence Business Voice ou Audioconférence sur CSP, Web Direct ou tout autre canal commercial Microsoft

#### <a name="additional-resources"></a>Ressources supplémentaires

- Pour plus d’informations sur Business Voice, visitez la [page des partenaires Microsoft 365 Business Voice](https://www.microsoft.com/microsoft-365/partners/businessvoice). 
- Pour plus d’informations sur cette promotion, consultez les [questions fréquentes (FAQ) pour les partenaires](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo).

### <a name="next-steps"></a>Étapes suivantes

- Familiarisez-vous avec ces opportunités de promotion pour réunions et appels, et partagez ces informations avec tous les contacts appropriés au sein de votre organisation.
- Incorporez ces promotions dans vos processus de ventes Microsoft 365.
- Sensibilisez les clients à la valeur offerte par l’ajout de Business Voice ou à Teams. 

________________
