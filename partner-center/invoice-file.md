---
title: Comprendre les champs des factures de facturation
ms.topic: article
ms.date: 05/18/2020
description: Comprendre les champs de votre fichier de facture pour la facturation de l’espace partenaires.
author: LauraBrenner
ms.author: labrenne
keywords: facturation, facture
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 609860227f11c9d4bc2806d87ac7e595e503bf07
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991967"
---
# <a name="partner-center-billing-invoices---learn-how-to-read-the-billing-and-one-time-charge-fields"></a>Factures de facturation de l’espace partenaires : Découvrez comment lire les champs de facturation et de frais à usage unique

**Rôles appropriés**

- Administrateur général
- Administrateur des utilisateurs
- Administrateur de la facturation
- Agent du support technique

Vous pouvez utiliser les tableaux suivants pour comprendre les champs des fichiers de facture de l’espace partenaires.

## <a name="invoice-file-fields"></a>Champs du fichier de facture

Les champs suivants s’affichent sur vos fichiers de facture.

| Champ | Définition |
| ----- | ---------- |
| US FEIN | Votre numéro d’identification d’employeur fédéral (FEIN). Il s’agit de votre numéro d’identificateur fiscal fédéral États-Unis. |
| Numéro de client | Votre numéro de client. |
| Facturer à | Adresse d’expédition de votre facture. Vous pouvez modifier le nom et/ou l’adresse de votre société dans votre profil de facturation de l’espace partenaires. |
| Frais basés sur les licences | Frais mensuels ou annuels fixes pour vos licences achetées basées sur l’utilisation, facturés à l’avance du service. Ce nombre correspond à la somme de tous les frais dans la colonne de **sous-total** (colonne **T**) de votre fichier de réconciliation basé sur les licences. |
| Frais basés sur l’utilisation | Votre utilisation d’Azure. Cela comprend les nouveaux services ou applications activés et utilisés au cours de la période de facturation. Ce nombre correspond à la somme de tous les frais dans la colonne **PretaxCharges** (colonne **Z**) de votre fichier de réconciliation basé sur l’utilisation. |
| Remises | Remise que le client reçoit du tarif normal de l’abonnement. Ce nombre est indiqué sous la forme d’un *montant fixe*, et non d’un prix unitaire ou d’une licence. |
| Crédits | Crédits ou ajustements pour les modifications apportées aux abonnements (par exemple, augmentation ou diminution du siège). |
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
