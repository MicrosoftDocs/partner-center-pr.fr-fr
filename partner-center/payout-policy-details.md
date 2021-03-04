---
title: Planifications et traitements des paiements
description: En savoir plus sur les versements et les transactions, tels que les calendriers de paiement et les processus de remboursement pour la place de marché commerciale et les autres transactions.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: 9c4ad89eb25e811c4bea11e7e7e5d3845ceafee6
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756851"
---
# <a name="payout-schedules-and-processes"></a>Planifications et traitements des paiements

**Rôles appropriés :**

- Administrateur des comptes
- Administrateur général

Cet article décrit le calendrier de paiement de Microsoft, où trouver l’état d’un paiement et le processus de non-paiement du client.

## <a name="payment-schedules"></a>Calendriers de paiement

Les sections suivantes décrivent notre processus de paiement des **contrat entreprise** et des transactions par **carte de crédit/facture** .

### <a name="enterprise-agreement-transactions"></a>Transactions Contrat Entreprise

Lorsqu’un client achète un produit à partir de Microsoft AppSource ou de la place de marché Azure à l’aide de ses Contrat Entreprise Microsoft existantes pour les transactions, nous détenons des paiements dans le cycle de paiement suivant 30 jours après la facture client. Les transactions pour lesquelles un client utilise une carte de crédit ont une période de 30 jours avant paiement.

