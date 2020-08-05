---
title: Permettre aux clients d’acheter leurs propres services dans CSP
description: Découvrez comment les partenaires du programme CSP peuvent permettre aux clients d’acheter leurs propres services, tels que les réservations Azure, pour un abonnement acheté pour eux dans l’espace partenaires.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3327ad560d38de042f42baf1f0a2daedda5d4ecf
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545640"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Autoriser les clients dans l’espace partenaires à acheter leurs propres produits ou services

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

- Une fois que vous avez activé (activé) les autorisations pour un client spécifique, vous êtes chargé de payer les achats ultérieurs effectués par ce client. Si les clients souhaitent échanger, annuler ou renouveler un achat qu’ils ont effectué (ou qu’ils souhaitent modifier l’étendue initiale d’une réservation), ils ne peuvent pas le faire eux-mêmes. Ils doivent vous demander, en tant que partenaire, de les aider à échanger, annuler et renouveler des achats, ou apporter des modifications ultérieures à l’étendue d’une réservation.  

- Une fois que vous avez activé les autorisations pour un client spécifique, vous n’êtes **pas** averti des achats ultérieurs effectués par le client.

- Les achats ultérieurs effectués par le client s’affichent dans l’espace partenaires, ainsi que tous les achats effectués par vous. Vous pouvez trouver ces achats sur la page **historique des commandes** du client, sur la page **réservations** ou dans le [**Journal d’activité**](activity-logs.md).

>[!NOTE]
> Pour plus d’informations sur les prix que le client va payer et sur la manière d’aider les clients à gérer leurs achats, consultez [aider les clients à gérer les réservations qu’ils achètent](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure

Les réservations Azure sont un excellent moyen d’acheter des services Azure à tarif réduit. Pour en savoir plus sur les avantages des réservations Azure, consultez [qu’est-ce que Azure reservations ?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Vous avez maintenant la possibilité d’acheter des réservations Azure pour le compte de vos clients, comme vous l’avez peut-être déjà fait. Ou, vous pouvez autoriser les clients à acheter leurs propres réservations Azure.

>[!NOTE]
> Une fois que vous avez donné l’autorisation aux clients d’acheter leurs propres réservations Azure, aidez-les à gérer les réservations qu’ils achètent. Pour plus d’informations, consultez [aider les clients à gérer les réservations qu’ils achètent](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

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

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Autorisations du client sur la page du compte." border="true":::

6. Sous **réservations Azure**, recherchez l’option **autoriser le client à acheter** .

7. Pour activer les autorisations des clients, déplacez le commutateur en regard de cette option sur la position **on** . Pour désactiver les autorisations des clients, déplacez le commutateur en position **off** .

>[!NOTE]
> Pour savoir ce qui se passe quand vous activez les autorisations d’un client pour acheter ses propres réservations Azure, consultez [vue d’ensemble des autorisations client dans l’espace partenaires](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Quand vous activez (ou désactivez) les autorisations des clients, le journal d’activité enregistre chaque action. (Ce journal est accessible lorsque vous sélectionnez l’icône d’engrenage en haut du tableau de bord de l’espace partenaires). Lorsque vous activez ou désactivez les autorisations du client, l’action s’affiche sous la forme **créer des autorisations d’achat** du client ou **Supprimer les autorisations d’achat du client** dans le journal d’activité.

## <a name="help-customers-manage-reservations-they-purchase"></a>Aider les clients à gérer les réservations qu’ils achètent

Une fois que vous avez donné l’autorisation aux clients d’acheter leurs propres réservations Azure, vous pouvez les aider à mieux gérer les ressources qu’ils achètent. Les clients peuvent gérer de nombreux aspects des réservations Azure directement à partir de la [portail Azure](https://portal.azure.com/). Ils auront besoin de votre aide pour gérer quelques-uns des autres aspects des réservations Azure qu’ils achètent dans votre abonnement CSP.  

Aidez les clients à comprendre plus sur la gestion de ces aspects des réservations Azure :

- Prix facturés par les clients pour les réservations Azure
- Comment les clients peuvent optimiser l’utilisation des réservations Azure
- Que se passe-t-il lorsque les clients achètent des réservations avec une étendue partagée ?
- Que se passe-t-il si les clients souhaitent modifier, annuler et renouveler une réservation, ou modifier son étendue ?

**Les prix des clients paient leurs réservations.** Votre client achète des réservations Azure sur la base d’un abonnement que vous avez acheté précédemment dans votre compte de facturation de partenaire CSP. Le prix du client pour toutes les réservations Azure qu’il achète en fonction de cet abonnement est également défini par vous-même. Ce prix peut être différent du tarif direct Web que le client voit dans le Portail Azure.

**Comment les clients peuvent optimiser leur utilisation d’une réservation.** Certains clients peuvent tirer parti d’en savoir plus sur l’optimisation de leur utilisation d’une réservation ou sur l’affectation de l’étendue initiale d’une réservation pendant son achat. Pour plus d’informations, demandez aux clients de lire [gérer des réservations pour les ressources Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Que se passe-t-il lorsqu’un client achète une réservation avec une étendue partagée ?** Lorsque les clients achètent une réservation basée sur un abonnement CSP antérieur et affectent une étendue partagée à cette réservation, toute remise fournie par le client par le fournisseur de services Cloud s’applique à l’utilisation correspondante pour tous les abonnements que le partenaire CSP a achetés pour ce client.

**Que doivent faire les clients s’ils souhaitent échanger, annuler ou renouveler un achat effectué ou modifier l’étendue initiale d’une réservation ?** Les clients doivent demander à leur partenaire de leur permettre de modifier l’étendue initiale d’une réservation. Ils ont également besoin de l’aide d’un partenaire pour échanger, annuler ou renouveler une réservation. Ils ne peuvent pas effectuer ces tâches elles-mêmes avec des réservations basées sur des abonnements achetés pour eux par un partenaire CSP.

## <a name="next-steps"></a>Étapes suivantes

- [Acheter des réservations Azure pour le compte de vos clients](azure-reservations-buying.md)

- [Espace partenaires-vendre des réservations Microsoft](azure-reservations.md)

- [Gérer des réservations Azure pour le compte de vos clients](azure-reservations-manage.md)
