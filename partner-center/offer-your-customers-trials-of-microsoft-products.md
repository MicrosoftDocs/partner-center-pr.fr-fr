---
title: Offrir aux clients des versions d’évaluation des produits Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Permettez aux clients d’essayer les produits d’abonnement Microsoft pendant 30 jours. Inscrivez-vous à ces versions d’évaluation gratuites dans le catalogue, comme beaucoup d’autres services en ligne.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151132"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Offrez aux clients une version d’essai gratuite de 30 jours des produits Microsoft

**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent des ventes

Un bon moyen d’introduire des clients auprès de nouveaux produits Microsoft est d’offrir des versions d’évaluation gratuites de 30 jours. Vous pouvez vous inscrire aux versions d’évaluation du catalogue comme beaucoup d’autres services en ligne. Tous les partenaires peuvent participer.

## <a name="available-trial-offers"></a>Offres d’essai disponibles

Vous trouverez toutes vos offres d’essai en suspens sur la page du **client** . Cette page répertorie tous les abonnements, y compris les versions d’évaluation gratuites et les abonnements payants. (Cette fonctionnalité n’est actuellement pas disponible en Chine.)

Chaque client bénéficie d’un essai gratuit pour chaque offre disponible. Par exemple, ils peuvent obtenir une version d’évaluation gratuite pour Microsoft 365 Business standard et une version d’évaluation gratuite pour Office 365 E3. Toutefois, si le client possède déjà l’offre, il ne peut pas utiliser une version d’évaluation gratuite pour cette offre.

### <a name="available-products"></a>Produits disponibles

Des versions d’évaluation gratuites sont disponibles pour les offres licesen les plus complètes et les plus populaires. De nouvelles offres d’essai peuvent être présentées sur une base mensuelle.

Les partenaires peuvent trouver des versions d’évaluation dans la liste des prix mensuels sur la page **tarification et offres** de l’espace partenaires. Les offres d’essai comporteront la valeur « version d’évaluation » dans la colonne **type de licence secondaire** de la liste de prix.

Actuellement, il n’y a **pas d’essai gratuit** pour les offres gouvernementales, les offres de formation ou les offres complémentaires.

## <a name="licenses-for-free-trial-offers"></a>Licences pour les offres d’essai gratuit

Tous les essais gratuits proposent 25 licences. Vous ne pouvez pas modifier ce nombre au cours de la période d’évaluation. Vous ne pouvez pas ajouter ou supprimer des licences dans la version d’évaluation gratuite. Une fois la version d’évaluation convertie en abonnement payant, vous pouvez ajouter des licences supplémentaires à l’abonnement.

Les licences d’essai doivent être affectées aux utilisateurs de la même façon que la licence des services payants est attribuée.

## <a name="sign-customers-up-for-trials"></a>Signer les clients pour les versions d’évaluation

Obtenir une version d’évaluation de votre client dans l’espace partenaires :

1. À partir de la **vente** dans l’espace partenaires, accédez au **catalogue**. 
2. Dans le catalogue, dans **fréquence de facturation**, sélectionnez **offre d’essai**. Cela permet d’afficher uniquement les versions d’évaluation gratuites et de désactiver les autres offres qui ne sont pas gratuites. Les versions d’évaluation s’affichent sous l’onglet **essais** du catalogue.
3. Sélectionnez la version d’évaluation gratuite que vous souhaitez proposer, puis sélectionnez **Envoyer**. Tous les essais sont effectués pendant 30 jours pendant lesquels vous ne serez pas facturé. Vous pouvez également le convertir en abonnement payant à tout moment pendant la période d’évaluation.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversion des versions d’évaluation en abonnements payants

