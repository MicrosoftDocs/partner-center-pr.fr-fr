---
title: Différences de facturation mensuelle et annuelle | Espace partenaires
ms.topic: article
ms.date: 11/25/2019
Description: En savoir plus sur les différences entre les cycles de facturation mensuel et annuel dans l’espace partenaires.
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: a05f64ac919cce0339f0033fa38a4b43e61d3c08
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390308"
---
# <a name="monthly-and-annual-billing-differences"></a>Différences de facturation mensuelle et annuelle

**S’applique à**

- Centre pour partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Agent d’administration
- Administration de facturation
- Administrateur global
- Administrateur de primes incitatives
- Utilisateur de primes incitatives
- Agent du support technique
- Commercial

Cette rubrique explique les différences entre la **facturation mensuelle** et la **facturation annuelle** dans l’espace partenaires, y compris les avantages et les cas d’usage. Vous avez la possibilité de payer certains abonnements de fournisseur de solutions Cloud (CSP) sur une base mensuelle ou annuelle.

## <a name="applicability"></a>Applicabilité

La plupart des abonnements basés sur une licence ont la possibilité d’utiliser l’option de facturation mensuelle ou annuelle. Les abonnements basés sur l’utilisation proposent uniquement une facturation mensuelle.

La facturation annuelle et mensuelle sont **par abonnement**, et  ***non* par licence**.

### <a name="find-subscription-applicability"></a>Rechercher l’applicabilité de l’abonnement

Vous pouvez identifier les fréquences de facturation disponibles pour chaque offre à l’aide de la colonne J de la matrice d’offre. Vous pouvez trouver la matrice d’offre dans la section **voir les offres et la tarification** de l’espace partenaires.

### <a name="applicable-partners"></a>Partenaires applicables

Tous les partenaires et types de partenaires peuvent choisir une facturation mensuelle ou annuelle.

### <a name="applicable-markets"></a>Marchés applicables

La facturation mensuelle et annuelle (pour les offres applicables) est disponible sur tous les marchés où le programme CSP est actuellement disponible.

## <a name="change-billing-frequency"></a>Changer la fréquence de facturation

Vous pouvez basculer entre chaque facture mensuelle et annuelle à tout moment. Vous pouvez modifier la fréquence de facturation si les besoins de votre entreprise évoluent.

Lorsque vous modifiez la fréquence de facturation à annuelle, le terme annuel est mis à jour pour refléter la date à laquelle vous avez modifié la fréquence de facturation. Une nouvelle date de renouvellement est également établie.

### <a name="monthly-to-annual-billing"></a>Facturation mensuelle à la facturation annuelle

Passer de la facturation mensuelle à la facturation annuelle peut être utile si vous avez plusieurs abonnements facturés tous les mois. Lorsque vous basculez vers la facturation annuelle, vous pouvez aligner les abonnements sur une date de facturation commune.

### <a name="annual-to-monthly-billing"></a>Facturation annuelle/mensuelle

Passer de la facturation annuelle à la facturation mensuelle peut être utile si vous souhaitez ajuster vos dates de facturation à celles de vos clients individuels.

## <a name="annual-billing"></a>Facturation annuelle

La facturation annuelle présente les avantages suivants :

- Flexibilité accrue en matière d'options de paiement.
- Meilleur alignement avec la facturation de vos clients.
- Réduction de l'impact des fluctuations de devises.
- Réduction des coûts d’exploitation en matière de facturation.

### <a name="configure-annual-billing"></a>Configurer la facturation annuelle

Si vous envisagez de passer à la facturation annuelle dans l’espace partenaires, veillez à prendre en compte la façon dont votre mouvement de vente sera affecté. Vous devez informer votre équipe et mettre à jour vos processus internes si nécessaire. Vous devez également passer en revue les modifications apportées à votre facture et à votre fichier de réconciliation basé sur une licence. 

