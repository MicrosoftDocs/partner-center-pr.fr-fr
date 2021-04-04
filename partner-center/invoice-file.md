---
title: Présentation des factures de facturation de l’espace partenaires
ms.topic: article
ms.date: 05/18/2020
description: Comprendre les champs de votre fichier de facture pour la facturation de l’espace partenaires. Les champs et les définitions de tous les champs de facturation et champs de frais d’une seule période sont inclus.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178899"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Présentation des champs de facturation de l’espace partenaires

**Rôles appropriés**

- Administrateur général
- Administrateur de la gestion des utilisateurs
- Administrateur de la facturation
- Agent du support technique

Vous pouvez utiliser les tableaux suivants pour comprendre les champs des fichiers de facture de l’espace partenaires.

## <a name="invoice-file-fields"></a>Champs du fichier de facture

Les champs suivants s’affichent sur vos fichiers de facture.

| Champ | Définition |
| ----- | ---------- |
| US FEIN | Votre numéro d’identification d’employeur fédéral (FEIN). Il s’agit de votre numéro d’identificateur fiscal fédéral États-Unis. |
| Numéro de client | Votre numéro de client. |
| Facturer à | Adresse d’expédition de votre facture. Vous pouvez modifier le nom et l’adresse de votre société dans votre profil de facturation de l’espace partenaires. |
| Frais basés sur les licences | Frais mensuels ou annuels fixes pour vos licences achetées basées sur l’utilisation, facturés à l’avance du service. Ce nombre correspond à la somme de tous les frais dans la colonne de **sous-total** (colonne **T**) de votre fichier de réconciliation basé sur les licences. |
| Frais basés sur l’utilisation | Votre utilisation d’Azure. Cela comprend les nouveaux services ou applications activés et utilisés au cours de la période de facturation. Ce nombre correspond à la somme de tous les frais dans la colonne **PretaxCharges** (colonne **Z**) de votre fichier de réconciliation basé sur l’utilisation. |
| Remises | Remise que le client reçoit du tarif normal de l’abonnement. Ce nombre est indiqué sous la forme d’un *montant fixe*, et non d’un prix unitaire ou d’une licence. |
| Crédits | Crédits ou ajustements pour les modifications apportées aux abonnements (par exemple, augmentation ou diminution de la licence). |
| Sous-total | Total avant taxes et crédits et crédits hors taxes. |
| Taxe | Taxe totale de vos frais actuels, telle qu’elle est totalisée dans la section de **Détails** à partir de la page 2 de votre facture. Ce nombre correspond à la somme de tous les frais dans la colonne **TaxAmount** (colonne **AA**) de votre fichier de réconciliation basé sur l’utilisation, et de la colonne **Tax** (colonne **U**) dans votre fichier de réconciliation basé sur les licences. |
| Autres crédits | Crédits à taxe exclusive. |
| Total des frais actuels | Montant dû dans votre devise de facturation pour la période de facturation. Ces frais sont dus à la date d’échéance du paiement. |
| Instructions de paiement | Description de la façon de payer votre facture, en fonction de votre région. *Veillez à toujours inclure votre numéro de facture lors de l’exécution d’un paiement.* |
| Numéro de facture | Numéro de votre facture. |
| Période de facturation | Période mensuelle menant à la date de la facture. Il s’agit de la période pendant laquelle les services basés sur l’utilisation sont consommés et les services basés sur des licences sont conciliés pour les ajustements de crédit ou les modifications de nombre de licences. |
| Date de facture | Date de facturation ou date anniversaire à laquelle votre facture est générée chaque mois. |
| Modalités de paiement | Conditions de paiement. Pour des achats à usage unique, cette durée est toujours de 60 jours. |
| Date d’échéance du paiement | Date à laquelle votre paiement doit être reçu. |
| Numéro de l’ordre d’achat du client | Votre ordre de numéro d’achat. |
| Service client | L’adresse du site Web où vous pouvez accéder au service client. |
| Bénéficiaire du service | Adresse à laquelle le service est utilisé. (Il s’agit de l’adresse de la société légale associée à l’aide à la société.) |

## <a name="one-time-charges-fields"></a>Champs de frais à usage unique

Les champs suivants s’appliquent uniquement aux **frais à usage unique** dans l’espace partenaires :

| Champ | Définition |
| ----- | ---------- |
| Date | Date d’achat. |
| Description | Nom du produit. |
| Quantité | Le nombre de produits (par exemple, réservations) achetés. |
| Prix unitaire | Prix par produit (par exemple, une réservation). |
| Remises | Les remises applicables. |
| Montant avant impôt | Sous-total des achats avant taxes. |
| Taxe de vente | Montant des taxes |
| Total | Montant total à payer. |
