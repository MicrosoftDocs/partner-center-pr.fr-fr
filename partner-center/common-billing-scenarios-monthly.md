---
title: Scénarios courants de facturation mensuelle
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Les scénarios courants dans l’espace partenaires lorsque vous utilisez la facturation mensuelle incluent l’ajout de nouveaux abonnements, la modification de la quantité de licences et la suspension des abonnements.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148650"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Exemples de scénarios de facturation mensuelle pour les nouveaux abonnements, modification des montants de licence ou interruptions

**Rôles appropriés**: agent admin | Administrateur de facturation | Agent du support technique | Agent des ventes

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) sont applicables si vous utilisez la facturation mensuelle dans l’espace partenaires.

## <a name="new-monthly-subscription"></a>Nouvel abonnement mensuel

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez la facturation mensuelle. Le fichier de réconciliation basé sur les licences du 15 janvier contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Frais de cycle   |4,00       |1        |4,00 |

Le fichier de rapprochement basé sur les licences du 15 février contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Frais de cycle   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Modifier le nombre de licences

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez la facturation mensuelle. Le fichier de réconciliation basé sur les licences du 15 janvier contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Frais de cycle   |4,00       |1        |4,00    |

Le 1er février, vous augmentez la quantité de licences de 1 à 2. Le fichier de rapprochement basé sur les licences du 15 février contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Instance de cycle au prorata   |-4,00       |1        |-4,00   |
|1/13/2018         |31/01/2018    | Instance de cycle au prorata   |2.45       |1        |2.45    |
|1/2/2018         |12/2/2018    | Instance de cycle au prorata   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Instance de cycle au prorata   |4,00       |2        |8,00    |

Le prix mensuel est de 4,00 et il y a 31 jours dans la période de service 1/13/2018-2/12/2018. Cela équivaut à un tarif quotidien de 0,129 (4/31).

Il y a 19 jours dans la période de proportion 1/13/2018 – 1/31/2018.

Prix unitaire de proportion = 2,451 = 19 x 0,129

Il y a 12 jours dans la période de proportisation 2/1/2018 – 2/12/2018.

Prix unitaire de proportion = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspendre avant 30 jours

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez la facturation mensuelle. Le fichier de réconciliation basé sur les licences du 15 janvier contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Frais de cycle   |4,00       |1        |4,00    |

Le 1er février, vous suspendez un abonnement. Le fichier de rapprochement basé sur les licences du 15 février contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Annuler les frais|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspendre après 30 jours

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez la facturation mensuelle. Le fichier de réconciliation basé sur les licences du 15 janvier contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Frais de cycle|4,00|1|4,00

Le fichier de rapprochement basé sur les licences du 15 février contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Frais de cycle|4,00|1|4,00

Le 1er mars, vous suspendez l’abonnement. Le fichier de rapprochement basé sur les licences du 15 mars contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Annuler les frais|-1,72|1|-1,72

Le prix mensuel est de 4,00 et il y a 28 jours dans la période de service 2/13/2018-3/12/2018. Cela équivaut à un tarif quotidien de 0,143 (4/28).

Prix unitaire = jours de la période de service x cours journalier x nombre de licences.

Il y a 12 jours dans la période d’annulation 3/1/2018 – 3/12/2018.

Par conséquent, le prix unitaire =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Étapes suivantes

- [Scénarios de facturation pour une période unique et sélection des achats récurrents](common-billing-scenarios-onetime-recurring.md)