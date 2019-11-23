---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389837"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| Champ | Définition |
| ----- | ---------- |
| Numéro d’identification américain FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| Numéro de client | Votre numéro de client. |
| Adresse de facturation | Adresse d’expédition de votre facture. You can change your company name and/or address in your Partner Center billing profile. |
| Frais basés sur la licence | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| Frais basés sur l’utilisation | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| Remises | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| Crédits | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| Sous-total | Total avant les taxes et frais et crédits hors taxes. |
| Taxe | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| Autres crédits | Crédits hors taxes. |
| Total des frais en cours | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| Instructions pour le paiement | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| Numéro de facture | Numéro de votre facture. |
| Période de facturation | The monthly period leading up to the invoice date. This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count. |
| Date de facturation | The billing date or anniversary date on which your invoice is generated each month. |
| Modalités de paiement | The payment term. Pour les achats ponctuels, le délai sera toujours de 60 jours. |
| Date d’échéance du paiement | The date by which your payment must be received. |
| Numéro du bon de commande du client | Your purchase number order. |
| Service client | The website address where you can access customer service. |
| Bénéficiaire du service | The address where the service is being used. (This is the legal company address associated with company vetting.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| Champ | Définition |
| ----- | ---------- |
| Date | Date d’achat. |
| Description | Nom du produit. |
| Quantité | The number of products (such as reservations) purchased. |
| Prix unitaire | Price per product (such as a reservation). |
| Remises | Toutes les remises applicables. |
| Montant hors taxe | Sous-total des achats avant impôts. |
| Taxe de vente | Montant des taxes. |
| Total | Total amount to be paid. |
