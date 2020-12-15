---
title: Définitions de données Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Le document fournit la liste de divers rapports et les définitions de données de chaque rapport, qui peuvent être téléchargés à partir de la page de rapport à télécharger Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501747"
---
# <a name="export--data-definitions"></a>Export : définitions de données 

 **Rôles appropriés** 

- Visionneuse de rapports 
- Visionneuse de rapports de la direction 

## <a name="introduction"></a>Introduction 

Le Hub télécharger des rapports dans le tableau de bord Insights vous permet d’exporter les jeux de données brutes.  

Les différents rapports, qui peuvent être téléchargés en même temps que la définition des données, sont les suivants : 

**Profil de partenaire**: les définitions de données des différents champs du rapport de profil sont : 


| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|MPNId|ID de Microsoft Partner Network|
|PartnerName|Nom du partenaire |
|PGA_MPNId|ID MPN du compte global du partenaire|
|PGA_PartnerName|Nom du compte global du partenaire|
|City|Ville du partenaire |
|Country|Emplacement du pays du partenaire |
|HierarchyLevel|Indique s’il s’agit d’un ID MPN global ou d’un ID MPN d’emplacement|

**Détails du client**: les définitions des données des différents champs du rapport Détails du client sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerName|Nom du client |
|CustomerTenantId|ID de locataire du client |
|CustomerTpid|Identificateur parent supérieur du client |
|CustomerSegment|Segment du client |
|CustomerMarket|Marché géographique du client  |
|CustomerStatus|État du client (active/inactive) |
|Produit|Le produit est vendu au client par MPN. Il s’agira de O365, D365, Enterprise Mobility, Power BI Microsoft Azure.|
|Référence|   Référence SKU de produit|
|Month| Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés|
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nom du partenaire|
|PartnerLocation|   Emplacement géographique du partenaire|
|PartnerAttributionType|    Type d’attribution de partenaire|
|SalesChannel|  Canal de vente|
|AvailableSeats|    Sièges disponibles| 
|RevenueUSD|    Revenu en USD|

**Performances du revendeur**: les définitions des données des différents champs des rapports de performances du revendeur sont les suivantes :

> [!Note]
> Les données de chiffre d’affaires et ACR sont uniquement disponibles pour les utilisateurs qui sont des visionneuses de rapports d’encadrement.

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|ResellerMpnid|Identificateur du Microsoft Partner Network du revendeur| 
|Nom du revendeur|Nom du revendeur|
|ResellerMarket|Pays du revendeur du marché| 
|IndirectProviderMPNId|Identificateur de Microsoft Partner Network du fournisseur indirect|
|IndirectProviderName|Nom du fournisseur indirect|
|Month|Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés|
|Produit|Nom du produit|
|SubscriptionID|Identificateur d’abonnement|
|AvailableSeats|Nombre de sièges disponibles|
|AssignedSeats|Nombre de sièges affectés|
|BilledRevenueUSD|Revenu facturé (en $)|
|CustomerName|Nom du client| 
|CustomerTPid|Identificateur parent supérieur du client| 
|CustomerSegment|Segment du client |
|CustomerMarket|Marché géographique du client |
|ResellerStatus|État du revendeur| 

**Détails des abonnements**: les définitions des données des différents champs du rapport Détails de l’abonnement sont :

>[!Note]
>Les données de chiffre d’affaires et ACR sont uniquement disponibles pour les utilisateurs qui sont des visionneuses de rapports exécutifs

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|SubscriptionId|    GUID de l’abonnement|
|SubscriptionStartDate| Date de début de l’abonnement|
|SubscriptionEndDate|   Date de fin de l’abonnement|
|SubscriptionState| État de l’abonnement (actif ou en cours d’exécution)|
|Month| Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés|
|IsAutoRenew|   Indique si l’abonnement est un renouvellement automatique ou non (o/N)|
|CustomerName|  Nom du client| 
|CustomerTenantId|  GUID du client|
|CustomerTpid|  Identificateur parent supérieur du client| 
|CustomerSegment|   Segment de marché du client| 
|CustomerMarket|    Marché géographique du client|
|Produit|   Produit vendu au client par le partenaire| 
|Référence|   Référence SKU du produit |
|MPNId| ID Microsoft Partner Network du partenaire |
|PartnerName|   Nom du partenaire |
|PartnerLocation|   Emplacement géographique du partenaire |
|PartnerAttributionType|    Type d’attribution de l’abonnement|
|SalesChannel|  Canal des ventes (direct/CSP, etc.) |
|AvailableSeats|    Siège actuellement disponible|
|RevenueUSD|    Revenu en USD|
|ID d’inscription| ID d’inscription de l’abonnement|

