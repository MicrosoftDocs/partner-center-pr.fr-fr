---
title: Scénarios de facturation courants | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
description: Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et ceux basés sur la licence sont attribués différemment.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturation, paiements, orders, l’utilisation, facturation basée sur les licences, la date anniversaire, terme, d’annulation, renouvellement, formule prix, fichier de réconciliation, fichier rapprocher
ms.localizationpriority: medium
ms.openlocfilehash: 2a619356577345923cd78499d2ae5a1f3c6c1614
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135319"
---
# <a name="common-billing-scenarios"></a>Exemples de facturation courants

**S’applique à**

-   Facturation de programme de fournisseur de solutions de cloud

Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et ceux basés sur la licence sont affectés différemment.

## <a name="in-this-section"></a>Dans cette section

-   [Facturation basée sur l’utilisation](#usagebased)

-   [Facturation basée sur les licences](#licensebased)

## <a href="" id="usagebased"></a>Facturation basée sur l’utilisation

La facturation basée sur l’utilisation est mensuelle, à terme échu, sur le jour anniversaire d’abonnement. Par exemple, si la date anniversaire de l'abonnement est le 15 du mois, vous serez facturé le 15 janvier pour la période du service allant du 15 décembre au 14 janvier. Vous serez facturé à nouveau sur le 15 février pour la période de service le 15 janvier – 14 février, etc. Les frais sont générés sur le jour d’anniversaire d’abonnement seront affiche sur le fichier suivant de facture et de la réconciliation.

Vous remarquerez peut-être parfois que des frais d’utilisation sont manquants dans votre facture, ou que l’utilisation d’un mois précédent est facturée dans la facture du mois en cours. Il ne s’agit pas d’une erreur ; Cela signifie simplement que le service a été horodaté, une fois que les services s’est produite. Utilisation signalée dans les 24 heures de la fin du cycle de facturation apparaît sur la facture du mois suivant. 

Basée sur l’utilisation des abonnements peuvent être suspendues à tout moment. 

La liste des prix des fournisseurs de solutions Cloud Azure est publiée chaque mois et est disponible sur la page Espace partenaires de vente-> Tarification et offres. Veuillez noter que les prix sont assujettis à des modifications quotidiennes, lesquelles seront indiquées dans l'onglet Historique des modifications de la liste tarifaire.

Les frais d’utilisation sont basés sur les prix quotidiens. Si le prix change au cours de la période de service, vous verrez une ligne de facturation pour chaque période de service calculée au prorata, ainsi que le prix applicable.

## <a href="" id="licensebased"></a>Facturation basée sur les licences

**Facturation :** Abonnements basés sur les licences sont facturés à l’avance le jour d’anniversaire d’abonnement.

**Journée d’anniversaire :** Le jour de l’anniversaire est le jour du mois que vous avez acheté l’abonnement. Par exemple, si vous avez acheté l’abonnement le 15 janvier, la date anniversaire sera le 15 de chaque mois.

**Terme :** Tous les abonnements basés sur licence ont une durée de payante de 12 mois qui commence à la date d’achat.

**Annulation :** Abonnements suspendus dans mois 1 sera crédité 100 %. Les abonnements suspendus au cours des mois 2 à 12 seront crédités au prorata.

**Renouvellement :** Tous les abonnements de licence basée le renouvellement automatique pendant 12 mois après que le terme payant commence.

## <a href="" id="licensebasedmonthly"></a>Scénarios de facturation mensuels

**Scénario 1 : Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation mensuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/02/2018         |12/03/2018    |Frais de cycle   |4,00       |1        |4,00    

**Scénario 2 : Modifier le nombre de licences**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation mensuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1er février, vous ajoutez une licence supplémentaire. Le 15 février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/01/2018        |12/02/2018    |Instance de cycle au prorata   |-4,00       |1        |-4,00    
|13/01/2018         |31/01/2018    | Instance de cycle au prorata   |2,45       |1        |2,45    
|01/02/2018         |12/02/2018    | Instance de cycle au prorata   |1,55       |2        |3,10    
|13/02/2018         |12/03/2018    | Instance de cycle au prorata   |4,00       |2        |8,00    

**Formules de prix unitaire :**

Le prix mensuel est de 4,00 dollars et il y a 31 jours dans la période de service (du 13/01/2018 au 12/02/2018). Cela équivaut à un prix journalier de 0,129 (4/31).

Il y a 19 jours dans la période de prorata (du 13/01/2018 au 31/01/2018).

Prix unitaire au prorata = 2,451 = 19 x 0,129

Il y a 12 jours dans la période de prorata (du 1/02/2018 au 2/12/2018).

Prix unitaire au prorata = 1,54 = 12 x 0,129

**Scénario 3 : Suspendre avant 30 jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation mensuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/01/2018         |12/02/2018    |Frais de cycle   |4,00       |1        |4,00    

Le 1er février, vous suspendez un abonnement. Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Annuler les frais|-4,00|1|-4,00

**Scénario 4 : Suspendre après 30 jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation mensuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/02/2018|Frais de cycle|4,00|1|4,00

Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/02/2018|12/03/2018|Frais de cycle|4,00|1|4,00

Le 1er mars vous suspendez l'abonnement. Le 15 mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/03/2018|Annuler les frais|-1,72|1|-1,72

**Formules de prix unitaire :**

Le prix mensuel est de 4,00 dollars et il y a 28 jours dans la période de service (du 13/02/2018 au 12/03/2018). Cela équivaut à un prix journalier de 0,143 (4/28).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 12 jours dans la période d'annulation (du 01/03/2018 au 12/03/2018). 

Par conséquent, le prix unitaire =-1.716 (12 x 0.143 x (-1)).

## <a name="annual-billing-scenarios"></a>Scénarios de facturation annuelle

**Scénario 1 : Nouvel abonnement**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l'achat|48,00|1|48,00

**Scénario 2 : Ajouter la licence après la date d’anniversaire abonnement mais avant la date de facturation**

Vous achetez un nouvel abonnement le 11/02/2017 avec une licence pour 211,20 USD par an. L'anniversaire de votre abonnement est fixé au 11 de chaque mois. Le système de facturation de Microsoft crée les lignes de facturation suivantes : 

-   Frais de 211,20 USD pour la période du 11/02/17 au 10/02/18. 

Le 12/02/17, vous achetez une deuxième licence. Votre date de facturation est le 14/02/17. Une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes : 

|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Frais au prorata à l'achat |211,20 |1 | 211,20 |

À l'anniversaire de votre abonnement, le 11/03/17, le système de facturation Microsoft crée les lignes de facturation suivantes pour l'augmentation du nombre de licences le 12/02/17 : 
-   Crédit de -211,20 USD pour la période du 11/02/17 au 10/02/18. 
-   Frais de 0,58 USD calculés au prorata par licence pour 1 licence pour la période du 11/02/17 au 11/02/17. 
-   Frais de 15,62 USD calculés au prorata par licence pour 2 licences pour la période du 12/02/17 au 10/03/17. 
-   Frais de 195,00 USD calculés au prorata par licence pour 2 licences pour la période du 11/03/2017 au 10/02/2018. 

Le 11/02/17, vous achetez un abonnement. Le 12/02/17, vous ajoutez une licence. Votre date de facturation est le 14/02/17. Le 11/02/18, votre abonnement est renouvelé.

Votre prochaine date de facturation est le 14/03/17, et une facture et un fichier de rapprochement sont générés. Le fichier de rapprochement contient les lignes de facturation suivantes : 

|Date de début de facturation  |Date de fin de facturation  |Type de facturation  |Prix unitaire |Quantité | Montant |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Instance de cycle au prorata |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Instance de cycle au prorata |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Instance de cycle au prorata |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Instance de cycle au prorata |195,00 |2 |390,00 |

Le 11/02/18, l'abonnement est renouvelé pour une autre période de 12 mois.


**Scénario 3 : Modifier le nombre de licences**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l'achat|48,00|1|48,00

Le 1er février, vous ajoutez une licence supplémentaire. Le 15 février, le fichier de rapprochement basé sur les licences contiendra les lignes de facturation suivantes :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/01/2018|12/01/2019|Instance de cycle au prorata|-48,00|1|-48,00
13/01/2018|31/01/2018|Instance de cycle au prorata|2,47|1|2,47
01/02/2018|12/01/2019|Instance de cycle au prorata|44,98|2|89,96

**Formules de prix unitaire :**

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 19 jours dans la période de service (du 13/01/2018 au 31/01/2018). 

Par conséquent, le prix unitaire = 2,47 (19 x 0,13 x 1)

Il y a 346 jours dans la période de service (du 01/02/2018 au 12/01/2019). 

Par conséquent, le prix unitaire = 44,98 (346 x 0,13 x 2)

**Scénario 4 : Suspendre avant 30 jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l'achat|48,00|1|48,00

Le 1er février vous suspendez votre abonnement. Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Annuler les frais|-48,00|1|-48,00

**Scénario 5 : Suspendre après 30 jours**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l'achat|48,00|1|48,00

Le 15 février, le fichier de rapprochement basé sur les licences ne contiendra aucune ligne de facturation pour cet abonnement.
Le 1er mars vous suspendez votre abonnement. Le 15 mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Annuler les frais|-41,34|1|-41,34

**Formules de prix unitaire :**

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 318 jours dans la période de service (du 01/03/2018 au 12/01/2019). 

Par conséquent, le prix unitaire = 41,34 (318 x 0,13 x 1) Dans la mesure où il s'agit d'un crédit, le prix unitaire est-41,34.

**Scénario 6 : Interrompre et réactiver**

Votre date de facturation est le 15 de chaque mois. Vous achetez le 13 janvier un nouvel abonnement avec une licence pour 4 $/mois et sélectionnez une facturation annuelle. Le 15 janvier, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Frais au prorata à l'achat|48,00|1|48,00

Le 1er février vous suspendez votre abonnement. Le 15 février, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/01/2018|12/01/2019|Annuler les frais|-48,00|1|-48,00

Le 1er mars vous réactivez votre abonnement. Le 15 mars, le fichier de rapprochement basé sur les licences contiendra la ligne de facturation suivante :

|Date de début de facturation |Date de fin de facturation |Type de facturation |Prix unitaire |Quantité |Montant |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
01/03/2018|12/01/2019|Frais au prorata à l'achat|41,34|1|41,34

**Formules de prix unitaire :**

Le prix annuel est de 48,00 dollars, ce qui équivaut à un prix journalier de 0,13 (48,00/365).

Prix unitaire = jours dans la période de service x prix journalier x nombre de licences.

Il y a 318 jours dans la période de service (du 01/03/2018 au 12/01/2019). 

Par conséquent, le prix unitaire = 41,34 (318 x 0,13 x 1)
