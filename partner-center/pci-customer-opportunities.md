---
title: Aperçus de l’espace partenaires-rapports de CloudAscent
description: En savoir plus sur les rapports de proportions CloudAscent dans l’espace partenaires. Contient des informations sur la propension d’un client pour l’achat de produits Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175278"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Rapports de proportions CloudAscent disponibles dans le tableau de bord espace partenaires

**Rôles appropriés**
- Visionneuse de rapports de la direction
- Visionneuse de rapports

Le tableau de bord espace partenaires fournit des données de propension téléchargeables à partir du programme CloudAscent. Les données montrent la propension des clients à acheter des produits Microsoft.  Cet article décrit la répartition de ces données, la manière d’utiliser le calcul de score et ce que cela signifie.

## <a name="summary-definitions"></a>Définitions de résumé

- **Clients SMC**: il s’agit du nombre total de clients dans le téléchargement de la distribution.  Les clients sont identifiés par un partenaire d’enregistrement.
- **Contrats d’expiration**: au cours de l’année fiscale en cours, nous fournissons le nombre d’accords arrivant à expiration.
- **Recettes arrivant à expiration**: le chiffre d’affaires associé aux contrats arrivant à expiration.
- **Ouvrir le revenu arrivant à expiration**: le chiffre d’affaires associé aux contrats d’expiration ouverts.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentation SMB CloudAscent

Le segment SMB (Small-Medium Business) est divisé en trois sous-segments distincts.

1. **Top non gérée** comprend les plus grands clients SMB qui ont le plus de chance pour Microsoft. Les principaux clients non gérés partagent des caractéristiques similaires à celles des comptes gérés, avec un grand nombre d’employés, des budgets et des dépenses informatiques importants, ainsi que de grandes quantités de revenus potentiels pour Microsoft.

   Nous définissons les deux principales méthodes non gérées :

   - **Top based user non gérée**: comprend les comptes avec 300 ou plus employés. Les comptes de User-Based sont des cibles intéressantes pour l’achat initial, ou l’extension de produits d’abonnement basés sur l’utilisateur, tels que M365, D365 ou surface.
   - **Top Compute non gérée** : comprend les comptes avec un potentiel Azure supérieur à 10 000 $. Les comptes basés sur le calcul incluent Azure existant. comptes avec un potentiel d’année future et des comptes importants qui n’ont pas encore acheté Azure, mais qui ont un potentiel pour Azure supérieur à 10 000 $.

2. Les entreprises de **taille moyenne** incluent les clients existants et les comptes potentiels de 25 à 300 employés.

3. **Small Business** comprend toutes les entreprises restantes comptant moins de 25 employés.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

Les principaux sous-segments **non gérés** et de **taille moyenne** représentent des clients LTV (High Life-Time value) pour Microsoft et des partenaires Microsoft. Par conséquent, il s’agit des domaines de priorité pour la croissance de ce segment. Dans ces deux sous-segments, nous sommes mieux positionnés pour acquérir le socket avec M365, monétiser davantage avec les applications métier D365/Azure et réaliser un LTV élevé pour Microsoft.

Aujourd’hui, nous avons deux domaines clés de l’opportunité : 1. notre client ajoute de la croissance. 2. Bien que nous puissions acquérir des sockets Cloud avec M365, nous avons une grande opportunité dans D365 et Azure.

La capture d’écran suivante représente les trois sous-segments SMB et les itinéraires optimisés sur le marché. CloudAscent hiérarchiser le profilage, la notation et la modélisation de tous les principaux comptes non gérés et de taille moyenne.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB utilise Machine Learning technologie pour diriger les ventes et le marketing des prédictions client au sein des principaux segments non gérés et de taille moyenne. Comment les signaux sont-ils collectés et convertis en recommandations de propension ?

- **Collecte de données**: les robots d’indexation recherchent et recueillent des milliards de signaux client en exécutant une commande ping sur les domaines de l’entreprise et en surveillant : billets de blog, communiqués de presse, flux sociaux et forums techniques.  Outre les signaux collectés, les informations firmographics sont collectées à partir de sources internes et externes telles que D&B, abonnement interne Microsoft et données transactionnelles.

