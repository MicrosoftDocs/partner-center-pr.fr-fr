---
title: Détails de la stratégie de paiement-Marketplace Microsoft commercial
description: Détails concernant les stratégies de paiement de la place de marché commercial, y compris les planifications et les versements.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 04/24/2020
ms.openlocfilehash: 17fedcf4ef3d474eab679a03eecb221c90342a04
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335668"
---
# <a name="payout-policy-details"></a>Détails de la politique de paiement

Cet article décrit le processus de paiement de Microsoft, le calendrier de paiement et la stratégie de réapprovisionnement, ainsi que l’emplacement de l’état d’un paiement.

## <a name="where-to-find-upcoming-payouts"></a>Où trouver les paiements à venir

Dans l’espace partenaires, sélectionnez l’icône **paiement** dans l’angle supérieur droit de l’écran :

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustre l’icône Revenu en haut à droite du portail Espace partenaires.":::

> [!TIP]
> Certains rôles de compte n’ont pas accès aux informations de paiement. Pour plus d’informations, consultez [rôles et autorisations](payout-statement.md#roles-and-permissions).

## <a name="payment-schedules"></a>Calendriers de paiement

Les sections suivantes décrivent notre processus de paiement.

### <a name="enterprise-agreement-transactions-after-may-1-2020"></a>Transactions Contrat Entreprise postérieures au 1er mai 2020

Nous avons effectué la mise à jour suivante pour notre modèle de paiement de l’éditeur de la place de marché commercial :

À compter du 1er mai 2020, nous mettons à jour notre politique de paiement relative aux produits achetés dans Microsoft AppSource ou la place de marché Azure par les clients disposant d’un Accord Entreprise Microsoft. Lorsqu’un client achète un produit à partir de la place de marché Azure ou AppSource à l’aide de son Accord Entreprise Microsoft existant pour les transactions, après le 1er mai, 2020 nous commencerons à émettre des paiements dans le cycle de paiement suivant 30 jours après la facture client. Un client qui utilise la carte de crédit dans une transaction est soumis aux mêmes conditions, à savoir une période d’attente de 30 jours avant paiement. Ce tableau présente les détails du calendrier de paiement.

> [!NOTE]
> Pour connaître les mesures que nous prenons en cas de défaut de paiement d’un client si nous vous avons déjà adressé le paiement, consultez [Processus en cas de défaut de paiement d’un client](#process-for-customer-non-payment) ci-dessous.

| Événement  | Date (UTC) | Visibilité du partenaire : rapport de revenu de l’Espace partenaires  |  Visibilité du partenaire : analytique de l’Espace partenaires\* |
| --- | --- | --- | --- |
| Transaction ou mois d’utilisation | 01/08/2020 – 31/08/2020 | N/A | **Rapport d’utilisation** : indication de la nouvelle consommation (actualisée toutes les quatre heures)<br>**Rapport sur les commandes** : N/A |
| Échéance (mois) | 31/08/2020 | N/A | **Rapport d’utilisation** : indication de la consommation à la fin du mois<br>**Rapport sur les commandes** : N/A |
| Commande générée | 03/09/2020 – 07/09/2020 | N/A | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Calculer le montant de revenu versé | 04/09/2020 – 10/09/2020 | Marqué **Non traité** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Paiement mensuel | 05/10/2020 | Marqué **À venir** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Date de paiement\** | 15/10/2020 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Facture client recueillie | 01/12/2020 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF  |
|  |  |  |  |

\* Le rapport d’utilisation et le rapport sur les commandes sont accessibles dans la section Analyser de l’Espace partenaires.</br>\** La date de paiement est exprimée en Heure standard du Pacifique (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Clients qui paient par carte de crédit ou sur facture

Tous les achats effectués par carte de crédit ou avec facture mensuelle sont assortis d’une période d’attente de 30 jours pour vérifier que les fonds sont encaissés et qu’il n’y a pas de rétrofacturation ou de fraude présumée.

| Événement  | Date (UTC) | Visibilité du partenaire : rapport de revenu de l’Espace partenaires  |  Visibilité du partenaire : analytique de l’Espace partenaires\*  |
| --- | --- | --- | --- |
| Transaction ou mois d’utilisation | 01/08/2019 – 31/08/2019 | N/A | **Rapport d’utilisation** : indication de la nouvelle consommation (actualisée toutes les quatre heures)<br>**Rapport sur les commandes** : N/A |
| Échéance (mois) | 31/08/2019 | N/A | **Rapport d’utilisation** : indication de la consommation à la fin du mois<br>**Rapport sur les commandes** : N/A |
| Commande générée | 03/09/2019 – 07/09/2019 | N/A | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Facture client recueillie | 07/09/2019 – 10/09/2019 | N/A | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Calculer le paiement | 08/09/2019 – 12/09/2019 | Marqué **Non traité** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Paiement mensuel | 05/11/2019\* | Marqué **À venir** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Date de paiement\** | 15/11/2019 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
|  |  |  |  |

\* Le rapport d’utilisation et le rapport sur les commandes sont accessibles dans la section Analyser de l’Espace partenaires.</br>\** La date de paiement est exprimée en Heure standard du Pacifique (PST).

### <a name="enterprise-agreement-transactions-prior-to-may-1-2020"></a>Transactions Contrat Entreprise antérieures au 1er mai 2020

Tous les achats effectués avant cette date sont traités et payés selon le calendrier ci-dessous une fois que Microsoft a encaissé le paiement des clients et traité les frais de la Place de marché.

| Événement  | Date (UTC)  | Visibilité du partenaire : rapport de revenu de l’Espace partenaires  |  Visibilité du partenaire : analytique de l’Espace partenaires\*  |
| --- | --- | --- | --- |
| Transaction ou mois d’utilisation | 01/08/2019 – 31/08/2019 | N/A | **Rapport d’utilisation** : indication de la nouvelle consommation (actualisée toutes les quatre heures)<br>**Rapport sur les commandes** : N/A |
| Échéance (mois) | 31/08/2019 | N/A | **Rapport d’utilisation** : indication de la consommation à la fin du mois<br>**Rapport sur les commandes** : N/A |
| Commande générée | 03/09/2019 – 07/09/2019 | N/A | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Facture client recueillie | 01/12/2019 | N/A | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Calculer le paiement | 05/12/2019 – 07/12/2019 | Marqué **Non traité** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Paiement mensuel | 05/01/2019 | Marqué **À venir** dans l’Historique des transactions du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
| Date de paiement\** | 15/01/2019 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu | **Rapport d’utilisation** : indication de la consommation avec OrderID/OrderLineItemID<br>**Rapport sur les commandes** : commandes client présentant l’état ACTIF |
|  |  |  |  |

\* Le rapport d’utilisation et le rapport sur les commandes sont accessibles dans la section Analyser de l’Espace partenaires.</br>\** La date de paiement est exprimée en Heure standard du Pacifique (PST).

## <a name="process-for-customer-non-payment"></a>Processus en cas de défaut de paiement d’un client

Dans de rares cas, Microsoft peut ne pas pouvoir encaisser les paiements de clients ayant effectué des achats sur la Place de marché commerciale. Quand un client ne paie selon le calendrier de facturation, Microsoft lance le processus de recouvrement. Ce processus prend environ quatre mois et suppose une communication permanente de la part de Microsoft. Si le paiement n’est pas reçu à la fin de ce processus, Microsoft passe les fonds en pertes et profits et les considère comme irrécouvrables.

Dans le cadre du processus de paiement présenté ici, Microsoft peut avoir déjà adressé un paiement à l’éditeur (vous) alors que les fonds sont finalement irrécouvrables. Nous avons donc mis en place un processus pour compenser ces montants. Pour vous avertir que votre paiement (déjà perçu) risque d’être compensé, vous recevrez une notification dès lors qu’un client est engagé dans le processus de recouvrement et que les achats sont susceptibles d’être passés en pertes et profits.

Microsoft recouvrera les paiements qu’il vous a déjà adressés en employant l’une des méthodes suivantes : (1) Microsoft se réserve le droit de déduire les montants dus des futurs paiements ; par exemple, si un montant déjà versé de 1 000 USD est considéré comme irrécouvrable et passé en pertes et profits, vos futurs paiements seront retenus tant que les 1 000 USD n’auront pas été récupérés, ou (2) Microsoft pourra demander un remboursement à l’éditeur ou lui adresser une facture correspondant aux montants non encaissés.

Le tableau suivant montre un exemple de planification :

| Événement | Date approximative | Visibilité du partenaire |
| --- | --- | --- |
| Exemple de date de paiement | 15/10/2020 | Marqué **Envoyé** dans l’Historique des transactions et dans la section Paiements du tableau de bord Revenu |
| Si le client ne paie pas Microsoft | 12/02/2020 – 05/12/2020 | Inchangée, comme ci-dessus |
| Le client reçoit un premier e-mail l’avisant d’un retard de paiement | 06/12/2020 | None |
| Le client reçoit des e-mails à intervalles réguliers pour l’aviser de l’urgence croissante | 7/12/2020 – 31/1/2021 | None |
| L’éditeur est avisé du passage probable en pertes et profits | 7/1/2021 | L’éditeur est notifié par e-mail que le client n’a pas encore envoyé le paiement. L’ID de transaction et le montant en dollars sont inclus. |
| Le client reçoit un avis d’expiration | 1/2/2021 | None |
| Fin du processus de recouvrement. Les fonds sont passés en pertes et profits | 15/2/2021 | L’éditeur est notifié par e-mail que les fonds ont été passés en pertes et profits. L’ID de transaction et le montant en dollars sont inclus. |
| Le paiement est déduit | 1/3/2021 | Une transaction négative figurera dans le Relevé des revenus de l’Espace partenaires de l’éditeur |
| Le paiement est retenu | 15/3/2021 | Les futurs paiements seront indiqués dans le Relevé des revenus de l’Espace partenaires. L’éditeur ne recevra pas de paiement tant que le solde sera négatif.  |
|||

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Nombre de jours pour que les paiements atteignent un compte de paiement

En général, nous envoyons tout paiement dû pour un mois donné le 15 de ce mois, mais il faut plus de temps pour que le paiement parvienne à votre compte. Le nombre de jours dépend du mode de paiement que nous utilisons pour votre compte, comme décrit ci-dessous.

> [!NOTE]
> Les jours indiqués ci-dessous sont approximatifs. Tout paiement peut prendre plus ou moins de temps pour atteindre votre compte.

| Mode de paiement     | Nombre de jours du délai de transfert au compte de paiement     |
|--------------------|--------------------------------------------|
| PayPal             | 1 jour ouvrable                             |
| ACH/SEPA           | 2 à 3 jours ouvrables                          |
| Virement bancaire      | 7 à 10 jours ouvrables                         |

## <a name="next-step"></a>étape suivante

- [Détails des taxes](tax-details-marketplace.md)
