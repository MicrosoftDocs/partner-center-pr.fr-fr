---
title: Annonces de mars 2021
description: Annonces du mois de mars 2021 pour l’Espace partenaires Microsoft, avec notamment les nouvelles fonctionnalités, les promotions, les offres, les marchés ou les changements apportés aux offres existantes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374384"
---
# <a name="march-2021-announcements"></a>Annonces de mars 2021

Cette page contient les annonces de l’Espace partenaires Microsoft de mars 2021.

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a>API de validation des adresses client CSP mise à jour disponible pour les tests

### <a name="categories"></a>Catégories

- Date : 31/03/2021
- Fonctions

### <a name="summary"></a>Résumé

Dans le cadre de notre engagement à aider les partenaires et les clients à exercer leur activité en toute confiance, nous invitons les partenaires dans le monde entier à tester les modifications apportées à l’API ValidateAddress.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires à facturation directe CSP et les fournisseurs indirects qui créent ou mettent à jour les détails des adresses client existantes

### <a name="details"></a>Détails

Chez Microsoft, la confiance est notre priorité. Nous nous engageons à fournir une méthode de validation des adresses client conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme CSP. Aujourd’hui 31 mars 2021, nous avons introduit des modifications à l’API ValidateAddress que nous souhaiterions vous convier à tester, avant de valider et publier ces modifications en juin 2021. 

Notez que ces modifications affectent uniquement l’API ValidateAddress. Les API CreateCustomer et UpdateBillingProfile ne sont pas affectées.

La réponse renverra l’un des messages d’état suivants :

| Statut | Description | Nombre d’adresses suggérées retournées |
|----------|-------------|-------------------|
| VerifiedShippable | L’adresse est vérifiée, et valide en tant qu’adresse d’expédition. | Unique |
| Verified | L’adresse est vérifiée. | Unique |
| InteractionRequired | Les adresses suggérées ont beaucoup changé et nécessitent une confirmation de l’utilisateur. | Unique |
| StreetPartial | La rue donnée dans l’adresse est partielle et nécessite davantage d’informations. | Multiple (maximum trois)|
| PremisesPartial | Les locaux donnés (numéro de bâtiment, numéro de suite, etc.) sont partiels et nécessitent davantage d’informations. | Multiple (maximum trois) |
| Multiple | Il existe plusieurs champs qui sont partiels dans l’adresse (y compris éventuellement StreetPartial et PremisesPartial). | Multiple (maximum trois) |
| Aucun | L’adresse est incorrecte. | Aucun |
| NotValidated | L’adresse n’a pas pu être envoyée au processus de validation.  | Aucun |

Une fois qu’une adresse a été soumise pour être validée par le biais de l’API ValidateAddress, le schéma de réponse suivant est retourné :

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Observez cet exemple de réponse : Notez que pour les États-Unis, la réponse retournera un suffixe supplémentaire à quatre chiffres pour la ligne de code postal si vous n’entrez que cinq chiffres pour le code postal.

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Étapes suivantes

- Partagez votre ID de locataire sandbox avec notre expert technique, Ali kaki, afin de l’inclure dans la série de tests et de pouvoir commencer à préparer la mise à jour.

- Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.

### <a name="questions"></a>Des questions ?

Si vous avez des questions ou si vous avez besoin d’un support pour vos opérations avec Microsoft, contactez votre groupe Yammer de support partenaire.

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Nouvelle expérience du centre d’administration Exchange (EAC)

### <a name="categories"></a>Catégories

- Date : 29/03/2021
- Fonctions

### <a name="summary"></a>Résumé

À compter du 27 avril 2021, le Centre d’administration Exchange proposera une nouvelle expérience qui améliorera l’efficacité quotidienne pour les utilisateurs.

### <a name="impacted-audience"></a>Public concerné

Administrateurs délégués accédant à Exchange par le biais de l’Espace partenaires

### <a name="details"></a>Détails

À compter du 27 avril 2021, les partenaires qui accèdent à Exchange par le biais de l’Espace partenaires seront redirigés vers le nouveau Centre d’administration Exchange.

Cette nouvelle expérience est actuellement disponible en préversion, et les administrateurs peuvent l’activer en sélectionnant le bouton bascule qui se trouvent dans le coin supérieur droit dans le Centre d’administration Exchange classique. Ils peuvent également accéder au nouveau Centre d’administration Exchange en sélectionnant la bannière « Essayer maintenant » visible dans toutes les pages.

Les avantages du nouveau Centre d’administration Exchange sont les suivants :

- Ajout d’insights, de rapports et de mécanismes d’alerte pour les problèmes liés au flux de courrier 

- Tableaux de bord personnalisés pour augmenter la productivité

Pour vous aider à naviguer dans la nouvelle expérience, des vidéos sont disponibles dans la section **Formation et guide** de la nouvelle expérience de Centre d’administration Exchange. Elles fournissent une vue d’ensemble de la façon dont vous pouvez utiliser le nouveau portail.

