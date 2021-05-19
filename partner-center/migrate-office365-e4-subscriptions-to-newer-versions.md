---
title: Migrer des abonnements Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition est mis hors service depuis le 7 avril 2017. Découvrez comment migrer vos abonnements client vers des versions plus récentes d’Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151557"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365

**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent d’administration | Agent des ventes

Le plan Office 365 Enterprise E4 est retiré, à compter du 7 avril 2017. Vous ne pouvez plus acheter de nouveaux abonnements Office 365 E4 après cette date, et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.

Lorsque les abonnements E4 se terminent, ils sont annulés. Pour garantir la continuité des clients, vous devez faire passer les clients avec des abonnements E4 arrivant à expiration à une option SKU prise en charge, comme indiqué ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients. 

> [!NOTE]  
> Les références SKU commerciales et gouvernementales d’Office 365 Enterprise E4 sont retirées.
 
Sur la page de détails de l’abonnement, l’état de l’abonnement E4 est passé à « expire le [date] » de « auto Renews on [date] ». 

Si vous utilisez l’API (CREST ou Partner Center), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = false. 

Les abonnements E4 seront configurés pour un renouvellement automatique = false en avril 7, 2017. Vous pouvez déplacer les clients vers un nouveau plan à tout moment. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Plans de remplacement Office 365 Enterprise E4 Edition

Vous pouvez choisir de conserver la même fonctionnalité avec E4 ou de faire en sorte que vos clients tirent parti des fonctionnalités et fonctionnalités plus récentes dans Office 365 et Skype entreprise online. Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires. Secure Product Enterprise E3 ou Secure productive Enterprise E5 peut être remplacé par les options suivantes pour Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivement.

- Option 1 : Office 365 Enterprise E5

- Option 2 : Office 365 Enterprise E3 + PBX Cloud de Skype entreprise

- Option 3 : Office 365 Enterprise E3 + licences d’accès client Skype entreprise plus (parité prix et fonctionnalité avec E4)

- Option 4 : Office 365 Enterprise E3


| Fonctionnalité | Option 1 : | Option 2 : | Option 3 | Option 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Bénéficier de toutes les fonctionnalités incluses dans Office 365 Enterprise E4 ? | Oui | Oui | Oui | Non |
| Numéros de téléphone gérés dans Office 365 ? | Oui | Oui | Non | Non |
| Numéros de téléphone gérés localement et dans Office 365 (déploiement hybride) ? | Oui | Oui | Non | Non |
| Option permettant d’ajouter un plan d’appel vocal RTPC ? | Oui | Oui | Non | Non |
| La Conférence RTPC ? | Oui | Non | Non | Non |
| Outils avancés pour la collaboration, l’analyse et la sécurité ? | Oui | Non | Non | Non |
| Des rapports interactifs, des tableaux de bord et des visualisations de données ? | Oui | Non | Non | Non | 
| Contrôle accru de la sécurité et de la conformité des données grâce à la confidentialité intégrée, à la transparence et aux contrôles utilisateur affinés ? | Oui | Non | Non | Non | 

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées. La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :

-   Acheter le nouvel abonnement
-   Réaffecter les licences utilisateur actuelles
-   Annuler l’ancien abonnement

Suivez ces étapes pour migrer l’abonnement Office 365 Enterprise E4 d’un client vers l’une des options du tableau ci-dessus.

### <a name="step-1---purchase-the-new-subscription"></a>Étape 1 : acheter le nouvel abonnement

1. Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.

2. Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.

   Votre client doit maintenant avoir des abonnements anciens et nouveaux, l’ancien abonnement Office 365 Enterprise E4 et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Étape 2 : réattribuer les licences des utilisateurs du client

1. Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **utilisateurs et licences**. La page utilisateurs et licences du client s’ouvre.

2. Pour réaffecter des licences utilisateur, sélectionnez l’utilisateur à réassigner, puis sélectionnez **gérer les licences**.

3. Sur la page **gérer les licences** , désactivez la case à cocher **Office 365 Enterprise E4** et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.

4. Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées.

5. Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.

Après avoir déplacé les licences utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client le plus élevé.

### <a name="step-3---cancel-the-old-subscription"></a>Étape 3 : annuler l’ancien abonnement

1. Dans le menu **espace partenaires** , sélectionnez **clients**. Sélectionnez le client que vous souhaitez déplacer, puis sélectionnez l’abonnement que vous souhaitez annuler.

2. Dans la page Détails de l’abonnement, définissez l’état de l’abonnement sur **suspendu**.

3. Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouvel abonnement est actif. L’abonnement suspendu est désapprovisionné automatiquement après 120 jours. Aucun frais n’est facturé au client pour l’ancien abonnement.



 



