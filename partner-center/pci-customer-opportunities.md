---
title: Aperçus de l’espace partenaires-rapports de CloudAscent
description: En savoir plus sur les rapports de proportions CloudAscent dans le tableau de bord espace partenaires.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 510f85b053ec17fa0a2a66217a19c006e7ca2bc9
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811333"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="8b77f-103">Rapports de proportions CloudAscent disponibles dans le tableau de bord espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8b77f-103">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="8b77f-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="8b77f-104">**Appropriate roles**</span></span>
- <span data-ttu-id="8b77f-105">Visionneuse de rapports de la direction</span><span class="sxs-lookup"><span data-stu-id="8b77f-105">Executive report viewer</span></span>
- <span data-ttu-id="8b77f-106">Visionneuse de rapports</span><span class="sxs-lookup"><span data-stu-id="8b77f-106">Report viewer</span></span>

<span data-ttu-id="8b77f-107">Le tableau de bord espace partenaires fournit des données de propension téléchargeables à partir du programme CloudAscent.</span><span class="sxs-lookup"><span data-stu-id="8b77f-107">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="8b77f-108">Les données montrent la propension des clients à acheter des produits Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b77f-108">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="8b77f-109">Cet article décrit la répartition de ces données, la manière d’utiliser le calcul de score et ce que cela signifie.</span><span class="sxs-lookup"><span data-stu-id="8b77f-109">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="8b77f-110">Définitions de résumé</span><span class="sxs-lookup"><span data-stu-id="8b77f-110">Summary definitions</span></span>

- <span data-ttu-id="8b77f-111">**Clients SMC**: il s’agit du nombre total de clients dans le téléchargement de la distribution.</span><span class="sxs-lookup"><span data-stu-id="8b77f-111">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="8b77f-112">Les clients sont identifiés par un partenaire d’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="8b77f-112">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="8b77f-113">**Contrats d’expiration**: au cours de l’année fiscale en cours, nous fournissons le nombre d’accords arrivant à expiration.</span><span class="sxs-lookup"><span data-stu-id="8b77f-113">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="8b77f-114">**Recettes arrivant à expiration**: le chiffre d’affaires associé aux contrats arrivant à expiration.</span><span class="sxs-lookup"><span data-stu-id="8b77f-114">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="8b77f-115">**Ouvrir le revenu arrivant à expiration**: le chiffre d’affaires associé aux contrats d’expiration ouverts.</span><span class="sxs-lookup"><span data-stu-id="8b77f-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Capture d’écran du tableau de bord Résumé des opportunités de clients.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="8b77f-117">Segmentation SMB CloudAscent</span><span class="sxs-lookup"><span data-stu-id="8b77f-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="8b77f-118">Le segment SMB (Small-Medium Business) est divisé en trois sous-segments distincts.</span><span class="sxs-lookup"><span data-stu-id="8b77f-118">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="8b77f-119">**Top non gérée** comprend les plus grands clients SMB qui ont le plus de chance pour Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b77f-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="8b77f-120">Les principaux clients non gérés partagent des caractéristiques similaires à celles des comptes gérés, avec un grand nombre d’employés, des budgets et des dépenses informatiques importants, ainsi que de grandes quantités de revenus potentiels pour Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b77f-120">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="8b77f-121">Nous définissons les deux principales méthodes non gérées :</span><span class="sxs-lookup"><span data-stu-id="8b77f-121">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="8b77f-122">**Top based user non gérée**: comprend les comptes avec 300 ou plus employés.</span><span class="sxs-lookup"><span data-stu-id="8b77f-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="8b77f-123">Les comptes basés sur les utilisateurs sont de bons objectifs pour la première utilisation ou l’extension de produits d’abonnement basés sur l’utilisateur, tels que M365, D365 ou surface.</span><span class="sxs-lookup"><span data-stu-id="8b77f-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="8b77f-124">**Top Compute non gérée** : comprend les comptes avec un potentiel Azure supérieur à 10 000 $.</span><span class="sxs-lookup"><span data-stu-id="8b77f-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="8b77f-125">Les comptes basés sur le calcul incluent Azure existant.</span><span class="sxs-lookup"><span data-stu-id="8b77f-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="8b77f-126">comptes avec un potentiel d’année future et des comptes importants qui n’ont pas encore acheté Azure, mais qui ont un potentiel pour Azure supérieur à 10 000 $.</span><span class="sxs-lookup"><span data-stu-id="8b77f-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="8b77f-127">Les entreprises de **taille moyenne** incluent les clients existants et les comptes potentiels de 25 à 300 employés.</span><span class="sxs-lookup"><span data-stu-id="8b77f-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="8b77f-128">**Small Business** comprend toutes les entreprises restantes comptant moins de 25 employés.</span><span class="sxs-lookup"><span data-stu-id="8b77f-128">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Client par type SMC.":::

