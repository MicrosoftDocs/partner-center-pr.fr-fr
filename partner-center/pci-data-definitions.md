---
title: Définitions de données Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Le document répertorie les différents rapports et leurs définitions de données, que vous pouvez télécharger à partir de la page de rapport à télécharger Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861391"
---
# <a name="export--data-definitions"></a>Export : définitions de données 

 **Rôles appropriés** 

- Visionneuse de rapports 
- Visionneuse de rapports de la direction 

## <a name="introduction"></a>Introduction 

En utilisant le Hub télécharger des rapports dans le tableau de bord Insights, vous pouvez exporter les jeux de données bruts. 

Les différents rapports, que vous pouvez télécharger avec leurs définitions de données, sont répertoriés dans les tableaux suivants : 

### <a name="partner-profile-report"></a>**Rapport sur les profils de partenaires**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| MPNId | Identificateur de Microsoft Partner Network (MPN) | 
| PartnerName | Nom du partenaire | 
| PGA_MPNId | Identificateur du compte global de partenaire MPN | 
| PGA_PartnerName | Nom du compte global du partenaire | 
| City | Emplacement de la ville du partenaire | 
| Pays ou région | Emplacement du pays du partenaire | 
| HierarchyLevel | Indique s’il s’agit d’un ID MPN global ou d’un ID MPN d’emplacement | 

### <a name="customer-details-report"></a>**Rapport Détails du client**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerName | Nom du client | 
| CustomerTenantId | Identificateur du locataire client | 
| CustomerTpid | Identificateur du parent supérieur du client | 
| CustomerSegment | Segment du client | 
| CustomerMarket | Marché géographique du client | 
| CustomerStatus | État du client (actif ou inactif) | 
| Produit | Le produit a été vendu au client par MPN : O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI ou Microsoft Azure | 
| SKU | Référence SKU de produit | 
| Month | Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttributionType | Type d’attribution du partenaire | 
| SalesChannel | Canal de vente | 
| AvailableSeats | Sièges disponibles | 
| RevenueUSD | Revenu en dollars américains | 

### <a name="reseller-performance-report"></a>**Rapport des performances du revendeur**

> [!Note]
> Les données de chiffre d’affaires et ACR sont uniquement disponibles pour les utilisateurs qui sont des visionneuses de rapports.

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| ResellerMPNid | Identificateur du Microsoft Partner Network du revendeur | 
| ResellerName | Nom du revendeur | 
| ResellerMarket | Pays du revendeur du marché | 
| IndirectProviderMPNId | Identificateur du fournisseur indirect Microsoft Partner Network | 
| IndirectProviderName | Nom du fournisseur indirect | 
| Month | Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés | 
| Produit | Nom du produit | 
| SubscriptionID | Identificateur de l’abonnement | 
| AvailableSeats | Nombre de sièges disponibles | 
| AssignedSeats | Nombre de sièges affectés | 
| BilledRevenueUSD | Revenu facturé en dollars américains | 
| CustomerName | Nom du client | 
| CustomerTPid | Identificateur du parent supérieur du client | 
| CustomerSegment | Segment du client | 
| CustomerMarket | Marché géographique du client | 
| ResellerStatus | État du revendeur | 

### <a name="subscription-details-report"></a>**Rapport Détails de l’abonnement**

>[!Note]
>Les données de chiffre d’affaires et ACR sont uniquement disponibles pour les utilisateurs qui sont des visionneuses de rapports.

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| SubscriptionId | GUID de l’abonnement | 
| SubscriptionStartDate | Date de début de l’abonnement | 
| SubscriptionEndDate | Date de fin de l’abonnement | 
| SubscriptionState | État de l’abonnement (actif ou en cours d’exécution) | 
| Month | Mois pour lequel l’utilisation et le chiffre d’affaires sont signalés | 
| IsAutoRenew | Indique si l’abonnement est un renouvellement autorenouvelé (oui ou non) | 
| CustomerName | Nom du client | 
| CustomerTenantId | GUID du client | 
| CustomerTpid | Identificateur parent supérieur du client | 
| CustomerSegment | Segment de marché du client | 
| CustomerMarket | Marché géographique du client | 
| Produit | Produit vendu au client par le partenaire | 
| SKU | Référence SKU du produit | 
| MPNId | ID Microsoft Partner Network du partenaire | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttributionType | Type d’attribution de l’abonnement | 
| SalesChannel | Canal de ventes-direct, CSP (fournisseur de solutions Cloud), etc. | 
| AvailableSeats | Siège actuellement disponible | 
| RevenueUSD | Revenu en dollars américains | 
| ID d’inscription | ID d’inscription de l’abonnement | 

