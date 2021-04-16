---
title: Calcul du prix unitaire effectif
ms.topic: how-to
ms.date: 04/02/2021
description: En savoir plus sur le prix unitaire effectif et sur la façon dont il est calculé. Cet article contient également un exemple de calcul.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528575"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Calcul du prix unitaire effectif pour la consommation des plans Azure

## <a name="the-effective-unit-price"></a>Le prix unitaire effectif

Le prix unitaire effectif est calculé au niveau du compteur (par opposition au niveau de la ressource) et est ajusté quotidiennement en fonction de l’utilisation du compteur.

Nous calculons le prix unitaire effectif à l’aide des trois facteurs suivants :

- Consommation, qui est surveillée quotidiennement tout au long du cycle de facturation
- Coût facturable pour le compteur
- Hiérarchisation (le cas échéant)

Étant donné que nous Surveillez la consommation quotidiennement tout au long du cycle de facturation, le prix unitaire effectif varie. Le prix final d’un cycle de facturation donné sera disponible après l’arrêt du calcul de consommation et la clôture de la période de facturation. Vous verrez la plupart des modifications de la consommation après la quatrième ou la cinquième décimale.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Déterminez si votre compteur utilise la tarification à plusieurs niveaux

Si vous ne savez pas si votre compteur utilise la tarification à plusieurs niveaux, utilisez la procédure ci-dessous pour le savoir. 

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).
2. Sélectionnez **vendre**, sélectionnez **tarification et offres**, puis sélectionnez **tarification du plan Azure**.
3. Localisez votre compteur par ID, puis téléchargez vos données de tarification. 

## <a name="sample-calculation"></a>Exemple de calcul

Le tableau ci-dessous donne un exemple de la façon dont nous calculons le prix unitaire effectif au cours de la période ouverte.

Dans le tableau, les valeurs suivantes s’appliquent : 

- **Up** = prix unitaire de la ressource/heure = 0,868

- **BCU** = unité de consommation facturable pour le compteur

- **BC** = coût facturable pour le compteur = BCU * UP * 0,85. Cela reflète un ajustement de la remise de 15% du PEC. Nous utilisons ensuite la limite inférieure de la fonction pour limiter la valeur à deux chiffres après la virgule décimale, afin de charger la quantité minimale. 

- **Prix unitaire effectif** = BCU/BC

>[!NOTE]

>Remarque : le compteur de cet exemple n’a pas de niveaux de tarification ou autres remises, c’est-à-dire les facteurs de prix unitaire effectifs dans les pourcentages de remise et autres ajustements.


| Date | BCU (unité de consommation facturable) | BC (coût facturable) | Prix unitaire effectif |
| ------ | ----------- | ----------- | ----------- |  
| 3-août | 29 | 21,39 | 0.737586206896552 |
| 10-août | 210,950039 | 155,63 | 0.737757626107858 |
| 25-août | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Étapes suivantes

- [Facturation et taxes](billing.md)
