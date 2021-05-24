---
title: Obtenir des insights de référence
ms.topic: article
ms.date: 04/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Passez régulièrement en revue vos données d’insights de référence dans l’Espace partenaires pour voir les tendances à traiter ou les domaines d’amélioration pour vous aider à atteindre vos objectifs métiers.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b1bb86a493ce81cb02b14c9555f82767d10f841c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855946"
---
# <a name="get-referral-insights-in-partner-center-and-find-out-how-your-referrals-are-doing"></a>Obtenir des insights de référence dans l’Espace partenaires et voir les performances de vos références

**Rôles appropriés** : Administrateur des références

La page **Opportunités de co-vente** dans la section **Analytique** de Références vous permet de voir l’état de vos références. Passez régulièrement en revue ces métriques pour identifier les tendances ou les domaines nécessitant votre attention, et faites un premier pas vers vos objectifs métier.

Pour afficher les données des insights de vos opportunités de co-vente, dans le menu de l’Espace partenaires, accédez à **Références > Analytique > Opportunités de co-vente**.

> [!Important]
> Le filtre de type de transaction est préappliqué, avec le type **Co-vente** sélectionné pour toutes les données. Si vous souhaitez analyser les données associées à des transactions privées et suivies par des partenaires, supprimez ce filtre.

## <a name="apply-filters"></a>Appliquer des filtres

Dans la zone supérieure de la page **Opportunités de co-vente**, vous pouvez sélectionner la période pour laquelle vous souhaitez afficher les données. La sélection par défaut est **3M** (trois mois), mais vous pouvez choisir d’afficher les données sur six mois ou un an. Vous pouvez également sélectionner **Personnalisée** pour voir les données de toutes les références sur une période spécifique.

Vous pouvez sélectionner le bouton **Filtres** pour ouvrir le volet permettant de filtrer toutes les données de cette page en fonction du nom du client, du pays, du type de marché, de la direction du marché, du nom de la solution et de l’état. Les détails de ces filtres sont fournis ci-dessous.

- **Nom du client** : La valeur par défaut est **Tous**, mais vous pouvez restreindre les données à un ou plusieurs clients, en les sélectionnant.
- **Pays** : La valeur par défaut est **Tous**, mais vous pouvez restreindre les données à un ou plusieurs pays du client, en les sélectionnant.
- **Type d’offre** : La valeur par défaut est **Co-vente**. Toutefois, vous pouvez sélectionner « Tous », ou limiter les données aux offres privées ou suivies par des partenaires en fonction de votre sélection.
- **Direction du marché** : la valeur par défaut est **Toutes**, mais vous pouvez choisir de limiter les données aux références **entrantes** (celles que vous avez reçues) ou aux références **sortantes** (celles que vous avez envoyées).
- **Nom de la solution** : La valeur par défaut est **Tous**, mais vous pouvez choisir de limiter les données aux références qui contiennent la ou les solutions que vous sélectionnez.
- **État** : La valeur par défaut est **Tous**, mais vous pouvez choisir de limiter les données aux références qui contiennent un ou plusieurs types d’état de référence que vous sélectionnez, comme « créé », « accepté », « refusé », « expiré », « perdu » ou « conclu ».

Les informations figurant dans tous les graphiques listés ci-après correspondent à la plage de dates et à tous les filtres que vous avez sélectionnés, sauf exception notée ci-dessous. Certaines sections vous permettent également d’appliquer des filtres supplémentaires, tels que le filtrage sur une solution spécifique.

## <a name="referrals-summary"></a>Résumé des références

Cette carte affiche une vue d’ensemble de l’état de vos opportunités de co-vente.

Le graphique affiche le nombre total de marchés, le nombre de marchés conclus, le nombre de marchés perdus et le volume total de marchés (en USD) pour la période sélectionnée.

