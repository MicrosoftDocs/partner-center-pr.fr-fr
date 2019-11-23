---
title: Proposer à vos clients des versions d’évaluation de produits Microsoft | Espaces partenaires
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vos clients peuvent tester des produits d’abonnement Microsoft pendant 30 jours. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384830"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Proposer à vos clients des offres d’essai de produits Microsoft

S'applique à :

- Espace partenaires

Une méthode efficace pour présenter les nouveaux produits Microsoft aux clients consiste à leur proposer des versions d'évaluation gratuites pendant 30 jours. Vous pouvez obtenir les versions d’évaluation figurant le catalogue comme vous le faites pour de nombreux autres services en ligne. Tous les partenaires peuvent participer.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Par exemple, ils peuvent obtenir un essai gratuit pour Office 365 Business Premium et un autre pour Office 365 E3. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

Des essais gratuits sont proposés pour les produits suivants :

- Office&nbsp;365 Business&nbsp;Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility + Security E5
- Formule Dynamics 365 Customer Engagement 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Nous fournissons des essais gratuits pour ces produits, car il s’agit des offres commerciales les plus complètes et les plus populaires. Il se peut que nous ajoutions d’autres offres d’essais gratuits à l’avenir.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. Dans le catalogue, à partir de **Périodicité de facturation**, cliquez sur **Offre de version d'évaluation**. Cela ne fait apparaître que les essais gratuits et désactive les offres payantes. Les versions d’évaluation s’affichent dans l’onglet **Versions d’évaluation** du catalogue.
3. Sélectionnez la version d’évaluation gratuite que vous voulez proposer, puis sélectionnez **Soumettre**. Toutes les versions d’évaluation sont valables 30 jours ; vous ne serez pas facturé pendant cette période. Vous pouvez également convertir une version d’évaluation en abonnement payant à tout moment pendant la période d’évaluation.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Accédez à la page des abonnements du client, puis sélectionnez l'essai gratuit.
2. Sélectionnez **Convertir la version d'évaluation en abonnement payant**.
3. Entrez le nombre de licences souhaité et la fréquence de facturation, puis sélectionnez **Appliquer**.
4. La facturation de l’abonnement payant commencera à la date de conversion et l'abonnement sera automatiquement renouvelé 12 mois à compter de cette dernière. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Convertir un abonnement d'évaluation en abonnement payant](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtenir une liste des offres de conversion de version d’évaluation](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. Il est recommandé de contrôler fréquemment ces dates afin de pouvoir prendre les mesures de suivi appropriées auprès des clients à l’approche du moment où ils doivent prendre une décision.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Facturation

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Si l’essai gratuit est converti en offre payante à facturation annuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de conversion. Si l’essai gratuit est converti en une offre payante avec facturation mensuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de facturation suivant la date de conversion.

### <a name="invoices"></a>Factures

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Primes incitatives

Free trials do not have an impact on incentives.

## <a name="support"></a>Assistance

For support on free trials, submit a service request through Partner Center.