### <a name="azure-usage-report"></a>**Rapport d’utilisation Azure**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| SubscriptionId | GUID de l’abonnement | 
| SubscriptionStartDate | Date du début de l’abonnement | 
| SubscriptionEndDate | Date de fin de l’abonnement | 
| SubscriptionState | État actuel de l’abonnement (ouvert, fermé, actif ou en période de grâce) | 
| Month | Date agrégée par mois | 
| NomService | Nom du service Azure | 
| MeterCategory | Nom de la catégorie de compteur | 
| UsageUnits | Nombre d’unités utilisées pendant le cycle de facturation | 
| CustomerName | Nom du client | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | ID parent du client supérieur | 
| CustomerSegment | Segment du client | 
| CustomerMarket | Marché géographique du client | 
| MPNId | ID de Microsoft Partner Network du client | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttributionType | Type d’attribution du partenaire | 
| SalesChannel | Canal des ventes (direct/CSP, indirect/CSP, direct, etc.) | 
| ACR_USD | Chiffre d’affaires consommé Azure (ACR) en dollars américains | 
| ID d’inscription | ID d’inscription de l’abonnement Azure | 

### <a name="office-365-license-usage-report"></a>**Rapport d’utilisation de la licence Office 365**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | ID parent du client supérieur | 
| WorkloadName | Skype entreprise, équipes, Exchange Online | 
| Month | Mois pour lequel l’utilisation est signalée | 
| PaidAvailableUnits | Nombre d’unités disponibles payantes | 
| MonthlyActiveUsers | Nombre d’utilisateurs actifs mensuels | 
| CustomerName | Nom du client | 
| CustomerMarket | Emplacement géographique du marché du client | 
| CustomerSegment | Segment du client | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttributionType | Type d’attribution du partenaire | 

### <a name="enterprise-mobility-license-usage-report"></a>**Rapport d’utilisation des licences Enterprise Mobility**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | ID parent du client supérieur | 
| WorkloadName | Nom de la charge de travail Enterprise Mobility + Security (EMS) | 
| Month | Mois pour lequel l’utilisation est signalée | 
| PaidAvailableUnits | Nombre d’unités disponibles payantes | 
| MonthlyActiveUsers | Nombre d’utilisateurs actifs mensuels | 
| CustomerName | Nom du client | 
| CustomerMarket | Emplacement géographique du marché du client | 
| CustomerSegment | Segment du client | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttributionType | Type d’attribution du partenaire | 

### <a name="dynamics-365-license-usage-report"></a>**Rapport d’utilisation de la licence Dynamics 365**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| SubscriptionId | GUID de l’abonnement | 
| SubscriptionStartDate | Date de début de l’abonnement | 
| SubscriptionEndDate | Date de fin de l’abonnement | 
| SubscriptionStatus | État de l’abonnement | 
| Month | Mois pour lequel l’utilisation est signalée | 
| RevSumDivisionName | Nom de la Division Rev Sum | 
| RevSumCategoryName | Nom de la catégorie Rev Sum | 
| SKU | Référence SKU du produit | 
| SKUId | ID de référence du produit | 
| FreeVsPaidSKU | Indique s’il s’agit d’une référence (SKU) gratuite ou payante | 
| Works Sales | Canal de vente utilisé pour la vente de l’abonnement | 
| DetailedSalesModel | Modèle de vente détaillé pour l’abonnement | 
| CustomerName | Nom du client | 
| CustomerTenantId | GUID du locataire client | 
| CustomerTpid | Identificateur parent supérieur du client | 
| CustomerSegment | Segment de marché du client | 
| CustomerMarket | Marché géographique du client | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttachType | Type d’attribution de l’abonnement | 
| AvailableSeats | Siège actuellement disponible | 
| AssignedSeats | Siège actuellement affecté | 
| ActiveSeats | Sièges actifs actuels | 
| DeploymentOpportunity | Opportunité de déploiement actuelle | 
| ActiveUsagePercent | Pourcentage d’utilisation actif actuel | 

### <a name="power-bi-license-usage-report"></a>**Rapport d’utilisation de la licence Power BI**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| SubscriptionId | GUID de l’abonnement | 
| SubscriptionStartDate | Date de début de l’abonnement | 
| SubscriptionEndDate | Date de fin de l’abonnement | 
| SubscriptionStatus | État de l’abonnement (actif, inactif ou période de grâce) | 
| Month | Date agrégée par mois | 
| SKU | Référence SKU du produit | 
| SKUId | ID de référence du produit | 
| FreeVsPaidSKU | Différentiation SKU gratuit ou payant | 
| Works Sales | Modèle de vente utilisé pour vendre l’abonnement | 
| DetailedSalesModel | Modèle de vente détaillé pour l’abonnement | 
| CustomerName | Nom du client | 
| CustomerTenantId | GUID du locataire client | 
| CustomerTpid | Identificateur du parent supérieur du client | 
| CustomerSegment | Segment de marché du client | 
| CustomerMarket | Marché géographique du client | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerLocation | Emplacement géographique du partenaire | 
| PartnerAttachType | Type d’attribution de l’abonnement | 
| AvailableSeats | Sièges actuellement disponibles | 
| AssignedSeats | Sièges actuellement affectés | 
| ActiveSeats | Sièges actifs actuels | 
| DeploymentOpportunity | Opportunité de déploiement actuelle | 
| ActiveUsagePercent | Pourcentage d’utilisation actif actuel | 