**Utilisation d’Azure**: les définitions de données des différents champs du rapport d’utilisation Azure sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|SubscriptionId|    GUID de l’abonnement|
|SubscriptionStartDate| Date du début de l’abonnement.|
|SubscriptionEndDate|   Date de fin de l’abonnement.|
|SubscriptionState| État actuel de l’abonnement (ouvert/fermé/actif/en période d’indisponibilité)|
|Month| Date agrégée par mois |
|NomService|   Nom du service Azure|
|MeterCategory| Nom de la catégorie de compteur|
|UsageUnits|    Nombre d’unités utilisées pendant le cycle de facturation |
|CustomerName|  Nom du client |
|CustomerTenantId|  ID de locataire du client |
|CustomerTpid|  ID parent du client supérieur |
|CustomerSegment|   Segment du client |
|CustomerMarket|    Marché géographique du client |
|MPNId  |ID de Microsoft Partner Network du client |
|PartnerName|   Nom du partenaire |
|PartnerLocation    |Emplacement géographique du partenaire |
|PartnerAttributionType |Type d’attribution de partenaire|
|SalesChannel|  Canal des ventes (direct/CSP indirect/CSP direct, etc.) |
|ACR_USD|   Chiffre d’affaires Azure consommé en USD|
|ID d’inscription| ID d’inscription de l’abonnement Azure|

**Office 365-utilisation de la licence**: les définitions des données des différents champs du rapport d’utilisation des licences Office 365 sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerTenantId|  ID de locataire du client| 
|CustomerTpid|  ID parent du client supérieur |
|WorkloadName|  SFB, équipes, EXO |
|Month| Mois pour lequel l’utilisation est signalée|
|PaidAvailableUnits|    Nombre d’unités disponibles payantes|
|MonthlyActiveUsers|    Nombre d’utilisateurs actifs mensuels|
|CustomerName|  Nom du client|
|CustomerMarket|    Emplacement géographique du marché du client |
|CustomerSegment|   Segment du client |
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nom du partenaire|
|PartnerLocation|   Emplacement géographique du partenaire|
|PartnerAttributionType|    Type d’attribution de partenaire|

**Enterprise Mobility – utilisation des licences**: la définition des données des différents champs du rapport EMS – utilisation des licences est la suivante :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerTenantId|  ID de locataire du client| 
|CustomerTpid|  ID parent du client supérieur |
|WorkloadName|  Nom de la charge de travail EMS |
|Month| Mois pour lequel l’utilisation est signalée|
|PaidAvailableUnits|    Nombre d’unités disponibles payantes|
|MonthlyActiveUsers|    Nombre d’utilisateurs actifs mensuels|
|CustomerName|  Nom du client|
|CustomerMarket|Emplacement géographique du marché du client |
|CustomerSegment|   Segment du client |
|MPNId| ID de Microsoft Partner Network|
|PartnerName|   Nom du partenaire|
|PartnerLocation|   Emplacement géographique du partenaire|
|PartnerAttributionType|    Type d’attribution de partenaire|

**Dynamics 365 – utilisation** de la licence : la définition des données des différents champs du rapport Dynamics 365 – utilisation des licences est la suivante :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|SubscriptionId|GUID de l’abonnement|
|SubscriptionStartDate| Date de début de l’abonnement|
|SubscriptionEndDate|   Date de fin de l’abonnement|
|SubscriptionStatus|    État de l’abonnement |
|Month| Mois pour lequel l’utilisation est signalée|
|RevSumDivisionName|    Nom de la Division Rev Sum|
|RevSumCategoryName|    Nom de la catégorie Rev Sum|
|Référence|   Référence SKU du produit |
|SKUId| ID de référence du produit |
|FreeVsPaidSKU| Indique s’il s’agit d’une référence gratuite ou payante |
|Works Sales|    Canal de vente utilisé pour la vente de l’abonnement|
|DetailedSalesModel|    Modèle de vente détaillé pour l’abonnement|
|CustomerName|  Nom du client |
|CustomerTenantId|  GUID du locataire client |
|CustomerTpid|  Identificateur parent supérieur du client |
|CustomerSegment|   Segment de marché du client |
|CustomerMarket|    Marché géographique du client |
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Nom du partenaire |
|PartnerLocation|   Emplacement géographique du partenaire |
|PartnerAttachType| Type d’attribution de l’abonnement|
|AvailableSeats|    Siège actuellement disponible|
|AssignedSeats| Siège actuellement affecté |
|ActiveSeats|   Sièges actifs actuels |
|DeploymentOpportunity| Opportunité de déploiement actuelle|
|ActiveUsagePercent|    Pourcentage d’utilisation actif actuel|
 