Une version d’évaluation gratuite n’est pas automatiquement convertie en abonnement payant. Après 30 jours, une version d’évaluation gratuite doit être convertie en abonnement payant ou [expire](#expiring-offers). Les versions d’évaluation gratuites ne peuvent pas être étendues.

Vous devez convertir votre version d’évaluation en abonnement payant. Pour ce faire, vous pouvez [utiliser l’espace partenaires](#convert-trials-using-partner-center) ou [les API de l’espace partenaires](#convert-trials-using-apis).

> [!NOTE]
> Les versions d’évaluation gratuites du client pour le programme du fournisseur de solutions Cloud (CSP) ne peuvent pas être converties en un autre locataire de programme (par exemple, EA, Open ou MOSP).

### <a name="convert-trials-using-partner-center"></a>Convertir des versions d’évaluation à l’aide de l’espace partenaires

Vous pouvez convertir des versions d’évaluation en abonnements payants à l’aide de l’espace partenaires :

1. Accédez à la page d’abonnement du client, puis sélectionnez la version d’évaluation gratuite.
2. Sélectionnez **convertir la version d’évaluation en abonnement payant**.
3. Entrez la quantité de licences et la fréquence de facturation souhaitées, puis sélectionnez **appliquer**.
4. La facturation de l’abonnement payant commence à la date de conversion, et la nouvelle mise à jour automatique de l’abonnement est de 12 mois à compter de la date de conversion. 

### <a name="convert-trials-using-apis"></a>Convertir les essais à l’aide d’API

Vous devrez peut-être modifier vos API pour adapter la conversion d’une version d’évaluation gratuite à un abonnement payant. Pour plus d’informations, consultez la documentation du développeur suivante :

- [Convertir un abonnement d’essai en abonnement payant](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtenir la liste des offres de conversion d’essai](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Essais sans conversions

Tous les essais ne peuvent pas être convertis en abonnements payants. Les partenaires peuvent utiliser une version d’évaluation qui n’a pas de conversion jusqu’à la date d’expiration. Les partenaires peuvent acheter des offres compatibles qui prennent en charge les mêmes services que l’offre d’évaluation.  Cette opération doit être effectuée avant l’expiration de la période d’essai afin de s’assurer que les services des offres nouvellement achetés s’alignent sur les services de la version d’évaluation. 

|**Version d’évaluation**   |**Offres de petites entreprises compatibles**   |**Offres d’entreprise compatibles**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Essai du Cloud commercial Microsoft Teams (initié par l’utilisateur)   |Microsoft 365 Business de base, Microsoft 365 Business standard Microsoft 365 Business Premium   | F3 (anciennement F1), Office 365 pour Enterprise (E1, E3 et E5), Microsoft 365 F1/F3, Microsoft 365 Entreprise (E3)   |

>[!NOTE]
>Les offres ci-dessus ont des plans de service similaires avec des fonctionnalités similaires, mais il peut y avoir des différences entre les offres.

### <a name="expiring-offers"></a>Offres arrivant à expiration

Vous ne serez pas averti de l’expiration des offres. Vous pouvez suivre les dates d’expiration à venir à l’aide de la vue client de l’espace partenaires ou en interrogeant l’API. Il est recommandé de contrôler fréquemment ces dates afin de pouvoir prendre les mesures de suivi appropriées auprès des clients à l’approche du moment où ils doivent prendre une décision.

Après l’expiration d’une période d’essai, un client qui tente de se connecter à cette version d’évaluation verra un message d’expiration. Toutefois, les données sont stockées en fonction des normes de rétention des données. Une fois que vous avez acheté un nouvel abonnement avec les mêmes plans de service, les informations de votre client sont à nouveau accessibles à partir de l’abonnement qui vient d’être activé.

## <a name="billing"></a>Facturation

La facturation annuelle et les versions d’évaluation gratuites sont les mêmes dans les clouds souverains et le cloud public. La seule différence est que les références SKU d’évaluation sont disponibles au moment du lancement.

## <a name="billing-for-free-trials"></a>Facturation pour les versions d’évaluation gratuites

Vous pouvez utiliser des versions d’évaluation gratuites pour des abonnements mensuels et facturés annuellement. Vous pouvez sélectionner la fréquence de facturation quand vous convertissez la version d’évaluation en abonnement payant.

La date de début de l’abonnement est basée sur la date de conversion. Si la version d’évaluation gratuite est convertie en offre payante avec facturation annuelle, la date de renouvellement de l’abonnement sera de 12 mois à compter de la date de la conversion. Si l’essai gratuit est converti en une offre payante avec facturation mensuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de facturation suivant la date de conversion.

### <a name="invoices"></a>Factures

Vous ne verrez pas les versions d’évaluation gratuites indiquées dans votre facture ou fichier de réconciliation basé sur une licence. Les versions d’évaluation gratuites s’affichent uniquement sur votre facture et votre fichier de rapprochement basé sur une licence après la conversion d’une version d’évaluation gratuite en abonnement payant. L’abonnement converti s’affiche de la même façon que n’importe quel nouvel abonnement.

### <a name="incentives"></a>Incentives

Les versions d’évaluation gratuites n’ont pas d’impact sur les incentives.

## <a name="support"></a>Support

Pour obtenir une assistance sur les versions d’évaluation gratuites, envoyez une demande de service via l’espace partenaires.