- **Machine learning**: les signaux sont alimentés dans le modèle machine learning qui génère un ensemble de données structurées de prédictions de ventes et marketing pour chaque client par produit Cloud et cluster.  Chaque client est évalué à l’aide d’un modèle similaire à la SMB de Microsoft qui détermine l’adéquation du client et Machine Learning algorithmes qui intègrent le comportement en ligne du client définissent comme intention. La notation est fusionnée en clusters qui indiquent la propension d’un client à acheter des produits Microsoft Cloud.

- **Optimisation**: le système machine learning optimise les modèles en consommant les données de transaction mensuellement et les données d’abonnement trimestriellement.  À l’aide des données de Win/Loss, le Machine Learning ajuste les algorithmes et vérifie que les modèles fonctionnent comme prévu en comparant les recommandations de cluster aux opportunités traitées dans MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

## <a name="cloudascent-propensity"></a>CloudAscent

Comment les recommandations de propension sont-elles créées ?

À l’aide des signaux collectés via des robots d’indexation et des données Web fournis par diverses sources, nous avons consolidé les données firmographics et les signaux des réseaux sociaux du client.  La notation utilise ces signaux et données dans des modèles de comparaison pour les modèles d’ajustement et de notation pour l’intention.

1. Ajustement du compte client

   - Points de données internes et externes qui définissent firmographics.

   - Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits.

   - L’ajustement ajusté est mis à jour tous les trimestres

2. Intention du compte client

   - Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client.

   - La notation intentionnelle est superposée sur ajuster pour définir les clusters.

   - La notation intentionnelle est mise à jour tous les mois.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

3. Clustering

   Les signaux pour l’adéquation et l’intention sont consolidés dans un score de clustering. CloudAscent a quatre clusters :

      - Agissez maintenant-clients prêts à l’emploi
      - Évaluer : clients prêts pour la commercialisation
      - Campagnes de sensibilisation aux lecteurs
      - Éduquer-éduquer et surveiller l’intention

   Le clustering permet aux utilisateurs de cibler des clients spécifiques pour des initiatives de vente et de marketing basées sur des facteurs de segment, par exemple : produit, géo, secteur et vertical.

   L’onglet **modèle de propensation** des classeurs CloudAscent partage le propension et le revenu estimé des espaces blancs. Pour définir le clustering de l’ajustement et de l’intention, nous allons suivre les étapes suivantes :

      1. En utilisant des modèles ML, nous commençons par calculer le score du client et le score d’intention sur une échelle de 100.  Les scores exacts varient en fonction des modèles ML.  Exemples de scores ci-dessous :

         |**Classification**|**Score**|
         |---------|:---------|
         |Élevé|75-100|
         |Moyenne|55-74|
         |Faible|30 - 54|
         |Très faible|0 - 29|

      2. À l’aide de la règle ci-dessus, nous classons les entreprises pour qu’elles soient élevées, moyennes, basses et très basses à la fois sur l’adaptabilité des clients et les signaux d’intention.

      3. Nous allons tracer les signaux d’ajustement et d’intention des clients sur une matrice 2D avec chaque intersection représentant la distribution.     Par exemple, haute adaptation + haute intention = a1, représentant la plus grande distribution.

      4. Enfin, ces segments regroupent les clusters.  Par exemple, a1, a2, a3, A4 forment le cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

   Pour ces clients, nous vous recommandons de cibler Act maintenant et d’évaluer les clients.

## <a name="cloudascent-products--models"></a>Modèles de & produits CloudAscent

Le graphique suivant fournit une vue de chaque modèle de propension dans CloudAscent :

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

Les modèles d’espace blanc sont composés de prédictions pour les clients Microsoft existants où ils ne disposent pas d’un produit et/ou sont des clients net New Prospect.

Les modèles de vente incitative utilisent des données de transaction pour prédire le potentiel de vente incitative dans Azure et les références SKU M365.

EOS partage les clients de fin de service pour Win 7, Office 2010, SQL Server et Windows Server. Les données de la surcharge sont extraites de MS sales et déplacées avec la modélisation de propension CloudAscent, le cas échéant. Les données de EOS résident dans le travail moderne et les ventes Azure sont exécutées.
