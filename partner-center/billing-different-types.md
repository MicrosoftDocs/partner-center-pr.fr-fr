---
title: Présentation des types de facturation dans l’Espace partenaires | Espace partenaires
ms.topic: article
ms.date: 03/01/2019
Description: Informations relatives aux différents types de facturation, périodes de facturation et dates de facturation
author: MaggiePucciEvans
ms.author: evansma
keywords: facturation, paiements, commandes, fichiers de rapprochement, fichier de rapp
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 38ad28fb74968d351d6031e21446f02d22f7e4fa
ms.sourcegitcommit: ba0b0eea3dbc028ec162f58b841ba9e3588f1dca
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/29/2019
ms.locfileid: "70134620"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Présentation des types de facturation dans l’Espace partenaires

**S’applique à**

-  Espace partenaires
-  Partenaires du programme Fournisseur de solutions Microsoft Cloud

Selon les types de produits que vous achetez pour vos clients, vous pouvez constater des périodes de facturation distinctes et être facturé à des jours différents du même mois. Cet article détaille ce qui a changé depuis le 1er mars 2019 et en quoi ces changements vous affectent.

## <a name="billing-for-recurring-charges"></a>Facturation des frais récurrents

L’expérience de facturation des frais récurrents liés aux abonnements basés sur une licence et sur l’utilisation ne change pas. Nous continuons de vous facturer le jour du mois que vous avez sélectionné comme date de facturation et votre période de facturation continue d'être le mois précédant cette date. Si vous avez sélectionné le 15 du mois comme date de facturation, vous êtes facturé pour toutes les activités du 15 du mois civil au 14 du mois civil suivant. Les factures et fichiers de rapprochement sont généralement disponibles 2 à 4 jours après la date de facturation.

Comme précédemment, nous vous facturons ces produits dans la devise du pays ou de la région où vous vous trouvez, quel que soit l'endroit où se trouve le client auquel vous avez vendu le produit.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturation ponctuelle et frais récurrents

Depuis le 1er mars 2019, nous avons introduit une nouvelle expérience de facturation pour les frais récurrents et ponctuels correspondants aux produits ISV Microsoft et tiers.

Pour ces produits, la période de facturation commence le premier jour du mois civil et se termine le dernier jour du mois civil. Votre facture est disponible le huitième jour du mois suivant. 

En d’autres termes, toutes les transactions effectuées entre le 1er mai et le 31 mai 2019 apparaissent sur votre facture le 8 juin. Toutes les transactions que vous effectuez entre le 1er et le 30 juin 2019 apparaissent sur votre facture le 8 juillet. Vous pouvez être facturé pour des achats récurrents et ponctuels sur la même facture. 

Vous pouvez également consulter le solde/la facture de votre compte chaque fois que vous le souhaitez (par exemple, entre le 1er mai et le 7 juin) et voir l’activité récente du compte sans devoir attendre la facture. Notez que lorsque nous publions votre facture le 8, elle inclut les taxes et autres frais et crédits applicables et dès lors, le montant final peut différer de ce qui s'affiche au cours de la période de facturation. 

Vous accédez à vos factures comme précédemment, dans l’Espace partenaires ou via l'API. Elles apparaissent avant minuit (UTC) le 8 du mois. 

