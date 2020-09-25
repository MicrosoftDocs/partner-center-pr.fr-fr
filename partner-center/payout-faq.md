---
title: FAQ sur le paiement du marché commercial Microsoft
description: Recevez des réponses aux questions courantes sur les paiements sur le marché commercial.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335665"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Questions courantes sur le paiement de la place de marché commercial

Cet article répond aux questions fréquemment posées sur les versements sur le marché commercial.

## <a name="earnings-incorrect-or-missing"></a>Résultats incorrects ou manquants

#### <a name="why-are-my-earnings-missing"></a>Pourquoi mes revenus manquent-ils ?

- La commande client ne peut pas encore être éligible au paiement. Pour les commandes client autres que l’entreprise, Microsoft doit recevoir le paiement du client avant que le serveur de publication ne soit éligible. Pour les commandes des clients d’entreprise, vos revenus seront disponibles 1-2 jours après la date de bon de commande. Vérifiez l’état de la commande dans les [rapports de commandes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Les bénéfices des transactions antérieures au 2019 juillet peuvent ne pas figurer dans le rapport historique des transactions. Vérifiez les instructions historiques dans le [téléchargement de paiement](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Vérifiez le [laps de temps du cycle de paiement](payment-thresholds-methods-timeframes.md) et comprenez quand vos revenus doivent apparaître dans le relevé de paiement.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Pourquoi le montant de mes revenus est-il différent de ce que je pensais ?

- Si la commande a été payée partiellement par votre client, le montant acquis sera basé sur le montant partiellement payé après déduction des frais et taxes appropriées.
- Vérifiez la responsabilité du paiement de la taxe par pays. Dans le cas de pays où la taxe est responsable de Microsoft, Microsoft collecte et déduire les taxes des revenus de l’éditeur. Le montant de la transaction indiqué dans la déclaration est postérieur au montant des taxes. Consultez les [Détails des taxes](tax-details-marketplace.md).
- Les offres SaaS et IaaS ont un tarif réduit de 10% au lieu de la valeur standard de 20%, ce qui laisse un taux de bénéfices de 90%. Cette promotion est valable jusqu’au 30 juin 2021.

En **savoir plus**sur le contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), les [Détails](payout-policy-details.md)de la stratégie de paiement, le [seuil de paiement, la méthode et le laps de temps](payment-thresholds-methods-timeframes.md), [dans la place de marché commercial, les](marketplace-get-paid.md) [Détails fiscaux](tax-details-marketplace.md), les [déclarations](payout-statement.md)de paiement, le [tableau de bord des commandes dans commercial Marketplace](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Rapprochement des bénéfices
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Comment faire concilier les relevés de paiement aux rapports de commande ou d’utilisation dans Analytics ?
Utilisez AssetID, orderID et l’ID d’article de ligne figurant dans le rapport historique des transactions de paiement avec les commandes analytiques et les rapports d’utilisation. Utilisez ce mappage :

- Historique des transactions de paiement. AssetID = ordre. OrderID
- Historique des transactions de paiement. OrderID & LineItem = usage. UsageReferenceID [OrderID : LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Comment faire savez-vous quand attendre des paiements pour mes commandes client ?
- Tout d’abord, à l’aide de votre assetID, vérifiez les commandes des clients dans les [rapports de commandes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Vérifiez le canal client pour votre abonnement client dans le [rapport clients](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Pour les clients d’entreprise, les revenus de l’éditeur s’affichent dans le relevé 1-2 jours après la date du bon de commande.
- Pour les clients n’appartenant pas à l’entreprise, les revenus de l’éditeur s’affichent dans le relevé 1-2 jours après la réception du paiement du client.

En **savoir plus**sur les [instructions de paiement](payout-statement.md), le [tableau de bord Orders dans commercial Marketplace Analytics](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Stratégies de paiement

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Comment faire trouver les frais d’Agence actuels et le taux de paiement ?

- Consultez le contrat d’éditeur de la place de marché commercial. Le tarif de l’Agence standard est de 20%. Les transactions éligibles de covente SaaS bénéficient d’un tarif réduit de 10%. Recherchez les annonces des frais liés aux agences promotionnelles.
- Dans votre relevé de paiement, le taux d’obtention spécifie le taux de paiement réel pour une transaction donnée.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Quand puis-je m’attendre à recevoir un paiement de la part de Microsoft une fois que les bénéfices apparaissent sur mon relevé ?
- Une fois que vous avez acquis un État non traité, vous pouvez vérifier la date d’échéance du mois pour le paiement de vos revenus. Une fois votre paiement préparé, l’état de votre obtention passe à « traité ».  Microsoft publie les paiements au 15 de l’échéance.
- Pour les commandes payées par carte de crédit, Microsoft conserve les paiements 30 jours jusqu’à ce que l’obtention soit mature.

 **Informations supplémentaires**: contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie](payout-policy-details.md)de paiement, [Détails fiscaux](tax-details-marketplace.md), [seuil de paiement, méthode et période](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Paiements et ajustements

#### <a name="why-is-my-payment-missing"></a>Pourquoi mon paiement est-il manquant ?

- Vérifiez que l’état de paiement et l’état du profil fiscal sont indiqués comme étant *valides* sur la [page vue d’ensemble](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Vous n’avez peut-être pas atteint le seuil minimal pour un paiement. Les bénéfices doivent être au moins de $50 USD pour recevoir un paiement.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Comment faire définir mon compte pour ne pas recevoir le paiement ?
Vous pouvez conserver les paiements dans le [profil de paiement](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); cochez simplement la case **conserver**. Microsoft vous contiendra le paiement jusqu’à ce que vous relâchiez le blocage.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Pourquoi est-ce que je reçois une devise différente de celle de l’achat ?

La devise de paiement est basée sur la devise que vous avez sélectionnée dans profil de paiement. La devise d’achat est basée sur la devise payée par le client.

#### <a name="how-do-i-reconcile-adjustments"></a>Comment faire rapprocher les ajustements ?

Les ajustements de paiement sont des corrections de paiement pour tenir compte des ajustements compensatoires, tels que les problèmes système. Dans l’instruction de paiement, ReasonCode indique la raison de l’ajustement. Celles-ci ne sont pas destinées à être réconcilier directement en transactions individuelles.

**Informations supplémentaires**: contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie](payout-policy-details.md)de paiement, [Détails fiscaux](tax-details-marketplace.md), [seuil de paiement, méthode et période](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Taxes

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Comment identifier la responsabilité du paiement de la taxe entre Microsoft ou le serveur de publication dans le relevé de paiement ?

Dans le téléchargement de l’historique des transactions, recherchez la colonne modèle fiscal. Cela indique géré par Microsoft ou ISV. Consultez les règles fiscales spécifiques aux pays et les implications de paiement dans les [Détails des taxes](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Comment faire télécharger les formulaires d’impôt sur les frais de service ?

Accédez à la page **paiement de paiement** , puis à la section **liste des paiements** . Un lien vers le formulaire d’impôt sur les frais de service s’affiche pour un paiement dont la taxe de service est facturée.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Comment faire télécharger un formulaire d’impôt à la retenue au format PDF ?

Accédez à la page *paiement de paiement* , puis à la section **liste des paiements** . Un lien vers un formulaire d’impôt à la retenue s’affiche à côté d’un paiement.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Où puis-je trouver des formulaires fiscaux annuels ?

Accédez à la [page de profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) pour afficher les formulaires fiscaux de l’année.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Comment faire Rechercher les taxes de retenue pour une transaction ?
La taxe à la retenue s’applique aux éditeurs américains qui ont classé un formulaire W-9. La taxe à la retenue est calculée sur un remboursement mensuel.

Informations **supplémentaires**: contrat d’éditeur de la place de [marché commercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), détails de la [stratégie de paiement](payout-policy-details.md)

## <a name="payout-statement-access"></a>Accès aux relevés de paiement

#### <a name="how-do-i-access-a-payout-statement"></a>Comment faire accéder à une déclaration de paiement ?

1. Vérifiez vos rôles. Vous devez disposer du rôle de *collaborateur financier* ou du *propriétaire du compte* pour accéder à la déclaration de paiement.
2. Dans la barre de navigation en haut à droite, sélectionnez l’icône **paiement** pour afficher votre relevé de paiement. Choisissez entre **l’historique des transactions**, le **paiement**et le **Téléchargement**.

Informations **supplémentaires**: [rôles et autorisations de paiement](payout-statement.md#roles-and-permissions), [instructions de paiement](payout-statement.md) 

## <a name="payout-statement-report"></a>Rapport de déclaration de paiement

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Que signifie chaque champ du téléchargement de la transaction ?

Consultez les [instructions de paiement](payout-statement.md) pour obtenir une liste détaillée des attributs et de leurs significations.

#### <a name="what-is-earning-status"></a>Qu’est-ce que l’État gain ?

Vous pouvez ainsi afficher vos revenus comme non traités, traités ou envoyés.

- Non **traité** : le bénéfice se trouve dans une période de dépôt jusqu’à la date d’échéance.
- **Traité** : les bénéfices ont évolué et sont préparés dans le paiement mensuel. Les paiements sont libérés du 15 de chaque mois.
- **Envoyé** : le paiement a été remis à votre banque en fonction de votre profil de paiement.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Comment faire télécharger les formulaires d’impôt sur les frais de service ?

Accédez à la page **paiement de paiement** , puis à la section **liste des paiements** . Un lien vers le formulaire d’impôt sur les frais de service s’affiche pour un paiement dont la taxe de service est facturée.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Comment faire télécharger un formulaire d’impôt à la retenue au format PDF ?

Accédez à la page **paiement de paiement** , puis à la section **liste des paiements** . Un lien vers un formulaire d’impôt à la retenue s’affiche à côté d’un paiement.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Où puis-je trouver des formulaires fiscaux annuels ?

Accédez à la [page de profil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) pour afficher les formulaires fiscaux de l’année.

Informations **supplémentaires**: [instructions de paiement](payout-statement.md), [téléchargement de l’historique des transactions](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Instructions historiques

#### <a name="how-do-i-view-historical-information"></a>Comment faire afficher les informations d’historique ?

L’instruction historique affiche la capture instantanée des données de paiement à partir du 2019 octobre. Malheureusement, les informations de paiement ici ne sont pas actualisées. Pour recevoir les informations les plus récentes, envoyez un ticket de support pour les données les plus récentes.

Informations **supplémentaires**: [instructions de paiement](payout-statement.md), [téléchargement de l’historique des transactions](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API d’exportation de paiement

#### <a name="how-do-i-download-payout-data"></a>Comment faire télécharger les données de paiement ?

Utilisez l' [API de paiement de partenaire](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Étapes suivantes

- [Recevoir un paiement dans la place de marché commerciale](marketplace-get-paid.md)