### <a name="teams-meetings-and-calls-report"></a>**Rapport des réunions et des appels des équipes**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | Identificateur du parent supérieur du client | 
| Month | Mois pour lequel l’utilisation est signalée | 
| Sous-charge de travail | Sous-charge de travail pour laquelle l’utilisation est signalée (réunions, appels ou systèmes de téléphonie) | 
| Nombre de réunions | Nombre de réunions | 
| Durée de la réunion | Durée totale de la réunion en heures | 

### <a name="teams-monthly-usage-report"></a>**Rapport d’utilisation mensuelle des équipes**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | Identificateur du parent supérieur du client | 
| Month | Mois pour lequel l’utilisation est signalée | 
| Sous-charge de travail | Sous-charge de travail pour laquelle l’utilisation est signalée (réunions, appels ou systèmes de téléphonie) | 
| Utilisateurs du Bureau | Nombre d’utilisateurs qui utilisent des équipes sur le Bureau | 
| Utilisateurs mobiles | Nombre d’utilisateurs qui utilisent des équipes sur des appareils mobiles | 
| Utilisateurs Web | Nombre d’utilisateurs qui utilisent des équipes sur le Web | 
| AllUpParticipants | Nombre d’utilisateurs uniques d’équipes pour le mois | 

### <a name="teams-usage-3p-apps-report"></a>**Rapport d’utilisation des applications 3P apps**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CustomerTenantId | ID de locataire du client | 
| CustomerTpid | ID parent du client supérieur | 
| Month | Mois pour lequel l’utilisation est signalée | 
| Nom de l’application 3P | Nom de l’application teams | 
| Nombre d’utilisateurs | Nombre d’utilisateurs pour l’application | 


### <a name="training-details-report"></a>**Rapport Détails de la formation**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| TrainingActivityId | Identificateur de l’apprentissage | 
| TrainingTitle | Titre de la formation | 
| TrainingType | Type de formation (certification ou examen) | 
| IndividualFirstName | Prénom du client | 
| IndividualLastName | Nom du client | 
| E-mail | ID de messagerie personnelle du client | 
| CorpEmail | ID de messagerie Office du client | 
| TrainingCompletionDate | Date d’achèvement de la formation | 
| Month | Mois pour lequel les données sont signalées | 
| IcMCP | Indique si l’utilisateur est un MCP (Microsoft Certified Professional) | 
| MCPID | ID MCP de l’utilisateur | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| PartnerCityLocation | Emplacement géographique de la ville du partenaire | 
| PartnerCountryLocation | Emplacement géographique du partenaire | 

### <a name="microsoft-learn-report"></a>**Rapport de Microsoft Learn**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| UserName | Nom de l’utilisateur | 
| UserId | GUID de l’utilisateur | 
| TrainingName | Nom de l’apprentissage | 
| TrainingType | Type de formation (module ou parcours d’apprentissage) | 
| Produits | Produit pour lequel le module d’apprentissage est applicable | 
| Rôles | Rôles applicables de l’apprentissage | 
| CompletionDate | Date d’achèvement de la formation | 
| MPNId | Identificateur de Microsoft Partner Network | 
| PartnerName | Nom du partenaire | 
| Pays ou région | Emplacement géographique du partenaire | 

### <a name="competency-summary-and-history-report"></a>**Résumé de la compétence et rapport historique**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CompetencyName | Nom de la compétence | 
| CompetencyLevel | Niveau de la compétence (or ou Silver) | 
| CompetencyStatus | État actuel de la compétence (active, inactive ou dans la période de grâce) | 
| CompetencyStartDate | Date de début de la compétence | 
| CompetencyEndDate | Date de fin de la compétence | 

