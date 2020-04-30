---
title: Accorder aux clients l’autorisation d’acheter leurs propres services
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires du programme CSP peuvent permettre aux clients d’acheter leurs propres services, tels que les réservations Azure, pour un abonnement acheté pour eux.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: abonnement, achat libre-service, RI libre-service, activer RI, désactiver RI, libre-service, achat client, autorisations client, instance réservée achat client, réservations Azure achat client, activer le libre-service, désactiver le libre-service
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255471"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a>Découvrez comment accorder aux clients l’autorisation d’acheter leurs propres produits ou services

**S’applique à**

- Espace partenaires
- Partenaires du programme Fournisseur de solutions Microsoft Cloud

**Rôles appropriés**

- Agent d’administration
- Agent commercial

Cet article montre comment un partenaire dans le programme du fournisseur de solutions Cloud (CSP) peut accorder à un client l’autorisation d’acheter certains de ses propres services ou ressources.

Les partenaires du programme CSP utilisent souvent l’espace partenaires et son marché commercial pour acheter des solutions et des services pour leurs clients. Les partenaires permettent ensuite à certains clients d’approvisionner ces services eux-mêmes directement à partir du Portail Azure.

Voici un exemple. Supposons que vous achetez un abonnement à un plan Azure pour un client dans l’espace partenaires. Vous décidez ensuite d’ajouter d’autres ressources ou services à cet abonnement au nom du client. Dans ce cas, vous pouvez ajouter des réservations Azure à l’abonnement du client (par exemple, en ajoutant des instances de machine virtuelle réservées). Vous pouvez ensuite autoriser le client à approvisionner ultérieurement les ressources de réservation Azure dans le Portail Azure.

