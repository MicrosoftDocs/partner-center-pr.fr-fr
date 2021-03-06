---
title: Migrer les abonnements Kaizala Pro vers Microsoft 365
description: Découvrez comment migrer des abonnements Kaizala Pro vers des versions Microsoft 365 ou Office 365. Lisez cet article pour plus d’informations sur la transition de vos clients.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146423"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrer des abonnements Kaizala Pro autonomes vers des versions Microsoft 365 ou Office 365

**Rôles appropriés**: sales agent

À compter du 1er juillet 2020, Microsoft met fin aux ventes du service autonome Kaizala Pro. Les clients ne seront plus en mesure d’acheter de nouveaux abonnements Kaizala Pro après cette date, et les abonnements Kaizala Pro existants ne seront pas renouvelés automatiquement lorsqu’ils expirent.

Pour garantir la continuité des clients, vous devez faire en sorte que les clients qui expirent les abonnements Kaizala Pro autonomes soient pris en charge, comme indiqué ci-dessous. Nous vous recommandons de déplacer les clients vers les nouveaux abonnements avant la date de fin annuelle de l’abonnement pour éviter les interruptions de service pour les clients.

Si vous utilisez l’API (à la fois CREST ou Partner Center), vous pouvez découvrir les abonnements arrivant à expiration en évaluant la date de fin de l’abonnement, ainsi que la propriété renouvellement automatique définie sur false : `auto renew = False` .

Les abonnements E4 seront définis `auto renew=False` sur le 1er juillet 2020. Vous pouvez déplacer les clients vers un nouveau plan à tout moment.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Plans de remplacement autonomes Kaizala Pro

Avec les nouveaux plans, vos clients peuvent tirer parti des fonctionnalités et fonctionnalités plus récentes dans Microsoft 365. Les détails de la tarification se trouvent dans la matrice liste de prix et liste des offres de l’espace partenaires.

- [**Microsoft 365 pour les entreprises**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), notamment :  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 pour la Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), notamment :
   - Microsoft 365 F3 (anciennement Microsoft 365 F1) et Office 365 F3
    
- [**Microsoft 365 pour les entreprises**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), notamment : 
   - Office 365 E1
   - Microsoft 365 E3 et Office 365 E3
   - Microsoft 365 E5 et Office 365 E5

- [**Microsoft 365 pour l’éducation**](https://www.microsoft.com/education/buy-license/microsoft365), notamment : 
    - Microsoft 365 A1 et Office 365 A1
    - Microsoft 365 A3 et Office 365 A3
    - Microsoft 365 A5 et Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Accompagner les clients vers les nouvelles formules de produit

Microsoft offre en permanence de nouveaux produits et services à nos partenaires. Dans ce cas, vous devrez peut-être mettre à niveau les clients vers de nouveaux services ou migrer leurs abonnements à partir des références SKU qui seront finalement arrêtées. La migration des clients des références SKU mises hors service vers les plus récentes nécessite les étapes suivantes :

R. Acheter le nouvel abonnement

B. Réaffecter les licences utilisateur actuelles

C. Annuler l’ancien abonnement


## <a name="migrate-your-customers-to-new-plans"></a>Migrer vos clients vers de nouveaux plans

### <a name="a-purchase-the-new-subscription"></a>R. Acheter le nouvel abonnement

1. Pour acheter le nouvel abonnement, dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous souhaitez déplacer, puis sélectionnez **Ajouter des abonnements**.

2. Sélectionnez l’abonnement que vous souhaitez acheter dans le catalogue (dans ce cas, l’une des options ci-dessus), entrez le nombre de licences, puis sélectionnez **Envoyer**.

Votre client doit maintenant avoir les anciens et les nouveaux abonnements, l’ancien abonnement Kaizala Pro standalone et le nouvel abonnement « cible », par exemple, l’option 1-Office 365 entreprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Réaffecter les licences utilisateur actuelles

1. Pour réaffecter les licences des utilisateurs du client, dans le menu **espace partenaires** , sélectionnez **clients**, sélectionnez le client que vous déplacez, puis sélectionnez **utilisateurs et licences**. La page utilisateurs et licences du client s’ouvre.

2. Pour réaffecter la licence utilisateur, sélectionnez l’utilisateur à réassigner, puis sélectionnez **gérer les licences**.

3. Sur la page **gérer les licences** , désactivez la case à cocher licence autonome Kaizala Pro, puis sélectionnez un nouveau plan de service pour l’abonnement vers lequel le client est déplacé.

4.  Sélectionnez **Envoyer**. Une page de confirmation indique les nouvelles licences attribuées. Poursuivez ce même processus pour les autres utilisateurs qui ont besoin d’attributions de licence.

### <a name="c-cancel-old-subscription"></a>C. Annuler l’ancien abonnement

Après avoir déplacé la licence utilisateur vers le nouveau service, vous pouvez annuler en toute sécurité l’abonnement mis hors service au niveau du client.

1.  Dans le menu **espace partenaires** , sélectionnez **clients**. Sélectionnez le client dont vous annulez l’abonnement.

2.  Dans la page Détails de l’abonnement, définissez l’abonnement sur **suspendu**.

3.  Sélectionnez **Envoyer**.

L’ancien abonnement est suspendu et le nouveau est activé. L’abonnement suspendu est désapprovisionné automatiquement après 120 jours. Aucun frais n’est facturé au client pour l’ancien abonnement.