### <a name="competency-performance-report"></a>**Rapport sur les performances des compétences**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| CompetencyName | Nom de la compétence | 
| CompetencyAttainmentOptionName | Nom de l’option de réalisation de la compétence | 
| Month | Mois pour lequel les métriques sont signalées | 
| MetricName | Nom de la mesure pertinente pour la compétence | 
| MetricMonthlyContribution | Contribution mensuelle de la mesure | 
| TTMAggregate | Métrique agrégée pour les 12 mois de fin | 
| AnniversaryYearAggregate | Mesure agrégée pour l’année anniversaire actuelle | 
| GoldThreshold | Exigences en matière de performances pour répondre aux compétences Gold | 
| SilverThreshold | Exigences en matière de performances pour répondre à la compétence Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Rapport de proportions du Microsoft 365 du Cloud**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nom du partenaire | Nom du partenaire | 
| ID de client | Numéro d’identification du client | 
| Numéro DUNS | Le numéro dun & Bradstreet (D&B) du client dont le score est évalué pour la distribution | 
| Nom du compte | Nom du compte | 
| Domain | Domaine du compte | 
| Taille de l’Organisation | Taille de l’Organisation | 
| Industrie | Secteur auquel appartient l’Organisation | 
| Vertical | La verticale du client dont le score est évalué pour la distribution, tel qu’identifié par Microsoft, D&B et d’autres normes du secteur | 
| Domaine | Zone géographique de l’emplacement | 
| Filiale | La filiale du client dont le score est évalué pour la distribution | 
| Secteur de vente | Le secteur de vente du client dont le score est évalué pour la distribution | 
| City | Emplacement géographique de la ville de l’Organisation | 
| État | Emplacement de l’état géographique de l’Organisation | 
| Code postal | Code postal de l’Organisation | 
| Pays ou région | Emplacement du pays géographique de l’Organisation | 
| Segment | Segment de marché | 
| Sous-segment | Sous-segment de marché | 
| Résumé du type SMC | Type SMC | 
| Top non gérée-base de calcul | Principaux clients non gérés : calcul | 
| Top non géré-base de l’utilisateur | Principaux clients non gérés – utilisateur | 
| IsNonProfit | Indique si l’organisation est non lucrative (oui ou non) | 
| Activer la cible de travail à distance Exchange Online | Clients disposant d’un abonnement Exchange Online, incitative à Microsoft 365 | 
| Activer l’acquisition locale à distance (version actuelle) avec la distribution ascendante Cloud-+ 10 licences | Client disposant d’un bureau local ou d’un client Windows en cours. Autrement dit, la version du client est ultérieure à la version de la fin de vie (EOL). Le client dispose de 10 licences ou plus. Client ayant un score de propensation. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version actuelle) avec la <10 licences Cloud Ascent | Client disposant d’un bureau local ou d’un client Windows actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 10 licences. Client ayant un score de propensation. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version actuelle) sans distribution ascendante Cloud-+ 10 licences | Client disposant d’un bureau local ou d’un client Windows actuel (autrement dit, une version postérieure à la fin de la vie). Le client dispose de 10 licences ou plus. Le client n’a pas de score de proportions. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version actuelle) sans distribution ascendante Cloud-<10 licences | Client disposant d’un bureau local ou d’un client Windows actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 10 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version EOL) avec la distribution ascendante Cloud-+ 10 licences | Client disposant d’un bureau en fin de vie ou d’un client Windows (c’est-à-dire une version EOL ou antérieure). Le client dispose de 10 licences ou plus. Le client a un score de propension. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version EOL) avec la <10 licences Cloud Ascent | Client disposant d’un bureau en fin de vie ou d’un client Windows (c’est-à-dire une version EOL ou antérieure). Le client a moins de 10 licences. Le client a un score de propension. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version EOL) sans la distribution ascendante Cloud-+ 10 licences | Client disposant d’un bureau local ou d’un client Windows actuel (autrement dit, une version EOL ou antérieure). Le client dispose de 10 licences ou plus. Le client n’a pas de score de proportions. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer l’acquisition locale à distance (version EOL) sans la <10 licences Cloud Ascent | Client disposant d’un bureau local ou d’un client Windows actuel (autrement dit, une version EOL ou antérieure). Le client a moins de 10 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler la conversion en Microsoft 365. | 
| Activer le travail à distance-potentiel de propension élevé pour Microsoft 365 (Act NowithEvaluate) | Prospect client avec une grande propension pour Microsoft 365 | 
| Activer le travail à distance-concurrence (zoom) avec Microsoft 365 | Client avec zoom et Microsoft 365, cible pour la conversion en équipes | 
| Activer le travail à distance-concurrence (zoom) sans Microsoft 365 | Client avec zoom, cible pour la conversion en équipes | 
| Réduire les coûts et gérer-Microsoft 365 E3 ciblé pour Microsoft 365 E5 | Client existant avec Microsoft 365 E3, cible pour Microsoft 365 E5 | 
| Réduisez les coûts et gérez les clients standard et de base Microsoft 365 Business ciblés pour Microsoft 365 Business Premium | Clients existants Microsoft 365 Business de base et Business standard, ciblés pour Microsoft 365 Business Premium | 
| Transformer la productivité de l’organisation-propension des surfaces | Le client montre une propension pour la surface | 
| M365Cluster | Identifie la propension d’un client pour l’achat de Microsoft 365. Target Act Now et évaluer les clusters, car ils produisent un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après agir maintenant et évaluez les clients comme ciblés. | 
| M365Fit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour nos meilleures entreprises (PME) pour comparer les clients et déterminer s’ils sont adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| M365Intent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| SurfaceCluster | Identifie la propension d’un client pour l’achat d’une surface en consolidant les recommandations d’adéquation et d’intention dans un cluster. Target Act Now et évaluer les clusters, car ils produisent un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après agir maintenant et évaluez les clients comme ciblés. | 
| SurfaceFit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour nos meilleurs SMB afin de comparer les clients et de déterminer s’ils sont susceptibles d’être adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| SurfaceIntent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| O365Cluster | Identifie la propension du client pour acheter Office 365. Target Act Now et évaluer les clusters, car ils produisent un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après agir maintenant et évaluez les clients comme ciblés. | 
| O365Fit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour nos meilleurs SMB afin de comparer les clients et de déterminer s’ils sont susceptibles d’être adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| O365Intent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| M365UpsellCustomer | Indique si le client affiche la propension de vente incitative pour Microsoft 365 | 
| A Google | Indique si le client affiche des signaux compétitifs pour la possession des produits Google | 
| A AWS | Indique si le client affiche des signaux compétitifs pour les produits Amazon Web Services (AWS) propriétaires | 
| A EA | Indique si un renouvellement est un contrat entreprise (EA) ou un abonnement EA | 
| A ouvert | Indique si un renouvellement est un accord Open ou Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Rapport de proportions du Cloud ascendant-Dynamics 365**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nom du partenaire | Nom du partenaire | 
| ID de client | Numéro d’identificateur du client | 
| Numéro DUNS | Le numéro dun & Bradstreet du client dont le score est évalué pour la propension | 
| Nom du compte | Nom du compte | 
| Domain | Domaine du compte | 
| Taille de l’Organisation | Taille de l’Organisation | 
| Industrie | Secteur auquel appartient l’Organisation | 
| Vertical | La verticale du client dont le score est évalué pour la distribution, tel qu’identifié par Microsoft, D&B et d’autres normes du secteur
| Domaine | Zone géographique de l’emplacement | 
| Filiale | La filiale du client dont le score est évalué pour la distribution | 
| Secteur de vente | Le secteur de vente du client dont le score est évalué pour la distribution | 
| City | Emplacement géographique de la ville | 
| État | Emplacement de l’état géographique | 
| Code postal | Code postal de l’Organisation | 
| Pays ou région | Emplacement du pays géographique | 
| Segment | Segment de marché | 
| Sous-segment | Sous-segment de marché | 
| Résumé du type SMC | La catégorisation d’un client : les principales bases d’utilisateurs non gérées sont des clients avec plus de 300 employés, les principales bases de calcul non gérées étant des clients avec un potentiel de trois ans Azure, les entreprises de taille moyenne sont des clients avec 25 employés ou plus, et les petites entreprises sont des clients comptant moins de 25 employés. | 
| Top non gérée-base de calcul | Principaux clients non gérés : calcul | 
| Top non géré-base de l’utilisateur | Principaux clients non gérés – utilisateurs | 
| IsNonProfit | Indique si l’organisation est non lucrative (oui ou non) | 
| Activer la vente numérique-taille Microsoft 365-siège >= 25 sièges (modèle de propension SalesPro) | Client sans Dynamics 365. Taille du siège : 25 +. Le partenaire doit cibler la vente croisée de Dynamics 365 SalesPro. | 
| Activer la vente numérique-Dynamics 365 SalesPro propension (Act Now ou Evaluate) | Clients à haut niveau de propension sans Dynamics 365. Le partenaire doit cibler Dynamics 365 SalesPro. | 
| Gestion des risques financiers & fraude-Dynamics local installation base-Navision (modèle de propension central de l’entreprise) | Client existant avec Navision local. Le partenaire doit cibler Dynamics 365 Business central. | 
| Gestion des risques financiers & les fraudes-Dynamics local install base-Dynamics AX (Dynamics 365 finance + Operations propensance Model) | Client existant avec AX local. Le partenaire doit cibler pour les opérations Dynamics 365 finance +. | 
| Gestion des risques financiers & fraude-base de l’installation locale de Dynamics-Great Plains (modèle de propensation central de l’entreprise) | Client existant avec des Great Plains locaux. Le partenaire doit cibler Dynamics 365 Business central. | 
| Gestion des risques financiers & fraudes-Dynamics local installation base-Solomon (Business central propensance Model) | Client existant avec Solomon local. Le partenaire doit cibler Dynamics 365 Business central. | 
| Gestion des risques financiers & fraude-Dynamics local installation base-autres (modèle de propension central de l’entreprise) | Client existant avec d’autres solutions locales non listées précédemment. Le partenaire doit cibler Dynamics 365 Business central. | 
| Créer des processus d’entreprise agile-Dynamics local installation base-AX/GP/SL/NAV/autre (modèle de propension Dynamics 365) | Créer des processus d’entreprise agile-Dynamics local installation base-AX/GP/SL/NAV/autre (modèle de propension Dynamics 365) | 
| Créer des processus d’entreprise agiles-Dynamics rivaliser base-Mendix/exposes/Salesforce (modèle de propension Dynamics 365) | Créer des processus d’entreprise agiles-Dynamics rivaliser base-Mendix/exposes/Salesforce (modèle de propension Dynamics 365) | 
| Créer des processus d’entreprise agile-base d’installation de Dynamics 365 finance + Operations | Clients Dynamics 365 finance + Operations existants. Partenaire pour cibler des applications Power Apps. | 
| Créer des processus d’entreprise agile-base d’installation de Dynamics 365 Business central | Clients Dynamics 365 Business central existants. Partenaire pour cibler des applications Power Apps. | 
| Créer des processus d’entreprise agile-base d’installation de Dynamics 365 Customer engagement | Clients existants de l’engagement client Dynamics 365. Partenaire pour cibler des applications Power Apps. | 
| Créez une chaîne d’approvisionnement résiliente : Windows et activez la première charge de travail Dynamics 365 en tant que gestion de la chaîne d’approvisionnement Dynamics 365 avec les clients SAP ou SAP ERP (planification des ressources d’entreprise) | Clients cibles pour la gestion de la chaîne logistique Dynamics 365 | 
| Créez une chaîne d’approvisionnement résiliente : gestion de la chaîne logistique Dynamics 365 entre les ventes croisées et/ou vente au détail ou commerce aux clients existants Dynamics 365 Customer engagement | Clients de l’engagement client Dynamics 365 existants à cibler pour la gestion de la chaîne logistique de vente croisée Dynamics 365. | 
| Créez une chaîne d’approvisionnement résiliente : gestion de la chaîne logistique Dynamics 365 entre les ventes croisées et/ou vente au détail ou commerce à Dynamics 365 client engagement et Oracle ou SAP | Clients Dynamics 365 engagement client existants avec Oracle ou SAP à cibler pour la gestion de la chaîne logistique Dynamics 365 | 
| D365BCCluster | Identifie la propension du client pour acheter Dynamics 365 Business central. Les clients qui présentent une propension pour Business central seront dans les catégories moyenne et petite. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| D365BCFit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour notre meilleur SMB afin de comparer les clients et de déterminer s’ils sont susceptibles d’être adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| D365BCIntent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| D365FOCluster | Identifie la propension du client pour acheter Dynamics 365 Finance and Operations. Les clients qui présentent une propension pour les opérations finance + seront dans les catégories principales non gérées. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| D365FOFit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour notre meilleur SMB afin de comparer les clients et de déterminer s’ils sont susceptibles d’être adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| D365FOIntent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| D365CECluster | Identifie la propension du client pour acheter Dynamics 365 engagement client. Les clients qui présentent une propension pour l’engagement client seront dans les catégories moyenne et petite. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| D365CEFit | Indique la taille de l’engagement client Dynamics 365 | 
| D365CEIntent | Indique l’intention de l’engagement client Dynamics 365 | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Indique si le client dispose d’un renouvellement ouvert pour Dynamics local AX ou CRM | 
| M365UpsellCustomer | Indique si le client affiche la propension de vente incitative pour Microsoft 365 | 
| A Google | Indique si le client affiche des signaux compétitifs pour la possession des produits Google | 
| A AWS | Indique si le client affiche des signaux compétitifs pour la possession des produits AWS | 
| A EA | Indique si un renouvellement est un abonnement EA ou EA | 
| A ouvert | Indique si un renouvellement est un accord Open ou Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Élévation de Cloud-rapport de proportions Azure**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nom du partenaire | Nom du partenaire | 
| ID de client | Numéro d’identificateur du client | 
| Numéro DUNS | Le numéro dun & Bradstreet du client dont le score est évalué pour la propension | 
| Nom du compte | Nom du compte | 
| Domain | Domaine du compte | 
| Taille de l’Organisation | Taille de l’Organisation | 
| Industrie | Industrie | 
| Vertical | La verticale du client dont le score est évalué pour la distribution, tel qu’identifié par Microsoft, D&B et d’autres normes du secteur | 
| Domaine | Zone géographique de l’emplacement | 
| Filiale | La filiale du client dont le score est évalué pour la distribution | 
| Secteur de vente | Le secteur de vente du client dont le score est évalué pour la distribution | 
| City | Emplacement géographique de la ville | 
| État | Emplacement de l’état géographique | 
| Code postal | Code postal de l’Organisation | 
| Pays ou région | Emplacement du pays géographique | 
| Segment | Segment de marché | 
| Sous-segment | Sous-segment de marché | 
| Résumé du type SMC | Type SMC | 
| Top non gérée-base de calcul | Principaux clients non gérés : calcul | 
| Top non géré-base de l’utilisateur | Principaux clients non gérés – utilisateurs | 
| IsNonProfit | Indique si l’organisation est non lucrative (oui ou non) | 
| Migrate-EOL Windows Server-EOL Windows Server IB avec la distribution ascendante de Cloud-5 + licences | Client qui possède un serveur Windows local en fin de vie (c’est-à-dire une version EOL ou antérieure). Le client dispose de 5 licences ou plus. Client ayant un score de propensation. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB avec la propensation de Cloud Ascent-<5 licences | Client qui possède un serveur Windows local en fin de vie (c’est-à-dire une version EOL ou antérieure). Le client a moins de 5 licences. Client ayant un score de propensation. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB sans distribution ascendante de Cloud-plus de 5 licences | Client qui possède un serveur Windows local en fin de vie (c’est-à-dire une version EOL ou antérieure). Le client a plus de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB sans distribution ascendante de Cloud-<5 licences | Client qui possède un serveur Windows local en fin de vie (c’est-à-dire une version EOL ou antérieure). A moins de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB avec la distribution ascendante de Cloud-5 + licences | Client qui a une SQL Server en fin de vie en local (c’est-à-dire une version EOL ou antérieure). Le client dispose de plus de 5 licences. Le client a un score de propension. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-fin de vie SQL-EOL SQL Server IB avec la propensation Cloud Ascent-<5 licences | Client qui a une SQL Server en fin de vie en local (c’est-à-dire une version EOL ou antérieure). A moins de 5 licences. Client ayant un score de propensation. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-fin de vie SQL-EOL SQL Server IB sans la distribution ascendante de Cloud-5 + licences | Client qui a une SQL Server en fin de vie en local (c’est-à-dire une version EOL ou antérieure). Le client dispose de 5 licences ou plus. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-fin de vie SQL-EOL SQL Server IB sans distribution ascendante Cloud-<5 licences | Client qui a une SQL Server en fin de vie en local (c’est-à-dire une version EOL ou antérieure). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer sur site Windows Server-actuel Windows Server IB avec la distribution ascendante de Cloud-5 + licences | Client disposant d’un serveur Windows local actuel (autrement dit, une version postérieure à la fin de la vie). Le client dispose de plus de 5 licences. Le client a un score de propension. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer localement Windows Server-Windows Server i b en cours avec la distribution ascendante de Cloud-<5 licences | Client disposant d’un serveur Windows local actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 5 licences. Le client a un score de propension pour Azure. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer localement Windows Server-Windows Server i b en cours sans la distribution ascendante de Cloud-5 + licences | Client disposant d’un serveur Windows local actuel (autrement dit, une version postérieure à la fin de la vie). Le client dispose de plus de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer localement Windows Server-Windows Server i b en cours sans la distribution ascendante de Cloud-<5 licences | Client disposant d’un serveur Windows local actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer vers Azure SQL ou des machines virtuelles SQL (VM)-actuel SQL Server IB avec la distribution ascendante de Cloud-5 + licences | Client disposant d’un SQL Server local actuel (autrement dit, une version postérieure à la fin de la vie). Le client dispose de plus de 5 licences. Le client a un score de propension. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB avec la distribution ascendante de Cloud-<5 licences | Client disposant d’un SQL Server local actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 5 licences. Le client a un score de propension. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB sans la distribution ascendante de Cloud-5 + licences | Client disposant d’un SQL Server local actuel (autrement dit, une version postérieure à la fin de la vie). Le client dispose de plus de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-migrer vers Azure SQL ou des machines virtuelles SQL-actuelle SQL Server IB sans distribution ascendante de Cloud-<5 licences | Client disposant d’un SQL Server local actuel (autrement dit, une version postérieure à la fin de la vie). Le client a moins de 5 licences. Le client n’a pas de score de proportions. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-OSS-migrer vers la base de code de l’Open source Shakespeare (OSS) | Client existant avec l’un des produits concurrents suivants : PostgreSQL, MySQL, MariaDB. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrate-OSS-Linux sur Azure | Client existant avec Linux. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-SAP-SAP sur Azure | Client existant avec SAP. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-bureau virtuel Windows-Services Bureau à distance IB | Identifie les clients avec des Services Bureau à distance Windows active. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer un bureau virtuel Windows-travail moderne de vente croisée sur Azure/WVD | Identifie les clients avec Microsoft 365 et ne dispose pas d’Azure. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-VMware IB | Client existant avec le produit : VMware. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Migrer-Citrix IB | Client existant avec le produit : Citrix Systems. Le partenaire doit cibler ce client pour la migration vers Azure. | 
| Innovation-Analytics-Power BI IB avec une grande distribution Azure | Les clients avec et active Power BI abonnement, notamment : Power BI-standalone Pro, Power BI-Azure Suites, Power BI-Suites Office, Power BI suite-Microsoft 365 | 
| Enable-DevOps avec GitHub-Visual Studio/MSDN IB | Identifie les clients avec les versions de Visual Studio actives | 
| Version Windows Server standard | Affiche la version des achats standard de Windows Server par le client | 
| Licence Windows Server standard | Affiche le type de licence des achats standard de Windows Server par le client | 
| Version du centre de données Windows Server | Affiche la version des achats du centre de données Windows par le client | 
| Licence du centre de données Windows Server | Affiche le type de licence des achats du centre de données Windows par le client | 
| AzureFit | Points de données internes et externes qui définissent firmographics. Adapter le score utilise un modèle lookalike pour notre meilleur SMB afin de comparer les clients et de déterminer s’ils sont susceptibles d’être adaptés aux produits Cloud Microsoft. Le score ajusté est mis à jour tous les trimestres. | 
| AzureIntent | Les signaux liés aux réseaux sociaux et l’intention du comportement en ligne d’un client. La notation intentionnelle est superposée à l’ajustement pour définir les clusters. La notation intentionnelle est mise à jour tous les mois. | 
| AzureCluster | Identifie la propension du client pour acheter Azure en regroupant les recommandations d’adéquation et d’intention dans un cluster. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| WindowsServerDataCenter_HasOpenRenewal | Indique si le client dispose d’un renouvellement ouvert pour Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Indique si le client dispose d’un renouvellement ouvert pour Windows Server standard | 
| AzureUpsellCustomer | Indique si le client affiche la propension de vente incitative pour Azure | 
| A Google | Indique si le client affiche des signaux compétitifs pour la possession des produits Google | 
| A AWS | Indique si le client affiche des signaux compétitifs pour la possession des produits AWS | 
| A EA | Indique si un renouvellement est un abonnement EA ou EA | 
| A ouvert | Indique si un renouvellement est un accord Open ou Open Value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Rapport de proportions de renouvellement d’accord sur le Cloud**