Désormais, avec la fonctionnalité des **autorisations du client** , vous offrez aux clients des options en libre-service avec les ressources Azure. En activant les autorisations pour le client, vous permettez aux clients d’acheter leurs propres ressources (par exemple, en achetant leurs propres réservations Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Vue d’ensemble des autorisations client dans l’espace partenaires

Utilisez la page **compte** client pour activer (ou désactiver) les autorisations des clients. Actuellement, cette fonctionnalité prend en charge :

- **Réservations Azure :** L’activation de cette autorisation permet au client d’acheter ses propres réservations Azure pour un abonnement Azure spécifique que vous avez acheté.

Avant d’activer les autorisations des clients, notez les points importants suivants :

- Par défaut, les autorisations du client sont automatiquement désactivées (désactivées) dans l’espace partenaires.
- Avant de pouvoir activer (ou désactiver) les autorisations pour un client, vous devez avoir le rôle d’agent d’administration dans l’espace partenaires.
  Les partenaires disposant du rôle agent commercial ou agent du support technique disposent d’un accès en lecture seule et ne peuvent pas activer ou désactiver les autorisations du client.
- Vous pouvez activer les autorisations (activer) pour n’importe quel client de votre choix.
- Vous pouvez activer (ou désactiver) les autorisations des clients à l’aide du tableau de bord de l’espace partenaires ou des API de l' [espace partenaires](https://docs.microsoft.com/partner-center/develop/manage-customers).
- Une fois que vous avez activé (activé) les autorisations pour un client spécifique, vous êtes chargé de payer les achats ultérieurs effectués par ce client. Si les clients souhaitent échanger, annuler ou renouveler un achat effectué, ils ne peuvent pas le faire eux-mêmes. Ils doivent vous demander, en tant que partenaire, de les aider à échanger, annuler ou renouveler ces achats.
- Une fois que vous avez activé les autorisations pour un client spécifique, vous n’êtes **pas** averti des achats ultérieurs effectués par le client.
- Les achats ultérieurs effectués par le client s’affichent dans l’espace partenaires, ainsi que tous les achats effectués par vous. Vous pouvez trouver ces achats sur la page **historique des commandes** du client, sur la page **réservations** ou dans le [**Journal d’activité**](activity-logs.md).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure

Les réservations Azure sont un excellent moyen d’acheter des services Azure à tarif réduit. Pour en savoir plus sur les avantages des réservations Azure, consultez [qu’est-ce que Azure reservations ?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Vous avez maintenant la possibilité d’acheter des réservations Azure pour le compte de vos clients, comme vous l’avez peut-être déjà fait. Ou, vous pouvez autoriser les clients à acheter leurs propres réservations Azure.

>[!NOTE]
> Une fois que vous avez donné l’autorisation aux clients d’acheter leurs propres réservations Azure, vous pouvez les aider à comprendre comment gérer les réservations qu’ils achètent. Par exemple, les clients peuvent souhaiter savoir comment optimiser leur utilisation d’une réservation ou comment modifier l’étendue d’une réservation. Pour plus d’informations sur ces rubriques, demandez aux clients de lire [gérer les réservations pour les ressources Azure]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Pour permettre aux clients d’acheter leurs propres réservations Azure

1. Vérifiez que le client dispose déjà d’un plan Azure ou d’un abonnement Azure global que vous avez acheté en son nom.

2. Vérifiez que le rôle **propriétaire** de cet abonnement a été attribué au client.

3. Activez les autorisations client (activez cette **fonctionnalité)** pour acheter leurs propres réservations Azure.

Chaque étape apparaît ci-dessous.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Vérifier que le client dispose déjà d’un abonnement Azure

Avant de fournir l’autorisation aux clients d’acheter leurs propres réservations Azure, vous devez vérifier que le client dispose d’un abonnement Azure ou d’un abonnement Azure global existant. Si le client n’affiche aucun abonnement Azure actuel dans l’espace partenaires, vous devez souscrire un abonnement avant d’activer ses autorisations client.

- Pour voir si un client dispose déjà d’un abonnement Azure, connectez-vous au tableau de bord de l’espace partenaires, puis sélectionnez **CSP** suivi de **clients**. Sélectionnez le client spécifique dans la liste. Sélectionnez ensuite **abonnements** et recherchez tous les abonnements basés sur l’utilisation pour Azure plan ou Azure global.

- Si un client n’a pas d’abonnement Azure, vous pouvez en acheter un. Consultez [acheter le plan Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Vérifiez que le rôle correct a été attribué au client dans Azure

Une fois que vous avez vérifié que le client dispose d’un abonnement Azure existant, vous devez également vérifier que les utilisateurs principaux associés à votre client se voient attribuer le rôle de **propriétaire** approprié pour cet abonnement Azure. Il s’agit de l’accès en fonction du rôle (RBAC) dont le client a besoin pour acheter des réservations Azure pour un abonnement Azure que vous avez acheté.

Certains partenaires ont peut-être déjà attribué le rôle de **propriétaire** aux clients souhaitant gérer et approvisionner activement leurs propres ressources Azure. Si vous avez déjà affecté l’état du **propriétaire** à un client pour gérer les abonnements précédents que vous avez achetés pour eux, vous pouvez ignorer cette étape.  

> [!IMPORTANT]
> Si un client ne se voit pas attribuer le rôle de **propriétaire** , il reçoit une erreur dans le portail Azure les empêchant d’acheter des réservations Azure.

Pour vérifier que le rôle **propriétaire** d’un abonnement Azure a été attribué au client :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Sélectionnez **CSP**, puis **clients** et sélectionnez le client spécifique.

3. Sélectionnez **abonnements** pour ce client et recherchez l’abonnement Azure spécifique.

4. Sélectionnez le bouton **gérer** en regard de l’abonnement de ce client. Cela ouvre le [portail Azure](https://portal.azure.com/).

5. Pour attribuer le rôle de **propriétaire** à un utilisateur spécifique, procédez comme suit [pour affecter un utilisateur en tant qu’administrateur](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Activer ou désactiver les autorisations des clients pour acheter leurs propres réservations Azure

Une fois que vous avez vérifié que le client dispose d’un abonnement Azure et que les utilisateurs se voient attribuer le rôle de **propriétaire** pour cet abonnement, vous êtes prêt à activer (activer) les autorisations des clients. Vous pouvez également utiliser ces étapes pour désactiver (désactiver) les autorisations des clients. Vous pouvez activer ou désactiver des autorisations client à l’aide du tableau de bord de l’espace partenaires ou des API de l' [espace partenaires](https://docs.microsoft.com/partner-center/develop/manage-customers).

Pour activer (ou désactiver) les autorisations des clients dans l’espace partenaires :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu de navigation de gauche, sélectionnez **CSP**, puis **Customers**. Une liste de clients s’affiche.

3. Sélectionnez un nom de client spécifique.

4. Sélectionnez **compte** dans le menu client. La page **compte** client s’affiche.

5. Recherchez la zone **autorisations du client** au bas de la page.

   ![Autorisations du client sur la page du compte](images/give-customers-permission-reservations.png)

6. Sous **réservations Azure**, recherchez l’option **autoriser le client à acheter** .

7. Pour activer les autorisations des clients, déplacez le commutateur en regard de cette option sur la position **on** . Pour désactiver les autorisations des clients, déplacez le commutateur en position **off** .

>[!NOTE]
> Pour savoir ce qui se passe quand vous activez les autorisations d’un client pour acheter ses propres réservations Azure, consultez [vue d’ensemble des autorisations client dans l’espace partenaires](give-customers-permission.md#overview-of-customer-permissions-in-partner-center). Quand vous activez (ou désactivez) les autorisations des clients, le journal d’activité enregistre chaque action. (Ce journal est accessible lorsque vous sélectionnez l’icône d’engrenage en haut du tableau de bord de l’espace partenaires). Lorsque vous activez ou désactivez les autorisations du client, l’action s’affiche sous la forme **créer des autorisations d’achat** du client ou **Supprimer les autorisations d’achat du client** dans le journal d’activité.

## <a name="see-also"></a>Voir aussi

- [Acheter des réservations Azure pour le compte de vos clients](azure-reservations-buying.md)
- [Espace partenaires-vendre des réservations Microsoft](azure-reservations.md)
- [Gérer des réservations Azure pour le compte de vos clients](azure-reservations-manage.md) 