---
title: Définir un budget de dépenses Azure pour les clients
ms.topic: how-to
ms.date: 06/03/2020
description: Découvrez comment définir ou supprimer des budgets de dépenses Azure mensuels pour vos clients, ainsi que pour afficher les données de dépense Azure et définir des notifications relatives au budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811249"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Définir, vérifier ou supprimer des budgets de dépenses Azure mensuels pour les clients dans l’espace partenaires

S’applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Vous pouvez [définir un budget de dépenses Azure mensuel pour vos clients](#set-azure-spending-budget) dans l’espace partenaires. Cela permet à vos clients de gérer leurs dépenses Azure. Cette option vous permet de comparer les dépenses Azure de vos clients au budget du mois. Il permet également à vos clients de budgétiser leurs dépenses Azure, de sorte que leur facture mensuelle n’est pas supérieure à celle qu’ils anticipent.

> [!NOTE]  
> Cette fonctionnalité n’est pas disponible dans les comptes de bac à sable (sandbox) ou de test en production (TIP).

Une fois que vous avez [défini un budget de dépenses Azure pour vos clients](#set-azure-spending-budget), vous pouvez également consulter l’utilisation des clients de l’une des manières suivantes. Ces options peuvent vous aider à identifier des services mal configurés ou des tendances inhabituelles susceptibles de suggérer des fraudes. Vous pouvez ensuite travailler avec vos clients pour identifier la cause racine et gérer les coûts. Si nécessaire, vous pouvez également [modifier le budget du client](#set-azure-spending-budget) sur une valeur supérieure.

- [Vérifier les dépenses Azure actuelles](#check-current-azure-spending)

- [Activer les notifications par courrier électronique lorsque la dépense d’un client est proche de sa limite budgétaire](#notifications-for-budget-limits)

- [Afficher les coûts totaux par service pour les abonnements basés sur l’utilisation](#itemized-costs-by-service)

Vous pouvez également [supprimer un budget de dépenses Azure](#remove-azure-spending-budget) pour le ou les clients à tout moment.

## <a name="azure-spending-data"></a>Données de dépense Azure

Les données de dépense Azure sont une *estimation* et les *montants de facturation réels peuvent varier*. La valeur des données *ne reflète pas* les taxes, crédits, ajustements ou autres frais qui peuvent s’appliquer.

Les données de dépense sont *actualisées une fois par jour*. Vos clients peuvent continuer à utiliser (et être facturés pour) les services et les ressources Azure, sauf si vous modifiez leurs paramètres de compte dans le Portail Azure.

## <a name="set-azure-spending-budget"></a>Définir le budget des dépenses Azure

Vous pouvez *définir un budget de dépenses Azure mensuel* pour plusieurs clients dans l’espace partenaires :

1. Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).

2. Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.

3. Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients pour lesquels vous souhaitez définir un budget.

4. Entrez une valeur pour le **Budget mensuel**.

5. Choisissez **appliquer** pour enregistrer vos modifications.

Vous pouvez également *définir un budget pour un client individuel* dans ses paramètres d’abonnement :

1. Connectez-vous au tableau de bord de l’Espace partenaires.

2. Dans le menu de gauche, sous **CSP**, choisissez **clients**.

3. Sur la page **clients** , sélectionnez le nom de la **société**du client.

4. Sur la page **abonnements** du client, sous **abonnement basé sur l’utilisation**, choisissez **modifier le budget**.

5. Entrez une valeur pour le budget.

6. Choisissez **appliquer** pour enregistrer vos modifications.

## <a name="remove-azure-spending-budget"></a>Supprimer le budget des dépenses Azure

Vous pouvez *supprimer un budget de dépenses Azure mensuel* pour vos clients dans l’espace partenaires :

1. Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).

2. Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.

3. Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients dont vous souhaitez supprimer le budget.

4. Choisissez **supprimer le budget**.

## <a name="check-current-azure-spending"></a>Vérifier les dépenses Azure actuelles

Vous pouvez à tout moment *suivre les dépenses et les budgets mensuels actuels de vos clients* :

1. Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).

2. Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.

3. Dans la page des **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, vous pouvez voir une vue d’ensemble des budgets mensuels des clients, des estimations de dépense actuelles et du pourcentage de budget utilisé.

## <a name="notifications-for-budget-limits"></a>Notifications pour les limites budgétaires

Vous pouvez *activer les notifications par courrier électronique* lorsque la dépense mensuelle de votre client est proche de sa limite budgétaire. Lorsque vous activez cette option, vous êtes averti lorsque les clients utilisent 80% ou plus de leur budget mensuel. Cette option vous permet de garder un œil sur votre facture Azure. Pour configurer les notifications par courrier électronique :

1. Connectez-vous à l’Espace partenaires.

2. Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.

3. Dans la page **dépenses Azure** , sous **notifications par courrier électronique**, basculez le paramètre **recevoir des e-mails** **sur activé**.

4. Choisissez **modifier l’adresse de messagerie** pour afficher l’adresse de messagerie des notifications.

5. Si l’adresse de messagerie *est incorrecte*, entrez l’adresse de messagerie appropriée, puis choisissez **mettre à jour**. Si l’adresse de messagerie *est correcte*, choisissez **Annuler**.

## <a name="itemized-costs-by-service"></a>Coûts totaux par service

Vous pouvez *afficher les coûts totaux (et l’utilisation estimée) par service pour les abonnements basés sur l’utilisation*:

1. Connectez-vous à l’Espace partenaires.

2. Dans le menu de gauche, sous **CSP**, choisissez **clients**.

3. Sur la page **clients** , sélectionnez le nom de la **société**du client.

4. Sur la page **abonnements** du client, sous **abonnements basés sur l’utilisation**, sélectionnez le nom de l' **abonnement**.

5. Sur la page de l’abonnement, vous pouvez passer en revue les **coûts** par service et l' **utilisation estimée** pour le mois en cours.
