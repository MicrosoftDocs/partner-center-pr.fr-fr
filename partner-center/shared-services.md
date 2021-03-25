---
title: Ajouter Azure Partner Shared Services
description: Utilisez les services partagés partenaires Azure pour acheter des abonnements Azure pour votre usage personnel et pour disposer d’une méthode uniforme pour l’achat, le suivi et la gestion d’Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 756fbfda3438933b50fc51936b396291986472a7
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028279"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Ajoutez des services partagés partenaires Azure pour que les partenaires puissent acheter des abonnements Azure pour leur propre usage

**Rôles appropriés**

- Administrateur général
- Agent d’administration
- Agent commercial

Azure Partner Shared Services est un nouveau type d’offre proposé aux partenaires dans le cadre du programme Fournisseur de solutions Cloud. Il leur permet d’acheter des abonnements Azure pour leur propre usage.Il permet aux partenaires d’utiliser une méthode uniforme pour l’achat, le suivi et la gestion d’Azure, en plus de la possibilité de consolider leurs contrats de licence et de revente Azure avec Microsoft. Avec les services partagés partenaires Azure, les partenaires ont désormais la même flexibilité pour utiliser les abonnements Azure dans CSP que dans les programmes Microsoft Contrat Entreprise et Web direct, en ouvrant des scénarios tels que les environnements de développement et de test, de déployer des charges de travail internes et d’héberger des services partagés ou des applications mutualisées.  

## <a name="create-the-shared-services-tenant"></a>Créer le locataire de services partagés

1. Accédez à **paramètres**  >  **paramètres du compte**  >  **services partagés**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Paramètres de compte > les services partagés":::

2. Si vous ne disposez pas déjà d’un locataire de services partagés, cliquez sur **créer des services partagés**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Créer des services partagés":::

3. Cela crée un locataire de services partagés et achète l’abonnement aux services partagés Azure CSP, à utiliser pour les ressources partagées et la charge de travail interne.

   :::image type="content" source="images/sharedservices5.png" alt-text="Créer le locataire et acheter l’abonnement":::

## <a name="about-the-azure--internalshared-services-offer"></a>À propos de l’offre Azure-Internal/Shared Services

- L’abonnement Azure-Internal/Shared Services est un nouveau type d’offre Azure dans CSP accessible via l’espace partenaires que les partenaires obtiennent pour leur propre utilisation d’Azure.

- Les abonnements aux services partagés des partenaires Azure sont éligibles et peuvent être utilisés pour l’achat de RIs.

- L’offre Azure-Internal/Shared Services ne peut être appliquée qu’au locataire des services partagés.

- La principale utilisation de l’abonnement Azure-Internal/Shared Services est de vous permettre d’utiliser Azure à des fins de développement. Le locataire partagé que vous utilisez pour approvisionner cette offre ne peut pas être utilisé pour d’autres services tels que les licences Office 365 ou Dynamics.

- Vous pouvez annuler l’abonnement comme tout autre abonnement. Accédez à **paramètres**  >  **Afficher tous les paramètres**  >  **services partagés**. Sélectionnez l’abonnement Azure-Internal/Shared Services et annulez-le.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Accès aux détails de la consommation des services partagés du partenaire Azure

Vous trouverez la consommation Azure sur votre facture CSP et le fichier de réconciliation. Elle sera incluse dans le cadre de Microsoft Azure article de la facture. Les informations détaillées sur la consommation sont disponibles dans le fichier de rapprochement enregistré par rapport au locataire créé pour cette offre.

## <a name="azure-partner-shared-services-pricing"></a>Tarification des services partagés des partenaires Azure

Pour afficher le nouveau fichier de tarification pour les services partagés partenaires Azure, accédez à la page **vendre** des  >  **tarifs et des offres** , puis sélectionnez la liste des prix du mois en cours. Dans les semaines à venir, une API de carte à tarif spécifique sera également publiée.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Offres de la place de marché et services partagés partenaires Azure

Depuis le 1er mars 2019, Azure Partner Shared Services (APSS) ne prend plus en charge les offres de la place de marché.

|**Support technique de la place de marché**   |**APSS pris en charge avant le 1er mars 2019**|**Après le 1er mars 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (apportez votre propre licence) et des services gratuits   | Oui   | Non|
|Autres offres de la place de marché tiers   | Non   |Non|

Les partenaires qui ont des services BYOL ou gratuits déployés à l’aide de APSS ne seront pas affectés. Toutefois, après le 1er mars, 2019, il ne sera pas en mesure d’acheter de nouveaux services BYOL ou gratuits.

Pour tirer parti du catalogue complet des offres de la place de marché disponibles (pas seulement les BYOL et les services gratuits), nous recommandons aux partenaires CSP de déployer les services partagés à l’aide d’abonnements Azure Web direct.  Les partenaires CSP qui ont déjà déployé des ressources BYOL et gratuites de service tierces à partir de la place de marché et souhaitent continuer à les utiliser et déployer d’autres offres tierces sont encouragés à migrer l’abonnement APSS vers Web direct [migrant des abonnements Azure existants](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Les partenaires, qui envisagent de continuer à utiliser l’abonnement APSS après le 1er mars 2019 et souhaitent déployer de nouveaux services [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) tiers ou des services gratuits, peuvent suivre les instructions des éditeurs de logiciels indépendants (ISV) pour les déployer dans leurs abonnements APSS.

## <a name="next-steps"></a>Étapes suivantes

- [Vendre des abonnements logiciels par le biais de CSP (fournisseur de solutions Cloud)](csp-software-subscriptions.md)