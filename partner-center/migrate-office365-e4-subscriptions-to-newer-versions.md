---
title: "Migrer des abonnements Office365E4 vers les nouvelles versions d’Office365 | Espace partenaires"
description: "L&quot;édition MicrosoftOffice365 EntrepriseE4 n’est plus disponible depuis le 7 avril2017. Découvrez comment migrer vos abonnements client vers des versions plus récentes d’Office365."
author: MaggiePucciEvans
ms.openlocfilehash: aa8bc051b85f60242b1cc08e05b8c2b2d22ac413
ms.sourcegitcommit: dab14e98f39e14025625a366ffcdd34c8c744376
ms.translationtype: HT
ms.contentlocale: fr-FR
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrer des abonnements Office365E4 vers les nouvelles versions d’Office365

**S’applique à**

-  Espace partenaires

La formule Office365 Entreprise E4 n’est plus disponible depuis le 7avril2017. Vous ne pouvez plus acheter de nouveaux abonnements Office365E4 après cette date et les abonnements E4 existants ne seront pas renouvelés automatiquement lorsqu’ils arriveront à expiration.

Lorsque les abonnements E4 prendront fin, ils seront annulés. Pour garantir la continuité des activités pour les clients, vous devez passer les clients ayant des abonnements E4 arrivant à expiration à une option de référence (SKU) prise en charge, répertoriée ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service. 

>**Remarque** Les références (SKU) Office365 EntrepriseE4 commercial et secteur public ne sont plus disponibles.
 
Sur la page des détails de l’abonnement, le statut de l'abonnement E4 «Renouvellements automatiques le [date]» est remplacé par «Expire le [date]». 

Si vous utilisez l’API (CREST ou Espace partenaires), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec la propriété de renouvellement automatique = False. 

Les abonnements E4 seront définis sur renouvellement automatique = False le 7 avril2017. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Formules de remplacement pour l'édition Office365 Entreprise E4

Vous pouvez choisir de conserver les mêmes fonctionnalités qu'avec E4 ou de faire bénéficier vos clients des nouvelles fonctions d'Office365 et de Skype Entreprise Online. Les détails de la tarification figurent sur la liste de prix et le tableau répertoriant les offres dans l'Espace partenaires. Secure Productive Enterprise E3 ou Secure Productive Enterprise E5 peut être remplacé dans les options suivantes respectivement par Office365 Entreprise E3 ou Office365 Entreprise E5.

- Option1: Office365 Entreprise E5

- Option2: Office365 Entreprise E3 + Cloud PBX de Skype Entreprise

- Option3: Office365 Entreprise E3 + Skype Entreprise, ainsi que les licences d’accès client (parité de prix et de fonctionnalités avec E4)

- Option4: Office365 Entreprise E3


| Fonctionnalité | Option1 | Option2 | Option3 | Option4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Obtenir toutes les fonctionnalités incluses dans Office365 Entreprise E4? | Oui | Oui | Oui | Non |
| Numéros de téléphone gérés dans Office365? | Oui | Oui | Non | Non |
| Numéros de téléphone gérés à la fois localement et dans Office365 (déploiement hybride)? | Oui | Oui | Non | Non |
| Option pour ajouter un plan d’appel vocal et RTC? | Oui | Oui | Non | Non |
| Conférence RTC? | Oui | Non | Non | Non |
| Outils avancés de collaboration, d'analyse et de sécurité? | Oui | Non | Non | Non |
| Rapports interactifs, tableaux de bord et visualisations de données? | Oui | Non | Non | Non | 
| Plus de contrôle sur la sécurité des données et la conformité avec une confidentialité, une transparence et des contrôles utilisateur pointus intégrés? | Oui | Non | Non | Non | 

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ces cas, vous pouvez avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître. La migration de clients depuis des références supprimées vers des références plus récentes doit respecter les étapes suivantes:

-   Acheter le nouvel abonnement
-   Réaffecter les licences utilisateur actuelles
-   Annuler l’ancien abonnement

Suivez ces étapes pour migrer l’abonnement Office365 Entreprise E4 d’un client vers l'une des options indiquées dans le tableau ci-dessus.

### <a name="step-1---purchase-the-new-subscription"></a>Étape1: acheter le nouvel abonnement

1. Dans le menu **Tableau de bord**, sélectionnez **Clients** et le client à déplacer, puis sélectionnez **Ajouter des abonnements**.

2. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**.

   Votre client doit maintenant avoir les anciens et les nouveaux abonnements, l'ancien abonnement Office365 Entreprise E4 et le nouvel abonnement «cible», par exemple, Option1: Office365 Entreprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Étape2: réaffecter les licences des utilisateurs du client

1. Dans le menu **Tableau de bord**, sélectionnez **Clients** et le client à déplacer, puis sélectionnez **Utilisateurs et licences**. La page Utilisateurs et licences du client s’ouvre.

2. Pour réaffecter les licences utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.

3. Dans la page **Gérer les licences**, désactivez la case à cocher de la licence **Office365 Entreprise E4**, puis sélectionnez une nouvelle formule de service pour l’abonnement auquel passe le client.

4. Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées.

5. Suivez la même procédure pour les autres utilisateurs du client qui ont besoin de la réaffectation de licences.

Une fois les licences utilisateur attribuées au nouveau service, vous pouvez en toute sécurité annuler l'abonnement retiré au premier niveau du client.

### <a name="step-3---cancel-the-old-subscription"></a>Étape3: annuler l’ancien abonnement

1. Dans le menu **Tableau de bord**, sélectionnez **Clients**. Sélectionnez le client que vous voulez déplacer, puis l’abonnement à annuler.

2. Dans la page des détails de l’abonnement, définissez l'état d'abonnement sur **Suspendu**.

3. Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est automatiquement désapprovisionné après 120jours. Aucun frais n’est facturé au client pour l’ancien abonnement.



 



