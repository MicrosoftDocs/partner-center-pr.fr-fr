---
title: Relevés de paiements
description: En savoir plus sur les relevés de paiement et les résumés, ainsi que sur la façon d’afficher et d’exporter vos données de paiement depuis l’espace partenaires Microsoft
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 4e9ab721fe356dbcdff7316a5ed5b52c81f2d4eb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152594"
---
# <a name="payout-statements"></a>Relevés de paiements

**Rôles appropriés**: administrateur de compte | Administrateur général

Le **relevé de paiement** présente une vue d’ensemble de vos paiements des offres vendues par le biais du marché commercial. Il affiche l’historique transactionnel de vos revenus, estime votre prochain paiement et affiche les tendances de paiement. Vous pouvez également télécharger l’historique des transactions et les relevés de paiement. Cet article explique comment accéder à votre relevé de paiement, ainsi que les différentes pages de paiement et téléchargements qui vous sont accessibles dans l’espace partenaires.

>[!NOTE]
>Vous verrez uniquement les données des ID et des programmes MPN auxquels vous êtes associé. Si vous souhaitez afficher des données supplémentaires, contactez votre administrateur de compte pour obtenir des autorisations. 

## <a name="roles-and-permissions"></a>Rôles et autorisations

Pour accéder à une déclaration de paiement, vous devez être affecté au **propriétaire du compte** ou au rôle **contributeur financier** .

| Rapports/pages | Propriétaire du compte | Manager | Développeur | Contributeur commercial | Collaborateur financier | Distributeur |
| --- | --- | --- | --- | --- | --- | --- |
| Rapport d’acquisition (comprenant des données en quasi-temps réel) | Affichage | Affichage | Aucun accès | Aucun accès | Affichage | Aucun accès |
| Rapport de commentaires/réponses | Peut afficher et envoyer des commentaires | Peut afficher et envoyer des commentaires | Peut afficher et envoyer des commentaires | Aucun accès | Aucun accès | Peut afficher et envoyer des commentaires |
| Rapport d’intégrité (comprenant des données en quasi-temps réel) | Affichage | Affichage | Affichage | Affichage | Aucun accès | Aucun accès |
| Rapport d’utilisation | Affichage | Affichage | Affichage | Affichage | Aucun accès | Aucun accès |
| Compte de paiement | Peut mettre à jour | Aucun accès | Aucun accès | Aucun accès | Peut mettre à jour | Aucun accès |
| Profil fiscal | Peut mettre à jour | Aucun accès | Aucun accès | Aucun accès | Peut mettre à jour | Aucun accès |
| Récapitulatif des paiements | Affichage | Aucun accès | Aucun accès | Aucun accès | Affichage | Aucun accès |
|

## <a name="access-your-payout-statement"></a>Accéder à votre déclaration de paiement

Connectez-vous à l' [espace partenaires](https://partner.microsoft.com/dashboard/home) et sélectionnez l’icône paiement dans le coin supérieur droit de l’écran pour accéder à ces différents résumés :

- Historique des transactions
- Paiements
- Exporter des données

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustre l’icône de paiement dans le coin supérieur droit du portail espace partenaires":::

Vous pouvez également utiliser l' [API](https://apidocs.microsoft.com/services/partnerpayouts) de paiement de partenaire pour vous connecter et obtenir directement les données de paiement et de transaction de paiement.


## <a name="transaction-history"></a>Historique des transactions