>[!NOTE]
>Ce changement n’implique pas la dépréciation de l’expérience de Centre d’administration Exchange classique. Vous serez avertis bien à l’avance de l’implémentation de ce changement.

### <a name="next-steps"></a>Étapes suivantes

- Consultez les [ressources à ce sujet](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), où vous pourrez voir des captures d’écran de la nouvelle expérience.

- Partagez ces informations avec les parties prenantes concernées de votre organisation. 

### <a name="questions"></a>Des questions ?

Pour toute question sur ces changements, consultez vos communautés Yammer appropriées.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations : Présentation du calendrier de lancement des produits

### <a name="categories"></a>Catégories

- Date : 25/03/2021
- Offres | Espace de travail moderne

### <a name="summary"></a>Résumé

En réponse aux commentaires des partenaires, Microsoft Operations va rationaliser les communications pour les lancements de produits.

### <a name="impacted-audience"></a>Public concerné

Partenaires CSP (Fournisseur de solutions Cloud)

### <a name="details"></a>Détails

Microsoft s’engage à améliorer continuellement les expériences des partenaires. Nous avons reçu des commentaires indiquant que vous receviez trop de communications de la part de Microsoft, y compris des annonces en double pour les lancements de produits.

En réponse à vos commentaires, Microsoft a rationalisé l’expérience de préparation aux lancements de produits pour les offres nouvelles et existantes.

Nous vous proposons désormais une vue mensuelle unique des lancements de produits, publiée dans la galerie des ressources Operations Readiness. Cette [vue mensuelle du calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) remplace les communications de lancement de produit individuelles dans la galerie des ressources Operations Readiness et dans les annonces de l’Espace partenaires.

Vous pouvez également accéder à ce [calendrier de lancement de produit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) à partir des [collections de la communauté](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), des [vues de calendrier](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) et des [bulletins CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/). Nous vous informerons quand nous publierons le calendrier de lancement de produit de chaque mois avec une annonce dans la galerie des ressources Operations Readiness.

Vous trouverez toujours des informations sur les offres nouvelles et existantes dans l’aperçu des tarifs et dans les journaux de modification des tarifs, ainsi que dans les blogs de produit, les guides de licences et les pages marketing des produits.

Le changement s’appliquera aux lancements pour les produits suivants :

- Dynamics local
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Serveur  
- Outils
- Teams et Telco

Nous continuerons à envoyer des annonces spécifiques pour les lancements de produits qui requièrent des détails Operations Readiness.

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources sur ce sujet et partagez ces informations avec les parties prenantes appropriées au sein de votre organisation.

### <a name="questions"></a>Vous avez des questions ?

Si vous avez d’autres questions sur ces offres, consultez vos communautés Yammer appropriées.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Changements des conditions d’intégration des clients CSP

### <a name="categories"></a>Catégories

- Date : 25/03/2021
- Fonctions

### <a name="summary"></a>Résumé

Dans le cadre de notre engagement à aider les partenaires et les clients à exercer leur activité en toute confiance, nous demanderons des informations supplémentaires sur les clients à compter du 25 mars 2021.

### <a name="impacted-audience"></a>Public concerné

Fournisseurs indirects et partenaires à facturation directe CSP qui ont des clients nouveaux ou existants dans les pays listés dans la section suivante.

### <a name="details"></a>Détails

Chez Microsoft, la confiance est notre priorité. Nous nous engageons à fournir une méthode de validation des clients conforme, sûre et sécurisée pour les transactions liées aux abonnements des clients dans le cadre du programme Fournisseur de solutions Cloud. Le 25 mars 2021, nous présenterons des améliorations de l’interface utilisateur et de l’API de l’Espace partenaires qui affecteront les partenaires répondant aux deux critères suivants :

1. Le partenaire a une relation de facturation directe avec Microsoft (ce qui signifie que le partenaire est un partenaire à facturation directe ou un fournisseur indirect).

2. Le partenaire fait affaire avec des clients nouveaux ou déjà existants dans les pays suivants :

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

Les partenaires qui satisfont aux critères devront soumettre l’**ID d’inscription d’entreprise** d’un client (également connu sous le nom de **code INN d’organisation** du client) et le **numéro de téléphone** lors de l’intégration de nouveaux clients ou de la modification des informations détaillées d’un client existant. Ces partenaires peuvent également entrer un **deuxième prénom** facultatif pour le client.

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

Les partenaires ayant des clients dans le reste du monde auront la possibilité le 25 mars 2021 d’entrer l’**ID d’inscription d’entreprise**, le **numéro de téléphone** et le **deuxième prénom** pour les clients, au titre d’informations facultatives.

### <a name="next-steps"></a>Étapes suivantes

- Pour obtenir des instructions plus détaillées, consultez la documentation technique et les questions fréquemment posées dans le [groupe de partenaires dédié](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).

