---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389677"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

S'applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Colonne | Description |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. Identique dans toutes les lignes. |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| Nom du client | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. Ce champ peut rester vide jusqu'au deuxième cycle de facturation. *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | Le pays dans lequel se trouve le client. |
| Numéro de facture | Le numéro de la facture dans laquelle la transaction spécifiée apparaît. |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| ID de commande | Unique identifier for an order in the Microsoft commerce platform. Not used for reconciliation. |
| Date de la commande | La date à laquelle la commande a été passée. |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | Le titre d'une référence spécifique. |
| Nom du produit | Le nom du produit. |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | Friendly name of a subscription. |
| ID d’abonnement | Unique identifier for a subscription in the Microsoft commerce platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Date de début des frais. L’heure indique toujours le début de la journée, 0:00. |
| ChargeEndDate | Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59. |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| Type de facturation | Le type de frais ou d’ajustement. |
| Prix unitaire | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | The unit price after adjustments have been made. |
| Quantité | Number of units. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | The type of unit being purchased. |
| DiscountDetails | An explanation of any applicable discount. |
| Sub Total | Total avant impôt. Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| Total | Total après impôts. Vérifie si les impôts sont retenus sur la facture. |
| Symbole monétaire | Type de devise. Chaque entité de facturation n’a qu’une devise. Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
