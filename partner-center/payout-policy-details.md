---
title: Planification du paiement et détails de la stratégie-place de marché Azure
description: En savoir plus sur les détails relatifs aux stratégies de paiement de la place de marché commercial, y compris les planifications et les prévisions.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 11/06/2020
ms.openlocfilehash: 8986ef1d2a16d939530ed49875a21c13b0b97868
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381390"
---
# <a name="payout-schedules-and-policy-details"></a>Planifications de paiement et détails de la stratégie

Cet article décrit le processus de paiement de Microsoft, le calendrier de paiement, où trouver l’état d’un paiement et le processus de non-paiement du client.

## <a name="payment-schedules"></a>Calendriers de paiement

Les sections suivantes décrivent notre processus de paiement des **accord entreprise** et des transactions par **carte de crédit/facture** .

### <a name="enterprise-agreement-transactions"></a>Transactions Accord Entreprise

Lorsqu’un client achète un produit à partir de Microsoft AppSource ou de la place de marché Azure à l’aide de ses Accord Entreprise Microsoft existantes pour les transactions, nous détenons des paiements dans le cycle de paiement suivant 30 jours après la facture client. Les transactions pour lesquelles un client utilise une carte de crédit ont une période de 30 jours avant paiement.

Un paiement se produit souvent avant que Microsoft ne collecte le paiement du client. Consultez la section [processus pour le non-paiement du client](#process-for-customer-non-payment) ci-dessous pour les actions que nous prenons si le client ne parvient pas à payer Microsoft, mais que nous avons déjà émis un paiement.

| Événement | Description | Visibilité des rapports | Bascul |
| --- | --- | --- | --- |
| Utilisation ou mois de transaction | Le client utilise ou achète un service. | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 1** |
| Le bon de commande est créé | Déterminer l’utilisation totale, total des transactions | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 2** |
| Le paiement de l’ISV est créé | Détermination des frais de l’Agence et des revenus du paiement | Marqué comme non traité dans l’historique des transactions dans l’instruction de paiement | **Mois 3 (1er semaine)** |
| Préparer le paiement | Les bénéfices sont préparés pour le paiement mensuel | Marqué comme étant à venir dans l’historique des transactions dans le relevé de paiement | **Mois 3 (1er semaine)** |
| **Date de paiement** | **Le paiement est envoyé au serveur de publication** | **Marqué comme envoyé dans l’historique des transactions et dans la section paiements de l’instruction de paiement** | **Mois 3 (au plus tard le 15)** |
| Facture payée par le client | Microsoft collecte le paiement du client | Aucun changement | **Du mois 4 au 12** |
|

\* La date de paiement est l’heure standard du Pacifique (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Clients qui paient par carte de crédit ou sur facture

Tous les achats effectués sur une carte de crédit ou une facture mensuelle ont une période de 30 jours pour garantir la collecte des fonds auprès du client.

| Événement | Description | Visibilité des rapports | Bascul |
| --- | --- | --- | --- |
| Utilisation ou mois de transaction | Le client utilise ou achète un service. | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 1** |
| Facture payée par le client | Déterminer le nombre total d’utilisations, la valeur totale de la transaction et le paiement du client | Tableau de bord d' [utilisation](/azure/marketplace/partner-center-portal/usage-dashboard) ou de [commande](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mois 2** |
| Le paiement de l’ISV est créé | Détermination des frais de l’Agence et des revenus du paiement | Marqué comme non traité dans l’historique des transactions dans l’instruction de paiement | **Mois 2** |
| Période de conservation de 30 jours | Assurez la collecte des fonds, des refacturations possibles et des demandes de remboursement | Marqué comme non traité dans l’historique des transactions dans l’instruction de paiement | **Mois 3** |
| Préparer le paiement | Les bénéfices sont préparés pour le paiement mensuel | Marqué comme étant à venir dans l’historique des transactions dans le relevé de paiement | **Première semaine du mois 4** |
| **Date de paiement** | **Le paiement est envoyé au serveur de publication** | **Marqué comme envoyé dans l’historique des transactions et dans la section paiements de l’instruction de paiement** | **Le mois 4 (au plus tard le 15)** |
|

\* La date de paiement est l’heure standard du Pacifique (PST).

## <a name="process-for-customer-non-payment"></a>Processus en cas de défaut de paiement d’un client

Dans de rares cas, Microsoft peut ne pas pouvoir encaisser les paiements de clients ayant effectué des achats sur la Place de marché commerciale. Quand un client ne paie selon le calendrier de facturation, Microsoft lance le processus de recouvrement. Ce processus prend environ quatre mois et suppose une communication permanente de la part de Microsoft. Si le paiement n’est pas reçu à la fin de ce processus, Microsoft passe les fonds en pertes et profits et les considère comme irrécouvrables.

Dans le cadre du processus de paiement présenté ici, Microsoft peut avoir déjà adressé un paiement à l’éditeur (vous) alors que les fonds sont finalement irrécouvrables. Nous avons donc mis en place un processus pour compenser ces montants. Pour vous avertir que votre paiement (déjà perçu) risque d’être compensé, vous recevrez une notification dès lors qu’un client est engagé dans le processus de recouvrement et que les achats sont susceptibles d’être passés en pertes et profits.

Microsoft recouvrera les paiements qu’il vous a déjà adressés en employant l’une des méthodes suivantes : (1) Microsoft se réserve le droit de déduire les montants dus des futurs paiements ; par exemple, si un montant déjà versé de 1 000 USD est considéré comme irrécouvrable et passé en pertes et profits, vos futurs paiements seront retenus tant que les 1 000 USD n’auront pas été récupérés, ou (2) Microsoft pourra demander un remboursement à l’éditeur ou lui adresser une facture correspondant aux montants non encaissés.

Voici un exemple de calendrier :

| Événement | Date approximative * | Visibilité du partenaire |
| --- | --- | --- |
| Exemple de date de paiement | 15/10/2020 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu |
| <font color="red">Si le client ne paie pas Microsoft</font> | 12/02/2020 – 05/12/2020 | Inchangée, comme ci-dessus |
| Le client reçoit un premier e-mail l’avisant d’un retard de paiement | 06/12/2020 | Aucune |
| Le client reçoit des e-mails à intervalles réguliers pour l’aviser de l’urgence croissante | 7/12/2020 – 31/1/2021 | None |
| L’éditeur est avisé du passage probable en pertes et profits | 7/1/2021 | L’éditeur est notifié par e-mail que le client n’a pas encore envoyé le paiement. L’ID de transaction et le montant en dollars sont inclus. |
| Le client reçoit un avis d’expiration | 1/2/2021 | None |
| Fin du processus de recouvrement. Les fonds sont passés en pertes et profits | 15/2/2021 | L’éditeur est notifié par e-mail que les fonds ont été passés en pertes et profits. L’ID de transaction et le montant en dollars sont inclus. |
| Le paiement est déduit | 1/3/2021 | Une transaction négative figurera dans le Relevé des revenus de l’Espace partenaires de l’éditeur |
| Le paiement est retenu | 15/3/2021 | Les futurs paiements seront indiqués dans le Relevé des revenus de l’Espace partenaires. L’éditeur ne recevra pas de paiement tant que le solde sera négatif.  |
|||

\* La date de paiement est l’heure standard du Pacifique (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Nombre de jours pour que les paiements atteignent un compte de paiement

En général, nous envoyons tout paiement dû pour un mois donné le 15 de ce mois, mais il faut plus de temps pour que le paiement parvienne à votre compte. Le nombre de jours dépend du mode de paiement que nous utilisons pour votre compte, comme décrit ci-dessous.

> [!NOTE]
> Les jours indiqués ci-dessous sont approximatifs. Tout paiement peut prendre plus ou moins de temps pour atteindre votre compte.

| Mode de paiement     | Nombre de jours du délai de transfert au compte de paiement     |
|--------------------|--------------------------------------------|
| PayPal             | 1 jour ouvrable                             |
| ACH/SEPA           | 2 à 3 jours ouvrables                          |
| Virement bancaire      | 7 à 10 jours ouvrables                         |
|

## <a name="next-steps"></a>Étapes suivantes

En savoir plus sur les [taxes](tax-details-marketplace.md).
