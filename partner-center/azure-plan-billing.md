---
title: Plan Azure - Facturation | Espace partenaires
ms.topic: article
ms.date: 10/04/2019
description: Décrit la structure des factures et fichiers de rapprochement
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171301"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nouvelle expérience de commerce pour les fournisseurs de solutions Cloud - Facturation Azure 

La facturation dans le cadre du plan Azure est une expérience simplifiée grâce à une date de facturation unique et une période de facturation par mois civil. Pour plus d’informations sur la plateforme de facturation, consultez le [Guide des opérations de commerce moderne de l’Espace partenaires](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).

## <a name="summary-of-billing-essentials"></a>Résumé des fondamentaux de la facturation

- **Date de la facture** : La facture et le fichier de rapprochement sont disponibles dans le tableau de bord/l’API de l’Espace partenaires au plus tard le 8 du mois (minuit UTC).

- **Période de facturation de la facture** : La période de facturation de la facture s’aligne sur le mois civil, par exemple, elle court du 1er au 31 octobre ou du 1er au 30 novembre.

- **Périodes de frais de service** : Les frais s’alignent sur le mois civil. Par exemple, si le partenaire facturé ajoute des services Azure par le biais d’un plan Azure le 15 octobre et que le client commence à consommer les services Azure le 15 octobre, alors le partenaire facturé reçoit la facture/le rapprochement le 8 novembre pour la consommation effectuée par le client pendant la période de service allant du 15 au 31 octobre. La facture du mois suivant qui va être générée le 8 décembre contient tous les frais relatifs à la période de service allant du 1er au 31 novembre.

- **Conditions de paiement de la facture**  : 60 jours nets.

- **Devise de la facture** : Les partenaires continuent à être facturés dans la devise officielle du pays du client. Par exemple, si le partenaire facturé est en Irlande avec des clients au Royaume-Uni, en Norvège et en Allemagne, alors le partenaire facturé reçoit une facture/un rapprochement en GBP, NOK et EUR.

- **Primes incitatives des partenaires** : Payées à 45 jours fin de mois.

##  <a name="access-your-invoices-and-recon-files"></a>Accéder à vos factures et à vos fichiers de rapprochement

L’administrateur général ou l’administrateur de facturation de votre entreprise reçoit un e-mail dès qu’une facture est consultable. 

**Pour accéder à la facture et au fichier de rapprochement**

1. Connectez-vous à l’Espace partenaires.

2. Dans le menu de l’Espace partenaires, sélectionnez **Facturation**.

3. Sélectionnez l’onglet correspondant au **mois civil** et à la devise qui vous intéressent.

![facturation](images/azure/billing1.png)

4. Sélectionnez la **facture et le fichier de rapprochement**.  

Pour voir l’historique des factures et des fichiers de rapprochement, développez la ligne d’historique de facturation située en dessous.

## <a name="read-the-invoice"></a>Lire la facture

1. La facture est disponible au plus tard le 8 de chaque mois.

2. Les partenaires ont 60 jours pour effectuer le paiement.

3. La période de facturation couvre un mois civil donné, par exemple, du 1er au 31 octobre.

4. Les frais sont nets d’ajustements (le montant est net de « crédit Partenaires pour les services managés »).

5. Consultez le fichier de rapprochement et le fichier d’utilisation quotidienne estimée pour obtenir d’autres informations sur la facturation.