<span data-ttu-id="8b77f-130">Les principaux sous-segments **non gérés** et de **taille moyenne** représentent des clients LTV (High Life-Time value) pour Microsoft et des partenaires Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b77f-130">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="8b77f-131">Par conséquent, il s’agit des domaines de priorité pour la croissance de ce segment.</span><span class="sxs-lookup"><span data-stu-id="8b77f-131">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="8b77f-132">Dans ces deux sous-segments, nous sommes mieux positionnés pour acquérir le socket avec M365, monétiser davantage avec les applications métier D365/Azure et réaliser un LTV élevé pour Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b77f-132">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="8b77f-133">Aujourd’hui, nous avons deux domaines clés de l’opportunité : 1.</span><span class="sxs-lookup"><span data-stu-id="8b77f-133">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="8b77f-134">notre client ajoute de la croissance. 2.</span><span class="sxs-lookup"><span data-stu-id="8b77f-134">our customer adds growth; 2.</span></span> <span data-ttu-id="8b77f-135">Bien que nous puissions acquérir des sockets Cloud avec M365, nous avons une grande opportunité dans D365 et Azure.</span><span class="sxs-lookup"><span data-stu-id="8b77f-135">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="8b77f-136">La capture d’écran suivante représente les trois sous-segments SMB et les itinéraires optimisés sur le marché.</span><span class="sxs-lookup"><span data-stu-id="8b77f-136">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="8b77f-137">CloudAscent hiérarchiser le profilage, la notation et la modélisation de tous les principaux comptes non gérés et de taille moyenne.</span><span class="sxs-lookup"><span data-stu-id="8b77f-137">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Capture d’écran des sous-segments SMB.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="8b77f-139">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="8b77f-139">CloudAscent Machine Learning</span></span>

<span data-ttu-id="8b77f-140">SMB utilise Machine Learning technologie pour diriger les ventes et le marketing des prédictions client au sein des principaux segments non gérés et de taille moyenne.</span><span class="sxs-lookup"><span data-stu-id="8b77f-140">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="8b77f-141">Comment les signaux sont-ils collectés et convertis en recommandations de propension ?</span><span class="sxs-lookup"><span data-stu-id="8b77f-141">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="8b77f-142">**Collecte de données**: les robots d’indexation recherchent et recueillent des milliards de signaux client en exécutant une commande ping sur les domaines de l’entreprise et en surveillant : billets de blog, communiqués de presse, flux sociaux et forums techniques.</span><span class="sxs-lookup"><span data-stu-id="8b77f-142">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="8b77f-143">Outre les signaux collectés, les informations firmographics sont collectées à partir de sources internes et externes telles que D&B, abonnement interne Microsoft et données transactionnelles.</span><span class="sxs-lookup"><span data-stu-id="8b77f-143">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="8b77f-144">**Machine learning**: les signaux sont alimentés dans le modèle machine learning qui génère un ensemble de données structurées de prédictions de ventes et marketing pour chaque client par produit Cloud et cluster.</span><span class="sxs-lookup"><span data-stu-id="8b77f-144">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="8b77f-145">Chaque client est évalué à l’aide d’un modèle similaire à la SMB de Microsoft qui détermine l’adéquation du client et Machine Learning algorithmes qui intègrent le comportement en ligne du client définissent comme intention.</span><span class="sxs-lookup"><span data-stu-id="8b77f-145">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="8b77f-146">La notation est fusionnée en clusters qui indiquent la propension d’un client à acheter des produits Microsoft Cloud.</span><span class="sxs-lookup"><span data-stu-id="8b77f-146">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="8b77f-147">**Optimisation**: le système machine learning optimise les modèles en consommant les données de transaction mensuellement et les données d’abonnement trimestriellement.</span><span class="sxs-lookup"><span data-stu-id="8b77f-147">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="8b77f-148">À l’aide des données de Win/Loss, le Machine Learning ajuste les algorithmes et vérifie que les modèles fonctionnent comme prévu en comparant les recommandations de cluster aux opportunités traitées dans MSX.</span><span class="sxs-lookup"><span data-stu-id="8b77f-148">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Capture d’écran des Machine Learning SMB.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="8b77f-150">CloudAscent</span><span class="sxs-lookup"><span data-stu-id="8b77f-150">CloudAscent Propensity</span></span>

