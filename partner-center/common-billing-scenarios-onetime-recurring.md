---
title: Scénarios de facturation courants pour une période unique et sélection des achats récurrents | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Scénarios de facturation courants dans l’espace partenaires pour une période unique et sélectionnez des achats récurrents (tels que l’achat d’abonnements, l’ajout d’abonnements, l’ajout et la suppression de sièges).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturation, paiements, achat unique, achat périodique, abonnements, sièges
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389637"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>Scénarios ponctuels de facturation et de sélection des achats périodiques

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) s’appliquent à [une seule fois et sélectionnent des frais périodiques](one-time-and-recurring-billing.md) dans l’espace partenaires.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Acheter un abonnement et ajouter un siège le même jour

Dans le scénario 1, vous achetez un abonnement le 11 juin à un prix unitaire de 4 $. Plus tard dans la journée, vous achetez un autre abonnement au même tarif.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 4 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 1 = 4,00.
- Refacturation au prorata de 8 $ pour la période de service du 10 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 30 x 2 = 8,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |1                 |4 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -4 $       |addQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |8 $         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Acheter un abonnement et ajouter d’autres abonnements ultérieurement

Dans le scénario 2, vous achetez un abonnement le 11 juin à un prix unitaire de $4 et le 12 juin, vous en achetez un autre pour le même produit au même prix.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 4 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de -3,87 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 1 = 3,87.
- Refacturation au prorata de 7,74 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 29 x 2 = 7,74.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez une licence)     |10/06/2019   |09/07/2019         |4 $         |1        |4 $            |Nouveau         |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -3,87 $       |addQuantity           |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |7,74 $       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Acheter un abonnement et supprimer un siège le même jour

Dans le scénario 3, vous achetez deux abonnements pour le même produit le 11 juin à un prix unitaire de $4. Plus tard dans la journée, vous supprimez l’un des sièges.  

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour deux licences pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 8 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 2 = 8,00.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 30 x 1 = 4,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |2                 |8 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -8 $       |removeQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 1      |4 $         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Acheter un abonnement et supprimer des sièges ultérieurement

Dans le scénario 4, vous achetez 2 abonnements le 11 juin à un prix unitaire de 4 $, puis le 12 juin, vous supprimez l’un des sièges.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de -7,74 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 2 = 7,74.
- Refacturation au prorata de 3,87 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 29 x 1 = 3,87.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez 2 licences)     |10/06/2019   |09/07/2019         |4 $         |2        |8 $       |Nouveau       |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -7,74 $       |removeQuantity           |
|12/06/2019 (vous avez 1 licence)    | 10/06/2019    |09/07/2019   |4 $    |1      |3,87 $    |removeQuantity |
