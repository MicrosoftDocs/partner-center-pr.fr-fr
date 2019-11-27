---
title: Proposer à vos clients des versions d’évaluation de produits Microsoft | Espaces partenaires
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vos clients peuvent tester des produits d’abonnement Microsoft pendant 30 jours. Vous pouvez vous inscrire à ces versions d’évaluation dans le catalogue, comme beaucoup d’autres services en ligne.
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

S’applique à :

- Espace partenaires

Une méthode efficace pour présenter les nouveaux produits Microsoft aux clients consiste à leur proposer des versions d'évaluation gratuites pendant 30 jours. Vous pouvez obtenir les versions d’évaluation figurant le catalogue comme vous le faites pour de nombreux autres services en ligne. Tous les partenaires peuvent participer.

## <a name="available-trial-offers"></a>Offres d’essai disponibles

Vous trouverez toutes vos offres d’essai en suspens sur la page du **client** . Cette page répertorie tous les abonnements, y compris les versions d’évaluation gratuites et les abonnements payants. (Cette fonctionnalité n’est actuellement pas disponible en Chine.)

Chaque client bénéficie d’un essai gratuit pour chaque offre disponible. Par exemple, ils peuvent obtenir un essai gratuit pour Office 365 Business Premium et un autre pour Office 365 E3. Toutefois, si le client possède déjà l’offre, il ne peut pas utiliser une version d’évaluation gratuite pour cette offre.

### <a name="available-products"></a>Produits disponibles

Des essais gratuits sont proposés pour les produits suivants :

- Office&nbsp;365 Business&nbsp;Premium
- Office 365 E3
- Office 365 E5 avec RTPC
- Office 365 E5 sans RTPC
- Enterprise Mobility + Security E5
- Formule Dynamics 365 Customer Engagement 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Nous fournissons des essais gratuits pour ces produits, car il s’agit des offres commerciales les plus complètes et les plus populaires. Il se peut que nous ajoutions d’autres offres d’essais gratuits à l’avenir.

Actuellement, il n’y a **pas d’essai gratuit** pour les offres gouvernementales, les offres de formation ou les offres complémentaires.

## <a name="licenses-for-free-trial-offers"></a>Licences pour les offres d’essai gratuit

Tous les essais gratuits proposent 25 licences. Vous ne pouvez pas modifier ce nombre au cours de la période d’évaluation. Vous ne pouvez pas ajouter ou supprimer des sièges dans la version d’évaluation gratuite. Une fois la version d’évaluation convertie en abonnement payant, vous pouvez ajouter des licences supplémentaires à l’abonnement.

Vous devez attribuer des licences d’évaluation et des sièges comme vous le feriez pour un service payant dans l’espace partenaires.

## <a name="sign-customers-up-for-trials"></a>Signer les clients pour les versions d’évaluation

Pour signer votre client en vue d’une version d’évaluation via l’espace partenaires :

1. À partir de la **vente** dans l’espace partenaires, accédez au **catalogue**. 
2. Dans le catalogue, à partir de **Périodicité de facturation**, cliquez sur **Offre de version d'évaluation**. Cela ne fait apparaître que les essais gratuits et désactive les offres payantes. Les versions d’évaluation s’affichent dans l’onglet **Versions d’évaluation** du catalogue.
3. Sélectionnez la version d’évaluation gratuite que vous voulez proposer, puis sélectionnez **Soumettre**. Toutes les versions d’évaluation sont valables 30 jours ; vous ne serez pas facturé pendant cette période. Vous pouvez également convertir une version d’évaluation en abonnement payant à tout moment pendant la période d’évaluation.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversion des versions d’évaluation en abonnements payants

