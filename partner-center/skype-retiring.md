---
title: Migration des abonnements Skype Entreprise Online Plan1 vers les nouvelles versions d’Office365 | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
Description: Transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option. We recommend moving customers to new subscriptions before the subscription’s yearly end date.
author: labrenne
ms.author: labrenne
keywords: Plans Skype Entreprise, retrait de Skype, Office365
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: c1e4f4611c6fe3c317339af1a036194031f3d095
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917621"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migration des abonnements Skype Entreprise Online Plan1 vers les nouvelles versions de MicrosoftOffice365

**S'applique à:**

- Espace partenaires

Le Plan1 de Skype Entreprise Online sera retiré à compter du 1eraoût2018. Passée cette date, les clients ne pourront plus acheter de nouveaux abonnements Skype Entreprise Plan1 et les abonnements existants ne se renouvelleront pas automatiquement lorsqu'ils expireront et aucune option de renouvellement ne sera proposée. Sur la page des détails de l’abonnement, le statut de l'abonnement Skype Entreprise Online Plan1 «Renouvellements automatiques le [date]» est remplacé par «Expire le [date]».  

Pour garantir la continuité des activités pour les clients, vous devez passer les clients ayant des abonnements Skype Entreprise Online Plan1 arrivant à expiration à une option de référence (SKU) prise en charge, répertoriée ci-dessous. Nous recommandons de passer les clients à de nouveaux abonnements avant la date de fin d'abonnement annuelle afin de leur éviter toute interruption de service. 

>[!NOTE]
>Les références (SKU) Skype Entreprise Online Plan1 commercial et secteur public ne sont plus disponibles.

Si vous utilisez l’API (CREST ou Espace partenaires), vous trouverez les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement avec la propriété de renouvellement automatique = False. Les abonnements Skype Entreprise Online Plan1 seront définis sur renouvellement automatique = False le 1erseptembre2018. Vous pouvez passer les clients vers une nouvelle formule à tout moment. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Formules de remplacement pour Skype Entreprise Online Plan1

Avec les nouvelles formules, vos clients peuvent profiter des nouvelles fonctions et fonctionnalités d'Office365. Les détails de la tarification figurent sur la liste de prix et le tableau répertoriant les offres dans l'Espace partenaires. 

- Option1: Office365 Entreprise F1
- Option2: Microsoft365 Entreprise F1
- Option 3: autres formules Office365

|**Fonctionnalité**    |**Option1**   |**Option2**   |**Option3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenir toutes les fonctionnalités incluses dans l'abonnement Skype Entreprise Online Plan1|Oui   |Oui   |Oui   |
|MI et présence |Oui   |Oui   |Oui   |
|Conversations audio et vidéo sur IP|Oui   |Oui   |Oui   
|Rejoindre des réunions en tant qu'utilisateur authentifié| Oui   |Oui   |Oui   |

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers des nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ces cas, vous pouvez avoir besoin de mettre à niveau les services de ses clients ou de migrer leurs abonnements à partir de références (SKU) qui vont progressivement disparaître. La migration de clients depuis des références supprimées vers des références plus récentes doit respecter les étapes suivantes:

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

### <a name="migrate-your-customers-to-new-plans"></a>Migrer vos clients vers de nouvelles formules

1. Pour acheter le nouvel abonnement, dans le **menu espace partenaires**, sélectionnez des **clients**, sélectionnez le client dont vous voulez déplacer, puis sélectionnez **Ajouter les abonnements**.

2. Sélectionnez l’abonnement à acheter dans le catalogue (en l’occurrence, l'une des options ci-dessus), indiquez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client doit maintenant avoir un ancien et un nouvel abonnement: l'ancien abonnement Skype Entreprise Online Plan1 et le nouvel abonnement «cible», par exemple, Option1: Office365 Entreprise F1.

3. Pour réaffecter les licences des utilisateurs du client, dans le menu **Espace partenaires** , sélectionnez les **clients**, sélectionnez le client que vous déplacez, puis sélectionnez **utilisateurs et licences**. La page Utilisateurs et licences du client s’ouvre.

4. Pour réaffecter la licence utilisateur, sélectionnez l’utilisateur à réaffecter, puis sélectionnez **Gérer les licences**.

5. Sur la page **Gérer les licences**, désactivez la case à cocher de la licence Skype Entreprise Online Plan1, puis sélectionnez une nouvelle formule de service pour l’abonnement auquel passe le client.

6. Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées. Suivez le même processus pour les autres utilisateurs qui ont besoin d'attributions de licences.

Une fois la licence utilisateur attribuée au nouveau service, vous pouvez en toute sécurité annuler l'abonnement retiré au niveau du client.

7. Dans le menu **Espace partenaires** , sélectionnez les **clients**. Sélectionnez le client dont vous annulez l’abonnement.

8. Dans la page des détails de l’abonnement, définissez l'état d'abonnement sur **Suspendu**.

9. Sélectionnez **Envoyer.**

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est automatiquement désapprovisionné après 120jours. Aucun frais n’est facturé au client pour l’ancien abonnement.