- Préparez l’intégration des modifications à l’aide de l’API Espace partenaires et de l’expérience utilisateur web. L’API et les SDK seront disponibles à des fins de test.

- Veillez à soumettre les données supplémentaires lors de l’intégration de nouveaux clients ou de la modification des détails de clients existants.

- Si vous utilisez une solution de fournisseur de panneau de contrôle (CPV), consultez le fournisseur concerné.

### <a name="questions"></a>Des questions ?

Si vous avez des questions liées à l’identificateur légal (également appelé code INN ou TIN), contactez votre conseiller fiscal ou le service des impôts local. Microsoft ne peut pas fournir d’aide sur les questions fiscales.

Si vous avez besoin de support pour vos opérations avec Microsoft, [ouvrez une demande de service](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Corrections apportées à la liste de prix des logiciels sous licence perpétuelle du 1er mars 2021

### <a name="categories"></a>Catégories

- Date : 23/03/2021
- Offres/marchés

### <a name="impacted-audience"></a>Public concerné

Les fournisseurs indirects et les partenaires de facturation directe réalisant des transactions pour des logiciels perpétuels dans le programme du fournisseur de solutions cloud 

### <a name="details"></a>Détails

La liste de prix pour les logiciels perpétuels publiée le 1er mars 2021 incluait des marchés qui ne devaient pas y figurer. La liste des prix pour les logiciels perpétuels a été mise à jour le 17 mars 2021 avec les corrections. Ces corrections ne s’appliquaient qu’aux éléments suivants :

- ID produit : DF77X4D43RKT 
- Nom du produit : mise à niveau de Windows 10 Famille vers Professionnel pour Microsoft 365 Business
- Marchés supprimés ou non pris en charge : AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Ces modifications s’appliquent uniquement au produit ci-dessus. Les autres produits n’ont pas été corrigés. 

### <a name="next-steps-and-resources"></a>Étapes suivantes et ressources

- Les partenaires qui réalisent des transactions liées à des logiciels perpétuels doivent télécharger la dernière liste de prix pour les logiciels perpétuels.
- Consultez les [codes pays/région](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) pour un mappage convivial de l’abréviation de deux lettres aux pays.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Mise en production du kit SDK sur .NET Standard (v1.17.0)

### <a name="categories"></a>Catégories

- Date : 23/03/2021

- Fonctions
 
### <a name="impacted-audience"></a>Public concerné

Les partenaires de facturation directe et les fournisseurs indirects participant au programme Fournisseur de solutions cloud (CSP) qui utilisent le SDK .NET de l’Espace partenaires.

### <a name="details"></a>Détails

À compter du 23 mars 2021, les partenaires peuvent télécharger la version de [MicrosoftPartnerCenter.NETSDK (Galerie NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) ainsi que les [exemples GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) publics du kit SDK de l’Espace partenaires. Cette version comprend les mises à jour apportées aux méthodes suivantes :

#### <a name="audit-updated-new-operation-types"></a>Audit mis à jour : nouveaux types d’opérations

Ajout de nouveaux [types d’opération](https://docs.microsoft.com/partner-center/develop/auditing-resources) pour savoir quand le client a approuvé et mis fin à la relation avec le DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Audit mis à jour : nouvelle ressource et nouveaux types d’opérations

Ajout de nouveaux [types de ressources et d’opérations](https://docs.microsoft.com/partner-center/develop/auditing-resources) pour la prise en charge du scénario de rôle d’annuaire client.

- Nouveau type de ressource « CustomerDirectoryRole »

- Types d’opérations « AddUserMember » et « RemoveUserMember »

#### <a name="sdk-updates-to-customer-accounts"></a>Mises à jour du kit de développement logiciel (SDK) pour les comptes client

- Prise en charge de GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Modifications supplémentaires

Les modifications suivantes sont introduites dans le cadre de New Commerce et sont actuellement disponibles par invitation uniquement aux partenaires qui font partie de la préversion technique de M365/D365 New Commerce. Les partenaires non inclus dans la préversion technique de New Commerce ne doivent pas notifier les impacts et doivent proposer une compatibilité descendante.

- Modifications du catalogue :

  - GET /products/{product-id}/skus/{sku-id}

- Acheter et gérer :
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Étapes suivantes

- Téléchargez la dernière version de [MicrosoftPartnerCenter.NETSDK (Galerie NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Télécharger et passer en revue les [exemples GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Offre de place de marché commerciale et primes incitatives pour fournisseurs de solutions cloud pour 2021 pour les offres éligibles

### <a name="categories"></a>Catégories

- Date : 18/03/2021
- Fonctions

### <a name="impacted-audience"></a>Public concerné

Fournisseurs indirects et partenaires de facturation directe du programme Fournisseur de solutions cloud 

### <a name="details"></a>Détails

Les fournisseurs indirects et les partenaires de facturation directe du programme fournisseur de solutions cloud peuvent vendre des offres tierces et gagner une prime incitative sous la forme d’une remise pour chaque offre tierce éligible traitée dans l’Espace partenaires ou le Portail Azure. La prime incitative se présente sous la forme d’une remise sur les ventes facturées pour les offres éligibles et est **disponible jusqu’au 30 juin 2021**.  

Continuez à vous familiariser avec cette prime incitative pour fournisseur de solutions cloud Commercial Marketplace Offer ci-dessous et contactez vos clients dès aujourd’hui pour identifier les offres adéquates afin de garantir leur réussite et leur transformation numérique.

Nous travaillons en partenariat avec des éditeurs de logiciels indépendants pour mettre sur le marché les solutions IaaS et SaaS les plus récentes pour les clients Microsoft. Les éditeurs de logiciels indépendants ont la possibilité de permettre les ventes de leurs offres via le canal partenaire Microsoft. Nos offres de prime incitative sont classées en deux catégories :

- Sélectionnez les offres SaaS et IaaS tierces avec le statut de co-vente encouragée Azure IP. 

- Applications SaaS intégrées à Teams ou au moins deux applications de productivité Microsoft 365, telles que PowerPoint, Word, Excel, Outlook ou SharePoint.

### <a name="next-steps-and-resources"></a>Étapes suivantes et ressources

- En savoir plus sur l’obtention de [primes incitatives pour partenaires](https://partner.microsoft.com/membership/partner-incentives) pour la vente d’applications de la place de marché éligibles. De nouvelles offres sont ajoutées chaque mois.  
- [Ressources de primes incitatives pour les partenaires de facturation directe - Fournisseur de solutions cloud](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Ressources de primes incitatives pour les fournisseurs indirects -Fournisseur de solutions cloud](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Consultez cette [Présentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) pour en savoir plus sur la vente des applications de la place de marché commerciale. Consultez les ressources supplémentaires [ici](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Explorez le catalogue de la place de marché commerciale dans l’[Espace partenaires](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) ou sur le [portail Azure](https://ms.portal.azure.com/#home)
- Utilisez des [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) pour intégrer des applications dans la place de marché de votre entreprise
- Contactez les éditeurs de logiciels indépendants qui vous intéressent
- Les fournisseurs indirects doivent s’intégrer à l’aide d’API et guider les revendeurs sur les applications à vendre

### <a name="questions"></a>Des questions ?  

Consultez [cet article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) pour obtenir une vue d’ensemble de la place de marché commerciale dans l’Espace partenaires.

Pour obtenir une assistance supplémentaire, vous pouvez créer une demande de support dans l’Espace partenaires. Pour en savoir plus, rendez-vous sur [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Mise à jour des prérequis et des noms de l’offre Power BI Premium

### <a name="categories"></a>Catégories

- Date : 18/03/2021
- Fonctions

### <a name="summary"></a>Résumé

La liste de prix finale du 1er avril 2021 sera mise à jour pour ajouter de la clarté aux dénominations et/ou aux informations sur la configuration requise pour les offres Power BI par utilisateur.

### <a name="impacted-audience"></a>Public concerné

Fournisseurs de solutions cloud directs et partenaires indirects

### <a name="details"></a>Détails

La liste de prix finale du 1er avril 2021 sera mise à jour pour ajouter de la clarté aux dénominations et/ou aux informations sur la configuration requise pour les offres Power BI par utilisateur.

Jusqu’à ce que la liste de prix finale ait été mise à jour, utilisez les informations de cette section pour vous assurer que le produit adéquat est commandé.

Les détails suivants montrent la référence SKU affectée et les détails de la configuration requise.

| Version préliminaire du nom d’affichage sur la liste de prix du 1er mars |  Nom d’affichage de l’offre mise à jour dans la liste de prix finale du 1er avril| ID de l’offre |
| ------ | ----------- | ----------- |
| Power BI Premium Per User Add-On (Nonprofit Staff Pricing)  |  Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Les clients doivent disposer de l’un des composants requis suivants pour acheter cette offre :

| Nom d’affichage de l’offre | ID de l’offre |
| ------ | ----------- |
| Microsoft 365 E5 (Nonprofit Staff Pricing)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (Nonprofit Staff Pricing)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (Nonprofit Staff Pricing) Trial|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

L’offre de Power BI Premium suivante contient une condition préalable requise pour l’achat :

| Nom d’affichage de l’offre | ID de l’offre |
| ------ | ----------- |
|   Power BI Premium Per User Add-On (Nonprofit Staff Pricing)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Les clients doivent disposer de cette configuration requise pour acheter cette offre :

| Nom d’affichage de l’offre | ID de l’offre |
| ------ |----------|
| Power BI Pro (Nonprofit Staff Pricing)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources sur ce sujet et partagez ces informations avec les parties prenantes appropriées au sein de votre organisation.  

### <a name="questions"></a>Vous avez des questions ?

Pour les questions sur ces offres, consultez vos communautés Yammer appropriées. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Mises à jour des prix de mars de Microsoft 365 F3

### <a name="categories"></a>Catégories

- Date : 16/03/2021
- Offres/marchés

### <a name="summary"></a>Résumé

La tarification incorrecte pour mars 2021 a été corrigée pour Microsoft 365 F3 en livres sterling (GBP) et en euros (EUR).

### <a name="impacted-audience"></a>Public concerné

Les partenaires qui achètent Microsoft 365 F3 en GBP ou EUR entre le 1er mars et le 17 mars 2021 via le programme fournisseur de solutions cloud (CSP).

### <a name="details"></a>Détails

Microsoft a résolu le problème de tarification incorrecte pour Microsoft 365 F3. Les prix incorrects étaient en GBP et EUR et uniquement pour les offres achetées entre le 1er mars et le 17 mars 2021. Les offres et les devises concernées sont reprises ci-dessous. 

| Nom de l’offre | Devise | ID de l’offre | ID de contenu |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Charity) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Commercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Les versions préliminaires des les listes de prix basés sur les licences pour mars et avril ont été mises à jour le 16 mars à 17H00 Heure du Pacifique.

### <a name="next-steps"></a>Étapes suivantes

- Les partenaires doivent retélécharger les listes de prix actuels basés sur les licences : la version préliminaire pour mars et avril, avec les corrections de prix, le cas échéant.  
- Microsoft va contacter les partenaires concernés au cours des prochaines semaines par courrier électronique pour les informer des étapes ultérieures liées à la correction des transactions affectées.

### <a name="questions"></a>Vous avez des questions ?

Pour toute autre question, consultez les communautés Yammer CSP appropriées.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Mettre à jour un nom de société légal dans l’Espace partenaires

### <a name="categories"></a>Catégories

- Date : 16/03/2021
- Assurer efficacité et adaptation

### <a name="summary"></a>Résumé

À partir de mars 2021, les partenaires du MPN (Microsoft Partner Network) et les revendeurs indirects CSP peuvent mettre à jour leur nom de société légal via l’Espace partenaires.

### <a name="impacted-audience"></a>Public concerné

Partenaires MPN et revendeurs indirects CSP (non applicables aux partenaires à facturation directe CSP)

### <a name="details"></a>Détails

À partir de mars 2021, les partenaires MPN et les revendeurs indirects CSP peuvent mettre à jour de manière autonome leur nom de société légal via l’Espace partenaires. Avec cette nouvelle fonctionnalité, les partenaires n’ont plus besoin de soumettre un ticket de support dans l’Espace partenaires pour mettre à jour le nom de leur société. Cela permet aux partenaires de gagner un temps précieux. 

Pour plus d’informations, consultez [Mettre à jour le profil de l’entreprise légale](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Assurez-vous que le nom de la société dans votre profil de société légal est exempt de fautes d’orthographe et d’abréviations, et qu’il correspond exactement à celui figurant au registre officiel des sociétés. Pour plus d’informations sur la mise à jour du profil de votre organisation, consultez [Vérifier le profil de votre organisation](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Étapes suivantes

Partagez ces informations dans votre organisation pour permettre à l’équipe compétente de passer en revue et de mettre à jour ses processus.

### <a name="questions"></a>Des questions ?

Pour toute autre question, consultez les communautés Yammer CSP appropriées.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Mise à jour de l’évolution du programme Fournisseur de solutions cloud (CSP) et changements du programme Open License

### <a name="categories"></a>Catégories

- Date : 15/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

De nouvelles offres logicielles perpétuelles commerciales et pour le secteur public vont être disponibles dans le programme CSP et des changements vont être apportés au programme Open Licensing.

### <a name="impacted-audience"></a>Public concerné

Distributeurs commerciaux et revendeurs managés qui vendent via le programme Open License, ainsi que tous les partenaires CSP qui effectuent des transactions sur les logiciels perpétuels

### <a name="details"></a>Détails

En septembre 2020, Microsoft a [annoncé](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) une série d’étapes dans notre parcours de transformation numérique pour étendre des opportunités aux partenaires du programme CSP, y compris la disponibilité des logiciels locaux pour les partenaires. Ces changements permettent aux partenaires de développer leur activité et d’étendre leur portée en tirant parti des licences logicielles dans le CSP, ce qui leur donne un avantage en termes de réussite dans le monde actuel où le cloud passe avant toute autre technologie. En outre, cela permet aux clients d’effectuer leur transition vers le cloud et offre aux partenaires la flexibilité nécessaire pour les environnements de cloud hybride des clients.

Dans la logique de cette transformation numérique, nous annoncerons les changements suivants :

- Le 1er juillet 2021 : aucun(e) référence SKU, produit ou promotion ne sera ajouté(e) à la liste des prix du programme Open License.

- 7 juillet 2021 : deux offres commerciales, une version authentique de Windows et Visual Studio Professional, ainsi que des offres du secteur public (gouvernement, éducation et organisme à but non lucratif ; voir [l’annonce](./2020-december.md#9)) seront ajoutées à la liste des prix logiciels perpétuels du CSP.  La liste des prix se trouve dans la section Logiciels de la page [Vendre > Tarification et offres](https://partnercenter.microsoft.com/pcv/sales) de l’Espace partenaires et sera republiée à cette date.

Pour obtenir des informations complètes sur l’évolution du programme CSP et les changements du programme Open License, consultez les **Étapes suivantes** ci-dessous.

### <a name="next-steps"></a>Étapes suivantes :

- Évolution du programme CSP : consultez les supports de préparation [Logiciels perpétuels dans le programme Fournisseur de solutions cloud](https://partner.microsoft.com/resources/collection/software-in-csp#/). Utilisez cette [carte de préparation](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) pour localiser rapidement les informations appropriées pour votre rôle.

- Changements du programme Open License : consultez les supports de préparation [Évolution du programme CSP et changements du programme Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/). Utilisez cette [carte de préparation](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) pour localiser rapidement les informations appropriées pour votre rôle.

### <a name="questions"></a>Questions

Pour toute autre question, consultez les communautés Yammer CSP appropriées.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Mise à jour d’une annonce précédente : évaluations Premium, extension du Gestionnaire de conformité

### <a name="categories"></a>Catégories

- Date : 15/03/2021
- Développer votre entreprise

### <a name="summary"></a>Résumé

Les offres d’essai ne doivent pas figurer dans la liste des prix et seront supprimées.

### <a name="impacted-audience"></a>Public concerné

Partenaires effectuant des transactions dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

Les offres d’essai ne doivent pas figurer dans la liste des prix. Elles seront supprimées de la liste des prix le 1er mai 2021.

L’annonce d’origine se trouve [ici](./2021-february.md#4).

### <a name="additional-resources"></a>Ressources supplémentaires

- [Sécurité et conformité de Microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Créer et gérer des évaluations dans le Gestionnaire de conformité Microsoft - Conformité Microsoft 365](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources sur ce sujet et partagez ces informations avec les parties prenantes appropriées au sein de votre organisation.

### <a name="questions"></a>Vous avez des questions ?

Si vous avez des questions sur ces offres, consultez les communautés Yammer appropriées.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrer vos solutions depuis One Commercial Partner (OCP) go-to market (GTM) vers la place de marché commerciale Microsoft

### <a name="categories"></a>Catégories

- Date : 12/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

À partir du 29 mars 2021, vous commencerez à découvrir les fonctionnalités One Commercial Partner (OCP) go-to market (GTM) limitées. Nous vous encourageons à migrer vos solutions vers la place de marché commerciale dans l’Espace partenaires.

### <a name="impacted-audience"></a>Public concerné

Organisations qui co-vendent des solutions dans OCP GTM

### <a name="details"></a>Détails

En décembre 2020, nous avons commencé notre migration de l’outil Microsoft OCP GTM vers la place de marché commerciale Microsoft dans l’Espace partenaires. Cette transition étend les capacités de la place de marché commerciale où vous pouvez présenter vos solutions à des millions de clients, partager de manière bidirectionnelle des opportunités avec d’autres vendeurs Microsoft et partenaires, et co-vendre des solutions innovantes.

L’étape suivante de la transition aura lieu le 29 mars 2021. C’est à ce moment-là que vous allez découvrir des fonctionnalités OCP GTM limitées, avec des champs qui seront désormais en lecture seule. Si vous co-vendez actuellement des solutions dans OCP GTM, nous vous encourageons à migrer vos solutions vers la place de marché commerciale pour tirer parti de ses fonctionnalités et simplifier votre expérience de publication. 

La migration vers la place de marché commerciale fait de l’Espace partenaires la destination principale de l’expérience de publication pour la co-vente. C’est là que vous pouvez continuer à développer votre activité en connectant vos solutions à nos clients partagés via les mêmes canaux et expériences dans les produits que ce que nous utilisons pour les produits Microsoft. [En savoir plus sur la place de marché commerciale](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Étapes suivantes

- Si vous n’avez pas encore migré vos solutions, suivez les instructions détaillées dans le [guide de transition](/azure/marketplace/co-sell-solution-migration) ou consultez le [tutoriel vidéo pas à pas](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) pour effectuer toutes les activités de migration et commencer à publier votre ou vos solutions dans la place de marché commerciale.

- Pour toute question relative aux fonctionnalités limitées dans OCP GTM, consultez la [FAQ sur les exigences de co-vente pour publier dans la place de marché commerciale Microsoft](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Consultez la section « Fonctionnalités limitées dans OCP GTM à partir du 29 mars 2021 ».)

### <a name="questions"></a>Vous avez des questions ?

Contactez le [support](https://partner.microsoft.com/support/?stage=1) si vous avez des questions ou si vous avez besoin de plus d’informations.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Développement de la nouvelle expérience commerciale dans le programme CSP pour Azure en Russie

### <a name="categories"></a>Catégories

- Date : 10/03/2021
- Fonctions

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires en Russie effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud (CSP).

### <a name="details"></a>Détails

À partir du 10 mars 2021, nous sommes ravis d’annoncer la disponibilité de la **nouvelle expérience commerciale dans CSP pour Azure en Russie**. Cette expérience permet de simplifier et d’améliorer la façon dont les clients achètent et utilisent les services Azure. Elle fournit également aux partenaires du programme CSP une vue cohérente de la tarification Azure entre les mouvements des ventes, la tarification en USD à des fins de cohérence générale, l’alignement des dates de facturation et l’accès à Azure Cost Management.

### <a name="next-steps"></a>Étapes suivantes

Plusieurs ressources sont disponibles pour présenter la nouvelle expérience commerciale Azure et fournir des informations supplémentaires. Recherchez les dernières FAQ, les parcours, les vidéos et bien plus encore dans la [Galerie de ressources des mises à jour du programme CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Téléchargement de logiciel et fourniture de clé de licence logicielle dans l’Espace partenaires

### <a name="categories"></a>Catégories

- Date : 04/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

La fonctionnalité de téléchargement de logiciel et de fourniture de clé de licence logicielle a été rétablie.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires fournisseurs de solutions Cloud (CSP) passant des commandes de logiciels avec abonnement perpétuel et pour serveur via l’Espace partenaires

### <a name="details"></a>Détails

En réponse au feedback des partenaires, nous rétablissons la fonctionnalité de fourniture de l’Espace partenaires permettant d’obtenir des logiciels et des clés de licence pour les commandes de logiciels avec abonnement perpétuel et pour serveur. Elle sera rétablie à son état antérieur à sa suppression du 19 janvier 2021. (Consultez l’[annonce](2020-september.md#17).)

Notez que les clés de licence et les liens de téléchargement des logiciels sont des ressources de propriété intellectuelle de valeur et très recherchées. En cas de fuite, elles peuvent rapidement être privées de leurs limites d’activation et entraîner une expérience négative pour les clients et les partenaires.

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources suivantes pour obtenir des instructions d’utilisation et des conseils importants sur la distribution des clés logicielles :

- [Vendre des logiciels locaux via le programme CSP](../csp-on-premise-software.md)
- [Nouveau guide des opérations commerciales de l’Espace partenaires](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Consultez la section **Guide de distribution des clés logicielles**.)

### <a name="questions"></a>Vous avez des questions ?

Si vous avez d’autres questions sur cet avis, consultez vos communautés Yammer appropriées.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrer vos transactions de Partner Sales Connect (PSC) vers l’Espace partenaires

### <a name="categories"></a>Catégories

- Date : 04/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

Partner Sales Connect (PSC) passera à un accès en lecture seule à partir du 31 mars 2021 : nous vous recommandons donc de commencer à migrer vos transactions de PSC vers l’Espace partenaires.

### <a name="impacted-audience"></a>Public concerné

Partenaires avec des transactions dans PSC

### <a name="details"></a>Détails

Dans le cadre de notre engagement partagé pour la croissance, la **co-vente avec Microsoft** est le chemin qui vous permet **d’être connu, d’exercer votre expertise et de développer votre empreinte client** pour des résultats positifs auprès des clients. Avec une transaction moyenne **3,5 fois plus rapide** que la normale, la gestion de votre expérience de co-vente dans l’Espace partenaires vous permet de vendre via les canaux Client direct, Partenaire et Revendeur Microsoft, et de gérer l’intégralité de votre pipeline de référence à un seul endroit.

**PSC** passera à l’**accès en lecture seule** à compter du **31 mars 2021** : nous vous recommandons donc de commencer votre migration vers l’Espace partenaires et d’accéder à ces améliorations de fonctionnalités : 

- Un **routage plus précis** des transactions que vous partagez avec Microsoft vers le revendeur, approprié en fonction du type d’assistance dont vous avez besoin.
- Une **validation préalable de l’éligibilité des transactions** pour les solutions éligibles aux incentives et pour répondre aux critères du programme ISV Connect, simplifiant le processus d’approbation et l’attestation de preuve d’exécution (POE) finale.
- **Expérience utilisateur homogène** pour gérer l’ensemble de vos opportunités de co-vente et des prospects qualifiés pour des ventes à un même endroit.

Nous avons aussi ajouté récemment de nouvelles fonctionnalités dans l’Espace partenaires pour vous aider dans votre migration :

- [Opérations en bloc pour les opportunités de co-vente](../bulk-operations.md)
- [Fonctionnalité de migration des transactions](../psc-to-pc.md) (Consultez la section **Migration des transactions PSC**.)

En utilisant l’expérience de co-vente de l’Espace partenaires, vos équipes commerciales auront davantage de temps pour se concentrer sur la gestion des prospects et des opportunités, sur la conclusion de transactions et sur la création de relations durables avec les clients.

### <a name="next-steps"></a>Étapes suivantes

Utilisez le [guide de transition](../psc-to-pc.md) de l’Espace partenaires pour vous aider tout au long des étapes de migration de vos transactions de PSC vers l’Espace partenaires.

### <a name="questions"></a>Vous avez des questions ?

Pour toute question supplémentaire, contactez le [support](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2">Nouveaux produits et nouvelles offres Microsoft Dynamics 365 disponibles le 1er avril 2021</a>

### <a name="categories"></a>Catégories

- Date : 04/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

Le 1er avril 2021, Microsoft lancera plusieurs nouveaux produits et nouvelles offres pour le programme Fournisseur de solutions Cloud (CSP).

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

Le 1er avril 2021, Microsoft lancera les nouveaux produits et offres suivants :

- Power BI Premium par utilisateur
- Licence d’abonnement utilisateur Customer Voice et Marketing - Extension géographie et segmentation

**Power BI Premium par utilisateur**

Microsoft va introduire les premières offres Power BI Premium par utilisateur. Power BI Premium est actuellement vendu seulement selon un modèle de capacités. Power BI Premium par utilisateur donne accès aux capacités de décisionnel et d’analytique. Sa licence par siège individuel flexible convient aux petites et moyennes entreprises.

Pour plus d’informations sur cette offre, consultez les [détails des versions de Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features).


**Détails de l'offre**

Notez que le nom de l’offre diffère légèrement de la préversion de la liste des prix.

| Nom de l’offre | ID de l’offre |
| ------ |----------- |
| Power BI Premium par utilisateur | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Per User for Faculty | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Per User for Students | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Per User (Nonprofit Staff Pricing) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Per User Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Per User Add-On for Faculty | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Per User Add-On for Students | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Per User Add-On (Nonprofit Staff Pricing) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Licence d’abonnement utilisateur Customer Voice et Marketing - Extension géographie et segmentation**

Suite au lancement de décembre 2020, les offres de licence d’abonnement utilisateur Customer Voice et Marketing Dynamics 365 ont été modifiées : de nouveaux pays et d’autres références SKU pour les organisations sans but lucratif et l’éducation y ont été ajoutés.

| Nom de l’offre | ID de l’offre |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL for Faculty | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Pour en savoir plus sur ces offres, visitez les pages suivantes :

- [Page d’accueil de Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Page d’accueil de Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Étapes suivantes

Passez en revue les ressources sur ce sujet et partagez ces informations avec les parties prenantes appropriées de votre organisation.  

### <a name="questions"></a>Vous avez des questions ?

Pour les questions sur ces offres, consultez vos communautés Yammer appropriées. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Impression universelle Microsoft est maintenant disponible dans certaines suites

### <a name="categories"></a>Catégories

- Date : 03/03/2021
- Fonctionnalités

### <a name="summary"></a>Résumé

Impression universelle Microsoft sera disponible à la vente dans des suites Microsoft 365 sélectionnées et comme module complémentaire autonome à partir du 1er mars 2021.

### <a name="impacted-audience"></a>Public concerné

Tous les partenaires effectuant des transactions commerciales dans le cadre du programme Fournisseur de solutions cloud

### <a name="details"></a>Détails

[Impression universelle](https://aka.ms/universalprint) est un service d’impression Microsoft 365 qui supprime la nécessité de serveurs d’impression locaux et permet aux appareils Windows d’imprimer sur des imprimantes inscrites auprès d’Azure. Il sera disponible à la vente à partir du 1er mars 2021.

Les utilisateurs bénéficient d’une impression sans pilotes, d’une découverte simplifiée des imprimantes basée sur l’emplacement et d’une expérience d’impression intuitive sans aucun apprentissage. Les appareils joints à Azure Active Directory (Azure AD) utilisent les informations d’identification Azure AD existantes pour imprimer de façon sécurisée. Les administrateurs gèrent l’impression en utilisant le portail Azure et peuvent facilement connecter des imprimantes grâce à la prise en charge native d’Impression universelle. Impression universelle peut être déployé avec des imprimantes non compatibles en utilisant un logiciel de connexion à Impression universelle.

Impression universelle sera disponible au lancement pour Windows E3, A3, E5 et A5, et pour Microsoft 365 BP, F3, E3, A3, E5 et A5.  

**Détails de l'offre**

Notez que le nom de l’offre diffère légèrement de la préversion de la liste des prix.

| Nom de l’offre | ID de l’offre | ID de contenu |
| ------ |----------- |----------- |  
| Universal Print volume add-on (500 jobs) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Universal Print volume add-on (500 jobs) for faculty - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Universal Print volume add-on (500 jobs) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Universal Print volume add-on (500 jobs) for faculty - Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Étapes suivantes

Familiarisez-vous avec la liste des prix et la [Vue d’ensemble d’Impression universelle](/universal-print/fundamentals/universal-print-whatis). Communiquez ces informations à tous les contacts concernés de votre organisation.

### <a name="questions"></a>Des questions ?

Pour les questions sur ces offres, consultez vos communautés Yammer appropriées.
