---
title: Scénarios de facturation courants | Espace partenaires
description: Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et les abonnements basés sur la licence sont affectés différemment.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: 9757b3c4cc03ea26744f995e4931c94952de2a10
ms.sourcegitcommit: 082795279b2beb9cecee3072cbabe584cfda1b9c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/21/2018
ms.locfileid: "4121114"
---
# <a name="common-billing-scenarios"></a>Scénarios de facturation courants

**S'applique à**

-   Facturation de programme de fournisseur de solutions cloud

Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et ceux basés sur la licence sont affectés différemment.

## <a name="in-this-section"></a>Dans cette section

-   [Facturation basée sur l’utilisation](#usagebased)

-   [Facturation basée sur la licence](#licensebased)

## <a href="" id="usagebased"></a>Facturation basée sur l’utilisation

La facturation basée sur l’utilisation est mensuelle, à terme échu, sur le jour anniversaire d’abonnement. Par exemple, si la date anniversaire de l'abonnement est le 15 du mois, vous serez facturé le 15 janvier pour la période du service allant du 15 décembre au 14 janvier. Vous serez facturé à nouveau le 15 février pour la période de service allant du 15 janvier au 14 février, etc. Les frais générés le jour de la date anniversaire de l'abonnement apparaîtront sur la facture et le fichier de rapprochement du mois suivant.

Un abonnement basé sur l’utilisation peut être interrompu à tout moment. 

La liste des prix des fournisseurs de solutions Cloud Azure est publiée chaque mois et est disponible sur la page Espace partenaires de vente-> Tarification et offres. Veuillez noter que les prix sont assujettis à des modifications quotidiennes, lesquelles seront indiquées dans l'onglet Historique des modifications de la liste tarifaire.

Les frais d’utilisation sont basés sur les prix quotidiens. Si le prix change au cours de la période de service, vous verrez une ligne de facturation pour chaque période de service calculée au prorata, ainsi que le prix applicable.

## <a href="" id="licensebased"></a>Facturation basée sur la licence

**Facturation:** les abonnements basés sur la licence sont facturés à l’avance sur le jour anniversaire d’abonnement.

**Date anniversaire:** la date anniversaire est le jour du mois où vous avez acheté l’abonnement. Par exemple, si vous avez acheté l’abonnement le 15 janvier, la date anniversaire sera le 15 de chaque mois.

**Période d'abonnement:** tous les abonnements basés sur la licence sont souscrits pour une période de 12mois, qui débute à la date d'achat.

**Annulation:** les abonnements suspendus durant le mois 1 seront crédité à 100%. Les abonnements suspendus au cours des mois 2 à 12 seront crédités au prorata.

**Renouvellement:** tous les abonnements basés sur la licence sont automatiquement renouvelés 12mois après le début de la période d'abonnement.

## <a href="" id="licensebasedmonthly"></a>Scénarios de facturation mensuelle

**Scénario1: Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Frais de cycle   |4,00       |1        |4,00    

**Scénario 2: Modification du nombre de licences**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1erfévrier, vous ajoutez une licence supplémentaire. Le 15février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Instance de cycle au prorata   |-4,00       |1        |-4,00    
|13/01/2018         |31/01/2018    | Instance de cycle au prorata   |2,45       |1        |2.45    
|01/02/2018         |12/02/2018    | Instance de cycle au prorata   |1,55       |2        |3,10    
|13/02/2018         |12/03/2018    | Instance de cycle au prorata   |4,00       |2        |8,00    

**Formules pour le prix unitaire:**

Le prix mensuel est de 4,00dollars et il y a 31jours dans la période de service (du 13/01/2018 au 12/02/2018). Cela équivaut à un prix journalier de 0,129 (4/31).

Il y a 19jours dans la période de prorata (du 13/01/2018 au 31/01/2018).

Prix unitaire au prorata=2,451=19x0,129

Il y a 12jours dans la période de prorata (du 1/02/2018 au 2/12/2018).

Prix unitaire au prorata=1,54=12x0,129

**Scénario3:Suspension avant 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1er février vous suspendez un abonnement. Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Frais d'annulation|-4,00|1|-4,00

**Scénario4:Suspension après 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Frais de cycle|4,00|1|4,00

Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Frais de cycle|4,00|1|4,00

Le 1ermars vous suspendez l'abonnement. Le 15mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Frais d'annulation|-1,72|1|-1,72

**Formules pour le prix unitaire:**

Le prix mensuel est de 4,00dollars et il y a 28jours dans la période de service (du 13/02/2018 au 12/03/2018). Cela équivaut à un prix journalier de 0,143 (4/28).

Prix unitaire=jours dans la période de servicexprix journalier xnombre de licences.

Il y a 12jours dans la période d'annulation (du 01/03/2018 au 12/03/2018). 

Par conséquent, le prix unitaire = -1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Scénarios de facturation annuelle

**Scénario1: Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

**Scénario2: Ajouter une licence après la date d'anniversaire de l'abonnement mais avant la date de facturation**

Vous achetez un nouvel abonnement le 11/02/2017 avec unelicence pour 211,20USD par an. L'anniversaire de votre abonnement est fixé au 11 de chaque mois. Le système de facturation de Microsoft crée les lignes de facturation suivantes: 

-   Frais de 211,20USD pour la période du 11/02/17 au 10/02/18. 

Le 12/02/17, vous achetez une deuxième licence. Votre date de facturation est le 14/02/17. Une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes: 
|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Frais au prorata à l'achat |211,20 |1 | 211,20 |
 
À l'anniversaire de votre abonnement, le 11/03/17, le système de facturation Microsoft crée les lignes de facturation suivantes pour l'augmentation du nombre de licences le 12/02/17: 
-   Crédit de -211,20USD pour la période du 11/02/17 au 10/02/18. 
-   Frais de 0,58USD calculés au prorata par licence pour 1licence pour la période du 11/02/17 au 11/02/17. 
-   Frais de 15,62USD calculés au prorata par licence pour 2licences pour la période du 12/02/17 au 10/03/17. 
-   Frais de 195,00USD calculés au prorata par licence pour 2licences pour la période du 11/03/2017 au 10/02/2018. 
 
Le 11/02/17, vous achetez un abonnement. Le 12/02/17, vous ajoutez une licence. Votre date de facturation est le 14/02/17. Le 11/02/18, votre abonnement est renouvelé.

Votre prochaine date de facturation est le 14/03/17, et une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes: 
|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Instance de cycle au prorata |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Instance de cycle au prorata |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Instance de cycle au prorata |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Instance de cycle au prorata |195,00 |2 |390,00 |
 
Le 11/02/18, l'abonnement est renouvelé pour une autre période de 12mois.


**Scénario 3: Modification du nombre de licences**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

Le 1erfévrier, vous ajoutez une licence supplémentaire. Le 15février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Instance de cycle au prorata|-48,00|1|-48,00
13/01/2018|31/01/2018|Instance de cycle au prorata|2,47|1|2,47
01/02/2018|12/01/2019|Instance de cycle au prorata|44,98|2|89,96

**Formules pour le prix unitaire:**

Le prix annuel est de 48,00dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire=jours dans la période de servicexprix journalierxnombre de licences.

Il y a 19jours dans la période de service (du 13/01/2018 au 31/01/2018). 

Par conséquent, le prix unitaire=2,47(19x0,13x1)

Il y a 346jours dans la période de service (du 01/02/2018 au 12/01/2019). 

Par conséquent, le prix unitaire=44,98(346x0,13x2)

**Scénario4:Suspension avant 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

Le 1erfévrier vous suspendez votre abonnement. Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais d'annulation|-48,00|1|-48,00

**Scénario5:Suspension après 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

Le 15février, le fichier de rapprochement basé sur les licences ne contiendra aucune ligne de facturation pour cet abonnement.
Le 1ermars vous suspendez votre abonnement. Le 15mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Frais d'annulation|-41,34|1|-41,34

**Formules pour le prix unitaire:**

Le prix annuel est de 48,00dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire=jours dans la période de servicexprix journalier xnombre de licences.

Il y a 318jours dans la période de service (du 01/03/2018 au 12/01/2019). 

Par conséquent, le prix unitaire=41,34(318x0,13x1) Dans la mesure où il s'agit d'un crédit, le prix unitaire est -41,34.

**Scénario 6: Suspension et réactivation**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

Le 1erfévrier vous suspendez votre abonnement. Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais d'annulation|-48,00|1|-48,00

Le 1ermars vous réactivez votre abonnement. Le 15mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Frais au prorata en cas d’achat|41,34|1|41,34

**Formules pour le prix unitaire:**

Le prix annuel est de 48,00dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire=jours dans la période de servicexprix journalier xnombre de licences.

Il y a 318jours dans la période de service (du 01/03/2018 au 12/01/2019). 

Par conséquent, le prix unitaire=41,34(318x0,13x1)