**Utilisation de la licence Power bi**: la définition des données des différents champs du rapport Power bi – utilisation des licences est la suivante :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|SubscriptionId|    GUID de l’abonnement|
|SubscriptionStartDate| Date de début de l’abonnement|
|SubscriptionEndDate|   Date de fin de l’abonnement|
|SubscriptionStatus|    État de l’abonnement (actif ou In-Active ou période de grâce)|
|Month| Date agrégée par mois |
|Référence|   Référence SKU du produit |
|SKUId| ID de référence du produit |
|FreeVsPaidSKU| Différentiation SKU gratuit ou payant |
|Works Sales|    Modèle de vente utilisé pour vendre l’abonnement|
|DetailedSalesModel|    Modèle de vente détaillé pour l’abonnement|
|CustomerName|  Nom du client |
|CustomerTenantId|  GUID du locataire client |
|CustomerTpid|  Identificateur parent supérieur du client| 
|CustomerSegment|   Segment de marché du client |
|CustomerMarket|    Marché géographique du client |
|MPNId| ID de Microsoft Partner Network |
|PartnerName|   Nom du partenaire |
|PartnerLocation|   Emplacement géographique du partenaire |
|PartnerAttachType| Type d’attribution de l’abonnement|
|AvailableSeats|    Sièges actuellement disponibles|
|AssignedSeats| Sièges actuellement affectés|
|ActiveSeats|   Sièges actifs actuels|
|DeploymentOpportunity| Opportunité de déploiement actuelle|
|ActiveUsagePercent|    Pourcentage d’utilisation actif actuel|

**Utilisation des équipes – réunions et appels**: les définitions de données des différents champs sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerTenantId|  ID de locataire du client |
|CustomerTpid|  ID parent du client supérieur |
|Month| Mois pour lequel l’utilisation est signalée|
|Sous-charge de travail|   Charge de travail secondaire pour laquelle l’utilisation est signalée (réunions, appels, systèmes de téléphonie)|
|Nombre de réunions| Nombre de réunions|
|Durée de la réunion|  Durée totale de la réunion en heures|

**Équipes-détails de l’utilisation mensuelle**: les définitions des données des différents champs sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerTenantId|  ID de locataire du client |
|CustomerTpid|  ID parent du client supérieur |
|Month| Mois pour lequel l’utilisation est signalée|
|Sous-charge de travail|   Charge de travail secondaire pour laquelle l’utilisation est signalée (réunions, appels, systèmes de téléphonie)|
|Utilisateurs du Bureau| Nombre d’utilisateurs utilisant teams sur le Bureau|
|Utilisateurs mobiles|  Nombre d’utilisateurs utilisant des équipes sur des appareils mobiles|
|Utilisateurs Web| Nombre d’utilisateurs utilisant des équipes sur le Web|
|AllUpParticipants| Nombre d’utilisateurs distincts d’équipes pour le mois|

**Utilisation des équipes – applications 3P**: les définitions de données des différents champs sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CustomerTenantId|  ID de locataire du client| 
|CustomerTpid|  ID parent du client supérieur |
|Month| Mois pour lequel l’utilisation est signalée|
|Nom de l’application 3P|   Nom de l’application teams|
|Nombre d’utilisateurs|    Nombre d’utilisateurs pour l’application|


**Détails** de la formation : les définitions des données des différents champs du rapport Détails de formation sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|TrainingActivityId|    Identificateur de l’apprentissage |
|TrainingTitle| Titre de la formation |
|TrainingType|  Type d’apprentissage (certification/examen)|
|IndividualFirstName|   Prénom du client| 
|IndividualLastName|    Nom du client| 
|E-mail| ID de messagerie personnelle du client|
|CorpEmail| ID de messagerie Office du client|
|TrainingCompletionDate|    Date d’achèvement de la formation |
|Month| Mois pour lequel les données sont signalées|
|IcMCP| Indique si l’utilisateur est un professionnel certifié Microsoft|
|MCPID| ID MCP de l’utilisateur|
|MPNId| ID de Microsoft Partner Network |
|PartnerName|   Nom du partenaire |
|PartnerCityLocation|   Emplacement géographique de la ville du partenaire |
|PartnerCountryLocation|    Emplacement géographique du partenaire |

**Microsoft Learn**: les définitions de données des différents champs du rapport d’Microsoft Learn sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|UserName|Nom de l’utilisateur| 
|UserId|GUID de l’utilisateur |
|TrainingName|Nom de l’apprentissage |
|TrainingType|Type d’apprentissage (chemin d’accès du module/Learning)|
|Produits|Produit pour lequel le module d’apprentissage est applicable|
|Rôles|Rôles applicables de l’apprentissage |
|CompletionDate|Date de fin de l’apprentissage |
|MPNId|ID de Microsoft Partner Network |
|PartnerName|Nom du partenaire |
|Country|Emplacement géographique du partenaire |

