---
title: Scénarios de facturation courants pour les transactions SaaS basées sur une licence | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Scénarios courants de facturation dans l’espace partenaires pour les transactions SaaS basées sur une licence.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturation, paiements, achat unique, achat périodique, abonnements, sièges
ms.localizationpriority: medium
ms.openlocfilehash: b808a3bbfc0856e03f1c775d7e3145a29c2239fb
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389607"
---
# <a name="billing-scenarios-for-license-based-saas-transactions"></a>Scénarios de facturation pour les transactions SaaS basées sur une licence

Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) sont applicables aux abonnements de Software as a service basés sur une licence (SaaS) dans l’espace partenaires.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertir un abonnement SaaS gratuit d’évaluation en abonnement payant

Ce scénario décrit la facturation pour le renouvellement d’un abonnement SaaS d’essai gratuit basé sur une licence. Le renouvellement convertit la version d’évaluation gratuite en abonnement payant à la fin de la période d’évaluation gratuite.

Dans cet exemple, vous avez acheté une version d’évaluation gratuite d’un abonnement SaaS (software as a service) basé sur une licence le 10 juin. Cette version d’évaluation gratuite est automatiquement renouvelée en tant qu’abonnement payant dès la fin de la période d’évaluation gratuite.

Les fichiers de rapprochement comporteront les frais suivants :

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de frais | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 $ | 1 | 0 $ | Nouveau | Évaluation gratuite |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 $ | 1 | 2 $ | Renouveler | Abonnement payant |

## <a name="cancel-a-free-trial-saas-subscription"></a>Annuler un abonnement SaaS d’évaluation gratuite

> [!TIP]
> Vous pouvez annuler à tout moment un abonnement SaaS d’essai gratuit basé sur une licence, même pendant la période d’évaluation gratuite.

Dans ce scénario, vous avez acheté un abonnement SaaS d’essai gratuit basé sur une licence le 1er juillet, puis vous l’avez annulé immédiatement dans l’espace partenaires. 

Le fichier de rapprochement inclut les frais suivants :

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de frais | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Nouveau | Évaluation gratuite |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Cancel | Évaluation gratuite |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertir un abonnement SaaS de compteur personnalisé en une autre référence (SKU)

Ce scénario décrit comment convertir un abonnement SaaS de compteur personnalisé d’une référence (SKU) vers une autre référence (SKU) pour le même produit, à la même date.

Dans ce scénario, vous avez acheté une référence (Silver) sous un produit et vous l’avez convertie en une autre référence (bronze) disponible dans le cadre de ce produit à la même date.

Le fichier de rapprochement inclut les frais suivants :

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de frais | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 $ | 1 | 20 $ | Nouveau | Abonnement SaaS à compteur personnalisé |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | 20 $ | 1 | -$20 | Convertir | Facture au prorata pour l’abonnement SaaS du compteur personnalisé |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 $ | 1 | 10 $ | Convertir | Abonnement SaaS à compteur personnalisé |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Acheter et annuler un abonnement SaaS client à la même date

Ce scénario décrit la facturation d’un abonnement SaaS client Meter que vous avez acheté et annulé par le biais de la Portail Azure à la même date.

Dans ce scénario, vous avez acheté un abonnement SaaS à compteur personnalisé sur la Portail Azure. Ensuite, vous avez annulé l’abonnement à la même date.

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de frais | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 $ | 1 | 10 $ | Nouveau | Abonnement SaaS à compteur personnalisé |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | 10 $ | 1 | -$10 | CancelImmediate | Abonnement SaaS à compteur personnalisé |
