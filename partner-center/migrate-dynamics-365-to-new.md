---
title: Migrer proposées par édition entreprise Dynamics 365 vers les nouvelles versions | L’espace partenaires
ms.topic: article
ms.date: 12/12/2018
description: Les abonnements Dynamics 365 Business Edition n’est plus peuvent être renouvelés.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968282"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrer proposées par édition entreprise Dynamics 365 vers les nouvelles versions 

**S'applique à**

- Espace partenaires

Effectifs 1er janvier 2019, les clients ayant des abonnements Dynamics 365 Business Edition peuvent n’est plus renouveler d’abonnement dans ces offres hérités; les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration. Sur la page des détails de l’abonnement, l’état d’abonnement changera par «Expire le [date]» «Renouvellements le [date]».

Pour garantir la continuité des activités pour les clients, vous devez passer les ceux dont les abonnements arrivant à expiration à une option pris en charge, répertoriée ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service.

Si vous utilisez l’API (CREST ou espace partenaires), vous pouvez trouver renouvellement des abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec l’automatique = False propriété. Les abonnements en question seront définies automatiquement renouvelé = False le 1er janvier 2019. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Les éditions d’entreprise Dynamics 365 en cours mis hors service

- Dynamics 365 pour Finance and Operations, Édition entreprise
- Dynamics 365 for Team Members, Édition entreprise

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - les nouvelles offres de Dynamics 365 Business Edition

Avec les nouvelles offres Dynamics Business Central, vos clients peuvent connecter leurs financials, ventes, service et les opérations pour simplifier le processus d’entreprise, d’améliorer les interactions avec le client et prendre des décisions avisées. Dynamics 365 Business Central est basée sur le cloud et disponible par le biais de partenaires du programme fournisseur de solutions Cloud (CSP) uniquement.
Dynamics 365 clients Édition entreprise sont autorisés à recevoir la transition à taux réduit de tarification pour l’entreprise nouvelle Central offre jusqu’au 30 juin 2020.

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