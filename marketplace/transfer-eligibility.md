---
title: 'Éligibilité du transfert : instructions pour le transfert d’un abonnement entre comptes de facturation, place de marché Azure'
description: Instructions pour les contrôles commerciaux avant le transfert d’un abonnement entre les comptes de facturation dans le Portail Azure.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007153"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Éligibilité du transfert pour un abonnement entre des comptes de facturation

Vous pouvez [transférer un abonnement](/azure/cost-management-billing/understand/subscription-transfer) d’un compte de facturation à un autre dans la section facturation du portail Azure. Avant un transfert, l’abonnement est analysé pour rechercher les produits tiers. Le transfert est autorisé uniquement si *tous les* produits sont désactivés pour le transfert (voir les [critères](#criteria-for-transfer-approval-or-denial) ci-dessous). Le système génère des messages d’erreur pertinents pour les applications dont l’effacement a échoué pour vous aider à déterminer les étapes suivantes.

> [!NOTE]
> Cet article ne s’applique pas aux offres SaaS, car les ressources SaaS sont attachées à un locataire, et non à un abonnement. Les ressources SaaS peuvent être transférées d’un compte de facturation à un autre, mais cette opération est effectuée par ressource et par le support Azure en tant que demande de support.

## <a name="criteria-for-transfer-approval-or-denial"></a>Critères d’approbation ou de refus de transfert

Vous ne pouvez pas transférer un abonnement si l’une de ses applications tierces répond à l’un des critères suivants :

- Le compte cible est commercial et l’application est refusée pour être vendue via des partenaires.
- L’application est sélectionnée pour les partenaires sélectionnés et le compte cible ne figure pas dans la liste verte.
- L’offre était une offre préliminaire dans le passé pour les abonnements sélectionnés ou était une offre privée et l’abonnement ne figure plus dans la liste verte.
- Le nouveau compte de facturation est dans une région différente de celle où l’offre est vendue et l’offre ne doit pas être vendue dans cette région.

Un transfert bloqué reste en vigueur jusqu’à ce que vous supprimiez la ressource de l’abonnement, après quoi vous pouvez réessayer le transfert.

## <a name="next-steps"></a>Étapes suivantes

[Obtenir de l’aide pour Microsoft AppSource et la place de marché Azure](get-support.md)

