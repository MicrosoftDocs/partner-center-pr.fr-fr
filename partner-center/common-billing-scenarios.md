---
title: "Scénarios de facturation courants | Espace partenaires"
description: "Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et les abonnements basés sur la licence sont affectés différemment."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 2ed2dded5f96c5f3887cd40db04cd21e548efe5f
ms.sourcegitcommit: 6d8b97724a100fc6861e9ed8d89ec47cc49f195e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/17/2017
---
# <a name="common-billing-scenarios"></a>Scénarios de facturation courants

**S'applique à**

-  Espace partenaires
-  Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis
-  Espace partenaires de MicrosoftCloud Allemagne

Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et ceux basés sur la licence sont affectés différemment.

## <a name="in-this-section"></a>Dans cette section

-   [Facturation basée sur l’utilisation](#usagebased)

-   [Facturation basée sur la licence](#licensebased)

## <a href="" id="usagebased"></a>Facturation basée sur l’utilisation

Seuls les services utilisés dans la période de facturation précédente vous sont facturés. Les services et applications Azure qui sont activés et utilisés pendant la période de facturation apparaissent sur la facture.

-   Les barèmes des services peuvent changer au cours du cycle de facturation.
    -   Augmentation de prix: préavis de 30jours.
    -   Les réductions de prix s’appliquent à compter du jour où elles prennent effet.
    -   Les abonnements existants sont facturés au taux en vigueur au début du cycle de facturation.
    -   Les nouveaux abonnements (créés au cours du cycle de facturation) sont facturés au taux en vigueur lorsque vous les avez ajoutés.
-   Si vous annulez un abonnement au cours du premier cycle de facturation, les frais d’utilisation apparaissent dans le fichier de rapprochement de la période pendant laquelle l’abonnement était actif.

## <a href="" id="licensebased"></a>Facturation basée sur la licence

**Facturation:** les abonnements basés sur la licence sont facturés à l’avance sur le jour anniversaire d’abonnement.

**Jour anniversaire:** les abonnements à facturation mensuelle sont alignés sur la date de facturation du partenaire et les abonnements à facturation annuelle sont alignés sur la date d'achat.

**Période gratuite:** les abonnements à facturation mensuelle bénéficient d'une période gratuite à partir de la date d’achat jusqu'à la date de facturation suivante du partenaire.

**Période d'abonnement:** tous les abonnements basés sur la licence sont souscrits pour une période de 12mois. La période d'abonnement commence à la date d’achat pour les abonnements à facturation annuelle et à la date de facturation suivant la date d’achat pour les abonnements à facturation mensuelle.

**Annulation:** les abonnements annulés dans les 30premiersjours de la période d'abonnement seront crédités à 100%. Les abonnements annulés après 30jours seront crédités au prorata.

**Renouvellement:** tous les abonnements basés sur la licence sont automatiquement renouvelés 12mois après le début de la période d'abonnement.

## <a href="" id="licensebasedmonthly"></a>Scénarios de facturation mensuelle

**Scénario1: Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         | 14/01/2018   |Frais d’abonnement   |0,00       |1       |0,00    
|15/01/2018         |14/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/02/2018         |14/03/2018    |Frais de cycle   |4,00       |1        |4,00    
Vous continuerez à être facturé le 15 de chaque mois jusqu'à ce que l’abonnement soit suspendu.

**Scénario 2: Modification du nombre de licences**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Frais d’abonnement   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1erfévrier, vous ajoutez une licence supplémentaire. Le 15février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/01/2018        |14/02/2018    |Instance de cycle au prorata   |-4,00       |1        |4,00    
|15/01/2018         |31/01/2018    | Instance de cycle au prorata   |2,21       |1        |2,21    
|01/02/2018         |14/02/2018    | Instance de cycle au prorata   |1,82       |2        |3,64    
|15/02/2018         |14/03/2018    | Instance de cycle au prorata   |4,00       |2        |8,00    

**Formules pour le prix unitaire:**

Le prix mensuel est de 4,00dollars et il y a 31jours dans la période de service (du 15/01/2018 au 14/02/2018). Cela équivaut à un prix journalier de 0,13 (4/31).

Il y a 17jours dans la période de prorata (du 15/01/2018 au 31/01/2018).

Prix unitaire au prorata=2,21=17x0,13

Il y a 14jours dans la période de prorata (du 01/02/2018 au 14/02/2018).

Prix unitaire au prorata=1,82=14x0,13

**Scénario3:Suspension avant 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |14/01/2018    |Frais d’abonnement   |0,00       |1        |0,00    
|15/01/2018         |14/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1erfévrier vous suspendez l'abonnement. Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/01/2018|14/02/2018|Frais d'annulation|-4,00|1|4,00

**Scénario4:Suspension après 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation mensuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|14/01/2018|Frais d’abonnement|0,00|1|0,00
15/01/2018|14/02/2018|Frais de cycle|4,00|1|4,00

Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/02/2018|14/03/2018|Frais de cycle|4,00|1|4,00

Le 1ermars vous suspendez l'abonnement. Le 15mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|14/03/2018|Frais d'annulation|-1,96|1|-1,96

**Formules pour le prix unitaire:**

Le prix mensuel est de 4,00dollars et il y a 28jours dans la période de service (du 15/02/2018 au 14/03/2018). Cela équivaut à un prix journalier de 0,14 (4/28).

Prix unitaire=jours dans la période de servicexprix journalier xnombre de licences.

Il y a 14jours dans la période d'annulation (du 01/03/2018 au 14/03/2018). 

Par conséquent, le prix unitaire=-1,96 (14x0,14x(-1)).

## <a name="annual-billing-scenarios"></a>Scénarios de facturation annuelle

**Scénario1: Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

**Scénario 2: Modification du nombre de licences**

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

**Scénario3:Suspension avant 30jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13janvier un nouvel abonnement avec une licence pour 4$/mois et sélectionnez une facturation annuelle. Le 15janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata en cas d’achat|48,00|1|48,00

Le 1erfévrier vous suspendez votre abonnement. Le 15février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante:
|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais d'annulation|-48,00|1|-48,00

**Scénario4:Suspension après 30jours**

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

Par conséquent, le prix unitaire=41,34(318x0,13x1) Dans la mesure où il s’agit d’un crédit, le prix unitaire est-41,34.

**Scénario 5: Suspension et réactivation**

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

