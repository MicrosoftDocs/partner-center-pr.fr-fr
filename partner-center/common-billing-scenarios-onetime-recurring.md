---
title: Facturation des achats ponctuels & périodique
ms.topic: article
ms.date: 05/05/2020
description: Pour obtenir des exemples de facturation de l’espace partenaires pour une seule fois et sélectionner des achats périodiques, lorsque vous achetez des abonnements, ajoutez des abonnements, ajoutez ou supprimez des sièges.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: facturation, paiements, achat unique, achat périodique, abonnements, sièges
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2c3467fdbe8457a7068a49000bd635b7c464cf29
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908201"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scénarios de facturation de l’espace partenaires pour une période unique et sélection des achats récurrents

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Agent du support technique
- Agent commercial

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) s’appliquent à [une seule fois et sélectionnent des frais périodiques](one-time-and-recurring-billing.md) dans l’espace partenaires.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Acheter un abonnement et ajouter un siège le même jour

Dans le scénario 1, vous achetez un abonnement le 11 juin à un prix unitaire de 4 $. Plus tard dans la journée, vous achetez un autre abonnement au même tarif.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 4 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 1 = 4,00.
- Refacturation au prorata de 8 $ pour la période de service du 10 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 30 x 2 = 8,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Proportion** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |1                 |4 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -4 $       |addQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |8 $         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Acheter un abonnement et ajouter d’autres abonnements ultérieurement

Dans le scénario 2, vous achetez un abonnement le 11 juin à un prix unitaire de $4 et le 12 juin, vous en achetez un autre pour le même produit au même prix.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 4 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de -3,87 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 1 = 3,87.
- Refacturation au prorata de 7,74 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 29 x 2 = 7,74.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Proportion** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez une licence)     |10/06/2019   |09/07/2019         |4 $         |1        |4 $            |Nouveau         |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -3,87 $       |addQuantity           |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |7,74 $       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Acheter un abonnement et supprimer un siège le même jour

Dans le scénario 3, vous achetez deux abonnements pour le même produit le 11 juin à un prix unitaire de $4. Plus tard dans la journée, vous supprimez l’un des sièges.  

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour deux licences pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 8 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 2 = 8,00.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 30 x 1 = 4,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Proportion** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |2                 |8 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -8 $       |removeQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 1      |4 $         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Acheter un abonnement et supprimer des sièges ultérieurement

Dans le scénario 4, vous achetez 2 abonnements le 11 juin à un prix unitaire de 4 $, puis le 12 juin, vous supprimez l’un des sièges.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de -7,74 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 2 = 7,74.
- Refacturation au prorata de 3,87 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 29 x 1 = 3,87.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Proportion** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez 2 licences)     |10/06/2019   |09/07/2019         |4 $         |2        |8 $       |Nouveau       |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -7,74 $       |removeQuantity           |
|12/06/2019 (vous avez 1 licence)    | 10/06/2019    |09/07/2019   |4 $    |1      |3,87 $    |removeQuantity |