Un paiement se produit souvent avant que Microsoft ne collecte le paiement du client. Consultez la section [processus pour le non-paiement du client](#process-for-customer-non-payment) ci-dessous pour les actions que nous prenons si le client ne parvient pas à payer Microsoft, mais que nous avons déjà émis un paiement.

| Événement | Description | Visibilité des rapports | Bascul |
| --- | --- | --- | --- |
| Utilisation ou mois de transaction | Le client utilise ou achète un service. | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 1** |
| Microsoft calcule le montant de facturation | Déterminer l’utilisation totale, total des transactions | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 2** |
| Paiement Posté | Détermination des frais de l’Agence et des revenus du paiement | Marqué comme non traité dans l’historique des transactions dans l' [instruction de paiement](payout-statement.md) | **Mois 3 (1er semaine)** |
| Préparer le paiement | Les bénéfices sont préparés pour le paiement mensuel | Marqué comme étant à venir dans l’historique des transactions dans le [relevé de paiement](payout-statement.md) | **Mois 3 (1er semaine)** |
| **Paiement envoyé** | **Le paiement est envoyé au serveur de publication** | **Marqué comme envoyé dans l’historique des transactions et dans la section paiements de l' [instruction de paiement](payout-statement.md)** | **Mois 3 (au plus tard le 15)** |
| Facture payée par le client | Microsoft collecte le paiement du client | Aucun changement | **Du mois 4 au 12** |
|

\* La date de paiement est l’heure standard du Pacifique (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Chronologie des paiements pour les clients du contrat entreprise.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transactions avec carte de crédit ou facture (chèque/câble)

Tous les achats effectués sur une carte de crédit ou une facture mensuelle ont une période de 30 jours pour garantir la collecte des fonds auprès du client.

| Événement | Description | Visibilité des rapports | Bascul |
| --- | --- | --- | --- |
| Utilisation ou mois de transaction | Le client utilise ou achète un service. | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 1** |
| Facture payée par le client | Déterminer le nombre total d’utilisations, la valeur totale de la transaction et le paiement du client | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 2** |
| Paiement Posté | Détermination des frais de l’Agence et des revenus du paiement | Marqué comme non traité dans l’historique des transactions dans l' [instruction de paiement](payout-statement.md) | **Mois 2** |
| période de conservation de 30 jours | Garantir la collecte des fonds, les refacturations possibles et les demandes de remboursement | Marqué comme non traité dans l’historique des transactions dans l' [instruction de paiement](payout-statement.md) | **Mois 3** |
| Préparer le paiement | Les bénéfices sont préparés pour le paiement mensuel | Marqué comme étant à venir dans l’historique des transactions dans le [relevé de paiement](payout-statement.md) | **Mois 4 (1er semaine)** |
| **Paiement envoyé** | **Le paiement est envoyé au serveur de publication** | **Marqué comme envoyé dans l’historique des transactions et dans la section paiements de l' [instruction de paiement](payout-statement.md)** | **Le mois 4 (au plus tard le 15)** |
|

\* La date de paiement est l’heure standard du Pacifique (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Chronologie des paiements pour les clients de la carte de crédit et de la facture.":::

## <a name="process-for-customer-non-payment"></a>Processus en cas de défaut de paiement d’un client

Dans de rares cas, Microsoft peut ne pas pouvoir encaisser les paiements de clients ayant effectué des achats sur la Place de marché commerciale. Quand un client ne paie selon le calendrier de facturation, Microsoft lance le processus de recouvrement. Ce processus prend environ quatre mois et suppose une communication permanente de la part de Microsoft. Si le paiement n’est pas reçu à la fin de ce processus, Microsoft passe les fonds en pertes et profits et les considère comme irrécouvrables.

Dans le cadre du processus de paiement présenté ici, Microsoft peut avoir déjà adressé un paiement à l’éditeur (vous) alors que les fonds sont finalement irrécouvrables. Nous avons donc mis en place un processus pour compenser ces montants. Pour vous avertir que votre paiement (déjà perçu) risque d’être compensé, vous recevrez une notification dès lors qu’un client est engagé dans le processus de recouvrement et que les achats sont susceptibles d’être passés en pertes et profits.

Microsoft recouvrera les paiements qu’il vous a déjà adressés en employant l’une des méthodes suivantes : (1) Microsoft se réserve le droit de déduire les montants dus des futurs paiements ; par exemple, si un montant déjà versé de 1 000 USD est considéré comme irrécouvrable et passé en pertes et profits, vos futurs paiements seront retenus tant que les 1 000 USD n’auront pas été récupérés, ou (2) Microsoft pourra demander un remboursement à l’éditeur ou lui adresser une facture correspondant aux montants non encaissés.

Voici un exemple de calendrier :

| Événement | Date approximative * | Visibilité du partenaire |
| --- | --- | --- |
| Exemple de date de paiement | 15/10/2020 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu |
| <font color="red">Si le client ne paie pas Microsoft</font> | 12/02/2020 – 05/12/2020 | Inchangée, comme ci-dessus |
| Le client reçoit un premier e-mail l’avisant d’un retard de paiement | 06/12/2020 | None |
| Le client reçoit des e-mails à intervalles réguliers pour l’aviser de l’urgence croissante | 7/12/2020 – 31/1/2021 | None |
| L’éditeur est avisé du passage probable en pertes et profits | 7/1/2021 | L’éditeur est notifié par e-mail que le client n’a pas encore envoyé le paiement. L’ID de transaction et le montant en dollars sont inclus. |
| Le client reçoit un avis d’expiration | 1/2/2021 | None |
| Fin du processus de recouvrement. Les fonds sont passés en pertes et profits | 15/2/2021 | L’éditeur est notifié par e-mail que les fonds ont été passés en pertes et profits. L’ID de transaction et le montant en dollars sont inclus. |
| Le paiement est déduit | 1/3/2021 | L’éditeur verra une transaction négative dans l’instruction de paiement de l’espace partenaires |
| Le paiement est retenu | 15/3/2021 | Les versements futurs seront affichés dans le relevé de paiement de l’espace partenaires. L’éditeur ne recevra pas de paiement tant que le solde sera négatif.  |
|||

\* La date de paiement est l’heure standard du Pacifique (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Nombre de jours pour que les paiements atteignent un compte de paiement

En général, nous envoyons tout paiement dû pour un mois donné le 15 de ce mois, mais il faut plus de temps pour que le paiement parvienne à votre compte. Le nombre de jours dépend du mode de paiement que nous utilisons pour votre compte, comme décrit ci-dessous.

> [!NOTE]
> Les jours indiqués ci-dessous sont approximatifs ; tout paiement peut prendre plus ou moins de temps pour atteindre votre compte.

| Mode de paiement     | Nombre de jours du délai de transfert au compte de paiement     |
|--------------------|--------------------------------------------|
| PayPal             | 1 jour ouvrable                             |
| ACH/SEPA           | 2 à 3 jours ouvrables                          |
| Virement bancaire      | 7 à 10 jours ouvrables                         |
|

## <a name="next-steps"></a>Étapes suivantes

- [Détails des taxes](tax-details-marketplace.md)