<span data-ttu-id="8b77f-151">Comment les recommandations de propension sont-elles créées ?</span><span class="sxs-lookup"><span data-stu-id="8b77f-151">How are propensity recommendations created?</span></span>

<span data-ttu-id="8b77f-152">À l’aide des signaux collectés via des robots d’indexation et des données Web fournis par diverses sources, nous avons consolidé les données firmographics et les signaux des réseaux sociaux du client.</span><span class="sxs-lookup"><span data-stu-id="8b77f-152">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="8b77f-153">La notation utilise ces signaux et données dans des modèles de comparaison pour les modèles d’ajustement et de notation pour l’intention.</span><span class="sxs-lookup"><span data-stu-id="8b77f-153">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="8b77f-154">Ajustement du compte client</span><span class="sxs-lookup"><span data-stu-id="8b77f-154">Customer Account Fit</span></span>

   - <span data-ttu-id="8b77f-155">Points de données internes et externes qui définissent firmographics.</span><span class="sxs-lookup"><span data-stu-id="8b77f-155">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="8b77f-156">Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits.</span><span class="sxs-lookup"><span data-stu-id="8b77f-156">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="8b77f-157">L’ajustement ajusté est mis à jour tous les trimestres</span><span class="sxs-lookup"><span data-stu-id="8b77f-157">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="8b77f-158">Intention du compte client</span><span class="sxs-lookup"><span data-stu-id="8b77f-158">Customer Account Intent</span></span>

   - <span data-ttu-id="8b77f-159">Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client.</span><span class="sxs-lookup"><span data-stu-id="8b77f-159">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="8b77f-160">La notation intentionnelle est superposée sur ajuster pour définir les clusters.</span><span class="sxs-lookup"><span data-stu-id="8b77f-160">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="8b77f-161">La notation intentionnelle est mise à jour tous les mois.</span><span class="sxs-lookup"><span data-stu-id="8b77f-161">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modèles prédictifs SMB CloudAscent.":::