| Nom de la colonne | Description des données | 
| :--------- | :--------- | 
| ID MPN | ID de Microsoft Partner Network | 
| Nom du partenaire | Nom du partenaire | 
| ID de client | Numéro d’identificateur du client | 
| Numéro DUNS | Le numéro dun & Bradstreet du client dont le score est évalué pour la propension | 
| Nom du compte | Nom du compte | 
| Domain | Domaine du compte | 
| Taille de l’Organisation | Taille de l’Organisation | 
| Industrie | Industrie | 
| Vertical | La verticale du client dont le score est évalué pour la distribution, tel qu’identifié par Microsoft, D&B et d’autres normes du secteur | 
| Domaine | Zone géographique de l’emplacement | 
| Filiale | La filiale du client dont le score est évalué pour la distribution | 
| Secteur de vente | Le secteur de vente du client dont le score est évalué pour la distribution | 
| City | Emplacement géographique de la ville | 
| État | Emplacement de l’état géographique | 
| Code postal | Code postal de l’Organisation | 
| Pays ou région | Emplacement du pays géographique | 
| Segment | Segment de marché | 
| Sous-segment | Sous-segment de marché | 
| Résumé du type SMC | Type SMC | 
| Top non gérée-base de calcul | Principaux clients non gérés : calcul | 
| Top non géré-base de l’utilisateur | Principaux clients non gérés – utilisateurs | 
| IsNonProfit | Indique si l’organisation est non lucrative (oui ou non) | 
| A Google | Indique si le client affiche des signaux compétitifs pour la possession des produits AWS | 
| A AWS | Indique si le client affiche des signaux compétitifs pour la possession des produits AWS | 
| Cluster Azure | Identifie la propension du client pour acheter Azure. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| Cluster D365 finance + Operations | Identifie la propension du client pour acheter Dynamics 365 Finance and Operations. Les clients qui présentent une propension pour les opérations finance + seront dans les catégories principales non gérées. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| Cluster D365 CE | Identifie la propension du client pour acheter Dynamics 365 engagement client. Les clients qui présentent une propension pour l’engagement client seront dans les catégories moyenne et petite. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| Cluster D365 BC | Identifie la propension du client pour acheter Dynamics 365 Business central. Les clients qui présentent une propension pour Business central seront dans les catégories moyenne et petite. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| Cluster Microsoft 365 | Identifie la propension du client pour l’achat de Microsoft 365. Target Act Now et évaluez les clusters, car ils produiront un rendement plus élevé. Ciblez et apprenez aux clients uniquement s’il y a toujours de la capacité après que vous avez ciblé Act maintenant et évalué les clients. | 
| Programme de licence | Identifie le type de programme de licence pour le renouvellement | 
| ID de l'accord | Identificateur de l’accord | 
| Date de fin de l’accord | Date de fin de l’accord | 
| Type d'expiration | Type d’expiration | 
| Chiffre d’affaires arrivant à expiration | Chiffre d’affaires associé aux abonnements arrivant à expiration | 
| A EA | Indique si un renouvellement est un abonnement EA ou EA | 
| A ouvert | Indique si un renouvellement est un accord Open ou Open Value | 
| Client Azure upsell | Indique si le client affiche la propension de vente incitative pour Azure | 
| Microsoft 365 client de vente incitative | Indique si le client affiche la propension de vente incitative pour Microsoft 365 | 
| RevSumDivisionName | Identifie le produit qui est en renouvellement | 

## <a name="next-steps"></a>Étapes suivantes

Pour plus d’informations, consultez [Télécharger des rapports](pci-download-reports.md).