**Résumé et historique des compétences**: la définition des données des différents champs du rapport Résumé et historique des compétences est la suivante :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CompetencyName|Nom de la compétence |
|CompetencyLevel|Niveau de compétence (Gold/Silver)|
|CompetencyStatus|État actuel de la compétence (actif/inactif/période de grâce)|
|CompetencyStartDate|Date de début de la compétence donnée| 
|CompetencyEndDate|Date de fin de la compétence donnée |

**Performances** de la compétence : les définitions des données des différents champs du rapport de performances des compétences sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|CompetencyName|    Nom de la compétence |
|CompetencyAttainmentOptionName|    Nom de l’option de réalisation de la compétence|
|Month| Mois pour lequel les métriques sont signalées|
|MetricName|    Nom de la métrique en rapport avec la compétence|
|MetricMonthlyContribution| Contribution mensuelle de la mesure|
|TTMAggregate|  Métrique agrégée pour les 12 mois de fin|
|AnniversaryYearAggregate|  Mesure agrégée pour l’année anniversaire actuelle|
|GoldThreshold| Exigences en matière de performances pour répondre aux compétences Gold|
|SilverThreshold|   Exigences en matière de performances pour répondre à la compétence Silver|

**Distribution ascendante du Cloud M365**: les définitions de données des différents champs du rapport de proportions du Cloud ascendant-M365 sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nom du partenaire|  Nom du partenaire|
|ID de client|   Numéro d’identificateur du client |
|Numéro DUNS|   Le numéro dun & Bradstreet du client dont le score est évalué pour la propension|
|Nom du compte|  Nom du compte |
|Domaine|    Domaine du compte|
|Taille de l’Organisation|  Taille de l’Organisation|
|Industrie|  Industrie  |
|Vertical|  La verticale du client dont le score est calculé pour la distribution, tel qu’identifié par Microsoft et d’autres normes du secteur (D&B)|
|Domaine|  Zone géographique de l’emplacement|
|Filiale|    La filiale du client dont le score est évalué pour la distribution|
|Secteur de vente|   Secteur de vente du client dont le score est évalué pour la distribution|
|City|  Emplacement géographique de la ville |
|État| Emplacement de l’état géographique|
|Code postal|   Code postal|
|Country|   Emplacement du pays géographique |
|Segment|   Segment de marché |
|Sous-segment|   Sous-segment Market |
|Résumé du type SMC|  Type SMC |
|Top non gérée-base de calcul|  Principaux clients non gérés : calcul|
|Top non géré-base de l’utilisateur| Principaux clients non gérés – utilisateur|
|IsNonProfit|   Si vous n’êtes pas lucratif ou lucratif (oui/non)|
|Activer la cible de travail à distance Exchange Online|   Clients disposant d’un abonnement Exchange Online, incitative à M365|
|Activer l’acquisition local à distance (version actuelle) avec la distribution de la version de Class-+ 10 licences|Le client qui a actuellement un client local Office ou Win (c’est-à-dire, les versions qui sont postérieures aux produits EOS). Le client dispose de 10 licences ou plus. Client ayant un score de propensation. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local à distance (version actuelle) avec la propensation de la <10 licences|Le client qui a actuellement un client local Office ou Win (c’est-à-dire, les versions qui sont postérieures aux produits EOS). Le client a moins de 10 licences. Client ayant un score de propensation. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local à distance (version actuelle) sans la distribution de la version de Class-+ 10 licences| Le client qui a actuellement un client local Office ou Win (c’est-à-dire, les versions qui sont postérieures aux produits EOS). Le client dispose de 10 licences ou plus. Le client n’a pas de score de proportions. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local à distance (version actuelle) sans propensation de la version de solution-<10 licences| Le client qui a actuellement un client local Office ou Win (c’est-à-dire, les versions qui sont postérieures aux produits EOS). Le client a moins de 10 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local à distance (EOS) à l’aide de la distribution de la solution Class-+ 10 licences|Client qui a un client local Office ou Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client dispose de 10 licences ou plus. Le client a un score de propension. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local à distance (EOS) avec une propensation de la <10 licences|Client qui a un client local Office ou Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client a moins de 10 licences. Le client a un score de propension. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition en local (EOS) à distance sans la distribution de la distribution de la solution-+ 10 licences| Le client qui a actuellement un client local Office ou Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client dispose de 10 licences ou plus. Le client n’a pas de score de proportions. Les partenaires doivent cibler la conversion en M365.|
|Activer l’acquisition local (EOS) à distance sans propensation de la <10 licences| Le client qui a actuellement un client local Office ou Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client a moins de 10 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler la conversion en M365.|
|Activer le travail à distance-Prospect de propension élevé pour M365 (Act Now/Evaluate)| Prospect client avec une grande propension pour M365.|
|Activer le travail à distance-concurrence (zoom) avec M365| Clients avec zoom et M365, ciblés pour la conversion en équipes|
|Activer le travail à distance-concurrence (zoom) sans M365|  Clients avec zoom, cible pour la conversion en équipes|
|Réduire les coûts et gérer-M365 E3 ciblé pour M365 E5| Client existant avec M365 E3, cible pour M365 E5|
|Réduisez les coûts et gérez les clients M365 BB et BS ciblés pour M365 BP|    Clients M365 BB et BS existants, ciblant ceux-ci pour M365 BP|
|Transformer la productivité de l’organisation-propension des surfaces|    Le client illustre la propension pour surface.|
|M365Cluster|Identifie la propension du client pour l’achat de M365.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|M365Fit|   Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|M365Intent|    Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|SurfaceCluster|    Cela identifie la propension du client pour l’achat de surface en consolidant les recommandations d’adéquation et d’intention dans un cluster.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|SurfaceFit|    Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|SurfaceIntent| Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|O365Cluster|   Cela identifie la propension du client pour acheter O365.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|O365Fit|   Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|O365Intent|    Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|M365UpsellCustomer|    Cela indique si le client présente une propension de vente incitative pour M365|
|A Google|    Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits Google|
|A AWS|   Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits AWS|
|A EA|    Cela indique si un renouvellement est un contrat entreprise (EA) ou un abonnement EA|
|A ouvert|  Cela indique si un renouvellement est un accord de valeur Open ou Open|