La page **historique des transactions** affiche le résumé de vos revenus, le paiement suivant estimé et la tendance de vos revenus et paiements au cours des 36 derniers mois. Vous pouvez également télécharger les détails des transactions à partir de cette section.<br><br>Ce rapport affiche tous les bénéfices éligibles au paiement, y compris les paiements qui n’ont pas encore été envoyés. Les bénéfices peuvent être facturés lorsqu’un ISV a effectué toutes les informations bancaires et fiscales de l’espace partenaires, a gagné >$50, le compte ISV est actif et le client a été facturé (pour les transactions EA) ou le paiement a été reçu (pour les transactions non-EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Présentation de la transaction.":::

- **Revenus envoyés cette année** : total des bénéfices et répartition des bénéfices qui ont été payés et seront payés dans le mois à venir.
- **Estimation du mois de paiement** – total des bénéfices attendus au cours des prochains mois.
- **Rémunérations et tendance des paiements** : montants mensuels de rémunération et de paiement pour les 36 derniers mois.
- **Télécharger** : Télécharger les détails de la transaction au format. csv ou. TSV.

Utilisez la sélection de plage de dates située dans le coin supérieur droit de la page pour filtrer la sortie de la page et afficher les 3, 6, 12 ou 36 mois précédents. Vous pouvez sélectionner une plage de dates personnalisée jusqu’à 36 mois. La plage de dates par défaut est 12 mois. Vous pouvez également filtrer par ID d’inscription, programme, ID de paiement, type de gain, levier et état. Les données sont disponibles pour l’exercice fiscal actuel (du 1er juillet au 30 juin) et dans les deux années fiscales précédentes.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Filtre de recherche en haut à droite de la page.":::

Pour afficher plus de détails sur un bénéfice, sélectionnez la flèche vers le bas située dans la partie droite de la page. Cela affichera le levier, le chiffre d’affaires, le produit et le client. Si, pour une raison quelconque, ces données ne sont pas disponibles, mais que vous avez besoin d’y accéder, contactez le support technique. Si le résultat est le résultat d’un ajustement et non d’une transaction, les champs produit et client ne s’affichent pas.

### <a name="transaction-history-summary"></a>Résumé de l’historique des transactions

Cet affichage présente les détails de l’offre, y compris l’origine des données acquises à partir du produit vendu, de l’État et du mois de paiement estimé.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historique des transactions.":::

- **Date d’audit** : date d’achat.
- **Type** de gain : le type de gain, par exemple la vente, la remise ou le co-op.
- **Montant total** : montant de l’obtention nette. Dans le Marketplace commercial, cela signifie qu’après déduction des frais standard de la place de marché.
- **État** : propose trois options :
    - À **venir** : les revenus sont en attente de période de refroidissement.
    - **Traité** : les bénéfices sont préparés pour le prochain paiement.
    - **Envoyé** : les revenus ont été payés.
- **Mois de paiement estimé** : le mois auquel les bénéfices sont payés. Pour plus d’informations, consultez la [section suivante](#estimated-payment-month) .

Les transactions en gain sont affichées une fois que la transaction respecte le droit au paiement. Pour comprendre la raison pour laquelle vous pouvez avoir des revenus manquants ou inattendus, consultez les [questions courantes sur le paiement](payout-faq.md#why-are-my-earnings-missing)de la place de marché commercial.

#### <a name="estimated-payment-month"></a>Mois de paiement estimé

La page historique des transactions comprend désormais un tableau qui indique le montant des paiements estimés pour les prochains mois. Vous pouvez également afficher et télécharger ces informations dans l’historique des transactions et les exportations du rapport de synthèse. Ces informations facilitent les réconciliations et les projections de paiement.

Le mois de paiement estimé est calculé en fonction des règles et des chronologies de la configuration du programme, et est traité dans le prochain cycle de paiement.

Le mois de paiement estimé est actuellement disponible pour tous les types de gains, à l’exception de la co-op, qui s’affichera comme **non applicable**. Pour les revenus antérieurs au 1er juillet 2020, le mois de paiement estimé apparaît comme étant **non disponible**.

Le tableau suivant montre un exemple de mois de paiement estimé.

| Month | Montant |
| ------ | :-----------: |
|  Sep-2020 |  $7 273,99   |
|  Oct-2020 | $8 692,30  |
|  Nov-2020 | $107,89  |

Le montant estimé peut varier par rapport à la quantité réelle pour diverses raisons :

- Réexécution de l’opération : si les bénéfices sont recalculés, le montant réel est différent.
- Ajustements : la quantité réelle varie en fonction des ajustements qui se sont produits ou qui ont été envoyés.
- Modification des règles : une modification des règles peut refléter le recalcul dans le montant réel payé
- Payable : si un échec de paiement se produit, le montant réel peut être différent.

Notez que votre paiement n’est publié que dans le mois projeté si le seuil et les règles d’éligibilité au paiement de votre programme sont atteints. Ces règles incluent, mais ne sont pas limitées à la liste ci-dessous :

- Votre profil fiscal doit être à jour
- Vos revenus doivent respecter ou dépasser le seuil minimal atteint défini dans le Guide de votre programme.
- Paiement en attente : Si vous sélectionnez l’option « conserver mon paiement » sur la page attribution des profils.
- Instrument de paiement non disponible : le paiement ou/et le profil fiscal n’est pas terminé.

### <a name="transaction-history-download"></a>Téléchargement de l’historique des transactions

Pour obtenir plus de détails sur un gain, sélectionnez **Télécharger** en haut de la page. Le tableau suivant décrit chaque colonne du rapport.

>[!NOTE]
>L’exportation du téléchargement de l’historique des transactions a deux nouveaux champs à partir du 2020 août :
>
>- **lastPaymentCurrency**  Devise dans laquelle le paiement le plus récent a été reçu, sur toutes les MPNs auxquelles le partenaire actuellement connecté a accès. Si aucun paiement n’est reçu, la dernière devise de paiement sera en dollars US.
>- **earningAmountInLastPaymentCurrency**  Montant acquis dans la dernière devise de paiement.

| Nom de la colonne | Description | Applicabilité des programmes d’incentives/places de marché |
| --- | --- | --- |
| agreementEndDate | Date de fin de l’accord | Incentives – certains programmes uniquement |
| agreementNumber | Numéro de l’accord | Incentives – certains programmes uniquement |
| agreementStartDate | Date de début de l’accord | Incentives – certains programmes uniquement |
| calculationDate | Date à laquelle le revenu a été calculé dans le système | Tous |
| claimId | Identificateur unique de la demande | Incentives – certains programmes uniquement |
| customerCountry | Pays/Région du client | marketplaces |
| customerEmail |  |  |
| customerName | Peut être vide | Programmes d’incentives uniquement (exception : OEM) et places de marché. Pour les transactions CSP, les Marketplaces affichent le nom du fournisseur de services de chiffrement. |
| customerTenantId |  |  |
| distributorId | Identificateur du serveur de distribution | Incentives – certains programmes uniquement |
| distributorName | Nom du serveur de distribution | Incentives – certains programmes uniquement |
| earningAmount | Montant du revenu dans la devise de la transaction d’origine | Tous |
| earningAmountInLastPaymentCurrency | Montant du revenu dans la dernière devise de paiement (ce champ est vide si aucun paiement antérieur n’a été effectué) |  |
| earningAmountUSD | Montant du revenu en USD | Tous |
| earningDate | Date du revenu | Tous |
| earningExchangeRate | Taux de change utilisé pour afficher le montant USD correspondant | Tous |
| earningId | Identificateur unique de chaque revenu | Tous |
| earningRate | Taux d’incentives appliqué au montant de la transaction pour générer un gain | Tous |
| earningType | Indique s’il s’agit de frais, d’une remise, d’une coopération, d’une vente, etc. | Tous |
| exchangeRateDate | Date du taux de change utilisée pour calculer le montant USD du revenu | Tous |
| externalReferenceId | Identificateur unique du programme | Programmes de paiement direct (incentives et places de marché) |
| externalReferenceIdLabel | Étiquette de l’identificateur unique | Programmes de paiement direct (incentives et places de marché) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Numéro de facture (applicable uniquement aux entreprises) | Incentives et places de marché-certains programmes uniquement |
| lastPaymentCurrency | Dernière devise de paiement (ce champ est vide si aucun paiement antérieur n’a été effectué) |  |
| lever | Indique une règle métier pour le revenu | Tous |
| LicensingProgramName | Nom du programme de licence |  |
| LineItemId | Ligne individuelle dans la facture d’un client |  |
| localProviderSeller | Fournisseur local/vendeur d’enregistrement |  |
| Mois de maturité | Le mois de paiement estimé | Tout |
| OrderId | Lié à la facture d’un client  | marketplaces |
| parentProductId | Identificateur de produit parent unique. S’il n’existe aucun produit parent pour la transaction, l’ID du produit parent = ID du produit. | marketplaces |
| parentProductName | Nom du produit parent. S’il n’existe aucun produit parent pour la transaction, le nom du produit parent = Nom du produit. | marketplaces |
| participantId | Identité principale du revenu partenaire dans le cadre du programme | Tous |
| participantIdType | Principalement l’ID de programme pour les programmes d’incentives et le vendeur pour les places de marché | Tous |
| participantName | Nom du partenaire de revenu | Tous |
| partnerCountryCode | Lieu/pays/région du partenaire de revenu | Tous |
| partNumber | Sera toujours vide | Certains programmes et places de marché incitants |
| paymentId | Identificateur unique permettant de mettre en corrélation toutes les transactions dans le rapport de transaction avec un paiement spécifique dans le rapport de paiement | Tout |
| paymentStatus | État du paiement | Tous |
| paymentStatusDescription | Description conviviale de l’état du paiement | Tous |
| productId | Identificateur de produit unique | marketplaces |
| ProductName | Nom du produit lié à la transaction | Tout |
| productType | Type de produit (par exemple, application, module complémentaire ou jeu) | marketplaces |
| Code du programme | Chaîne à mapper avec le nom du programme |  |
| programName | Nom du programme d’incentives/du Store | Tous |
| purchaseOrderCoverageEndDate | Sera toujours vide | Programme d’incentives – AGI |
| purchaseOrderCoverageStartDate | Sera toujours vide | Programme d’incentives – AGI |
| purchaseOrderType | Sera toujours vide | Programme d’incentives – AGI |
| purchaseTypeCode | Sera toujours vide | Programme d’incentives – AGI |
| quantité | Varie selon le programme. Indique la quantité facturée pour les programmes transactionnels | Tous |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identificateur du revendeur | Incentives – certains programmes uniquement |
| resellerName | Nom du revendeur |  |
| SkuId | ID de la référence SKU, tel que défini lors de la publication. Une offre peut englober de nombreuses références SKU, mais une référence SKU ne peut être associée qu’à une seule offre. Incentives – certains programmes uniquement |  |
| storeFee | Montant retenu par Microsoft en guise de frais pour la mise à disposition de l’application ou du module complémentaire sur le Store | marketplaces |
| subscriptionEndDate | Date de fin de l’abonnement | Incentives – certains programmes uniquement |
| subscriptionId | Identificateur d’abonnement associé au client | Incentives – certains programmes uniquement |
| subscriptionStartDate | Date de début de l’abonnement | Incentives – certains programmes uniquement |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Tiers responsable du versement des taxes (ventes, consommation ou TVA/GST) | marketplaces |
| taxRemitted | Montant des taxes versées (ventes, consommation ou TVA/GST) | marketplaces |
| taxState | État du client |  |
| taxZipCode | Code postal du client |  |
| tpan | Indique le réseau publicitaire tiers | Annonces de la place de marché uniquement |
| transactionAmount | Montant de la transaction dans la devise de transaction d’origine en fonction du revenu généré | Tous |
| transactionAmountUSD | Montant de la transaction en USD | Tous |
| transactionCountryCode | Code du pays/région dans lequel la transaction s’est produite |  |
| transactionCurrency | Devise dans laquelle la transaction du client d’origine a été effectuée (il ne s’agit pas de la devise locale du partenaire) | Tous |
| transactionDate | Date de la transaction Utile pour les programmes où de nombreuses transactions contribuent à un revenu | Tous |
| transactionExchangeRate | Date du taux de change utilisé pour afficher le montant en USD correspondant de la transaction | Tous |
| transactionId | Identificateur unique de la transaction | Tous |
| transactionPaymentMethod | Moyen de paiement client utilisé pour la transaction (par exemple, carte, facturation d’opérateur de téléphonie mobile ou PayPal) | marketplaces |
| transactionType | Type de transaction (par exemple achat, remboursement, contrepassation ou rétrofacturation) | marketplaces |
| charge de travail | Charge de travail | Incentives – certains programmes uniquement |
|

### <a name="transaction-adjustment-codes"></a>Codes de réglage des transactions

Le tableau suivant répertorie les codes de raison des ajustements et leurs descriptions.

|**Code de raison**   |**Description**   |
|------------------|:-------------------------------------|
| Conformité AR | Ajustement qui réduit les bénéfices lorsque les factures Microsoft ne sont pas payées à temps par le partenaire. |
| Substitution de co-op | Ajustement qui transfère les bénéfices de la coopération vers une autre période ou qui convertit les bénéfices de la co-op en remise. |
| Ajustement des opérations | Ajustement qui corrige les erreurs de calcul du système Microsoft. |
| Ajustement OPS Microsoft incorrect Calc | Ajustement qui corrige les incorrections. |
| Ajustement OPS Microsoft incorrect | Ajustement pour les calculs incalculés liés à l’inscription. |
| Mappage des partenaires (abonnement) MCI/CSP | Ajustement qui corrige le mauvais alignement de l’abonnement. |
| Exception de stratégie | Ajustement qui remplace une règle de programme.  |
| Bénéfice sur la période précédente | Ajustement pour les bénéfices en dehors de la période de gains en cours. |

## <a name="payments"></a>Paiements

La page **paiements** détaille l’argent que vous avez obtenu auprès de Microsoft. Il indique également à quel moment et dans quelle mesure vous allez être payé.

>[!Note]
> Pour être éligible au paiement, votre produit doit atteindre le [seuil de paiement](payment-thresholds-methods-timeframes.md) de 50 $. Pour plus d’informations, consultez le [contrat Microsoft Publisher](/legal/marketplace/msft-publisher-agreement).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Écran de présentation des paiements.":::

- **Total payé cette année** : le total cumulé payé pour vous cette année, en dollars américains, pour tous vos programmes.
- **Prochain paiement estimé** : le seul paiement suivant qui vous vient (même s’il y en a d’autres disponibles prochainement), en dollars américains.
- **Dernier paiement** : montant (en dollars américains), nom du programme et programme de votre paiement le plus récent.
- **Paiement par source** – montant des paiements (en dollars américains), par programme, au cours des 12 derniers mois.

### <a name="payments-list"></a>Liste des paiements

La table **de la liste des paiements** affiche les paiements payés et en attente. Vous pouvez télécharger les informations fiscales sur les frais de service au format PDF et afficher les détails d’un paiement donné.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exporter l’historique des transactions":::

- **Payant** : tous les paiements envoyés avec succès. Choisissez l’année dans le menu déroulant pour filtrer sur les paiements lancés au cours de cette année.
- **En attente** : paiements à venir.
- **Taxe sur les frais de service (formulaire PDF)** : disponible pour les paiements soumis à un impôt sur les frais de service. Les taxes sur les frais de service sont indiquées dans d' **autres taxes**.
- **Afficher** : redirige vers l’historique des transactions avec une liste des revenus inclus dans le paiement.

Pour comprendre la raison pour laquelle vous pouvez avoir des revenus manquants ou inattendus, consultez les [questions courantes sur le paiement](payout-faq.md#why-are-my-earnings-missing)de la place de marché commercial.

### <a name="payment-status"></a>État du paiement

Le tableau suivant décrit les différents États de gains.

| État du bénéfice | Motif | Intervention nécessaire du partenaire ? |
| --- | --- | --- |
| Non traité | Le revenu est éligible au paiement. Il reste dans cet État pour une période de refroidissement telle que définie dans le Guide du programme pour les incentives. | Non |
| À venir | Commande de paiement générée en attente de révisions internes avant le traitement du paiement. | Non |
| Facture fiscale en attente | Votre facture fiscale est incomplète ou non valide. | Vous devez mettre à jour votre facture fiscale avant de pouvoir être payé |
| Rejeté pendant la vérification | Le paiement a été rejeté pendant la révision. | Contactez le Support Microsoft pour obtenir des détails |
| Échec | Le paiement a échoué en raison d’une erreur système Microsoft. | Contacter le support Microsoft pour plus d’informations |
| En cours | Le paiement est en cours. | Non |
| Paiement incorrect | Le remboursement est en cours. | Non |
| Envoyé | Le paiement a été envoyé à votre banque. | Non |
| Retraitement | Le paiement a rencontré une erreur système Microsoft et est en cours de retraitement. | Non |
| Inversé | Le paiement a été inversé par votre banque et sera renvoyé dans le prochain cycle de paiement. | Non |
| Facture fiscale rejetée | Votre facture fiscale a été rejetée pendant la vérification. Tous les paiements en attente seront mis en attente tant que l’examen de la facture fiscale n’aura pas été effectué. | Contacter le support Microsoft pour plus d’informations |
| Facture fiscale en cours de vérification | Votre facture fiscale est en cours de vérification. Votre paiement sera débloqué une fois que la facture fiscale aura été approuvée. | Non |
| Rejeté | Le paiement a été rejeté par votre banque. | Contactez votre banque pour obtenir des détails. |
|

### <a name="payments-download"></a>Paiements téléchargés

 Le tableau suivant décrit chaque colonne du rapport. Pour obtenir plus de détails sur vos paiements, sélectionnez **Télécharger** en haut de la page paiements.

| Nom de la colonne | Description |
| --- | --- |
| participantID | Identité principale du revenu partenaire dans le cadre du programme |
| participantIDType | En général, ID de programme pour les programmes d’incentives et l’ID de vendeur pour les programmes Store |
| participantName | Nom du partenaire de revenu |
| programName | Incentives/nom du programme de stockage |
| earned | Montant du chiffre d’affaires dans la devise d’arrivée pour le programme/ID de participant en question |
| earnedUSD | Montant de chiffres d’affaires enregistré pour le programme/ID de participant, en USD |
| withheldTax | Montant des taxes retenues dans la devise d’arrivée pour le programme/ID de participant |
| salesTax | Montant total des taxes dans le paiement à la devise pour le programme/participantID (applicable aux programmes d’incentives uniquement) |
| serviceFeeTax | Montant total de serviceFeeTax dans la devise d’arrivée pour le programme/ID de participant (s’applique uniquement aux programmes du Store et à la Place de marché Azure) |
| totalPayment | Paiement total dans la devise locale à l’exclusion de la retenue à la source et en incluant les taxes sur les ventes (le cas échéant) pour le programme/ID de participant |
| currencyCode | Code de la devise d’arrivée |
| paymentMethod | Mode de paiement utilisé pour payer le partenaire, par exemple, le virement bancaire électronique, l’avoir |
| paymentId | Identificateur unique du paiement. Ce numéro figure généralement sur votre relevé bancaire (s’applique uniquement aux paiements SAP). |
| paymentStatus | État du paiement |
| paymentStatusDescription | Description conviviale de l’état du paiement |
| paymentDate | Date à laquelle le paiement a été envoyé par Microsoft |
|

## <a name="export-data"></a>Exporter des données

La page **exporter des données** n’est pas actualisée automatiquement. Vous devrez peut-être l’actualiser manuellement pour afficher les données les plus récentes. Sélectionnez l’un des trois onglets pour exporter l' **historique des transactions**, les **paiements**, le résumé de la **transaction** ou l' **instruction historique**.

Votre filtre peut entraîner une erreur **aucune donnée n’est disponible** . Cela peut se produire si vous avez laissé la période de temps par défaut sélectionnée à trois mois, puis sélectionné un ID de paiement d’un produit en dehors de cette période. Si cela se produit, augmentez votre période et réessayez.

Voici un exemple d’exportation de paiements :

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Exporter le rapport de paiements.":::

### <a name="historical-statements"></a>Instructions historiques

Le résumé des **données d’exportation** permet également d’accéder aux instructions historiques.

> [!NOTE]
> Une instruction historique est un instantané et n’est pas actualisée. Contactez le [support technique](https://partner.microsoft.com/support/v2/?stage=1) et demandez les données les plus récentes si nécessaire.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportez les instructions historiques.":::

- L’historique des transactions avant le 1er juillet 2019 est géré séparément et utilise des champs différents des rapports historiques ultérieurs.
- L’historique des transactions héritées comporte une colonne appelée « réservé » qui correspond à la colonne « bénéfices » dans l’historique moderne, sauf qu’elle exclut tous les bénéfices dont l’État est égal à « paiement envoyé ».
- Les filtres 3 mois, 6 mois ou 12 mois ne s’appliquent pas à la section Instructions historiques.

### <a name="historical-statement-downloads"></a>Téléchargement des instructions historiques

Le tableau suivant décrit chaque colonne dans une instruction historique.

| Nom du champ | Description |
| --- | --- |
| Source du chiffre d’affaires | Source de votre chiffre d’affaires en fonction de l’origine de la transaction (par exemple, Microsoft Store, Windows Phone Store, Windows Store 8 ou publicité) |
| ID de commande | Identificateur de commande unique. Cet ID vous permet d’identifier les transactions d’achat avec leurs transactions de non-achat respectives, comme les remboursements ou les rétrofacturations. Les deux ont le même ID de commande. De même, s’il existe un coût de fractionnement dans lequel plusieurs modes de paiement ont été utilisés pour un seul achat, vous pouvez lier les transactions d’achat. |
| ID de transaction | Identificateur de transaction unique. |
| Date et heure de la transaction | Date et heure auxquelles la transaction a eu lieu (UTC). |
| ID du produit parent | Identificateur de produit parent unique. S’il n’existe aucun produit parent pour la transaction, l’ID du produit parent = ID du produit. |
| Product ID | Identificateur de produit unique. |
| Nom du produit parent | Nom du produit parent. S’il n’existe aucun produit parent pour la transaction, le nom du produit parent = Nom du produit. |
| Nom du produit | Nom du produit |
| Type de produit | Type de produit (par exemple, application, module complémentaire ou jeu) |
| Quantité | Quand la source du chiffre d’affaires est le Microsoft Store pour Entreprises, la Quantité représente le nombre de licences achetées. Pour toutes les autres sources de chiffre d’affaires, la Quantité est toujours égale à 1. Même quand une même transaction est fractionnée en deux lignes en raison de l’utilisation de deux modes de paiement, chaque ligne présente une Quantité égale à 1. |
| Type de transaction | Type de transaction (par exemple, achat, remboursement, contrepassation ou rétrofacturation) |
| Mode de paiement | Moyen de paiement client utilisé pour la transaction (par exemple, carte, facturation d’opérateur de téléphonie mobile ou PayPal) |
| Pays/région | Pays/région où la transaction a eu lieu |
| Fournisseur local/vendeur | Fournisseur local/vendeur d’enregistrement |
| Devise de la transaction | Devise de la transaction |
| Montant de la transaction | Montant de la transaction |
| Taxes versées | Montant des taxes versées (ventes, consommation ou TVA/GST) |
| Encaissements nets | Montant de la transaction moins les taxes versées |
| Frais du Store | Pourcentage des encaissements nets retenu par Microsoft en guise de frais pour la mise à disposition de l’application ou du module complémentaire sur le Store |
| Revenus des applications | Encaissements nets moins les frais du Store |
| Taxes retenues | Montant d’impôt sur le revenu retenu (inclus dans le fichier CSV **Réservé**) |
| Paiement | Revenus des applications moins la retenue à la source éventuellement applicable (montant affiché dans Devise de la transaction). Non inclus dans le fichier CSV **Réservé**. |
| Taux de change | Taux de change utilisé pour convertir la devise de la transaction en devise de paiement |
| Devise de paiement | Devise dans laquelle votre paiement est effectué |
| Paiement converti | Montant du paiement converti en devise de paiement en utilisant le taux de change |
| Modèle de paiement des taxes | Tiers responsable du versement des taxes (ventes, consommation ou TVA/GST) |
| Date et heure d’éligibilité | Date et heure auxquelles le produit de la transaction devient éligible au paiement (UTC). Quand un paiement est créé, il comprend le produit de la transaction avec une date et heure d’éligibilité antérieures à la date de création du paiement (uniquement inclus dans le fichier CSV **Réservé**). |
| Charges | Présente une décomposition de tous les détails de charges agrégés dans la colonne Montant de la transaction (uniquement incluse pour la Place de marché Azure ; non incluse dans le fichier CSV **Réservé**). |
|||

## <a name="next-steps"></a>Étapes suivantes

- [API de paiement partenaire](https://apidocs.microsoft.com/services/partnerpayouts)
- [Détails de la politique de paiement](payout-policy-details.md)
- Pour obtenir de l’aide sur la facturation, contactez le [support éditeur](https://partner.microsoft.com/support/v2/?stage=1) de la Place de marché commerciale.