Une version d’évaluation gratuite n’est pas automatiquement convertie en abonnement payant. Après 30 jours, une version d’évaluation gratuite doit être convertie en abonnement payant ou [expire](#expiring-offers). Les versions d’évaluation gratuites ne peuvent pas être étendues.

Vous devez convertir votre version d’évaluation en abonnement payant. Pour ce faire, vous pouvez [utiliser l’espace partenaires](#convert-trials-using-partner-center) ou [les API de l’espace partenaires](#convert-trials-using-apis).

> [!NOTE]
> Les versions d’évaluation gratuites du client pour le programme du fournisseur de solutions Cloud (CSP) ne peuvent pas être converties en un autre locataire de programme (par exemple, EA, Open ou MOSP).

### <a name="convert-trials-using-partner-center"></a>Convertir des versions d’évaluation à l’aide de l’espace partenaires

Vous pouvez convertir des versions d’évaluation en abonnements payants à l’aide du tableau de bord espace partenaires comme suit :

1. Accédez à la page des abonnements du client, puis sélectionnez l'essai gratuit.
2. Sélectionnez **Convertir la version d'évaluation en abonnement payant**.
3. Entrez le nombre de licences souhaité et la fréquence de facturation, puis sélectionnez **Appliquer**.
4. La facturation de l’abonnement payant commencera à la date de conversion et l'abonnement sera automatiquement renouvelé 12 mois à compter de cette dernière. 

### <a name="convert-trials-using-apis"></a>Convertir les essais à l’aide d’API

Vous devrez peut-être modifier vos API pour adapter la conversion d’une version d’évaluation gratuite à un abonnement payant. Pour plus d’informations, consultez la documentation du développeur suivante :

- [Convertir un abonnement d'évaluation en abonnement payant](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtenir une liste des offres de conversion de version d’évaluation](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Offres arrivant à expiration

Vous ne serez pas averti de l’expiration des offres. Vous pouvez suivre les dates d’expiration à venir à l’aide de la vue client de l’espace partenaires ou en interrogeant l’API. Il est recommandé de contrôler fréquemment ces dates afin de pouvoir prendre les mesures de suivi appropriées auprès des clients à l’approche du moment où ils doivent prendre une décision.

Après l’expiration d’une période d’essai, un client qui tente de se connecter à cette version d’évaluation verra un message d’expiration. Toutefois, les données sont stockées en fonction des normes de rétention des données. Une fois que vous avez acheté un nouvel abonnement avec les mêmes plans de service, les informations de votre client sont à nouveau accessibles à partir de l’abonnement qui vient d’être activé.

## <a name="billing"></a>Facturation

La facturation annuelle et les versions d’évaluation gratuites sont les mêmes dans les clouds souverains et le cloud public. La seule différence est que les références SKU d’évaluation sont disponibles au moment du lancement.

## <a name="billing-for-free-trials"></a>Facturation pour les versions d’évaluation gratuites

Vous pouvez utiliser des versions d’évaluation gratuites pour des abonnements mensuels et facturés annuellement. Vous pouvez sélectionner la fréquence de facturation quand vous convertissez la version d’évaluation en abonnement payant.

La date de début de l’abonnement est basée sur la date de conversion. Si l’essai gratuit est converti en offre payante à facturation annuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de conversion. Si l’essai gratuit est converti en une offre payante avec facturation mensuelle, la date de renouvellement de l’abonnement sera 12 mois à compter de la date de facturation suivant la date de conversion.

### <a name="invoices"></a>Factures

Vous ne verrez pas les versions d’évaluation gratuites indiquées dans votre facture ou fichier de réconciliation basé sur une licence. Les versions d’évaluation gratuites s’affichent uniquement sur votre facture et votre fichier de rapprochement basé sur une licence après la conversion d’une version d’évaluation gratuite en abonnement payant. L’abonnement converti s’affiche de la même façon que n’importe quel nouvel abonnement.

### <a name="incentives"></a>Primes incitatives

Les versions d’évaluation gratuites n’ont pas d’impact sur les incentives.

## <a name="support"></a>Assistance

Pour obtenir une assistance sur les versions d’évaluation gratuites, envoyez une demande de service via l’espace partenaires.