![facture](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>Lire le fichier de rapprochement

1. Chaque compteur d’abonnement Azure peut avoir jusqu’à deux lignes de facturation sur le fichier de rapprochement.

2. Si le compteur est éligible à un type de remise ou crédit (par exemple, des remises de niveau 1 ou le crédit Partenaires pour les services managés) pendant tout le mois civil, alors le fichier de rapprochement ne contient qu’une seule ligne de facturation. La colonne **PriceAdjusmentDescription** fait référence à la remise ou au crédit gagné. Le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires ou toute autre remise.

3. Si le compteur n’est pas éligible au crédit Partenaires pour les services managés pendant tout le mois civil, alors le fichier de rapprochement ne contient qu’une seule ligne de facturation et le prix unitaire effectif correspond au prix de vente au détail (à savoir, le prix unitaire).

4. Si le compteur est éligible au **crédit Partenaires pour les services managés** pendant une partie du mois, le fichier de rapprochement contient deux lignes de facturation. Une ligne représente les jours pendant lesquels le compteur est éligible et la seconde ligne représente les jours où il n’est pas éligible. 

## <a name="read-the-daily-usage-file"></a>Lire le fichier d’utilisation quotidienne

- Les compteurs d’abonnement dans le cadre d’un plan Azure sont évalués et cumulés quotidiennement. 

- Le **crédit Partenaires pour les services managés** est déterminé et appliqué quotidiennement.

- Chaque compteur d’abonnement a une ligne pour chaque jour du mois où une consommation a eu lieu.

- Dans l’exemple ci-dessous :

  - Le compteur est éligible au **crédit Partenaires pour les services managés** du 1er au 3 juillet. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.

   - Le compteur n’est pas éligible au **crédit Partenaires pour les services managés** du 4 au 7 juillet. Notez que le prix unitaire effectif est le prix de vente au détail.

    - Le compteur est éligible au **crédit Partenaires pour les services managés** du 8 au 31 juillet. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>Facture dans la devise du client 

Les services Azure fournis par l’intermédiaire d’un plan Azure sont facturés en USD et facturés dans la devise officielle du pays du client. Si la devise de facturation n’est pas USD, alors le taux de change utilisé est indiqué à la dernière page de la facture. Les taux de change sont déterminés tous les mois et appliqués à la facture suivante. Pour obtenir la liste complète des devises des pays, consultez la [grille des devises client et la disponibilité des offres de nouveau commerce par pays](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V). 

Microsoft utilise [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) pour déterminer le taux de change utilisé pour effectuer la conversion des devises. Le taux de change est actualisé et disponible le jour précédant le premier jour du mois auquel il s’applique.

**Exemple**:  Les frais d’utilisation pour la période de service qui va du 1er au 31 août sont facturés à l’aide du taux de change publié le 1er août. Ces frais apparaissent dans la facture de septembre et le taux de change est indiqué à la dernière page de la facture. 

Les utilisateurs locataires des partenaires continuent de voir des informations connexes propres à leurs rôles concernant tous les clients et toutes les commandes, quelle que soit la devise de facturation. De plus, l’utilisateur peut voir toutes les factures dans toutes les devises.  
 
## <a name="azure-reservations"></a>Réservations Azure 

Si vous achetez des [réservations Azure](https://docs.microsoft.com/partner-center/azure-reservations) par le biais d’un plan Azure, il est uniquement possible de choisir la facturation ponctuelle dans l’Espace partenaires. La facturation mensuelle est disponible sur le portail Azure. La facturation mensuelle sera disponible dans l’Espace partenaires à une date ultérieure. 

## <a name="azure-cost-management"></a>Azure Cost Management 

Les outils Azure Cost Management permettent aux organisations de visualiser, gérer et optimiser les coûts sur Microsoft Azure. Cette fonctionnalité sera disponible sur la portail Azure. Les partenaires disposeront d’une solution toujours active à faible latence avec les fonctionnalités suivantes disponibles : 

- Analyses plus précises et alertes budgétaires 
- API et connecteurs Power BI 
- Vue multiclient 
- Gratuité de la gestion des coûts Azure 
- Élargissement des rôles/utilisateurs 

Pour plus d’informations sur cette fonctionnalité disponible pour les contrats Entreprise depuis février 2019, consultez [Azure Cost Management](https://azure.microsoft.com/services/cost-management). Cette fonctionnalité est disponible uniquement avec les services Azure achetés dans le cadre de cette nouvelle expérience de commerce Azure pour les fournisseurs de solutions Cloud. 
 
## <a name="azure-spending"></a>Dépenses Azure 

Un outil relatif aux dépenses Azure sera disponible dans l’Espace partenaires pour la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud. Quand cette expérience sera appliquée, cet outil permettra aux partenaires de voir :  

- Le budget total d’un client 
- Les dépenses totales estimées sur un plan Azure existant 
- Le pourcentage d’utilisation des clients à chaque période de facturation 

Étant donné que le modèle de facturation des services Azure par le biais d’un plan Azure correspond à une consommation après paiement, pour éviter une facture plus importante que prévu, les partenaires peuvent appliquer un budget mensuel et suivre le pourcentage d’utilisation. Un budget peut être appliqué à un seul client ou à plusieurs clients à la fois. 

![Dépenses Azure](images/azure/azurespend.png)

**Pour plus d’informations**

-  Le mode de calcul du crédit Partenaires se trouve dans la liste de tarifs disponible dans le tableau de bord de votre Espace partenaires. 
   
-  [Acheter le plan Azure](purchase-azure-plan.md)

-  [Tarifs de la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud](azure-plan-price-list.md)
