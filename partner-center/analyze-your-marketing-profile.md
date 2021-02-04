---
title: Analyser vos clients
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment utiliser la page prospects Insights pour voir comment vous capturez l’attention de vos clients cibles et générez des références.
author: vikrambmsft
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 1f8d9f04920a4f2a0fab40523c217835d9b0e4ef
ms.sourcegitcommit: 9cb7dc98faae06c255dbc025f8e452d75380c16a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/04/2021
ms.locfileid: "99530831"
---
# <a name="analyze-your-leads---see-how-well-you-attract-target-customers-and-potential-referrals"></a>Analysez vos prospects : déterminez dans quelle mesure vous attirez les clients cibles et les références potentielles
<!-- 
https://go.microsoft.com/fwlink/?linkid=849120
-->

**Rôles appropriés**

- Administrateur des références

La page **prospects** sous la section **analytique** dans références vous permet de voir comment vos références sont en cours d’exécution. Passez régulièrement en revue ces métriques pour identifier les tendances ou les domaines nécessitant votre attention, et faites un premier pas vers vos objectifs métier.

Pour afficher les données de vos prospects, dans le menu de l’espace partenaires, accédez à **références > analyser > prospects**.

## <a name="apply-filters"></a>Appliquer des filtres

Près du haut de la page des **clients** , vous pouvez sélectionner la période pour laquelle vous souhaitez afficher les données. La sélection par défaut est **3M** (3 mois), mais vous pouvez choisir d’afficher les données sur une période de 6 mois ou 1 an à la place. Vous pouvez également sélectionner **Personnalisée** pour voir les données de toutes les références sur une période spécifique.

Vous pouvez cliquer sur le bouton Filtres pour ouvrir le volet permettant de filtrer toutes les données de cette page en fonction du nom du client, du pays, du type de marché, de la direction du marché, du nom de la solution et de l’état. Les détails de ces filtres sont fournis ci-dessous.

- **Nom du client** : La valeur par défaut est **Tous**, mais vous pouvez restreindre les données à un ou plusieurs clients, en les sélectionnant.
- **Pays** : La valeur par défaut est **Tous**, mais vous pouvez restreindre les données à un ou plusieurs pays du client, en les sélectionnant.
- **Programme de référence**: la valeur par défaut est **tout**, mais vous pouvez limiter les données à un programme de référence spécifique. Ce filtre est visible uniquement si votre organisation est inscrite dans le programme de référence.
- **État** : La valeur par défaut est **Tous**, mais vous pouvez choisir de limiter les données aux références qui contiennent un ou plusieurs types d’état de référence que vous sélectionnez, comme accepté, refusé, expiré, perdu ou conclu.
- **Type de qualification**: la valeur par défaut est **tout**, mais vous pouvez choisir de limiter les données aux références qui sont soit des prospects de la place de marché, soit des prospects qualifiés.

Les informations figurant dans tous les graphiques listés ci-après correspondent à la plage de dates et à tous les filtres que vous avez sélectionnés, sauf exception notée ci-dessous. Certaines sections vous permettent également d’appliquer des filtres supplémentaires, tels que le filtrage sur une solution spécifique.

## <a name="referrals-summary"></a>Résumé des références

Cette carte présente une vue d’ensemble de l’exécution de vos clients.

Le graphique affiche le nombre total de visites de page, le nombre de clics de bouton d’appel à l’action (partenaire de contact), le nombre de prospects générés après que les clients ont cliqué sur l’appel à l’action et le nombre total de prospects gagnés pour la période sélectionnée.

Les métriques de changement de pourcentage (affichées en rouge ou en vert, avec un indicateur de flèche) indiquent la différence entre le **dernier mois complet de la plage de dates sélectionnée** et le **premier mois complet de cette plage**. Par exemple, supposons que la date actuelle est le 15 juin et que vous avez sélectionné le filtre **3M** pour afficher les données des trois derniers mois. Dans ce cas, ces métriques affichent la différence entre le mois de mai (dernier mois complet dans la période sélectionnée) et le mois de mars (premier mois complet dans la période sélectionnée). La plage de dates sélectionnée étant les derniers **3M**, la comparaison s’effectuerait entre les données du mois de mai et les données du mois de mars.

:::image type="content" source="images/referrals/leadsanalyticssummary.png" alt-text="Image représentant la carte de résumé de l’analytique des clients.":::

## <a name="conversion-funnel"></a>Entonnoir de conversion

Cette section affiche un indicateur visuel de la façon dont vos marchés passent d’un état à un autre tout au long de leur cycle de vie. Vous pouvez afficher l’intégralité du cycle de vie en fonction du volume de marchés, ainsi que la valeur des marchés en USD en fonction du tableau croisé dynamique principal de cette section. La première section est étiquetée avec le type de l’offre pour vous fournir un indicateur visuel du volume ou de la valeur par type. Il y a également une section, **prospects du passé**, qui est utilisée pour indiquer les transactions que vous avez prises en acceptant/refusant ou en les marquant comme étant gagnées/perdues au cours de la période sélectionnée pour le rapport. Vous pouvez appliquer des filtres pour afficher la progression des marchés entre les différentes phases de leur cycle de vie.

