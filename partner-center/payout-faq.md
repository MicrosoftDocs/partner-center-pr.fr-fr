---
title: FAQ sur le paiement du marché commercial Microsoft
description: Recevez des réponses aux questions courantes sur les paiements sur le marché commercial. Comprend des réponses sur la raison pour laquelle vos revenus sont différents de ceux attendus.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532019"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Questions courantes sur le paiement de la place de marché commercial

Cet article répond aux questions fréquemment posées sur les versements sur le marché commercial.

## <a name="earnings-incorrect-or-missing"></a>Résultats incorrects ou manquants

#### <a name="why-are-my-earnings-missing"></a>Pourquoi mes revenus sont-ils manquants ?

- La commande client n’est peut-être pas encore éligible au paiement. Pour les commandes client autres que les commandes d’entreprise, Microsoft doit recevoir le paiement du client avant que le revenu de l’éditeur ne soit éligible. Pour les commandes des clients d’entreprise, vos revenus seront disponibles un à deux jours après la date du bon de commande. Vérifiez l’état de la commande dans les [rapports sur les commandes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Les revenus des transactions antérieures à juillet 2019 peuvent ne pas figurer dans le rapport historique des transactions. Consultez les relevés historiques dans [Téléchargement des revenus](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Vérifiez le [laps de temps du cycle de paiement](payment-thresholds-methods-timeframes.md) et comprenez quand vos revenus doivent apparaître dans le relevé de paiement.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Pourquoi le montant de mes revenus est-il différent de ce que je pensais ?

- Si la commande a été payée partiellement par votre client, le montant acquis sera basé sur le montant partiellement payé après déduction des frais et taxes appropriées.
- Vérifiez la responsabilité du paiement de la taxe par pays. Dans le cas de pays où Microsoft est responsable de la taxe, Microsoft collecte et déduit les taxes des revenus de l’éditeur. Le montant de la transaction indiqué dans le relevé est le montant après paiement des taxes. Consultez [Détails des taxes](tax-details-marketplace.md).
- Les offres SaaS et IaaS ont un tarif réduit de 10% au lieu de la valeur standard de 20%, ce qui laisse un taux de bénéfices de 90%. Cette promotion est valable jusqu’au 30 juin 2021.

En **savoir plus** sur le contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), les [Détails](payout-policy-details.md)de la stratégie de paiement, le [seuil de paiement, la méthode et le laps de temps](payment-thresholds-methods-timeframes.md), [dans la place de marché commercial, les](marketplace-get-paid.md) [Détails fiscaux](tax-details-marketplace.md), les [déclarations](payout-statement.md)de paiement, le [tableau de bord des commandes dans commercial Marketplace](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Rapprochement des bénéfices
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Comment faire pour rapprocher les relevés de paiement avec les rapports de commande ou d’utilisation dans Analytics ?
Utilisez AssetID, orderID et l’ID d’article de ligne figurant dans le rapport historique des transactions de paiement avec les commandes analytiques et les rapports d’utilisation. Utilisez ce mappage :

- History.AssetID de transaction de paiement = order.OrderID
- History.OrderID & LineItem de transaction de paiement = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Comment faire pour connaître la date de paiement pour mes commandes client ?
- Tout d’abord, à l’aide de votre assetID, vérifiez les commandes des clients dans les [rapports de commandes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Vérifiez le canal client pour votre abonnement client dans le [rapport clients](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Pour les clients d’entreprise, les revenus de l’éditeur s’affichent dans le relevé 1-2 jours après la date du bon de commande.
- Pour les clients n’appartenant pas à l’entreprise, les revenus de l’éditeur s’affichent dans le relevé 1-2 jours après la réception du paiement du client.

En **savoir plus** sur les [instructions de paiement](payout-statement.md), le [tableau de bord Orders dans commercial Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Politiques de paiement

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Comment faire pour trouver les frais d’agence actuels et le taux de paiement ?

- Consultez le Contrat des éditeurs de la Place de marché commerciale. Les frais d’agence standard s’élèvent à 20 %. Les transactions SaaS Co-Sell éligibles bénéficient d’un tarif réduit de 10%. Vérifiez si des annonces signalant des promotions applicables aux frais d’agence ont été publiées.
- Dans votre relevé de paiement, le taux d’obtention spécifie le taux de paiement réel pour une transaction donnée.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Quand puis-je m’attendre à recevoir un paiement de la part de Microsoft une fois que les revenus apparaissent sur mon relevé ?
- Une fois que vos revenus sont à l’état Non traité, vous pouvez vérifier la date d’échéance afin de connaître le mois durant lequel le paiement de vos revenus sera traité. Une fois votre paiement préparé, l’état de votre obtention passe à « traité ».  Microsoft effectue les paiements le 15 du mois de l’échéance.
- Pour les commandes payées par carte de crédit, Microsoft conserve les paiements 30 jours jusqu’à ce que l’obtention soit mature.

 **Informations supplémentaires** : contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie](payout-policy-details.md)de paiement, [Détails fiscaux](tax-details-marketplace.md), [seuil de paiement, méthode et période](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Paiements et ajustements

#### <a name="why-is-my-payment-missing"></a>Pourquoi mon paiement est-il manquant ?

- Vérifiez que l’état de paiement et l’état du profil fiscal sont indiqués comme étant *valides* sur la [page vue d’ensemble](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Vous n’avez peut-être pas atteint le seuil minimal pour un paiement. Les bénéfices doivent être d’au moins $50 USD pour que vous puissiez recevoir un paiement.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Comment faire définir mon compte pour ne pas recevoir le paiement ?
Vous pouvez conserver les paiements dans le [profil de paiement](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); cochez simplement la case **conserver**. Microsoft vous contiendra le paiement jusqu’à ce que vous relâchiez le blocage.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Pourquoi est-ce que je reçois un paiement dans une devise différente de celle de l’achat ?

La devise du paiement est basée sur la devise que vous avez sélectionnée dans le profil de paiement. La devise de l’achat est basée sur la devise payée par le client.

#### <a name="how-do-i-reconcile-adjustments"></a>Comment faire pour rapprocher les ajustements ?

Les ajustements de paiement sont des corrections de paiement afin de tenir compte des ajustements compensatoires, tels que les problèmes système. Dans le relevé de paiements, ReasonCode indique la raison de l’ajustement. Les ajustements ne sont pas destinés à être rapprochés directement avec les transactions individuelles.

**Informations supplémentaires** : contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie](payout-policy-details.md)de paiement, [Détails fiscaux](tax-details-marketplace.md), [seuil de paiement, méthode et période](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Taxes

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Comment identifier la responsabilité du paiement de la taxe (Microsoft ou l’éditeur) dans le relevé de paiements ?

Dans le téléchargement de l’historique des transactions, recherchez la colonne indiquant le modèle des taxes. Cela indique si elles sont gérées par Microsoft ou par l’ISV. Consultez les règles fiscales propres aux pays et les implications en matière de paiement dans [Détails des taxes](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Comment faire pour télécharger les formulaires fiscaux relatifs aux frais de service ?

Accédez à la page **Payout Payment** , puis à la section **List of Payment**. Un lien vers le formulaire fiscal sur les frais de service s’affiche pour un paiement dont les frais de service sont facturés.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Comment faire pour télécharger un formulaire fiscal de retenue à la source au format PDF ?

Accédez à la page *Payout Payment* , puis à la section **List of Payment**. Un lien vers un formulaire fiscal de retenue à la source s’affiche à côté d’un paiement.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Où puis-je trouver des formulaires fiscaux de fin d’exercice ?

Accédez à la [page de profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) pour afficher les formulaires fiscaux de fin d’exercice.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Comment faire pour trouver la retenue à la source pour une transaction ?
La retenue à la source s’applique aux éditeurs américains qui ont rempli un formulaire W-9. La retenue à la source est calculée sur un paiement mensuel.

Informations **supplémentaires** : contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie de paiement](payout-policy-details.md)

## <a name="payout-statement-access"></a>Accès aux relevés de paiement

#### <a name="how-do-i-access-a-payout-statement"></a>Comment faire pour accéder à un relevé de paiements ?

1. Vérifiez vos rôles. Pour accéder au relevé de paiements, vous devez avoir le rôle de *contributeur financier* ou *propriétaire du compte*.
2. Dans la barre de navigation en haut à droite, sélectionnez l’icône **paiement** pour afficher votre relevé de paiement. Choisissez entre **l’historique des transactions** , le **paiement** et le **Téléchargement**.

Informations **supplémentaires** : [rôles et autorisations de paiement](payout-statement.md#roles-and-permissions), [instructions de paiement](payout-statement.md) 

## <a name="payout-statement-report"></a>Rapport de déclaration de paiement

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Que signifie chaque champ du téléchargement de transaction ?

Consultez les [instructions de paiement](payout-statement.md) pour obtenir une liste détaillée des attributs et de leurs significations.

#### <a name="what-is-earning-status"></a>Qu’est-ce que l’état « earning » ?

Vous pouvez ainsi afficher vos revenus comme non traités, traités ou envoyés.

- Non **traité** : le bénéfice se trouve dans une période de dépôt jusqu’à la date d’échéance.
- **Traité** : les bénéfices ont évolué et sont préparés dans le paiement mensuel. Les paiements sont libérés du 15 de chaque mois.
- **Envoyé** : le paiement a été remis à votre banque en fonction de votre profil de paiement.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Comment faire pour télécharger les formulaires fiscaux relatifs aux frais de service ?

Accédez à la page **Payout Payment** , puis à la section **List of Payment**. Un lien vers le formulaire fiscal sur les frais de service s’affiche pour un paiement dont les frais de service sont facturés.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Comment faire télécharger un formulaire d’impôt à la retenue au format PDF ?

Accédez à la page **Payout Payment** , puis à la section **List of Payment**. Un lien vers un formulaire fiscal de retenue à la source s’affiche à côté d’un paiement.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Où puis-je trouver des formulaires fiscaux de fin d’exercice ?

Accédez à la [page de profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) pour afficher les formulaires fiscaux de fin d’exercice.

Informations **supplémentaires** : [instructions de paiement](payout-statement.md), [téléchargement de l’historique des transactions](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Instructions historiques

#### <a name="how-do-i-view-historical-information"></a>Comment faire afficher les informations d’historique ?

Le relevé historique affiche l’instantané des données de paiement à compter d’octobre 2019. Malheureusement, les informations de paiement ici ne sont pas actualisées. Pour recevoir les informations les plus récentes, envoyez un ticket de support pour les données les plus récentes.

Informations **supplémentaires** : [instructions de paiement](payout-statement.md), [téléchargement de l’historique des transactions](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API d’exportation de paiement

#### <a name="how-do-i-download-payout-data"></a>Comment faire pour télécharger des données de paiement ?

Utilisez l' [API de paiement de partenaire](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Étapes suivantes

- [Recevoir un paiement dans la place de marché commerciale](marketplace-get-paid.md)
