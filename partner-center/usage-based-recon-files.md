---
title: Usage-based reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand usage-based reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 3cf0f20ed266fa5302264ef07092d47c050a9206
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389777"
---
# <a name="usage-based-file-fields"></a>Champs des fichiers basés sur l’utilisation

S'applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

To reconcile your charges against a customer's usage, compare the **ResellerID**, **ResellerName**, and **ResellerBillableAccount** from the reconciliation file with the **Customer name** and **Subscription ID** from Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Fields in usage-based reconciliation files

Les champs suivants décrivent les services utilisés et leurs taux.

| Colonne | Description | Sample value(s) |
| ------ | ----------- | ------------ |
| PartnerID | Partner identifier, in GUID format. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Partner name. | *Contoso, Ltd.* |
| PartnerBillableAccountID | Partner account identifier. | *1010578050* |
| CustomerName | Customer's organization name, as reported in Partner Center. *Very important for reconciling the invoice with your system information.* | *Test customer* |
| MPNID | MPN identifier of the CSP partner. | *4390934* |
| ResellerMPNID | MPN identifier of the reseller of record for the subscription. For more information, see [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| InvoiceNumber | Le numéro de la facture dans laquelle la transaction spécifiée apparaît. | *D020001IVK* |
| ChargeStartDate | Start date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle). L’heure indique toujours le début de la journée, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | End date of billing cycle, except when presenting dates of previously uncharged latent usage data (from previous bill cycle). L’heure indique toujours la fin de la journée, 23:59. | *2/28/2019 23:59* |
| SubscriptionID | Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. May be useful to identify the subscription when contacting support. Not used for reconciliation. *This is not the same as the **Subscription ID** on the Partner Admin Console.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Nickname for the service offering. | *Microsoft Azure* |
| SubscriptionDescription | Line of business of the service offering. | *Microsoft Azure* |
| OrderId | Identificateur unique pour une commande dans la plateforme de facturation Microsoft. May be useful to identify the subscription when contacting support. Not used for reconciliation. | *566890604832738111* |
| ServiceName | Nom du service Azure en question. | *VIRTUAL MACHINES* |
| ServiceType | The specific type of Azure service. | *Service Bus – Individual or Pack*, *SQL Azure database – Business or Web Edition* |
| ResourceGUID | Identificateur unique spécifique pour toutes les données de service et la structure de tarification. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| Nom_ressource | Nom de la ressource Azure. | *Data Transfer In (GB)* , *Data Transfer Out (GB)* |
| Région | The region to which the usage applies. Primarily used to assign rates to data transfers, because rates vary by region. | *Asia Pacific*, *Europe*, *Latin America*, *North America* |
| SKU | Unique Microsoft identifier for an offer. | *7UD-00001* |
| DetailLineItemId | An identifier and quantity to itemize different rates for a service or resource in a given billing period. For Azure tiered pricing, there may be one rate for up to a certain quantity of billable units, then a different rate after that quantity. | *1* |
| ConsumedQuantity | The amount of service consumed (such as hours or GB) during the reporting period. Inclut également toute utilisation non facturée pour les périodes précédentes. | *11* |
| IncludedQuantity | Unités incluses dans le cadre de l’offre. Typically not present in CSP. | *0* |
| OverageQuantity | Units not included as part of the offer. These must be paid for by the partner. Equal to **ConsumedQuantity** minus **IncludedQuantity**. | *11* |
| ListPrice | Offer price in effect at subscription's start date. | *$0.0808* |
| PretaxCharges | Equal to **ListPrist** multiplied by **OverageQuantity**, rounded to the nearest cent. | *$0.085* |
| TaxAmount | Tax amount charged. Based on your market's tax rules and specific circumstances. | *$0.08* |
| PostTaxTotal | Total après impôts, le cas échéant. | *$0.93* |
| Symbole monétaire | Type de devise. Chaque entité de facturation n’a qu’une devise. Check that it matches your first invoice and then after any major billing platform updates. | *EUR* |
| PretaxEffectiveRate | Prix avant impôts par unité. Equal to **PretaxCharges** divided by **OverageQuantity**, rounded to the nearest cent. | *$0.08* |
| PostTaxEffectiveRate | Prix après impôts par unité. Equal to **PostTaxTotal** divided by **OverageQuantity**, rounded to the nearest cent. Or, equal to **PretaxEffectiveRate** plus thet tax rate per unit amoun, rounded to the nearest cent. | *$0.08* |
| ChargeType | The [type of charge](recon-file-charge-types.md) or adjustment. | See [charge types](recon-file-charge-types.md). |
| CustomerBillableAccount | Unique account identifier in the Microsoft billing platform. | *1280018095* |
| UsageDate | Date du déploiement du service. | *2/1/2019 0:00* |
| MeteredRegion | Identifies the location of a data center within the region (for services where this value is applicable and populated). | *East Asia*, *South East Asia*, *North Europe*, *West Europe*, *North Central US*, *South Central US* |
| MeteredService | Identifies the individual Azure service usage when it's not specifically identified in the **ServiceName** column. For example, data transfers are reported as *Microsoft Azure - All Services* in the **ServiceName** column. | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Subheading for **MeteredService** field that provides additional clarification of Azure service usage. | *EXTERNAL* |
| Project | Customer-defined name for their service instance. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | The number of Azure Service Bus connections that were provisioned and utilized on a given day. | *1.000000 Connections / 30 days* (if you had an individually provisioned connection during a 30-day month), *25 Connections / 30 Days – Used: 1.000000* (if you had a 25 pack of Service Bus connections provisioned and you utilized 1 during that day) |
| CustomerID | Unique Microsoft identifier for the customer, in GUID format. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Customer's domain name. Ce champ peut rester vide jusqu'au deuxième cycle de facturation. | *example.onmicrosoft.com* |
| Unit | The unit of the resource **Name**. | *GB* or *HOURS* |
