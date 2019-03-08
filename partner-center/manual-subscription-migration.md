---
title: Migrer Dynamics 365 et le Plan d’Engagement client à partir de Basic (offres qualifiés) aux versions plus récentes | Partenaires
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 pour les ventes / Customer Engagement Plan à partir des abonnements de base (offre qualifié) peut ne plus être renouvelé.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Offres Dynamics 365, renouveler les offres, les nouvelles références SKU de Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586942"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions

**S’applique à**

-  Espace partenaires

À compter du 1 janvier 2019, les clients avec Dynamics 365 pour les ventes / Customer Engagement Plan à partir des abonnements de base (offre qualifié) ne pouvez plus renouveler ces offres hérités ; les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent. Sur la page de détails de l’abonnement, l’état de l’abonnement passe « Expire le [date] » à partir de « Auto renouvelle le [date] ». 


Pour garantir la continuité des activités pour les clients, vous devez passer celles avec des abonnements arrivant à expiration à une option de prise en charge, répertoriés ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service.

Si vous utilisez l’API (CREST ou partenaires), vous pouvez trouver d’abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que l’automatiquement renouvelés = propriété False. Les abonnements en question seront définies sur auto renouveler = False sur le 1 janvier 2019. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

### <a name="the-dynamics-365-offers-being-retired"></a>Le Dynamics 365 offre en cours de retrait

- Dynamics 365 pour les ventes Enterprise Edition CRMOL Basic (offre qualifiée)
- Dynamics 365 pour l’édition entreprise de vente CRMOL Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour l’édition entreprise de vente CRMOL Basic (offre qualifiée) pour les étudiants
- Dynamics 365 pour les ventes Enterprise Edition (tarification secteur public) CRMOL Basic (offre qualifiée)
- Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour les ventes, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 pour les ventes, Édition entreprise (tarification secteur public) à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée)
- Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour le module complémentaire d’Édition Enterprise de ventes pour CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 pour le module complémentaire de vente Enterprise Edition (tarification secteur public) pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (tarification secteur public) CRMOL Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants
- Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan, Édition entreprise (tarification secteur public) à partir de SA pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 Customer Engagement Plan, Édition entreprise à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (tarification secteur public) module complémentaire pour CRM Basic (offre qualifiée)
- Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 Customer Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les enseignants



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 pour les ventes / plans de Customer Engagement Plan à partir de remplacement de Basic (offre qualifié)

**Offres supprimées**   

- Dynamics 365 pour les ventes de CRM Basic ou CRMOL Basic (offre qualifiée)
- Plan d’Engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (offre qualifiée)

**Options de remplacement**
- Dynamics 365 pour les professionnels de vente (nouveau)
- Dynamics 365 pour les professionnels de vente (nouveau)
- Dynamics 365 pour le Service client
- Plan d’Engagement client Dynamics 365 ou
- Membres de l’équipe Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Déplacement des clients à partir de références (SKU) retirée vers les plus récents nécessite les étapes suivantes dans cet ordre :

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

## <a name="purchase-the-new-plan-for-your-customer"></a>Le nouveau plan d’achat pour votre client

1. Sélectionnez **clients** à partir de la navigation de gauche puis le client que vous souhaitez déplacer vers un nouvel abonnement.
2. Sélectionnez **ajouter un abonnement**.
3. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client aura maintenant à l’ancien abonnement et le nouveau. L’étape suivante consiste à réassigner des licences pour les utilisateurs du client.

1. Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client vous font la transition.
2. Sélectionnez **Utilisateurs et licences**.
3. Pour réattribuer une licence à un utilisateur, sélectionnez l’utilisateur, puis **gérer les licences**. 
4. Sur le **gérer les licences** page, désactivez la Dynamics 365 pour les ventes / Plan d’Engagement client à partir de Basic (offre qualifié) licence case à cocher et sélectionnez un nouveau plan de service pour l’abonnement que le client se déplace vers. 
5. Sélectionnez **Envoyer**. Vous effectuerez ceci pour chaque utilisateur qui a besoin de la nouvelle licence. 

Une fois que vous avez déplacé les licences vers un nouvel abonnement, vous pouvez annuler l’ancien abonnement. 

1. Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client vous font la transition.
2. Dans la page de détails d’abonnement, la valeur est l’ancien abonnement **Suspended** et sélectionnez **envoyer**.

L’ancien abonnement est interrompu et le nouvel abonnement est actif. L’abonnement suspendu est automatiquement désapprovisionné après 120 jours. Votre client n’entraîne aucun coût supplémentaire pour l’ancien abonnement.
 

 



