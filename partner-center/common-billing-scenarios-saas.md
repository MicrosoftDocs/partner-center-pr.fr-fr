---
title: Facturation-transactions SaaS basées sur une licence
ms.topic: article
ms.date: 05/05/2020
description: En savoir plus sur les scénarios courants de facturation dans l’espace partenaires pour les transactions SaaS basées sur une licence.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d65d23057ea0354fc77b1cc8a9c7fb16a343b3ee
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444568"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Scénarios de facturation courants pour les transactions SaaS basées sur une licence dans l’espace partenaires

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Agent du support technique
- Agent commercial


Ces exemples de [scénarios de facturation courants](common-billing-scenarios.md) sont applicables aux abonnements de Software as a service basés sur une licence (SaaS) dans l’espace partenaires.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertir un abonnement SaaS gratuit d’évaluation en abonnement payant

Ce scénario décrit la facturation pour le renouvellement d’un abonnement SaaS d’essai gratuit basé sur une licence. Le renouvellement convertit la version d’évaluation gratuite en abonnement payant à la fin de la période d’évaluation gratuite.

Dans cet exemple, vous avez acheté une version d’évaluation gratuite d’un abonnement SaaS (software as a service) basé sur une licence le 10 juin. Cette version d’évaluation gratuite est automatiquement renouvelée en tant qu’abonnement payant dès la fin de la période d’évaluation gratuite.

Les fichiers de rapprochement comporteront les frais suivants :

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de dépense | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 1 | 0 $ | Nouveau | Essai gratuit |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 $ | 1 | 2 $ | Renouveler | Abonnement payant |

## <a name="cancel-a-free-trial-saas-subscription"></a>Annuler un abonnement SaaS d’évaluation gratuite

> [!TIP]
> Vous pouvez annuler à tout moment un abonnement SaaS d’essai gratuit basé sur une licence, même pendant la période d’évaluation gratuite.

Dans ce scénario, vous avez acheté un abonnement SaaS d’essai gratuit basé sur une licence le 1er juillet, puis vous l’avez annulé immédiatement dans l’espace partenaires.

Le fichier de rapprochement inclut les frais suivants :

| Date d’achat | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de dépense | Description de l’abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Nouveau | Essai gratuit |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Annuler | Essai gratuit |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertir un abonnement SaaS de compteur personnalisé en une autre référence (SKU)

Ce scénario décrit comment convertir un abonnement SaaS de compteur personnalisé d’une référence (SKU) vers une autre référence (SKU) pour le même produit, à la même date.

Dans ce scénario, vous avez acheté une référence (Silver) sous un produit et vous l’avez convertie en une autre référence (bronze) disponible dans le cadre de ce produit à la même date.

Le fichier de rapprochement inclut les frais suivants :

| Date d’achat | Référence | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de dépense | Description de l’abonnement |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Argent | 10/06/2019 | 10/06/2019 | 20 $ | 1 | 20 $ | Nouveau | Abonnement SaaS à compteur personnalisé |
| 10/06/2019 | Argent | 10/06/2019 | 10/06/2019 | 20 $ | 1 | -$20 | Convertir | Facture au prorata pour l’abonnement SaaS du compteur personnalisé |
| 10/06/2019 | Bronze | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Convertir | Abonnement SaaS à compteur personnalisé |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Acheter et annuler un abonnement SaaS client à la même date

Ce scénario décrit la facturation d’un abonnement SaaS client Meter que vous avez acheté et annulé par le biais de la Portail Azure à la même date.

Dans ce scénario, vous avez acheté un abonnement SaaS à compteur personnalisé sur la Portail Azure. Ensuite, vous avez annulé l’abonnement à la même date.

| Date d’achat | Référence | Date de début de facturation | Date de fin de la facturation | Prix unitaire | Quantité unitaire | Montant total | Type de dépense | Description de l’abonnement |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Bronze | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Nouveau | Abonnement SaaS à compteur personnalisé |
| 10/06/2019 | Bronze | 10/06/2019 | 10/06/2019 | $10 | 1 | -$10 | CancelImmediate | Abonnement SaaS à compteur personnalisé |