:::image type="content" source="images/referrals/leadsanalyticsfunnel.png" alt-text="Image représentant l’entonnoir de conversion pour les références.":::

## <a name="leads-by-geography"></a>Opportunités par zone géographique

Cette section affiche les pays/régions d’où proviennent les références, ainsi que les détails de chaque pays/région. Il existe une vue tabulaire des détails des marchés pour chaque pays, ainsi qu’une vue cartographique de tous les pays. Vous pouvez cliquer sur un pays spécifique dans la table ou cliquer sur la vue cartographique pour effectuer un zoom sur un pays spécifique.

:::image type="content" source="images/referrals/leadsanalyticsgeodistribution.png" alt-text="Image représentant la distribution géographique des références.":::

## <a name="leads-by-program"></a>Opportunités par programme

Cette combinaison de tables et de graphiques vous permet de voir quels sont les prospects de votre programme de référence qui pilotent le plus de références et la valeur la plus élevée.
La table contient le total des clients, les clients qui ont été acceptés avec dans le contrat SLA (24 heures) en termes de pourcentage et absolu, les clients arrivés à expiration et les clients qui se sont associés à l’État gagné, ainsi que la valeur totale des succès gagnée dans la devise USD. Il y a également un graphique de tendance des prospects à droite du tableau qui indique le nombre total de demandes et la valeur de transaction gagnée en devise USD, en fonction du programme sélectionné. La sélection par défaut correspond à l’ensemble des solutions.

:::image type="content" source="images/referrals/leadsanalyticsreferralsprogram.png" alt-text="Une image présentant le programme de références qualifiées domine les performances.":::

## <a name="declined--lost-reasons"></a>Raisons de refus et de perte

Cette section vous aide à analyser les raisons pour lesquelles les clients sont marqués comme **refusés** ou **perdus** par votre entreprise. Les options proposées dans ces représentations sont les mêmes que celles choisies lors de la fermeture du prospect, telles qu’elles ont été refusées ou perdues.

:::image type="content" source="images/referrals/leadsanalyticsreasons.png" alt-text="Image représentant les raisons sélectionnées par le partenaire pour refuser ou rendre un prospect perdu.":::

## <a name="comparison-charts"></a>Graphiques de comparaison

La section de comparaison vous aide à comparer les données relatives aux clients en fonction de plusieurs dimensions sur le volume et de la valeur des succès gagnés dans le tableau croisé dynamique USD.
Les trois dimensions que vous pouvez choisir pour comparer les données sont :

- Type de qualification
- Marchés
- Programme de référence

Lorsque type de qualification est sélectionné, vous avez la possibilité de comparer les performances de référence de par rapport aux prospects de la place de marché et aux prospects qualifiés. Pour les marchés et le programme de référencement, vous pouvez choisir jusqu’à trois options différentes pour comparer leurs performances. Le premier graphique, qui est un graphique à barres, présente les données avec une tendance mois après mois, basée sur le tableau croisé dynamique principal, qui est le volume ou la valeur des marchés conclus. Un graphique à secteurs figure également à droite du graphique à barres et affiche les pourcentages de distribution pour les mêmes données.

:::image type="content" source="images/referrals/leadsanalyticscompare.png" alt-text="Image représentant la section de comparaison.":::

## <a name="raw-data-table"></a>Table des données brutes

Le tableau ci-dessous contenant toutes les données brutes relatives aux clients vous permet d' **Exporter** rapidement les données pour toute analyse détaillée ou personnalisée que vous souhaitez effectuer.

:::image type="content" source="images/referrals/leadsanalyticsrawdata.png" alt-text="Image représentant la table de données brutes pour les clients.":::

## <a name="no-data"></a>Pas de données

Il peut y avoir plusieurs raisons pour lesquelles vous obtenez un graphique vide comme ci-dessous lorsque vous accédez à l’analytique des clients, comme décrit ci-dessous.

- Il n’existe aucune donnée pour ce compte. Essayez de créer des marchés pour remplir ce rapport.
- Un problème de connectivité réseau est survenu. Vérifiez votre connexion Internet et réessayez.
- Aucun enregistrement ne correspond aux filtres que vous avez appliqués. Essayez de réinitialiser les filtres.
- Il y a un délai entre le changement d’État du prospect et le même pour être mis à jour dans le rapport d’analyse. Vérifiez le rapport après 24 heures.

:::image type="content" source="images/referrals/nodata.png" alt-text="Image qui n’indique aucune visualisation des données pour les responsables.":::

> [!TIP]
> Pour voir comment vos opportunités de co-vente sont exécutées, consultez la [page Co-vendre opportunités Insights](referral-insights.md).

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les prospects](manage-leads.md)
