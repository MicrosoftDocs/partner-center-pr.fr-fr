---
title: Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365 | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'édition Microsoft Office 365 Entreprise E4 n’est plus disponible depuis le 7 avril 2017. Découvrez comment migrer vos abonnements client vers des versions plus récentes d’Office 365.
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390878"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrer des abonnements Office 365 E4 vers les nouvelles versions d’Office 365

**S’applique à**

-  Centre pour partenaires

**Rôles appropriés**
-   Administrateur global
-   Administrateur des utilisateurs
-   Agent d’administration
-   Commercial

La formule Office 365 Entreprise E4 n’est plus disponible depuis le 7 avril 2017. Vous ne pouvez plus acheter de nouveaux abonnements Office 365 E4 après cette date et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration.

Lorsque les abonnements E4 prendront fin, ils seront annulés. Pour garantir la continuité des activités pour les clients, vous devez passer les clients ayant des abonnements E4 arrivant à expiration à une option de référence (SKU) prise en charge, répertoriée ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients. 

> [!NOTE]  
>  Les références SKU commerciales et gouvernementales d’Office 365 Enterprise E4 sont retirées.
 
Sur la page des détails de l’abonnement, le statut de l'abonnement E4 « Renouvellements automatiques le [date] » est remplacé par « Expire le [date] ». 

Si vous utilisez l’API (CREST ou Espace partenaires), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec la propriété de renouvellement automatique = False. 

Les abonnements E4 seront définis sur renouvellement automatique = False le 7 avril 2017. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Formules de remplacement pour l'édition Office 365 Entreprise E4

Vous pouvez choisir de conserver les mêmes fonctionnalités qu'avec E4 ou de faire bénéficier vos clients des nouvelles fonctions d'Office 365 et de Skype Entreprise Online. Les détails de la tarification figurent sur la liste de prix et le tableau répertoriant les offres dans l'Espace partenaires. Secure Productive Enterprise E3 ou Secure Productive Enterprise E5 peut être remplacé dans les options suivantes respectivement par Office 365 Entreprise E3 ou Office 365 Entreprise E5.

- Option 1 : Office 365 Entreprise E5

- Option 2 : Office 365 Entreprise E3 + Cloud PBX de Skype Entreprise

- Option 3 : Office 365 Entreprise E3 + Skype Entreprise, ainsi que les licences d’accès client (parité de prix et de fonctionnalités avec E4)

- Option 4 : Office 365 Entreprise E3


| Composant | Option 1 | Option 2 | Option 3 | Option 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Obtenir toutes les fonctionnalités incluses dans Office 365 Entreprise E4 ? | Oui | Oui | Oui | Non |
| Numéros de téléphone gérés dans Office 365 ? | Oui | Oui | Non | Non |
| Numéros de téléphone gérés à la fois localement et dans Office 365 (déploiement hybride) ? | Oui | Oui | Non | Non |
| Option pour ajouter un plan d’appel vocal et RTC ? | Oui | Oui | Non | Non |
| Conférence RTC ? | Oui | Non | Non | Non |
| Outils avancés de collaboration, d'analyse et de sécurité ? | Oui | Non | Non | Non |
| Rapports interactifs, tableaux de bord et visualisations de données ? | Oui | Non | Non | Non | 
| Plus de contrôle sur la sécurité des données et la conformité avec une confidentialité, une transparence et des contrôles utilisateur pointus intégrés ? | Oui | Non | Non | Non | 

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ces cas, vous pouvez avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître. La migration de clients depuis des références supprimées vers des références plus récentes doit respecter les étapes suivantes :

-   Acheter le nouvel abonnement
-   Réaffecter les licences utilisateur actuelles
-   Annuler l’ancien abonnement

Suivez ces étapes pour migrer l’abonnement Office 365 Entreprise E4 d’un client vers l'une des options indiquées dans le tableau ci-dessus.

### <a name="step-1---purchase-the-new-subscription"></a>Étape 1 : acheter le nouvel abonnement

1. Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.

2. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**.

   Votre client doit maintenant avoir des abonnements anciens et nouveaux, l’ancien abonnement Office 365 Enterprise E4 et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Étape 2 : réaffecter les licences des utilisateurs du client

1. Dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **utilisateurs et licences**. La page utilisateurs et licences du client s’ouvre.

2. Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.

3. Dans la page **Gérer les licences**, désactivez la case à cocher de la licence **Office 365 Entreprise E4**, puis sélectionnez une nouvelle formule de service pour l’abonnement auquel passe le client.

4. Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées.

5. Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.

Une fois les licences utilisateur attribuées au nouveau service, vous pouvez en toute sécurité annuler l'abonnement retiré au premier niveau du client.

### <a name="step-3---cancel-the-old-subscription"></a>Étape 3 : annuler l’ancien abonnement

1. Dans le menu **espace partenaires** , sélectionnez **clients**. Sélectionnez le client que vous voulez déplacer, puis l’abonnement à annuler.

2. Dans la page des détails de l’abonnement, définissez l'état d'abonnement sur **Suspendu**.

3. Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est automatiquement désapprovisionné après 120 jours. Aucun frais n’est facturé au client pour l’ancien abonnement.



 



