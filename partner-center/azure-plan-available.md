---
title: Services Azure disponibles dans Azure CSP
description: Cette section indique les services Azure qui sont disponibles dans le programme Fournisseur de solutions Azure Cloud (CSP) et ceux qui ne le sont pas.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.date: 03/05/2020
ms.openlocfilehash: 29020fc4861bb11f15f7a892dda4d92f0c19fe07
ms.sourcegitcommit: af3ecd7f35e5bb3b87f5f683335c76e287f2a9b8
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83369276"
---
# <a name="available-azure-services-in-azure-csp"></a>Services Azure disponibles dans Azure CSP

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général
- Agent du support technique
- Agent commercial
- Administrateur de la gestion des utilisateurs

## <a name="available-azure-services-in-azure-csp"></a>Services Azure disponibles dans Azure CSP

Cet article liste les services Azure qui sont disponibles dans le programme Fournisseur de solutions Azure Cloud (CSP) et ceux qui ne le sont pas. Il traite également de la disponibilité du service pour les clouds nationaux [Microsoft Azure Allemagne](https://azure.microsoft.com/overview/clouds/germany/) et [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
>Le programme Azure CSP n’est pas disponible pour le cloud [Azure Chine]( https://www.azure.cn/).

## <a name="global-cloud"></a>Cloud global

Tous les services basés sur le modèle Azure Resource Manager sont disponibles dans le programme CSP.  Les services non basés sur Azure Resource Manager ne sont pas disponibles dans le programme CSP.  

## <a name="csp-specific-service-configurations"></a>Configuration des services dans le programme CSP

Les services suivants nécessitent une configuration spéciale dans le programme CSP :

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Seuls les utilisateurs du locataire client peuvent accéder aux données de leur environnement Time Series Insights. Par défaut, les partenaires peuvent gérer l’environnement Time Series Insights de leur client. Toutefois, s’ils ont besoin d’accéder aux données qu’il contient, ils doivent être ajoutés au locataire du client.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Vous pouvez désormais acheter les produits listés ci-dessous dans Visual Studio Marketplace, à l’exception des extensions tierces.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Abonnements Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Formation Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Pour vous aider à démarrer, nous avons créé des vidéos et une documentation expliquant [comment configurer, acheter et gérer Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) dans le programme CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Produits de la Place de marché Azure dans Azure CSP

Tous les produits de la Place de marché Azure ne sont pas encore disponibles dans les abonnements Azure CSP.

- Services Azure basés sur Microsoft : ces services sont disponibles. Consultez le tableau et les commentaires précédents.

- Produits BYOL (apportez votre propre licence) : ces produits sont disponibles. La liste complète des produits BYOL disponibles dans la Place de marché Azure se trouve dans la [page consacrée aux produits BYOL de la Place de marché Azure](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Produits tiers avec paiement à l’utilisation disponibles sur la Place de marché Azure : ces produits sont disponibles si le fournisseur a publié son annonce via le canal CSP. Pour plus d’informations, consultez [Vendre des abonnements à des produits de la Place de marché Azure](https://aka.ms/marketplaceincsp).

- Citrix XenApp Essentials : les partenaires peuvent acheter XenApp Essentials pour les clients du programme CSP. Pour plus d’informations, consultez le blog Citrix suivant : [Distribution of XenApp Essentials now available through Microsoft Cloud Solution Provider Channel](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Clouds nationaux

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

## <a name="next-steps"></a>Étapes suivantes

- [Découvrez](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) les fonctionnalités pour Azure qui sont disponibles dans l’Espace partenaires.

- [Créez](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) votre premier client dans Azure CSP et déployez des services Azure.