|**Expérience de facturation**|**Type(s) de produit**|**Date de facturation**|**Période de facturation**|**Devise de facturation**|**Activité actuelle disponible ?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Frais récurrents des abonnements basés sur la licence et l’utilisation |Tous les produits du [catalogue de services en ligne](https://partner.microsoft.com/commerce/preferredoffers/list). Exemples : Office 365, Microsoft 365, Azure Active Directory, Azure (paiement à l’utilisation), Dynamics 365, PowerBI Pro |Date que vous avez sélectionnée lors de la création de votre compte Espace partenaires |Mois précédant votre date de facturation. |Devise du pays ou de la région où vous vous trouvez. Par exemple, si votre entreprise est située au Royaume-Uni, nous vous facturons en livres sterling (GBP). Si votre entreprise est située en Inde, nous vous facturerons en roupies indiennes (INR).  |Non |
|Frais récurrents et ponctuels pour les produits ISV Microsoft et tiers |Tous les abonnements SaaS, réservations Azure et produits logiciels (perpétuels et basés sur un abonnement) proposés par Microsoft et des éditeurs de logiciels indépendants. Consultez les produits disponibles sur la [Place de marché](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). À titre d'exemple, le logiciel SUSE Linux (abonnement logiciel), Windows Server 2019 Essentials (logiciel perpétuel) et l’abonnement au produit Azure ISV SaaS y figurent. |Le 8 de chaque mois |Du premier au dernier jour de chaque mois civil |Devise du pays/région où se trouve votre client. Vous recevez des factures et fichiers de rapprochement distincts dans la devise du pays ou de la région de chaque client auquel vous avez vendu un produit au cours de la période de facturation. |Oui |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Scénarios de facturation des achats ponctuels et périodiques
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scénario 1 - Acheter un abonnement, puis ajouter un siège le même jour

Dans le scénario 1, vous achetez un abonnement le 11 juin à un prix unitaire de 4 $. Plus tard dans la journée, vous achetez un autre abonnement au même tarif. 

Le fichier de rapprochement inclut les éléments suivants : 
-   Facture de 4 $ pour la période de service du 10 juin au 9 juillet. 
-   Refacturation au prorata de 4 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 1 = 4,00.
-   Refacturation au prorata de 8 $ pour la période de service du 10 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 30 x 2 = 8,00.

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |1                 |4 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -4 $       |addQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |8 $         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Scénario 2 - Acheter un abonnement, puis en ajouter ultérieurement d'autres

Dans le scénario 2, vous achetez un abonnement le 11 juin à un prix unitaire de $4 et le 12 juin, vous en achetez un autre pour le même produit au même prix. 

Le fichier de rapprochement inclut les éléments suivants : 
-   Facture de 4 $ pour la période de service du 10 juin au 9 juillet. 
-   Refacturation au prorata de -3,87 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 1 = 3,87.
-   Refacturation au prorata de 7,74 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (4/30) x 29 x 2 = 7,74.

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez une licence)     |10/06/2019   |09/07/2019         |4 $         |1        |4 $            |Nouveau         |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |1        | -3,87 $       |addQuantity           |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 2      |7,74 $       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scénario 3 - Acheter un abonnement, puis supprimer un siège le même jour

Dans le scénario 3, vous achetez deux abonnements pour le même produit le 11 juin à un prix unitaire de $4. Plus tard dans la journée, vous supprimez l’un des sièges.  

Le fichier de rapprochement inclut les éléments suivants : 
-   Facture de 8 $ pour deux licences pour la période de service du 10 juin au 9 juillet. 
-   Refacturation au prorata de 8 $ pour la période de service du 11 juin au 11 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 30 x 2 = 8,00.
-   Refacturation au prorata de 4 $ pour la période de service du 11 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 30 x 1 = 4,00.

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019      |10/06/2019   |09/07/2019         |4 $                |2                 |8 $            |Nouveau         |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -8 $       |removeQuantity           |
|11/06/2019     | 10/06/2019    |09/07/2019        |4 $        | 1      |4 $         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Scénario 4 - Acheter un abonnement, puis supprimer ultérieurement des sièges

Dans le scénario 4, vous achetez 2 abonnements le 11 juin à un prix unitaire de 4 $, puis le 12 juin, vous supprimez l’un des sièges. 

Le fichier de rapprochement inclut les éléments suivants : 
-   Facture de 8 $ pour la période de service du 10 juin au 9 juillet. 
-   Refacturation au prorata de -7,74 $ pour la période de service du 11 juin au 12 juin. Il s’agit de la période au cours de laquelle vous aviez 2 licences. Calcul = (prix mensuel/total des jours dans la période de service) x jours dans la période de service au prorata x nombre de licences = (4/30) x 29 x 2 = 7,74.
-   Refacturation au prorata de 3,87 $ pour la période de service du 12 juin au 9 juillet. Il s’agit de la période au cours de laquelle vous aviez 1 licence. Calcul = (4/30) x 29 x 1 = 3,87.

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/06/2019 (vous avez 2 licences)     |10/06/2019   |09/07/2019         |4 $         |2        |8 $       |Nouveau       |
|12/06/2019     | 10/06/2019    |09/07/2019        |4 $        |2        | -7,74 $       |removeQuantity           |
|12/06/2019 (vous avez 1 licence)    | 10/06/2019    |09/07/2019   |4 $    |1      |3,87 $    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Scénarios de facturation liés aux transactions SaaS basées sur une licence d’essai gratuit
### <a name="scenario-5--renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Scénario 5 - Renouveler un abonnement SaaS basé sur une licence d'essai gratuit vers un abonnement payant au terme de la période d’essai gratuite

