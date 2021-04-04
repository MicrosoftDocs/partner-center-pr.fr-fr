---
title: Migrer des abonnements Dynamics 365 qualifiés
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment migrer des abonnements Dynamics 365 de base qualifiés vers un nouvel abonnement avant l’expiration des abonnements existants.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132738"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrer Dynamics 365 et Plan Customer Engagement à partir de Basic (offres qualifiées) vers une version plus récente

**Rôles appropriés**

- Administrateur général
- Administrateur de la gestion des utilisateurs
- Agent d’administration
- Agent commercial

À compter du 1er janvier 2019, les clients disposant de Dynamics 365 pour le plan d’engagement commercial/client des abonnements de base (offres qualifiées) ne peuvent plus renouveler ces offres héritées. les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent. Sur la page de détails de l’abonnement, l’état de l’abonnement passe à « expire le [date] » dans « auto Renews on [date] ». 

Pour garantir la continuité des clients, vous devez les transférer avec des abonnements arrivant à expiration vers une option prise en charge, comme indiqué ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.

Si vous utilisez l’API (CREST ou Partner Center), vous pouvez rechercher les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux. Les abonnements en question seront configurés pour renouveler automatiquement = faux le 1er janvier 2019. Vous pouvez déplacer les clients vers un nouveau plan à tout moment. 

### <a name="the-dynamics-365-offers-being-retired"></a>Les offres Dynamics 365 en cours de retrait

- Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée)
- Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour Sales Enterprise Edition CRMOL Basic (offre qualifiée) pour les élèves
- Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) CRMOL Basic (offre qualifiée)
- Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour Sales Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les élèves
- Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 pour Sales Enterprise Edition Add-On pour CRM de base (offre qualifiée)
- Dynamics 365 pour Sales Enterprise Edition Add-On pour CRM de base (offre qualifiée) pour les enseignants
- Dynamics 365 pour Sales Enterprise Edition Add-On pour CRM de base (offre qualifiée) pour les élèves
- Dynamics 365 pour Sales Enterprise Edition (tarification gouvernementale) Add-On pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) CRMOL Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les élèves
- Dynamics 365 Customer engagement plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants
- Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les élèves
- Dynamics 365 Customer engagement plan Enterprise Edition de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 Customer engagement plan Enterprise Edition Add-On pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition (tarification gouvernementale) Add-On pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer engagement plan Enterprise Edition Add-On pour CRM Basic (offre qualifiée) pour les élèves
- Dynamics 365 Customer engagement plan Enterprise Edition Add-On pour CRM Basic (offre qualifiée) pour les enseignants



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 pour les ventes/le plan d’engagement des clients des plans de remplacement de base (offres qualifiées)

**Offres mises hors service**   

- Dynamics 365 pour les ventes à partir de CRM Basic ou CRMOL Basic (offre qualifiée)
- Plan d’engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (offre qualifiée)

**Options de remplacement**
- Dynamics 365 pour le professionnel des ventes (nouveauté)
- Dynamics 365 pour le professionnel des ventes (nouveauté)
- Dynamics 365 pour le service client
- Plan d’engagement client Dynamics 365 ou
- Membres de l’équipe Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Le déplacement de clients des références SKU hors service vers des versions plus récentes requiert les étapes suivantes dans cet ordre :

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

## <a name="purchase-the-new-plan-for-your-customer"></a>Acheter le nouveau plan pour votre client

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous souhaitez déplacer vers le nouvel abonnement.
2. Sélectionnez **Ajouter un abonnement**.
3. Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client dispose désormais de l’ancien abonnement et du nouveau. L’étape suivante consiste à réattribuer les licences aux utilisateurs du client.

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sélectionnez **utilisateurs et licences**.
3. Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **gérer les licences**. 
4. Sur la page **gérer les licences** , désactivez la case à cocher Dynamics 365 pour le plan Sales/Customer engagement de base (offre qualifiée) et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé. 
5. Sélectionnez **Envoyer**. Vous effectuerez cette opération pour chaque utilisateur qui a besoin de la nouvelle licence. 

Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement. 

1. Sélectionnez **clients** dans la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sur la page Détails de l’abonnement, définissez l’ancien abonnement sur **suspendu** , puis sélectionnez **Envoyer**.

L’ancien abonnement est maintenant suspendu et le nouvel abonnement est actif. L’abonnement suspendu est désapprovisionné automatiquement après 120 jours. Votre client n’aura aucuns frais supplémentaires pour l’ancien abonnement.
 

 



