---
title: Migrer Dynamics 365 Business Edition offre vers les versions plus récentes | Espace partenaires
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Les abonnements Dynamics 365 Business Edition ne peuvent plus être renouvelés.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offres, renouvellement d’offres, nouvelles références (SKU) Dynamics 365
ms.openlocfilehash: fc6964135058a805a32f81b09974b8e6d08e85d6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653299"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrer proposées par édition entreprise Dynamics 365 vers les nouvelles versions 

**S’applique à**

- Espace partenaires

À compter du 1er janvier 2019, les clients disposant d’abonnements Dynamics 365 Business Edition ne peuvent plus renouveler ces offres héritées. les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent. Sur la page de détails de l’abonnement, l’état de l’abonnement passe à « expire le [date] » dans « auto Renews on [date] ».

Pour garantir la continuité des clients, vous devez les transférer avec des abonnements arrivant à expiration vers une option prise en charge, comme indiqué ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.

Si vous utilisez l’API (CREST ou Partner Center), vous pouvez rechercher les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux. Les abonnements en question seront configurés pour renouveler automatiquement = false le 1er janvier 2019. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Les éditions Business de Dynamics 365 en cours de retrait

- Dynamics 365 pour Finance and Operations, édition Business
- Dynamics 365 pour les membres de l’équipe, édition Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business central-les nouvelles offres Dynamics 365 Business Edition

Grâce aux nouvelles offres Dynamics Business central, vos clients peuvent connecter leurs finances, ventes, services et opérations afin de rationaliser les processus d’entreprise, d’améliorer les interactions avec les clients et de prendre de meilleures décisions. Dynamics 365 Business central est basé sur le Cloud et disponible uniquement via les partenaires du programme fournisseur de solutions Cloud (CSP).
Les clients Dynamics 365 Business Edition peuvent bénéficier d’une tarification avec remise pour les nouvelles offres professionnelles jusqu’au 30 juin 2020.

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers des nouvelles formules de produit

 Le déplacement de clients des références SKU hors service vers des versions plus récentes requiert les étapes suivantes dans cet ordre :

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

## <a name="purchase-the-new-plan-for-your-customer"></a>Acheter le nouveau plan pour votre client

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous souhaitez déplacer vers le nouvel abonnement.
2. Sélectionnez **Ajouter un abonnement**.
3. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client dispose désormais de l’ancien abonnement et du nouveau. L’étape suivante consiste à réattribuer les licences aux utilisateurs du client.

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sélectionnez **Utilisateurs et licences**.
3. Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **gérer les licences**. 
4. Sur la page **gérer les licences** , désactivez la case à cocher Dynamics 365 pour le plan Sales/Customer engagement de base (offre qualifiée) et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé. 
5. Sélectionnez **Envoyer**. Vous effectuerez cette opération pour chaque utilisateur qui a besoin de la nouvelle licence. 

Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement. 

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sur la page Détails de l’abonnement, définissez l’ancien abonnement sur **suspendu** , puis sélectionnez **Envoyer**.

L’ancien abonnement est maintenant suspendu et le nouvel abonnement est actif. L’abonnement suspendu est automatiquement désapprovisionné après 120 jours. Votre client n’aura aucuns frais supplémentaires pour l’ancien abonnement.