Les métriques de changement de pourcentage (affichées en rouge ou en vert, avec un indicateur de flèche) indiquent la différence entre le **dernier mois complet de la plage de dates sélectionnée** et le **premier mois complet de cette plage**. Par exemple, supposons que la date actuelle est le 15 juin et que vous avez sélectionné le filtre **3M** pour afficher les données des trois derniers mois. Dans ce cas, ces métriques affichent la différence entre le mois de mai (dernier mois complet dans la période sélectionnée) et le mois de mars (premier mois complet dans la période sélectionnée). La plage de dates sélectionnée étant les derniers **3M**, la comparaison s’effectuerait entre les données du mois de mai et les données du mois de mars.

:::image type="content" source="images/referrals/cosellanalyticssummary.png" alt-text="Image représentant la carte de résumé de l’analytique des opportunités de co-vente.":::

## <a name="conversion-funnel"></a>Entonnoir de conversion

Cette section affiche un indicateur visuel de la façon dont vos marchés passent d’un état à un autre tout au long de leur cycle de vie. Vous pouvez afficher l’intégralité du cycle de vie en fonction du volume des transactions, ainsi que la valeur des offres en USD en fonction du champ dynamique principal de cette section. La première section est étiquetée avec l’état et le type de l’offre, afin de fournir un indicateur visuel du volume ou de la valeur pour chaque type. Il existe également une section, **Références du passé**, qui est utilisée pour indiquer les marchés que vous avez entrepris d’accepter/refuser ou de marquer comme conclus/perdus au cours de la période sélectionnée pour le rapport. Vous pouvez appliquer des filtres pour afficher la progression des marchés entre les différentes phases de leur cycle de vie.

Les offres entrantes de co-vente peuvent être fusionnées en offres « Acceptées », « Refusées » ou « Expirées », puisque les partenaires doivent Accepter ou Refuser les offres de co-vente entrantes.

:::image type="content" source="images/referrals/inbound.png" alt-text="Image montrant l’état des références entrantes.":::

Les offres sortantes privées, de co-vente ou suivies par des partenaires seront fusionnées en offres « Créées » lors de leur création par les partenaires.

:::image type="content" source="images/referrals/outbound.png" alt-text="Image montrant l’état des références sortantes.":::

:::image type="content" source="images/referrals/cosell-analytics-funnel-v2.png" alt-text="Image représentant l’entonnoir de conversion pour les références.":::

## <a name="deals-by-geography"></a>Marchés par zone géographique

Cette section affiche les pays/régions d’où proviennent les références, ainsi que les détails de chaque pays/région. Il existe une vue tabulaire des détails des marchés pour chaque pays, ainsi qu’une vue cartographique de tous les pays. Vous pouvez sélectionner un pays spécifique dans la table ou sélectionner la vue cartographique pour effectuer un zoom sur un pays spécifique.

:::image type="content" source="images/referrals/cosell-analytics-geo-distribution-v2.png" alt-text="Image représentant la distribution géographique des références.":::

## <a name="deals-by-solutions"></a>Marchés par solutions

Ce graphique vous permet de voir quelles solutions donnent le plus de références et la plus grande valeur de marché. La table comprend trois champs dynamiques : co-vente, privées et suivies par des partenaires.
En fonction de votre sélection de tableau croisé dynamique, vous pouvez voir les performances des marchés agrégées par solution.

> [!NOTE]
> Si plusieurs solutions sont comprises dans un marché, le tableau affichera le même marché compté dans toutes ces solutions. Vous ne devez pas ajouter les valeurs associées aux solutions et les comparer à d’autres métriques de volume de référence. Cette vue a pour but de vous aider à comprendre les performances des marchés avec un tableau croisé dynamique de solution.

Le tableau contient le nombre total de marchés qui comportent la solution et les états correspondants, comme les marchés conclus, les marchés perdus, les marchés expirés, ainsi que la valeur totale des marchés conclus et perdus en USD. Un graphique de tendances des marchés figure également à droite du tableau et indique le nombre total de marchés et la valeur des marchés gagnée en USD, en fonction de la solution sélectionnée. La sélection par défaut correspond à l’ensemble des solutions.

