---
title: Transition des clients vers le plan Azure | Espace partenaires
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment faire passer facilement vos clients au plan Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567235"
---
# <a name="transition-your-customers-to-azure-plan"></a>Faire passer vos clients au plan Azure

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général
- Agent du support technique
- Agent commercial
- Administrateur de la gestion des utilisateurs

Les fournisseurs indirects et les partenaires de facturation directe peuvent passer à la nouvelle expérience de commerce disponible dans le programme CSP pour Azure. (Les revendeurs indirects devront utiliser leurs fournisseurs indirects.) Les clients pourront acheter des services cloud de façon simplifiée, que ce soit auprès de partenaires, de vendeurs Microsoft ou directement sur le Web.

La possibilité de transition s’adresse uniquement aux clients qui passent à la nouvelle expérience de commerce pour Azure et qui ont signé le Contrat client Microsoft, et non à d’autres offres du programme CSP, comme Office 365 ou Dynamics 365.

## <a name="available-azure-services-in-azure-csp"></a>Services Azure disponibles dans Azure CSP

Cette section indique les services Azure qui sont disponibles dans le programme Fournisseur de solutions Azure Cloud (CSP) et ceux qui ne le sont pas. Il traite également de la disponibilité du service pour les clouds nationaux [Microsoft Azure Allemagne](https://azure.microsoft.com/overview/clouds/germany/) et [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
>Le programme Azure CSP n’est pas disponible pour le cloud [Azure Chine]( https://www.azure.cn/).

### <a name="global-cloud"></a>Cloud global 

Tous les services basés sur le modèle Azure Resource Manager sont disponibles dans le programme CSP.  Les services non basés sur Azure Resource Manager ne sont pas disponibles dans le programme CSP.  

### <a name="csp-specific-service-configurations"></a>Configuration des services dans le programme CSP

Les services suivants nécessitent une configuration spéciale dans le programme CSP :

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Seuls les utilisateurs du locataire client peuvent accéder aux données de leur environnement Time Series Insights. Par défaut, les partenaires peuvent gérer l’environnement Time Series Insights de leur client. Toutefois, s’ils ont besoin d’accéder aux données qu’il contient, ils doivent être ajoutés au locataire client. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Vous pouvez désormais acheter les produits listés ci-dessous dans Visual Studio Marketplace, à l’exception des extensions tierces.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Abonnements Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Formation Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Pour vous aider à démarrer, nous avons créé des vidéos et une documentation expliquant [comment configurer, acheter et gérer Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) dans le programme CSP.

### <a name="azure-marketplace-items-in-azure-csp"></a>Produits de la Place de marché Azure dans Azure CSP

Tous les produits de la Place de marché Azure ne sont pas encore disponibles dans les abonnements Azure CSP.

- Services Azure basés sur Microsoft : ces services sont disponibles. Consultez le tableau et les commentaires précédents.

- Produits BYOL (apportez votre propre licence) : ces produits sont disponibles. La liste complète des produits BYOL disponibles dans la Place de marché Azure se trouve dans la [page consacrée aux produits BYOL de la Place de marché Azure](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Produits tiers avec paiement à l’utilisation disponibles sur la Place de marché Azure : ces produits sont disponibles si le fournisseur a publié son annonce via le canal CSP. Pour plus d’informations, consultez [Vendre des abonnements à des produits de la Place de marché Azure](https://aka.ms/marketplaceincsp).   

- Citrix XenApp Essentials : les partenaires peuvent acheter XenApp Essentials pour les clients du programme CSP. Pour plus d’informations, consultez le blog Citrix suivant : [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

### <a name="national-clouds"></a>Clouds nationaux 
Le tableau suivant présente une liste régulièrement mise à jour comprenant les produits, services et fonctionnalités Azure qui sont disponibles dans le cadre du programme CSP pour les clouds nationaux. 

| Produit, service ou fonctionnalité Azure | US Government | Allemagne |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Ordinateurs virtuels  |  X  |  X  |
|  Services cloud  |    |    |
|  Groupes de machines virtuelles identiques  |  X  |  X  |
|  Fonctions  |    |    |
|  Azure Container Service  |    |    |
|  **Mise en réseau**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Équilibreur de charge  |  X  |  X  |
|  Passerelle VPN  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Stockage**  |    |    |
|  Stockage  |  X  |  X  |
|  Secours  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web + Mobile**  |    |    |
|  App Service  |  X  |  X  |
|  Azure App Service sur Linux  |    |  X  |
|  Gestion des API  |  X  |    |
|  Content Delivery Network  |    |    |
|  Services Multimédia  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Recherche Azure  |    |    |
|  Fonctionnalité Logic Apps d’Azure App Service  |    |    |
|  **Conteneurs**  |    |    |
|  App Service  |  X  |  X  |
|  Azure App Service sur Linux  |    |  X  |
|  Batch (Fichier de commandes)  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Bases de données**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Cache Redis  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database pour MySQL  |    |    |
|  Azure Database pour PostgreSQL  |    |    |
|  **Données + Analytique**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **IA + Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **IoT (Internet des objets)**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Services basés sur l’emplacement  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Integration**  |    |    |
|  StorSimple  |  X  |    |
|  Gestion des API  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Fonctionnalité Logic Apps d’Azure App Service  |    |    |
|  **Sécurité + Identité**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Security Center  |  X  |  X  |
|  **Outils de développement**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Supervision + gestion**  |    |    |
|  Advisor  |    |    |
|  Secours  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Planificateur  |  X  |  X  |
|  Automatisation  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Applications managées Azure  |    |    |
|  Azure Migrate  |    |    |
|  Groupes d'administration  |    |  

### <a name="next-steps"></a>Étapes suivantes

- [Découvrez](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) les fonctionnalités pour Azure qui sont disponibles dans l’Espace partenaires.

- [Créez](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) votre premier client dans Azure CSP et déployez des services Azure.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Passer d’offres CSP existantes à un plan Azure

Vous pouvez faire basculer les offres CSP Azure existantes d’un client vers les services Azure relevant du plan Azure de la nouvelle expérience de commerce du programme CSP, et ce à partir de l’Espace partenaires. Pour cela, le partenaire et le client doivent avoir établi une relation de revendeur via l’Espace partenaires, et le client doit avoir signé le Contrat client Microsoft.

### <a name="select-transition-to-azure-plan"></a>Sélectionner la transition vers le plan Azure

1. Sélectionnez le plan Azure pour votre client.

2. Sélectionnez **Transition de la facturation vers un plan Azure**.

![transition](images/azure/transition1.png)

3. Sélectionnez **Continuer**.

![transition](images/azure/transition2.png)

Votre client sera transféré vers le plan Azure.

**Le workflow de transition automatise les étapes prérequises** :

- Achat d’un ou plusieurs plans Azure
- Un plan par client dans les scénarios CSP Direct  
- Un plan par revendeur  

Par exemple, un partenaire a acheté deux offres Microsoft Azure et a inclus deux partenaires de référence distincts dans l’achat. Dans ce cas, le workflow de transition achète deux plans Azure (un par revendeur) et mappe automatiquement les abonnements Azure respectifs dans le cadre des plans Azure.  

**Mappage d’un abonnement Azure à un plan Azure**

Après l’achat d’un ou plusieurs plans Azure, notre système mappe les abonnements Azure existants aux plans Azure. La progression peut être examinée sur le portail Azure et dans l’Espace partenaires. 

4. Revenez à la page de **Abonnements** de l’Espace partenaires de votre client pour mettre à jour sa limite budgétaire dans sa devise locale. 

![Transition](images/azure/transition3.png)

>[!NOTE]
>Le budget que vous définissez dans l’Espace partenaires n’est pas reporté sur le portail Azure. Vous devez aussi définir le budget et l’alerte sur le portail Azure.

Quand vous passez au plan Azure, vous ne pouvez plus acheter d’abonnements Azure pour ce client. Vous devez créer les abonnements relevant du plan Azure sur le portail Azure.

>[!NOTE]
> Tous les abonnements Azure achetés via RBAC dans le plan Azure sont tarifés et facturés en monnaie locale. Les taux de change ne seront pas utilisés.

### <a name="track-your-transition-details"></a>Suivre les détails de votre transition

Vous pouvez suivre la progression de la transition sur le portail Azure et dans l’Espace partenaires.

![Afficher les détails](images/azure/details1.png)

**Impact sur la facturation des partenaires**

Si vous opérez la transition d’un client à partir d’une offre Azure CSP existante, les impacts sur la facturation seront les suivants :

- Votre facture CSP existante portera sur l’ensemble de votre consommation jusqu’à la date de fin de l’abonnement Azure CSP d’origine.

- Si vous disposiez de droits d’accès d’administrateur à l’abonnement CSP existant, vous continuerez d’y avoir accès une fois la migration de l’abonnement effectuée.

Pour opérer la transition de contrats Entreprise directs vers des inscriptions CSP et Serveur et des inscriptions Cloud vers des services Azure, consultez [Obtenir la propriété de facturation d’abonnements Azure pour un Contrat Partenaire Microsoft](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

**Journal d’audit** :

Pour rapprocher la facturation, affichez l’historique de vos abonnements « Microsoft Azure » (0145P) dans la page **Abonnements**. 

L’abonnement « Microsoft Azure » (0145P) comporte deux parties :
1. Abonnement Commerce 
2. Abonnement Azure (droit d’utilisation)

Une fois la transition terminée, l’abonnement Azure est rattaché à un nouveau plan Azure et l’abonnement Commerce est suspendu de façon à éviter toute communication de consommation supplémentaire.  

>[Remarque] : Quand l’abonnement Microsoft Azure (0145P) est acheté dans le cadre du programme CSP, l’abonnement Commerce et l’abonnement Azure (droit d’utilisation) ont la même valeur. Ce n’est qu’en cas de changements ou de transferts de propriété de facturation que les valeurs diffèrent. 

**Problèmes de transition**

Pendant les transitions, aucun problème n’est censé se produire selon nous. Si cela devait se produire, nous vous en informerons dans le workflow de transition proprement dit. Il n’y aura aucune perturbation dans l’utilisation d’Azure.  

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)