**Distribution ascendante du Cloud D365**: les définitions de données des différents champs du rapport de proportions du Cloud ascendant-D365 sont les suivantes :

| **Nom de la colonne** | **Description des données** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nom du partenaire|  Nom du partenaire|
|ID de client|   Numéro d’identificateur du client |
|Numéro DUNS|   Le numéro dun & Bradstreet du client dont le score est évalué pour la propension|
|Nom du compte|  Nom du compte |
|Domaine|    Domaine du compte|
|Taille de l’Organisation|  Taille de l’Organisation|
|Industrie|  Industrie  |
|Vertical|  La verticale du client dont le score est calculé pour la distribution, tel qu’identifié par Microsoft et d’autres normes du secteur (D&B)
|Domaine|  Zone géographique de l’emplacement|
|Filiale|    La filiale du client dont le score est évalué pour la distribution|
|Secteur de vente|   Secteur de vente|
|City|  Emplacement géographique de la ville |
|État| Emplacement de l’état géographique|
|Code postal|   Code postal|
|Country|   Emplacement du pays géographique |
|Segment|   Segment de marché |
|Sous-segment|   Sous-segment Market |
|Résumé du type SMC|  La catégorisation d’un client : les principales bases d’utilisateurs non gérées sont des clients avec plus de 300 employés. les principales bases de calcul non gérées sont des clients avec un potentiel de 10 000 $ dans Azure, les entreprises de taille moyenne étant des clients comptant 25 employés ou plus, les petites entreprises sont des clients comptant moins de 25 employés.|
|Top non gérée-base de calcul   |Principaux clients non gérés : calcul|
|Top non géré-base de l’utilisateur| Principaux clients non gérés – utilisateurs|
|IsNonProfit|   Si vous n’êtes pas lucratif ou lucratif (oui/non)|
|Activer la vente numérique-M365-taille de siège >= 25 sièges (modèle de propension SalesPro)|   Client sans D365. Taille du siège : 25 +. Les partenaires doivent cibler la vente croisée de D365 SalesPro|
|Activer la vente numérique-D365 SalesPro propension (Act Now/Evaluate) |Clients de propension élevés sans D365.  Les partenaires doivent cibler D365 SalesPro.|
|Gestion des risques financiers & fraude-Dynamics on-local install base-Navision (modèle de propension BC)|Client existant avec local Navision.  Le partenaire doit cibler D365 BC|
|Gestion des risques financiers & fraude-Dynamics on-local install base-AX (modèle de propension F&O)    |Client existant avec local AX.  Le partenaire doit cibler D365 F&O|
|Gestion des risques financiers & fraude-Dynamics on-local install base-Great Plains (modèle de propensation BC)|  Client existant avec local Great Plains.  Le partenaire doit cibler D365 BC|
|Gestion des risques financiers & fraude-Dynamics on-local install base-Solomon (modèle de propension BC)|Client existant avec local Solomon.  Le partenaire doit cibler D365 BC|
|Gestion des risques financiers & fraude-Dynamics on-local install base-others (modèle de propension BC) |Un client existant avec d’autres solutions local non mentionnées ci-dessus.  Le partenaire doit cibler D365 BC|
|Créer des processus d’entreprise agile-Dynamics on-local install base-AX/GP/SL/NAV/autre (modèle de propension D365)|   Créer des processus d’entreprise agile-Dynamics on-local install base-AX/GP/SL/NAV/autre (modèle de propension D365)|
|Créer des processus d’entreprise agiles-Dynamics rivaliser base-Mendix/exposes/Salesforce (modèle de propension D365)| Créer des processus d’entreprise agiles-Dynamics rivaliser base-Mendix/exposes/Salesforce (modèle de propension D365)|
|Créer des processus d’entreprise agiles-D365 F&O installation de base |Clients D365 F&O existants.  Partenaire pour cibler des applications Power Apps.|
|Créer des processus d’entreprise agile-base d’installation D365 BC| Clients D365 BC existants. Partenaire pour cibler des applications Power Apps.|
|Créer des processus d’entreprise agile-base d’installation D365 CE| Clients D365 CE existants. Partenaire pour cibler des applications Power Apps.|
|Créez une chaîne d’approvisionnement résiliente : Gagnez et activez la première charge de travail D365 en tant que chaîne d’approvisionnement D365 avec des clients ERP non-Oracle/SAP|  Ciblez les clients pour la chaîne logistique D365.|
|Créez une chaîne d’approvisionnement résiliente (chaîne d’approvisionnement D365 Cross-Sell) et/ou commerciale/commerce pour les clients D365 CE existants |Clients D365 CE existants à cibler pour la chaîne logistique D365 de vente croisée|
|Créez une chaîne d’approvisionnement résiliente, D365 sup. Chaîne et/ou vente au détail/commerce à D365 CE et (Oracle ou SAP)| Clients D365 CE existants avec Oracle ou SAP à cibler pour la chaîne d’approvisionnement D365|
|D365BCCluster| Cela identifie la propension du client pour acheter D365 Business central.  Les clients qui affichent la propension pour BC seront dans les catégories moyenne et petite.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|D365BCFit| Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|D365BCIntent|  Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|D365FOCluster| Cela identifie la propension du client pour l’achat de D365 Finance and Operations.  Les clients qui affichent la propension pour F&O seront dans les catégories principales non gérées. Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|D365FOFit| Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|D365FOIntent|  Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|D365CECluster| Cela identifie la propension du client pour acheter D365 engagement client.  Les clients qui affichent la propension pour CE seront dans les catégories moyenne et petite.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|D365CEFit| Ajuster pour D365 CE|
|D365CEIntent|  Intention pour D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Cela indique si un client dispose d’un renouvellement ouvert pour Dynamics on-local AX ou CRM.|
|M365UpsellCustomer|    Cela indique si le client présente une propension de vente incitative pour M365|
|A Google|    Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits Google|
|A AWS|   Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits AWS|
|A EA |Cela indique si un renouvellement est un contrat entreprise (EA) ou un abonnement EA|
|A ouvert|  Cela indique si un renouvellement est un accord de valeur Open ou Open|

