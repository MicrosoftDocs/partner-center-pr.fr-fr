---
title: Scénarios de facturation courants | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Scénarios de facturation courants dans l’espace partenaires pour la facturation annuelle (par exemple, l’ajout de nouveaux abonnements, l’ajout de licences avant la date de facturation, la modification de la quantité de licences et la suspension et la réactivation des abonnements).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturation, paiements, commandes, utilisation, facturation basée sur la licence, date anniversaire, terme, annulation, renouvellement, formule prix, fichier de rapprochement, fichier de rapprochement
ms.localizationpriority: medium
ms.openlocfilehash: 91b8e318e2122f9510b160339984cc0743c318ee
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389627"
---
# <a name="annual-billing-scenarios"></a>Scénarios de facturation annuelle

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) sont applicables si vous utilisez la facturation annuelle dans l’espace partenaires.

## <a name="new-annual-subscription"></a>Nouvel abonnement annuel

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l’achat|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Ajouter une licence après la date anniversaire de l’abonnement, mais avant la date de facturation

Vous achetez un nouvel abonnement le 11/02/2017 avec une licence pour 211,20 USD par an. L'anniversaire de votre abonnement est fixé au 11 de chaque mois. Le système de facturation de Microsoft crée les lignes de facturation suivantes :

- Frais de 211,20 USD pour la période du 11/02/17 au 10/02/18.

Le 12/02/17, vous achetez une deuxième licence. Votre date de facturation est le 14/02/17. Une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes :

|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Frais au prorata à l'achat |211,20 |1 | 211,20 |

À l'anniversaire de votre abonnement, le 11/03/17, le système de facturation Microsoft crée les lignes de facturation suivantes pour l'augmentation du nombre de licences le 12/02/17 :

- $211,20 crédit pour la période 2/11/17-2/10/18.
- Frais de 0,58 USD calculés au prorata par licence pour 1 licence pour la période du 11/02/17 au 11/02/17.
- Frais de 15,62 USD calculés au prorata par licence pour 2 licences pour la période du 12/02/17 au 10/03/17.
- Frais de 195,00 USD calculés au prorata par licence pour 2 licences pour la période du 11/03/2017 au 10/02/2018.

Le 11/02/17, vous achetez un abonnement. Le 12/02/17, vous ajoutez une licence. Votre date de facturation est le 14/02/17. Le 11/02/18, votre abonnement est renouvelé.

Votre prochaine date de facturation est le 14/03/17, et une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes :

|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Instance de cycle au prorata |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Instance de cycle au prorata |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Instance de cycle au prorata |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Instance de cycle au prorata |195,00 |2 |390,00 |

Le 11/02/18, l'abonnement est renouvelé pour une autre période de 12 mois.

## <a name="change-license-quantity"></a>Modifier le nombre de licences

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février, vous ajoutez une licence supplémentaire. Le 15 février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Instance de cycle au prorata|-48,00|1|-48,00
13/01/2018|31/01/2018|Instance de cycle au prorata|2,47|1|2,47
01/02/2018|12/01/2019|Instance de cycle au prorata|44,98|2|89,96

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 19 jours dans la période de service (du 13/01/2018 au 31/01/2018).

Par conséquent, le prix unitaire = 2,47 (19 x 0,13 x 1)

Il y a 346 jours dans la période de service (du 01/02/2018 au 12/01/2019).

Par conséquent, le prix unitaire = 44,98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Suspendre avant 30 jours

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février vous suspendez votre abonnement. Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Annuler les frais|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Suspendre après 30 jours

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 15 février, le fichier de rapprochement basé sur les licences ne contiendra aucune ligne de facturation pour cet abonnement.
Le 1er mars vous suspendez votre abonnement. Le 15 mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Annuler les frais|-41,34|1|-41,34

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 318 jours dans la période de service (du 01/03/2018 au 12/01/2019).

Par conséquent, le prix unitaire = 41,34 (318 x 0,13 x 1) Dans la mesure où il s'agit d'un crédit, le prix unitaire est-41,34.

## <a name="suspend-and-reactivate"></a>Interrompre et réactiver

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février vous suspendez votre abonnement. Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Annuler les frais|-48,00|1|-48,00

Le 1er mars vous réactivez votre abonnement. Le 15 mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Frais au prorata à l’achat|41,34|1|41,34

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 318 jours dans la période de service (du 01/03/2018 au 12/01/2019).

Par conséquent, le prix unitaire = 41,34 (318 x 0,13 x 1)
