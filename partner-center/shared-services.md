---
title: Ajouter Azure Partner Shared Services
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Utilisez les services partagés partenaires Azure pour acheter des abonnements Azure pour votre usage personnel et pour disposer d’une méthode uniforme pour l’achat, le suivi et la gestion d’Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, services partagés, locataire
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62989c58284de46834f02abc01041c454e725a81
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425948"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Ajoutez des services partagés partenaires Azure pour que les partenaires puissent acheter des abonnements Azure pour leur propre usage

**S’applique à**

- Espace partenaires

Azure Partner Shared Services est un nouveau type d’offre proposé aux partenaires dans le cadre du programme Fournisseur de solutions Cloud. Il leur permet d’acheter des abonnements Azure pour leur propre usage.Il permet aux partenaires d’utiliser une méthode uniforme pour l’achat, le suivi et la gestion d’Azure, en plus de la possibilité de consolider leurs contrats de licence et de revente Azure avec Microsoft. Avec les services partagés partenaires Azure, les partenaires ont désormais la même flexibilité pour utiliser les abonnements Azure dans CSP que dans les programmes Microsoft Accord Entreprise et Web direct, en ouvrant des scénarios tels que les environnements de développement et de test, de déployer des charges de travail internes et d’héberger des services partagés ou des applications mutualisées.  

## <a name="create-the-shared-services-tenant"></a>Créer le locataire de services partagés

1. Accédez à **paramètres**  >  **Afficher tous les paramètres**  >  **services partagés**.

   ![* * Paramètres de compte * * > * * services partagés * *](images/sharedservices2.png)

2. Si vous ne disposez pas déjà d’un locataire de services partagés, cliquez sur **créer des services partagés**.

   ![Créer des services partagés](images/sharedservices3.png)

3. Cela crée un locataire de services partagés et achète l’abonnement aux services partagés Azure CSP, à utiliser pour les ressources partagées et la charge de travail interne.

   ![Créer le locataire et acheter l’abonnement](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>À propos de l’offre Azure-Internal/Shared Services

- L’abonnement Azure-Internal/Shared Services est un nouveau type d’offre Azure dans CSP accessible via l’espace partenaires que les partenaires obtiennent pour leur propre utilisation d’Azure. 

- Azure-Internal/Shared Services offre n’est pas éligible pour les remises et les incentives.

- L’offre Azure-Internal/Shared Services ne peut être appliquée qu’au locataire des services partagés.

- La principale utilisation de l’abonnement Azure-Internal/Shared Services est de vous permettre d’utiliser Azure à des fins de développement. Le locataire partagé que vous utilisez pour approvisionner cette offre ne peut pas être utilisé pour d’autres services tels que Office 365 ou les sièges Dynamics. 

- Vous pouvez annuler l’abonnement comme tout autre abonnement. Accédez à **paramètres**  >  **Afficher tous les paramètres**  >  **services partagés**. Sélectionnez l’abonnement Azure-Internal/Shared Services et annulez-le.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Accès aux détails de la consommation des services partagés du partenaire Azure

Vous trouverez la consommation Azure sur votre facture CSP et le fichier de réconciliation. Elle sera incluse dans le cadre de Microsoft Azure article de la facture. Les informations détaillées sur la consommation sont disponibles dans le fichier de rapprochement enregistré par rapport au locataire créé pour cette offre. 

## <a name="azure-partner-shared-services-pricing"></a>Tarification des services partagés des partenaires Azure

Pour afficher le nouveau fichier de tarification des services partagés partenaires Azure, consultez la page **vendre**des  >  **tarifs et des offres** , puis sélectionnez la liste des prix du mois en cours. Dans les semaines à venir, une API de carte à tarif spécifique sera également publiée.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Offres de la place de marché et services partagés partenaires Azure

Depuis le 1er mars 2019, Azure Partner Shared Services (APSS) ne prend plus en charge les offres de la place de marché.

|**Support technique de la place de marché**   |**APSS pris en charge avant le 1er mars 2019**|**Après le 1er mars 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (apportez votre propre licence) et des services gratuits   | Oui   | Non|
|Autres offres de la place de marché tiers   | Non   |Non|

Les partenaires qui ont des services BYOL ou gratuits déployés à l’aide de APSS ne seront pas affectés. Toutefois, après le 1er mars, 2019, il ne sera pas en mesure d’acheter de nouveaux services BYOL ou gratuits.

Pour tirer parti du catalogue complet des offres de la place de marché disponibles (pas seulement les BYOL et les services gratuits), nous recommandons aux partenaires CSP de déployer les services partagés à l’aide d’abonnements Azure Web direct.  Les partenaires CSP qui ont déjà déployé des ressources BYOL et gratuites de service tierces à partir de la place de marché et souhaitent continuer à les utiliser et déployer d’autres offres tierces sont encouragés à migrer l’abonnement APSS vers Web direct [migrant des abonnements Azure existants](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Les partenaires, qui envisagent de continuer à utiliser l’abonnement APSS après le 1er mars 2019 et souhaitent déployer de nouveaux services [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) tiers ou des services gratuits, peuvent suivre les instructions des éditeurs de logiciels indépendants (ISV) pour les déployer dans leurs abonnements APSS.