**Distribution de Ascent-Azure Cloud**: les définitions de données des différents champs du rapport de proportions de Ascent-Azure Cloud sont les suivantes :

|**Nom de la colonne** |**Description des données** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nom du partenaire|  Nom du partenaire|
|ID de client|   Numéro d’identificateur du client |
|Numéro DUNS|   Le numéro dun & Bradstreet du client dont le score est évalué pour la propension|
|Nom du compte|  Nom du compte |
|Domaine|    Domaine du compte|
|Taille de l’Organisation|  Taille de l’Organisation|
|Industrie|  Industrie  |
|Vertical|  La verticale du client dont le score est calculé pour la distribution, tel qu’identifié par Microsoft et d’autres normes du secteur (D&B)|
|Domaine|  Zone géographique de l’emplacement|
|Filiale|    La filiale du client dont le score est évalué pour la distribution|
|Secteur de vente|   Secteur de vente|
|City|  Emplacement géographique de la ville |
|État| Emplacement de l’état géographique|
|Code postal|   Code postal|
|Country|   Emplacement du pays géographique |
|Segment|   Segment de marché |
|Sous-segment|   Sous-segment Market |
|Résumé du type SMC|  Type SMC |
|Top non gérée-base de calcul|  Principaux clients non gérés : calcul|
|Top non géré-base de l’utilisateur| Principaux clients non gérés – utilisateurs|
|IsNonProfit|   Si vous n’êtes pas lucratif ou lucratif (oui/non)|
|Migrer-EOS Win Server-EOS Windows Server IB avec la fonction de distribution de la|   Client qui a un serveur local Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client dispose de 5 licences ou plus. Client ayant un score de propensation.  Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB avec les licences de <5|   Client disposant de la fin de service (local) sur le serveur Win (c’est-à-dire les versions antérieures à et incluant des produits EOS). Le client a moins de 5 licences. Client ayant un score de propensation.  Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB sans la distribution de |Client qui a un serveur local Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). Le client a plus de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB sans la <5 licences|    Client qui a un serveur local Win (c’est-à-dire des versions antérieures à et incluant des produits EOS). A moins de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-EOS SQL-EOS SQL Server IB avec la distribution de la fonction de distribution de l’offre-5 + licences|  Client disposant de local SQL Server (c’est-à-dire, versions antérieures à et incluant des produits EOS). Le client dispose de plus de 5 licences. Le client a un score de propension.  Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-EOS SQL-EOS SQL Server IB avec la propensation de la <5 licences|  Client disposant de local SQL Server (c’est-à-dire, versions antérieures à et incluant des produits EOS). A moins de 5 licences. Client ayant un score de propensation. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-EOS SQL-EOS SQL Server IB sans la distribution de Class-5 + licences|   Client disposant de local SQL Server (c’est-à-dire, versions antérieures à et incluant des produits EOS). Le client dispose de 5 licences ou plus. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-EOS SQL-EOS SQL Server IB sans propension de la <5 licences|   Client disposant de local SQL Server (c’est-à-dire, versions antérieures à et incluant des produits EOS). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer un serveur Win local sur un serveur Windows Server i b en cours avec des licences.|   Le client qui a actuellement un serveur Win local (c’est-à-dire les versions qui sont postérieures aux produits EOS). Le client dispose de plus de 5 licences. Le client a un score de propension. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer sur un serveur Win local-Current Windows Server IB avec la propensation de la <5 licences|   Le client qui a actuellement un serveur Win local (c’est-à-dire les versions qui sont postérieures aux produits EOS). Le client a moins de 5 licences. Le client a un score de propension pour Azure. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer un serveur Win local sur un serveur Windows Server i b en cours sans les licences|    Le client qui a actuellement un serveur Win local (c’est-à-dire les versions qui sont postérieures aux produits EOS). Le client dispose de plus de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer un serveur Win local sur un serveur Windows Server i b en cours sans aucune distribution de <5 licences |Le client qui a actuellement un serveur Win local (c’est-à-dire les versions qui sont postérieures aux produits EOS). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB avec la distribution de la fonction de distribution de l’objet-5 + licences|  Le client qui a actuellement SQL Server local (autrement dit, les versions qui sont postérieures aux produits EOS). Le client dispose de plus de 5 licences. Le client a un score de propension. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB avec la propensation de la <5 licences|  Le client qui a actuellement SQL Server local (autrement dit, les versions qui sont postérieures aux produits EOS). Le client a moins de 5 licences. Le client a un score de propension. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer vers des machines virtuelles SQL Azure ou SQL-actuelle SQL Server IB sans la distribution de Class-5 + licences|   Le client qui a actuellement SQL Server local (autrement dit, les versions qui sont postérieures aux produits EOS). Le client dispose de plus de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB sans propensation de la <5 licences|   Le client qui a actuellement SQL Server local (autrement dit, les versions qui sont postérieures aux produits EOS). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-OSS-migrer vers la base de BD OSS| Client existant avec l’un des produits concurrents suivants : PostgreSQL, MySQL, MariaDB. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrate-OSS-Linux sur Azure |Client existant avec le produit : Linux. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-SAP-SAP sur Azure|  Client existant avec le produit : SAP. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-WVD-RDS IB |Identifie les clients avec des Services Bureau à distance Windows active. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-WVD-travail moderne à vente croisée à Azure/WVD|   Identifie les clients avec M365 et ne dispose pas d’Azure. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-VMware IB|   Client existant avec le produit : VMware. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Migrer-Citrix IB|   Client existant avec le produit : Citrix Systems. Les partenaires doivent cibler ces clients pour la migration vers Azure.|
|Innovation-Analytics-Power BI IB avec une grande distribution Azure|   Les clients avec et active Power BI abonnement, notamment : Power BI-standalone Pro, Power BI-Azure Suites, Power BI-Office, Suites Power BI-M365|
|Enable-DevOps avec GitHub-VisualStudio/MSDN IB|    Clients identifiés avec des studios visuels actifs|
|Version de Win Server standard|   Cela montre la version des achats standard de Windows Server par le client|
|Licence Win Server standard|   Le type de licence des achats Windows Server standard est ainsi affiché par le client.|
|Version du centre de données du serveur Win|    Cela montre la version des achats du centre de données Windows par le client|
|Licence du centre de données du serveur Win| Cela indique le type de licence des achats du centre de données Windows par le client.|
|AzureFit|  Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle similaire à notre meilleur SMB pour comparer les clients et voir s’ils sont susceptibles d’être adaptés à Microsoft Cloud produits. Le score ajusté est mis à jour tous les trimestres.|
|AzureIntent|   Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée sur ajuster pour définir les clusters. La notation intentionnelle est mise à jour tous les mois.|
|AzureCluster|  Cela identifie la propension du client pour acheter Azure en regroupant les recommandations d’adéquation et d’intention dans un cluster.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|WindowsServerDataCenter_HasOpenRenewal|    Cela indique si un client est en cours de renouvellement pour un centre de données Windows Server|
|WindowsServerStandard_HasOpenRenewal|  Cela indique si un client est en cours de renouvellement pour un serveur Windows Server standard|
|AzureUpsellCustomer|   Cela indique si le client présente une propension de vente incitative pour Azure|
|A Google|    Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits Google|
|A AWS|   Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits AWS|
|A EA |Cela indique si un renouvellement est un contrat entreprise (EA) ou un abonnement EA|
|A ouvert|  Cela indique si un renouvellement est un accord de valeur Open ou Open|

