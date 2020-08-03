---
title: Facturation des achats ponctuels & périodique
ms.topic: article
ms.date: 05/05/2020
description: Pour obtenir des exemples de facturation de l’espace partenaires pour une seule fois et sélectionner des achats récurrents, lorsque vous achetez des abonnements, ajoutez des abonnements, ajoutez ou supprimez des licences.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5349a78b788c060999c98440edf962a64cb43112
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468393"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scénarios de facturation de l’espace partenaires pour une période unique et sélection des achats récurrents

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Agent du support technique
- Agent commercial

Il s’agit de [scénarios de facturation courants](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Acheter un abonnement et ajouter une licence le même jour

Dans le scénario 1, vous achetez un abonnement le 11 juin à un prix unitaire de 4 $. Plus tard dans la journée, vous achetez un autre abonnement au même tarif.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 4 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 1 = 4,00.
- Refacturation au prorata de 8 $ pour la période de service du 10 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 30 x 2 = 8,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de dépense** |
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

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez une licence)     |10/06/2019   |09/07/2019         |4 $         |1        |4 $            |Nouveau         |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -3,87 $       |addQuantity           |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |7,74 $       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Acheter un abonnement et supprimer une licence le même jour

Dans le scénario 3, vous achetez deux abonnements pour le même produit le 11 juin à un prix unitaire de $4. Plus tard le même jour, vous supprimez l’une des licences.  

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour deux licences pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de 8 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 2 = 8,00.
- Refacturation au prorata de 4 $ pour la période de service du 11 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 30 x 1 = 4,00.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |2                 |8 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -8 $       |removeQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 1      |4 $         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Acheter un abonnement et supprimer des licences ultérieurement

Dans le scénario 4, vous achetez 2 abonnements le 11 juin à un prix unitaire de $4 et, le 12 juin, vous supprimez l’une des licences.

Le fichier de rapprochement inclut les éléments suivants :

- Facture de 8 $ pour la période de service du 10 juin au 9 juillet.
- Refacturation au prorata de -7,74 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 2 = 7,74.
- Refacturation au prorata de 3,87 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 29 x 1 = 3,87.

|**Date d’achat**   |**Début de facturation** |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de dépense** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez 2 licences)     |10/06/2019   |09/07/2019         |4 $         |2        |8 $       |Nouveau       |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -7,74 $       |removeQuantity           |
|12/06/2019 (vous avez 1 licence)    | 10/06/2019    |09/07/2019   |4 $    |1      |3,87 $    |removeQuantity |