Dans ce scénario, vous achetez un abonnement SaaS (software as a service) basé sur une licence d’essai gratuit le 10 juin et celui-ci est automatiquement renouvelé en tant qu’abonnement payant au terme de la période d'essai gratuite. 

Les fichiers de rapprochement incluent les éléments suivants : 
- Facture de 0 $ pour la période de service du 10 juin au 9 juillet 
- Facture de 2 $ pour la période de service du 10 juillet au 9 août

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/06/2019 (vous avez 1 licence)      |10/06/2019   |09/07/2019         |0 $                |1                 |0 $            |Nouveau         |
|10/07/2019 (vous avez 1 licence)     | 10/07/2019    |09/08/2019        |2 $        |1        | 2 $       |renouveler           |

### <a name="scenario-6--cancel-a-license-based-free-trial-saas-subscription"></a>Scénario 6 - Annuler un abonnement SaaS basé sur une licence d'essai gratuit

À tout moment, vous pouvez annuler un abonnement SaaS (software as a service) basé sur une licence d'essai gratuit, même pendant la période d’essai gratuite. 

Dans ce scénario, vous achetez un abonnement SaaS basé sur une licence d'essai gratuit le 1er juillet, puis l’annulez immédiatement dans l’Espace partenaires. 

Le fichier de rapprochement inclut les éléments suivants : 
- Facture de 0 $ pour la période de service du 10 juin au 9 juillet pour le nouvel achat
- Facture de 0 $ pour la période de service du 10 juin au 9 juillet pour l'annulation

|**Date d’achat**   |**Début de facturation**  |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/06/2019 (vous 11 licences)      |10/06/2019   |09/07/2019         |0 $                |11                |0 $            |Nouveau         |
|10/06/2019 (vous n’avez aucune licence)     | 10/06/2019    |09/07/2019        |0 $        |11       | 0 $       |annuler           |

### <a name="scenario-7--convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Scénario 7 - Convertir un abonnement SaaS avec personnalisé d'une référence SKU à une autre pour le même produit le même jour

Dans ce scénario, vous achetez une référence SKU (Silver) sous un produit et la convertissez en une autre référence SDK (Bronze) disponible sous ce produit le même jour. 

Le fichier de rapprochement inclut les éléments suivants : 
- Facture Silver de 0 $ pour la période de service du 10 juin 2019 au 9 juillet 2020
- Refacturation Silver de 20 $ pour la période de service du 10 juin 2019 au 9 juillet 2020
- Facture Bronze de 0 $ pour la période de service du 10 juin 2019 au 9 juillet 2020

|**Date d’achat**   |**Référence SKU**   |**Début de facturation**   |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/06/2019 (vous avez 1 licence) |Silver     |10/06/2019   |10/06/2019         |20 $        |1         |20 $            |Nouveau      |
|10/06/2019 (vous avez 1 licence) |Silver    | 10/06/2019    |10/06/2019        |20 $        |1       | -20 $       |Convertir           |
|10/06/2019 (vous avez 1 licence) |Bronze    | 10/06/2019    |10/06/2019        |10 $        |1       | 10 $       |Convertir           |

### <a name="scenario-8--purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Scénario 8 - Acheter et annuler un abonnement SaaS avec compteur personnalisé à partir de la Portail Azure le même jour 

Dans ce scénario, vous achetez un abonnement SaaS avec compteur personnalisé sur le portail Azure, puis l'annulez le même jour. 

|**Date d’achat**   |**Référence SKU**   |**Début de facturation**   |**Fin de facturation**  |**Prix unitaire**  |**Quantité**  |**Montant** |**Type de facturation** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/06/2019 (vous avez 1 licence) |Bronze     |10/06/2019   |10/06/2019         |10 $        |1         |10 $            |Nouveau      |
|10/06/2019 (vous n'avez aucune licence) |Bronze    | 10/06/2019    |10/06/2019        |10 $        |1       | -10 $       |CancelImmediate  |