**Distribution de renouvellements cloud Ascent-Agreement**: les définitions de données des différents champs du rapport de proportions de renouvellements de l’accord de Cloud ascendant sont les suivantes :

|**Nom de la colonne** |**Description des données** |
|---------|:---------|
|ID MPN|    ID de Microsoft Partner Network|
|Nom du partenaire|  Nom du partenaire|
|ID de client|   Numéro d’identificateur du client |
|Numéro DUNS|   Le numéro dun & Bradstreet du client dont le score est évalué pour la propension|
|Nom du compte|  Nom du compte |
|Domaine|    Domaine du compte|
|Taille de l’Organisation|  Taille de l’Organisation|
|Industrie|  Industrie  |
|Vertical|  La verticale du client dont le score est calculé pour la distribution, tel qu’identifié par Microsoft et d’autres normes du secteur (D&B)|
|Domaine|  Zone géographique de l’emplacement|
|Filiale|    La filiale du client dont le score est évalué pour la distribution|
|Secteur de vente|   Secteur de vente|
|City|  Emplacement géographique de la ville |
|État| Emplacement de l’état géographique|
|Code postal|   Code postal|
|Country|   Emplacement du pays géographique |
|Segment|   Segment de marché |
|Sous-segment|   Sous-segment Market |
|Résumé du type SMC|  Type SMC |
|Top non gérée-base de calcul|  Principaux clients non gérés : calcul|
|Top non géré-base de l’utilisateur| Principaux clients non gérés – utilisateurs|
|IsNonProfit|Si vous n’êtes pas lucratif ou lucratif (oui/non)|
|A Google|Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits AWS|
|A AWS|Cet indicateur détermine si un client présente des signaux compétitifs pour la possession des produits AWS|
|Cluster Azure|Cela identifie la propension du client pour acheter Azure.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|Cluster D365 F&O|  Cela identifie la propension du client pour l’achat de D365 Finance and Operations.  Les clients qui affichent la propension pour F&O seront dans les catégories principales non gérées.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|Cluster D365 CE|   Cela identifie la propension du client pour acheter D365 engagement client.  Les clients qui affichent la propension pour CE seront dans les catégories moyenne et petite.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|Cluster D365 BC|   Cela identifie la propension du client pour acheter D365 Business central.  Les clients qui affichent la propension pour BC seront dans les catégories moyenne et petite.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|Cluster M365|  Cela identifie la propension du client pour l’achat de M365.  Les clusters agissent maintenant et l’évaluation doit être ciblée, car ils produiront un rendement plus élevé.  Assurez-vous que les clients doivent être ciblés uniquement s’il reste de la capacité après avoir ciblé Act Now et évalué les clients.|
|Programme de licence|   Cela identifie le type de programme de licence pour le renouvellement|
|ID de l'accord|  Identificateur de l’accord|
|Date de fin de l’accord|    Date de fin de l’accord |
|Type d'expiration|   Type d’expiration|
|Chiffre d’affaires arrivant à expiration|  Chiffre d’affaires associé aux abonnements arrivant à expiration|
|A EA|    Cela indique si un renouvellement est un contrat entreprise (EA) ou un abonnement EA|
|A ouvert|  Cela indique si un renouvellement est un accord de valeur Open ou Open|
|Client Azure upsell| Cela indique si le client présente une propension de vente incitative pour Azure|
|Client de vente incitative M365|  Cela indique si le client présente une propension de vente incitative pour M365|
|RevSumDivisionName|    Cela identifie le produit qui est utilisé pour le renouvellement|

## <a name="next-steps"></a>Étapes suivantes

Pour obtenir des rapports, consultez [Télécharger des rapports](pci-download-reports.md).