Vous devrez également mettre à [jour vos API pour la facturation annuelle](#required-api-changes).

#### <a name="required-api-changes"></a>Modifications requises de l’API

Pour tirer parti de la facturation annuelle, certaines modifications de vos API sont nécessaires.

- [Order. BillingCycle, propriété](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Créer une commande](https://docs.microsoft.com/partner-center/develop/create-an-order)

Pour plus d’informations sur les API de l’espace partenaires, voir toutes les [ressources et la documentation du développeur de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placement des commandes

Le type de fréquence de facturation, y compris l’option de facturation annuelle, est affecté à l' **offre** en tant qu’attribut. Il n’existe pas d’offre unique spécifique pour les commandes avec facturation annuelle. Toutefois, vous pouvez donner à une offre un nom plus explicite pour aider les clients à faire facilement la distinction.

### <a name="select-annual-billing"></a>Sélectionner la facturation annuelle

Lorsque vous ajoutez un nouvel abonnement, vous êtes invité à choisir la fréquence de facturation. Vous pouvez choisir l’option de facturation annuelle à ce stade. Lorsque vous sélectionnez la facturation annuelle, toutes les offres disponibles s’affichent.

### <a name="billing-time"></a>Heure de facturation

Vous serez facturé à votre date de facturation suivante. Par exemple, si votre date de facturation est le 1er du mois et que vous achetez un abonnement facturé annuellement le 29 octobre 2019, vous êtes facturé le 1er novembre 2019. En supposant que vous n’apportez aucune modification de licence, vous êtes facturé à nouveau le 1er novembre 2020. Si vous apportez une modification de licence, vous recevrez un crédit et refacturera à la prochaine date de facturation.

### <a name="annual-renewals"></a>Renouvellements annuels

La date de renouvellement de votre abonnement sera de douze mois après la date de début du service. La période de service commence à la date de création de l’abonnement.  Par exemple, un abonnement créé le 10 janvier 2019 est renouvelé le 10 janvier 2020.

Vous serez facturé à la prochaine date de facturation qui suit la date de renouvellement de l’abonnement. Par exemple, si vous achetez un abonnement à facturation annuelle le 15 janvier 2018 et que votre date de facturation est le 20 janvier, votre abonnement sera renouvelé le 15 janvier 2019. Vous serez facturé pour le renouvellement le 20 janvier 2019.

### <a name="split-subscription-billing-frequency"></a>Fréquence de facturation de fractionnement d’abonnement

Il n’est pas possible de fractionner un **seul abonnement** de sorte qu’une partie soit facturée chaque mois et que l’autre partie soit facturée annuellement. L’abonnement entier doit avoir la même fréquence de facturation (facturation mensuelle ou annuelle).

Pour les clients avec **plusieurs abonnements** de la même offre, il peut être possible d’avoir différentes fréquences de facturation par abonnement. Certaines offres sont limitées à un abonnement par client. Si l’offre n’est pas limitée, un client peut avoir plusieurs abonnements d'une même offre avec des fréquences de facturation différentes. Vous trouverez les détails des limites et restrictions de chaque offre dans la colonne I du tableau des offres. Vous pouvez trouver la matrice d’offre dans la section **voir les offres et la tarification** de l’espace partenaires.

### <a name="free-subscription-period"></a>Période d’abonnement gratuite

Les abonnements avec une fréquence de facturation annuelle ne bénéficient pas d’une période gratuite. La durée payée de douze mois commence à la date d’achat. Ces conditions diffèrent de celles des abonnements à fréquence de facturation mensuelle qui bénéficient d'une période gratuite entre la date d’achat et la date de facturation qui suit.

### <a name="adding-and-removing-licenses"></a>Ajout et suppression de licences

Vous pouvez modifier le nombre de licences de vos abonnements à tout moment. L'ajout de licences supplémentaires n’aura aucune incidence sur la fréquence de facturation.

Vous pouvez à tout moment ajouter ou supprimer des licences.  Vous recevrez un crédit et une facture au prorata à la date de facturation suivante après avoir modifié le nombre de licences.

Si votre abonnement existant a une facturation annuelle, il n’est pas possible d’ajouter des licences avec facturation mensuelle à cet abonnement. Une fois que vous achetez un abonnement à facturation annuelle, toutes les licences supplémentaires respecteront la même fréquence de facturation. Si par la suite vous devez acheter des licences à facturation mensuelle, vous devrez acheter un nouvel abonnement.

### <a name="add-on-offers"></a>Offres complémentaires

L'abonnement au module complémentaire aura automatiquement la même fréquence de facturation que l’abonnement parent. La facturation annuelle est disponible pour les offres complémentaires. 

### <a name="cancelling-subscriptions"></a>Annulation des abonnements

La politique d’annulation est la même pour toutes les fréquences de facturation.

Pour la facturation annuelle, si l’abonnement est annulé au cours des 30 premiers jours de la période de 12 mois payée, vous recevrez un crédit de 100% à la prochaine date de facturation. Si l’abonnement est annulé après 30 jours de la période de 12 mois payée, vous recevrez un crédit au prorata à la prochaine date de facturation.

### <a name="moving-subscriptions-between-partners"></a>Déplacement d’abonnements entre partenaires

Les clients ne peuvent pas déplacer des abonnements d’un partenaire à un autre. Cela s’applique aussi bien aux abonnements à facturation mensuelle qu'annuelle.

Le nouveau partenaire doit acheter un nouvel abonnement pour le compte du client. Il n’est pas possible de déplacer des abonnements entre partenaires.

### <a name="reactivating-subscriptions"></a>Réactivation des abonnements

Vous pouvez réactiver un abonnement jusqu’à 90 jours après la date de la suspension. Les frais calculés au prorata seront facturés à la date de facturation suivante. La date de renouvellement de l’abonnement reste identique.

## <a name="pricing"></a>Tarification

### <a name="offer-pricing"></a>Tarifs de l’offre

Le prix de l’offre au moment de l’achat est garanti pour la durée de l’abonnement facturé complet (un mois pour la facturation mensuelle, 12 mois pour la facturation annuelle). Lors du renouvellement d’un abonnement, le prix est basé sur la liste des prix en vigueur à la date du renouvellement. Le nouveau prix est garanti pour la période d’abonnement suivante.

Si le prix d’une offre diminue au cours de la période de facturation, le montant facturé ne change pas. Le prix est défini pour la période de facturation complète au moment de l’achat. Cela s’applique à la facturation mensuelle et annuelle.

### <a name="cancellation-credits"></a>Crédits d’annulation

Le crédit pour une licence ou un abonnement annulé est calculé comme suit :

**Crédit d’annulation** = ((* * prix mensuel * * * 12)/365) \* **jours restants dans le délai de douze mois** \* nombre de licences annulées.

## <a name="reconciliation-file"></a>Fichier de rapprochement

### <a name="find-subscriptions-billing-frequency"></a>Rechercher la fréquence de facturation de l’abonnement

Passez en revue votre fichier de réconciliation basé sur les licences pour savoir si votre abonnement est facturé mensuellement ou annuellement. Ces informations se trouvent dans la colonne **AA**.

Pour savoir si vous pouvez modifier un abonnement mensuel à la facturation annuelle, voir [Rechercher l’applicabilité](#find-subscription-applicability)de l’abonnement.

### <a name="reconciliation-file-changes-for-annual-billing"></a>Modifications des fichiers de rapprochement pour la facturation annuelle

Lorsque vous achetez ou renouvelez un abonnement avec la facturation annuelle, votre fichier de réconciliation basé sur les licences sera modifié comme suit.

Une nouvelle ligne sur le fichier de réconciliation basé sur les licences, à la date de la première facturation suivant l’achat ou un nouvel abonnement.

Si aucune modification n'est apportée à l’abonnement, aucune ligne n'apparaît sur les fichiers de rapprochement pour les mois 2 à 12 de la période d'abonnement. Si une modification est apportée à l’abonnement au cours de la période de douze mois, un crédit et une facture au prorata s’affichent dans le prochain fichier de rapprochement une fois la modification effectuée.

La modification suivante du fichier de rapprochement s’affiche lorsque l’abonnement est renouvelé. Elle s’affiche à la première date de facturation qui suit le renouvellement.

### <a name="usage-file-changes-for-annual-billing"></a>Modifications du fichier d’utilisation pour la facturation annuelle

Les modifications de l’abonnement facturé annuel suivant apparaissent dans la colonne P de votre fichier d’utilisation.

- **Frais liés au prorata en cas d’achat**: l’achat initial d’un abonnement annuel.
- **Taux**de l’instance de cycle : modification de la licence entraînant un crédit et une refacturation.
- **Frais d’annulation**: [annulation d’un abonnement annuel](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Annulation de l’abonnement annuel

Lors de l’annulation d’un abonnement facturé annuellement, le fichier de réconciliation contient un article pour un crédit d’annulation.

Si l’annulation se produit au cours des 30 premiers jours de la période de 12 mois, l’abonnement sera crédité à 100%. Si l’annulation se produit après les 30 premiers jours, l’abonnement sera crédité au prorata.

### <a name="adding-licenses-to-annual-subscription"></a>Ajout de licences à l’abonnement annuel

Lorsque vous ajoutez des licences à un abonnement, le fichier de réconciliation contient un crédit et une facture au prorata. Cela s’applique aux abonnements mensuels et annuels.

### <a name="price-lists-for-annual-billing"></a>Tarifs pour la facturation annuelle

Les tarifs de l’espace partenaires affichent les tarifs mensuels. Aucun prix annuel n’est indiqué. Vous pouvez calculer le prix annuel en multipliant le prix mensuel par douze.

### <a name="offer-matrix"></a>Matrice d’offre

Les ID d’offre dans la matrice d’offre sont les mêmes pour toutes les fréquences de facturation. Il n’existe pas d’ID unique pour les offres qui peuvent être facturées annuellement.

## <a name="incentives"></a>Primes incitatives

### <a name="incentives-calculation"></a>Calcul des incentives

Les incentives sont calculés en fonction du **chiffre d’affaires facturé**et  ***non* du revenu ajusté**. Les paiements des primes obtenues seront versés conformément à notre stratégie présentée dans nos guides des primes du programme Fournisseur de solutions Cloud.

Lorsqu’un abonnement facturé annuellement est vendu, le chiffre d’affaires de cet abonnement est reconnu pour le calcul des incentives sur la base du chiffre d’affaires facturé.

### <a name="payout"></a>Paiement

Actuellement, tous les paiements d’incentives sont effectués deux fois par an. Ces paiements sont versés 45 jours après la fin du semestre.

### <a name="rates"></a>Tarifs

Les partenaires gagnent des incentives sur toutes les transactions éligibles, quel que soit le mode de facturation d’un abonnement. Les revenus des incentives sont calculés en fonction du taux d’incentives global (qui est appliqué au revenu facturé pour la période), de l’accélérateur local (pour toutes les zones géographiques dans lesquelles il existe des accélérateurs locaux) et de toute campagne globale (le cas échéant).

### <a name="contacts"></a>Contacts

Pour toute question sur les incentives, contactez l’équipe de support technique régional appropriée :

| Région | Adresse électronique |
| ------ | ------------- |
| Amérique du Nord | <ocina@microsoft.com> |
|Amérique latine & Brésil | <ocilatam@microsoft.com> |
| MOYEN | <ociemea@microsoft.com> |
| APOAC (à l’exception du Japon) | <ociapgc@microsoft.com> |
| Japan | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspendu

Si vous suspendez un abonnement (dans l’espace partenaires ou via les API) dans les 30 jours suivant votre achat, vous recevrez un crédit de 100%, quelle que soit la fréquence de facturation.

Pour la facturation annuelle :

1. Le partenaire achète l’abonnement le 1er janvier. Une ligne facture facturation est créée pour la période de service du 1er janvier au 31 décembre.
2. Le partenaire interrompt l’abonnement le 25 janvier. Une ligne de facturation de crédit est créée pour la période de service du 1er janvier au 31 décembre.
3. Réactive l’abonnement le 29 janvier. Une ligne facture facturation est créée pour la période de service du 29 janvier au 31 décembre.

Pour la facturation mensuelle :

1. Le partenaire achète l’abonnement le 1er janvier. Une ligne facture facturation est créée pour la période de service du 1er janvier au 31 janvier.
2. Le partenaire interrompt l’abonnement le 25 janvier. Une ligne de facturation de crédit est créée pour la période de service du 1er janvier au 31 janvier.
3. Le partenaire réactive l’abonnement le 29 janvier. Une ligne facture facturation est créée pour la période de service du 29 janvier au 31 janvier.