:::image type="content" source="images/referrals/cosell-analytics-solutions-v2.png" alt-text="Image présentant les performances des solutions.":::

## <a name="declined--lost-reasons"></a>Raisons de refus et de perte

Cette section vous aide à analyser les raisons pour lesquelles les marchés sont marqués comme **refusés** ou **perdus** par votre entreprise. Les options proposées dans ces représentations sont les raisons choisies par les vendeurs lors de la conclusion du marché comme étant refusé ou perdu.

:::image type="content" source="images/referrals/cosellanalyticsreasons.png" alt-text="Image affichant les raisons sélectionnées par le partenaire lors du refus ou de la perte d’un marché.":::

## <a name="comparison-charts"></a>Graphiques de comparaison

La section de comparaison vous aide à comparer les données relatives aux références en fonction de plusieurs dimensions dans le tableau croisé dynamique, sur le volume et sur la valeur des marchés conclus en USD. Les trois dimensions que vous pouvez choisir pour comparer les données sont :

- Type de marché
- Marchés
- Solutions

Lorsque le type de transaction est sélectionné, vous pouvez comparer les performances des références en ce qui concerne les opportunités de co-vente, les transactions privées et les transactions suivies par des partenaires. Pour les marchés et les solutions, vous pouvez sélectionner jusqu’à trois options différentes pour comparer les performances. Le premier graphique, qui est un graphique à barres, présente les données avec une tendance mois après mois, basée sur le tableau croisé dynamique principal, qui est le volume ou la valeur des marchés conclus. Un graphique à secteurs figure également à droite du graphique à barres et affiche les pourcentages de distribution pour les mêmes données.

:::image type="content" source="images/referrals/cosell-analytics-compare-v2.png" alt-text="Image représentant la section de comparaison.":::

## <a name="raw-data-table"></a>Table des données brutes

La table ci-dessous, qui contient toutes les données brutes relatives aux opportunités de co-vente, vous permet d’**exporter** rapidement les données pour toute analyse détaillée ou personnalisée que vous souhaitez effectuer.

:::image type="content" source="images/referrals/cosellanalyticsrawdata.png" alt-text="Image représentant la table des données brutes pour les références.":::

## <a name="no-data"></a>Pas de données

Plusieurs raisons peuvent expliquer que vous obteniez un graphique vide comme ci-dessous lorsque vous accédez à l’analytique de co-vente, comme décrit ci-dessous.

- Il n’existe aucune donnée pour ce compte. Essayez de créer des marchés pour remplir ce rapport.
- Un problème de connectivité réseau est survenu. Vérifiez votre connexion Internet et réessayez.
- La page se charge avec le filtre par défaut pour les marchés de co-vente. Si vous avez uniquement des marchés privés, réinitialisez le filtre de type de marché.
- Aucun enregistrement ne correspond aux filtres que vous avez appliqués. Essayez de réinitialiser les filtres.
- Il y a un délai entre le changement d’état de l’opportunité et sa mise à jour dans le rapport d’analyse. Vérifiez le rapport après 24 heures.

:::image type="content" source="images/referrals/nodata.png" alt-text="Image n’indiquant aucune visualisation de données pour les références.":::

> [!NOTE]
> La page **Insights de référence** affiche uniquement des données pour les références générées dans l’Espace partenaires. Elle n’affiche pas de données pour les références générées via [Partner Sales Connect ](psc-to-pc.md) ou d’autres mécanismes.

> [!TIP]
> Pour voir comment votre profil d’entreprise s’exécute dans l’expérience [Rechercher un fournisseur de solutions](https://www.microsoft.com/solution-providers/home), consultez [Page Insights du profil d’entreprise](analyze-your-marketing-profile.md).

## <a name="next-steps"></a>Étapes suivantes

- [Développer votre activité avec les références Microsoft](referrals.md)
- [Analyser vos prospects](analyze-your-marketing-profile.md)