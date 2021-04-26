---
title: Migrer des abonnements Skype entreprise
description: Découvrez comment et quand migrer certains clients avec l’expiration des abonnements Skype for Business Online plan 1 aux nouvelles versions d’Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: f395987ef647fa6f7ed264c6476ddae419eabc34
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002856"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrer des abonnements Skype Entreprise Online Plan 1 vers une version plus récente d'Office 365

**Rôles appropriés**

- Agent commercial

Le plan 1 de Skype entreprise Online sera mis hors service, à compter du 1er août 2018. Après cette date, les clients ne peuvent plus acheter les nouveaux abonnements du plan 1 Skype entreprise et les abonnements existants ne seront pas renouvelés automatiquement lorsqu’ils expirent et ne fourniront pas d’option de renouvellement. Sur la page de détails de l’abonnement, l’état de l’abonnement du plan 1 de Skype entreprise Online est passé à « expire le [date] » de « auto Renews on [date] ».  

Pour garantir la continuité des clients, vous devez faire passer les clients avec des abonnements Skype for Business Online plan 1 arrivant à une option SKU prise en charge, comme indiqué ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients. 

>[!NOTE]
>Skype entreprise Online plan 1 références SKU commerciales et gouvernementales sont retirées.

Si vous utilisez l’API (CREST ou Partner Center), recherchez les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique = faux. Les abonnements Skype entreprise Online plan 1 seront configurés pour un renouvellement automatique = faux le 1er septembre 2018. Vous pouvez déplacer les clients vers un nouveau plan à tout moment. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Plans de remplacement du plan 1 de Skype entreprise Online

Avec les nouveaux plans, vos clients peuvent tirer parti des fonctionnalités et fonctionnalités plus récentes d’Office 365. Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires. 

- Option 1 : Office 365 entreprise F1
- Option 2 : Microsoft 365 Entreprise F1
- Option 3 : autres plans Office 365

|**Fonctionnalité**    |**Option 1 :**   |**Option 2 :**   |**Option 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenir toutes les fonctionnalités incluses dans le plan 1 de Skype entreprise Online|Oui   |Oui   |Oui   |
|Messagerie instantanée et présence |Oui   |Oui   |Oui   |
|Audio et vidéo d’égal à égal sur IP|Oui   |Oui   |Oui   
|Joindre des réunions en tant qu’utilisateur authentifié| Oui   |Oui   |Oui   |

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées. La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :

- Acheter le nouvel abonnement
- Réaffecter les licences utilisateur actuelles
- Annuler l’ancien abonnement

### <a name="migrate-your-customers-to-new-plans"></a>Migrer vos clients vers de nouveaux plans

1. Pour acheter le nouvel abonnement, dans le **menu espace partenaires**, sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.

2. Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**. 

Votre client doit maintenant avoir les anciens et les nouveaux abonnements, l’ancien abonnement à Skype entreprise Online (plan 1) et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 Enterprise F1.

3. Pour réaffecter les licences des utilisateurs du client, dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous déplacez, puis sélectionnez **utilisateurs et licences**. La page utilisateurs et licences du client s’ouvre.

4. Pour réaffecter la licence utilisateur, sélectionnez l’utilisateur à réassigner, puis sélectionnez **gérer les licences.**

5. Sur la page **gérer les licences** , désactivez la case à cocher licence Skype entreprise Online plan 1 et sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.

6. Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées. Poursuivez ce même processus pour les autres utilisateurs qui ont besoin d’attributions de licence.

Après avoir déplacé la licence utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client.

7. Dans le menu **espace partenaires** , sélectionnez **clients**. Sélectionnez le client dont vous annulez l’abonnement.

8. Dans la page Détails de l’abonnement, définissez l’abonnement sur **suspendu**.

9. Sélectionnez **Envoyer.**

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est désapprovisionné automatiquement après 120 jours. Aucun frais n’est facturé au client pour l’ancien abonnement.

## <a name="next-steps"></a>Étapes suivantes

- [Conseillers : créez et envoyez une invitation à la version d’évaluation pour que les clients essaient Office 365](advisors-create-a-trial-invitation.md)
- [Conseillers : créez votre base de clients avec des offres d’essai et des offres d’achat Office 365](advisors-build-your-business.md)
- [Conseillers : créer une offre d’achat](advisor-create-a-purchase-offer.md)
