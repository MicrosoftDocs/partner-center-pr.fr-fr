---
title: Facturation annuelle-scénarios courants
ms.topic: article
ms.date: 05/05/2020
description: 'Facturation annuelle de l’espace partenaires : lorsque vous ajoutez de nouveaux abonnements, ajoutez des licences avant la date de facturation, modifiez le nombre de licences ou suspend/réactivez les abonnements.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 086a7d359e1b903684af4ecddac37eda584e55f8
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435458"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Scénarios courants de facturation annuelle dans l’espace partenaires

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Agent du support technique
- Agent commercial

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) sont applicables si vous utilisez la facturation annuelle dans l’espace partenaires.

## <a name="new-annual-subscription"></a>Nouvel abonnement annuel

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez facturation annuelle. Le fichier de réconciliation basé sur une licence du 15 janvier contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Frais au prorata à l’achat|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Ajouter une licence après la date anniversaire de l’abonnement, mais avant la date de facturation

Vous achetez un nouvel abonnement sur 2/11/17 avec une licence pour $211.20/year. Votre anniversaire d’abonnement est défini comme le 11 de chaque mois. Le système de facturation Microsoft crée les lignes de facturation suivantes :

- Frais de 211,20 USD pour la période du 11/02/17 au 10/02/18.

Le 2/12/17, vous achetez une deuxième licence. La date de facturation est 2/14/17. Un fichier de facture et de rapprochement sont générés. Le fichier de réconciliation contient les lignes de facturation suivantes :

|Date de début de facturation  |Date de fin de la facturation  |Type de frais  |Unit Price |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Frais au prorata à l'achat |211,20 |1 | 211,20 |

À la date anniversaire de votre abonnement, 3/11/17, le système de facturation Microsoft crée les lignes de facturation suivantes pour l’augmentation de la licence sur 2/12/17 :

- $211,20 crédit pour la période 2/11/17-2/10/18.
- $0,58 facturation au prorata par licence pour 1 licence pour la période 2/11/17-2/11/17.
- $15,62 facturation au prorata par licence pour 2 licences pour la période 2/12/17-3/10/2017.
- $195,00 facturation au prorata par licence pour 2 licences pour la période 3/11/2017-2/10/2018.

Le 2/11/17, vous achetez un abonnement. Le 2/12/17, vous ajoutez une licence. La date de facturation est 2/14/17. Le 2/11/18, votre abonnement renouvelle.

La prochaine date de facturation est le 3/14/17 et une facture & fichier de rapprochement sont générés. Le fichier de réconciliation contient les lignes de facturation suivantes :

|Date de début de facturation  |Date de fin de la facturation  |Type de frais  |Unit Price |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Instance de cycle au prorata |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Instance de cycle au prorata |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Instance de cycle au prorata |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Instance de cycle au prorata |195,00 |2 |390,00 |

Le 2/11/18, l’abonnement renouvelle pour une durée de 12 mois.

## <a name="change-license-quantity"></a>Modifier le nombre de licences

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez facturation annuelle. Le fichier de réconciliation basé sur une licence du 15 janvier contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février, vous augmentez la quantité de licences de 1 à 2. Le fichier de rapprochement basé sur une licence du 15 février contient les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Instance de cycle au prorata|-48,00|1|-48,00
1/13/2018|31/01/2018|Instance de cycle au prorata|2.47|1|2.47
1/2/2018|1/12/2019|Instance de cycle au prorata|44,98|2|89,96

Le prix annuel est de 48,00, ce qui équivaut au tarif quotidien de 0,13 (48.00/365).

Prix unitaire = jours de la période de service x cours journalier x nombre de licences.

Il y a 19 jours dans la période de service 1/13/2018 – 1/31/2018.

Par conséquent, le prix unitaire est égal à 2,47 (19X 0,13 x1)

La période de service 2/1/2018-1/12/2019 contient 346 jours.

Par conséquent, le prix unitaire est égal à 44,98 (346x 130 x2)

## <a name="suspend-before-30-days"></a>Suspendre avant 30 jours

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez facturation annuelle. Le fichier de réconciliation basé sur une licence du 15 janvier contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février, vous suspendez votre abonnement. Le fichier de rapprochement basé sur une licence du 15 février contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Annuler les frais|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Suspendre après 30 jours

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez facturation annuelle. Le fichier de réconciliation basé sur une licence du 15 janvier contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Frais au prorata à l’achat|48,00|1|48,00

Le fichier de rapprochement basé sur une licence du 15 février ne contient aucune ligne de facturation pour cet abonnement.
Le 1er mars, vous suspendez votre abonnement. Le fichier de réconciliation basé sur une licence du 15 mars contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Annuler les frais|-41,34|1|-41,34

Le prix annuel est de 48,00, ce qui équivaut au tarif quotidien de 0,13 (48.00/365).

Prix unitaire = jours de la période de service x cours journalier x nombre de licences.

La période de service 3/1/2018-1/12/2019 contient 318 jours.

Par conséquent, le prix unitaire est égal à 41,34 (318x 0,13 x1). Étant donné qu’il s’agit d’un crédit, le prix unitaire est-41,34.

## <a name="suspend-and-reactivate"></a>Interrompre et réactiver

La date de facturation est le 15 de chaque mois. Le 13 janvier, vous achetez un nouvel abonnement avec une licence de $4/mois et sélectionnez facturation annuelle. Le fichier de réconciliation basé sur une licence du 15 janvier contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Frais au prorata à l’achat|48,00|1|48,00

Le 1er février, vous suspendez votre abonnement. Le fichier de rapprochement basé sur une licence du 15 février contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Annuler les frais|-48,00|1|-48,00

Le 1er mars, vous réactivez votre abonnement. Le fichier de réconciliation basé sur une licence du 15 mars contient la ligne de facturation suivante :

|Date de début de facturation |Date de fin de la facturation |Type de frais |Unit Price |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Frais au prorata à l’achat|41,34|1|41,34

Le prix annuel est de 48,00, ce qui équivaut au tarif quotidien de 0,13 (48.00/365).

Prix unitaire = jours de la période de service x cours journalier x nombre de licences.

La période de service 3/1/2018-1/12/2019 contient 318 jours.

Par conséquent, le prix unitaire est égal à 41,34 (318x 0,13 x1).
