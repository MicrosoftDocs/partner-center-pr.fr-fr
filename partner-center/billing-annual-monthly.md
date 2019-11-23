---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389767"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

S'applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>Applicabilité

Most licensed-based subscriptions have the option for either monthly or annual billing option. Les abonnements basés sur l’utilisation proposent seulement une facturation mensuelle.

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

La facturation annuelle présente les avantages suivants :

- Flexibilité accrue en matière d’options de paiement.
- Meilleur alignement avec la facturation de vos clients.
- Réduction de l’impact des fluctuations des devises.
- Réduction des coûts d’exploitation en matière de facturation.

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

Pour tirer parti de la facturation annuelle, certaines modifications de vos API sont nécessaires.

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. Cependant, vous pouvez donner à une offre un nom plus explicite pour aider les clients à faire facilement la distinction.

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. Vous pouvez choisir l’option de facturation annuelle à ce stade. When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

Vous serez facturé à votre date de facturation suivante. For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. La période du service commence à la date de création de l’abonnement.  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

Vous serez facturé à la prochaine date de facturation qui suit la date de renouvellement de l’abonnement. Par exemple, si vous achetez un abonnement à facturation annuelle le 15 janvier 2018 et que votre date de facturation est le 20 janvier, votre abonnement sera renouvelé le 15 janvier 2019. Vous serez facturé pour le renouvellement le 20 janvier 2019.

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. Certaines offres sont limitées à un seul abonnement par client. Si l’offre n’est pas limitée, un client peut avoir plusieurs abonnements d’une même offre avec des fréquences de facturation différentes. Vous trouverez les détails des limites et restrictions de chaque offre dans la colonne I du tableau des offres. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. Ces conditions diffèrent de celles des abonnements à fréquence de facturation mensuelle, qui bénéficient d’une période gratuite entre la date d’achat et la date de facturation qui suit.

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

Vous pouvez modifier le nombre de licences de vos abonnements à tout moment. L’ajout de licences supplémentaires n’aura aucune incidence sur la fréquence de facturation.

Vous pouvez à tout moment ajouter ou supprimer des licences.  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. Une fois que vous achetez un abonnement à facturation annuelle, toutes les licences supplémentaires respecteront la même fréquence de facturation. Si par la suite vous devez acheter des licences à facturation mensuelle, vous devrez acheter un nouvel abonnement.

### <a name="add-on-offers"></a>Add-on offers

L’abonnement au module complémentaire aura automatiquement la même fréquence de facturation que l’abonnement parent. Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

La politique d’annulation est la même pour toutes les fréquences de facturation.

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. Ceci s’applique aussi bien aux abonnements à facturation mensuelle qu’annuelle.

Le nouveau partenaire doit acheter un nouvel abonnement pour le compte du client. It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. Les frais calculés au prorata seront facturés à la date de facturation suivante. La date de renouvellement de l’abonnement reste identique.

## <a name="pricing"></a>Tarification

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). Lors du renouvellement d’un abonnement, le prix est basé sur la liste des prix en vigueur à la date du renouvellement. The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

Si aucune modification n’est apportée à l’abonnement, aucune ligne n’apparaît sur les fichiers de rapprochement pour les mois 2 à 12 de la période d’abonnement. If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. Elle apparaît à la première date de facturation qui suit le renouvellement.

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. Si l’annulation se produit après les 30 premiers jours, l’abonnement sera crédité au prorata.

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. Vous pouvez calculer le prix annuel en multipliant le prix mensuel par 12.

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>Primes incitatives

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. Les paiements des primes obtenues seront versés conformément à notre stratégie présentée dans les guides de primes incitatives de notre programme Fournisseur de solutions Cloud.

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>Revenu

Currently, all incentive payments are made twice a year. Ces paiements sont versés 45 jours après la fin du semestre.

### <a name="rates"></a>Tarifs

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>Contacts

For questions about incentives, contact the appropriate regional incentives support team:

| Région | Adresse e-mail |
| ------ | ------------- |
| Amérique du Nord | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| Japon | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
