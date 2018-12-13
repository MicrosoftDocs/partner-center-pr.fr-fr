---
title: Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions | L’espace partenaires
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / du Plan Engagement client à partir des abonnements Basic (offre qualifiés) n’est plus peut être renouvelé.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968269"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrer de Dynamics 365 et du Plan Engagement client à partir de Basic (offres qualifiés) vers les nouvelles versions

**S'applique à**

-  Espace partenaires

Les clients le 1er janvier 2019 efficaces avec Dynamics 365 for Sales / du Plan Engagement client à partir des abonnements Basic (offre qualifiés) pouvez renouveler n’est plus ces offres hérités; les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration. Sur la page des détails de l’abonnement, l’état d’abonnement changera par «Expire le [date]» «Renouvellements le [date]». 


Pour garantir la continuité des activités pour les clients, vous devez passer les ceux dont les abonnements arrivant à expiration à une option pris en charge, répertoriée ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service.

Si vous utilisez l’API (CREST ou espace partenaires), vous pouvez trouver renouvellement des abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec l’automatique = False propriété. Les abonnements en question seront définies automatiquement renouvelé = False le 1er janvier 2019. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

### <a name="the-dynamics-365-offers-being-retired"></a>Le Dynamics 365 propose en cours mis hors service

- Dynamics 365 pour vente Enterprise Edition CRMOL Basic (qualifiée offre)
- Dynamics 365 pour vente Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants
- Dynamics 365 pour vente Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants
- Dynamics 365 pour vente Enterprise Edition (tarification du gouvernement des États-Unis) CRMOL Basic (qualifiée offre)
- Dynamics 365 Édition entreprise de vente à partir de SA pour CRM Basic (qualifiée offre)
- Dynamics 365 Édition entreprise de vente à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 Édition entreprise de vente à partir de SA CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 pour vente Enterprise Edition (tarification du gouvernement des États-Unis) à partir de SA pour CRM Basic (qualifiée offre)
- Dynamics 365 de vente Enterprise Edition extension pour CRM Basic (qualifiée offre)
- Dynamics 365 de vente Enterprise Edition extension pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 de vente Enterprise Edition extension CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 de vente Enterprise Edition (tarification du gouvernement des États-Unis) extension pour CRM Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) CRMOL Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les étudiants
- Dynamics 365 client Engagement Plan Enterprise Edition CRMOL Basic (offre qualifiée) pour les enseignants
- Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA pour CRM Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) à partir de SA pour CRM Basic (qualifiée offre)
- Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA CRM Basic (offre qualifiée) pour les étudiants
- Édition entreprise de Plan d’Engagement client Dynamics 365 à partir de SA pour CRM Basic (offre qualifiée) pour les enseignants
- Dynamics 365 client Engagement Plan Enterprise Edition extension pour CRM Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition (tarification du gouvernement des États-Unis) module complémentaire pour CRM Basic (qualifiée offre)
- Dynamics 365 client Engagement Plan Enterprise Edition module complémentaire CRM Basic (offre qualifiée) pour les étudiants
- Dynamics 365 client Engagement Plan Enterprise Edition module complémentaire pour CRM Basic (offre qualifiée) pour les enseignants



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / plans du Plan Engagement client à partir de remplacement Basic (offre qualifiés)

**Offres retirés**   

- Dynamics 365 for Sales à partir de CRM Basic ou CRMOL Basic (qualifiée offre)
- Plan d’Engagement client Dynamics 365 à partir de CRM Basic ou CRMOL Basic (qualifiée offre)

**Options de remplacement**
- Dynamics 365 destinée aux professionnels de vente (nouveau)
- Dynamics 365 destinée aux professionnels de vente (nouveau)
- Dynamics 365 for Customer Service
- Plan d’Engagement client Dynamics 365 ou
- Membres de l’équipe Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers des nouvelles formules de produit

Transfert des clients à partir de références (SKU) retiré vers les plus récentes doit respecter les étapes suivantes dans l’ordre suivant:

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

## <a name="purchase-the-new-plan-for-your-customer"></a>Acheter le nouveau plan pour votre client

1. Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous voulez déplacer vers le nouvel abonnement.
2. Sélectionnez **Ajouter un abonnement**.
3. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client possède alors à la fois l’ancien abonnement et une nouvelle. L’étape suivante consiste à réaffecter les licences aux utilisateurs du client.

1. Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sélectionnez **Utilisateurs et licences**.
3. Pour réaffecter une licence à un utilisateur, sélectionnez l’utilisateur, puis sélectionnez **Gérer les licences**. 
4. Sur la page **Gérer les licences** , désactivez le Dynamics 365 for Sales / Plan d’Engagement client à partir de Basic (offre qualifiés) licence case à cocher et sélectionnez une nouvelle formule de service de l’abonnement du client est transféré sur. 
5. Sélectionnez **Envoyer**. Vous ferez cela pour chaque utilisateur qui ont besoin de la nouvelle licence. 

Une fois que vous avez déplacé les licences vers le nouvel abonnement, vous pouvez annuler l’ancien abonnement. 

1. Sélectionnez **clients** à partir de la navigation de gauche, puis sélectionnez le client que vous déplacez.
2. Sur la page des détails abonnement, définissez l’ancien abonnement sur **suspendu** et sélectionnez **Soumettre**.

L’ancien abonnement est désormais suspendu et le nouvel abonnement est actif. L’abonnement suspendu est automatiquement désapprovisionné après 120jours. Votre client n’induit aucun coût supplémentaire pour l’ancien abonnement.
 

 