3. <span data-ttu-id="8b77f-163">Clustering</span><span class="sxs-lookup"><span data-stu-id="8b77f-163">Clustering</span></span>

   <span data-ttu-id="8b77f-164">Les signaux pour l’adéquation et l’intention sont consolidés dans un score de clustering.</span><span class="sxs-lookup"><span data-stu-id="8b77f-164">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="8b77f-165">CloudAscent a quatre clusters :</span><span class="sxs-lookup"><span data-stu-id="8b77f-165">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="8b77f-166">Agissez maintenant-clients prêts à l’emploi</span><span class="sxs-lookup"><span data-stu-id="8b77f-166">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="8b77f-167">Évaluer : clients prêts pour la commercialisation</span><span class="sxs-lookup"><span data-stu-id="8b77f-167">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="8b77f-168">Campagnes de sensibilisation aux lecteurs</span><span class="sxs-lookup"><span data-stu-id="8b77f-168">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="8b77f-169">Éduquer-éduquer et surveiller l’intention</span><span class="sxs-lookup"><span data-stu-id="8b77f-169">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="8b77f-170">Le clustering permet aux utilisateurs de cibler des clients spécifiques pour des initiatives de vente et de marketing basées sur des facteurs de segment, par exemple : produit, géo, secteur et vertical.</span><span class="sxs-lookup"><span data-stu-id="8b77f-170">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="8b77f-171">L’onglet **modèle de propensation** des classeurs CloudAscent partage le propension et le revenu estimé des espaces blancs.</span><span class="sxs-lookup"><span data-stu-id="8b77f-171">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="8b77f-172">Pour définir le clustering de l’ajustement et de l’intention, nous allons suivre les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8b77f-172">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="8b77f-173">En utilisant des modèles ML, nous commençons par calculer le score du client et le score d’intention sur une échelle de 100.</span><span class="sxs-lookup"><span data-stu-id="8b77f-173">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="8b77f-174">Les scores exacts varient en fonction des modèles ML.</span><span class="sxs-lookup"><span data-stu-id="8b77f-174">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="8b77f-175">Exemples de scores ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="8b77f-175">Example Scores Below:</span></span>

         |<span data-ttu-id="8b77f-176">**Classification**</span><span class="sxs-lookup"><span data-stu-id="8b77f-176">**Classification**</span></span>|<span data-ttu-id="8b77f-177">**Score**</span><span class="sxs-lookup"><span data-stu-id="8b77f-177">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="8b77f-178">Élevé</span><span class="sxs-lookup"><span data-stu-id="8b77f-178">High</span></span>|<span data-ttu-id="8b77f-179">75-100</span><span class="sxs-lookup"><span data-stu-id="8b77f-179">75 - 100</span></span>|
         |<span data-ttu-id="8b77f-180">Moyenne</span><span class="sxs-lookup"><span data-stu-id="8b77f-180">Medium</span></span>|<span data-ttu-id="8b77f-181">55-74</span><span class="sxs-lookup"><span data-stu-id="8b77f-181">55 - 74</span></span>|
         |<span data-ttu-id="8b77f-182">Faible</span><span class="sxs-lookup"><span data-stu-id="8b77f-182">Low</span></span>|<span data-ttu-id="8b77f-183">30 - 54</span><span class="sxs-lookup"><span data-stu-id="8b77f-183">30 - 54</span></span>|
         |<span data-ttu-id="8b77f-184">Très faible</span><span class="sxs-lookup"><span data-stu-id="8b77f-184">Very Low</span></span>|<span data-ttu-id="8b77f-185">0 - 29</span><span class="sxs-lookup"><span data-stu-id="8b77f-185">0 - 29</span></span>|

      2. <span data-ttu-id="8b77f-186">À l’aide de la règle ci-dessus, nous classons les entreprises pour qu’elles soient élevées, moyennes, basses et très basses à la fois sur l’adaptabilité des clients et les signaux d’intention.</span><span class="sxs-lookup"><span data-stu-id="8b77f-186">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="8b77f-187">Nous allons tracer les signaux d’ajustement et d’intention des clients sur une matrice 2D avec chaque intersection représentant la distribution.</span><span class="sxs-lookup"><span data-stu-id="8b77f-187">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="8b77f-188">Par exemple, haute adaptation + haute intention = a1, représentant la plus grande distribution.</span><span class="sxs-lookup"><span data-stu-id="8b77f-188">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="8b77f-189">Enfin, ces segments regroupent les clusters.</span><span class="sxs-lookup"><span data-stu-id="8b77f-189">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="8b77f-190">Par exemple, a1, a2, a3, A4 forment le cluster Act Now.</span><span class="sxs-lookup"><span data-stu-id="8b77f-190">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modèles CloudAscent.":::

   <span data-ttu-id="8b77f-192">Pour ces clients, nous vous recommandons de cibler Act maintenant et d’évaluer les clients.</span><span class="sxs-lookup"><span data-stu-id="8b77f-192">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="8b77f-193">Modèles de & produits CloudAscent</span><span class="sxs-lookup"><span data-stu-id="8b77f-193">CloudAscent Products & Models</span></span>

<span data-ttu-id="8b77f-194">Le graphique suivant fournit une vue de chaque modèle de propension dans CloudAscent :</span><span class="sxs-lookup"><span data-stu-id="8b77f-194">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modèle de propension CloudAscent.":::

<span data-ttu-id="8b77f-196">Les modèles d’espace blanc sont composés de prédictions pour les clients Microsoft existants où ils ne disposent pas d’un produit et/ou sont des clients net New Prospect.</span><span class="sxs-lookup"><span data-stu-id="8b77f-196">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="8b77f-197">Les modèles de vente incitative utilisent des données de transaction pour prédire le potentiel de vente incitative dans Azure et les références SKU M365.</span><span class="sxs-lookup"><span data-stu-id="8b77f-197">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="8b77f-198">EOS partage les clients de fin de service pour Win 7, Office 2010, SQL Server et Windows Server.</span><span class="sxs-lookup"><span data-stu-id="8b77f-198">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="8b77f-199">Les données de la surcharge sont extraites de MS sales et déplacées avec la modélisation de propension CloudAscent, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="8b77f-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="8b77f-200">Les données de EOS résident dans le travail moderne et les ventes Azure sont exécutées.</span><span class="sxs-lookup"><span data-stu-id="8b77f-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
