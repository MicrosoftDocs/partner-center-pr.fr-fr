---
title: Utiliser l’analytique de l’espace partenaires pour Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment afficher vos données d’entreprise à l’aide de l’application Partner Center Analytics pour Power BI (pour les partenaires directs dans CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855027"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Afficher vos données d’entreprise avec l’application Partner Center Analytics pour Microsoft Power BI



**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent commercial | Agent d’administration

## <a name="view-your-business-data"></a>Afficher vos données d’entreprise

Obtenir une représentation visuelle de vos données d’entreprise avec l’application Partner Center Analytics pour Power BI, notamment :

- Croissance de votre base de clients, abonnements et licences

- Utilisation de produits Office 365, Microsoft Dynamics et Microsoft Azure

- Unités de consommation quotidienne par ressource contrôlée de chaque abonnement Azure au cours des 60 derniers jours

- Coût estimé (basé sur la carte de taux la plus récente)

- Possibilité d’exporter des jeux de données et de créer des rapports personnalisés, notamment par client.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>À propos de la version préliminaire de l’application Partner Center Analytics

- Cette application est destinée aux partenaires directs dans le programme du fournisseur de solutions Cloud uniquement. Les autres partenaires du fournisseur CSP (revendeurs indirects, par exemple) ne pourront pas se connecter.

- Les coûts estimés sont des données de facturation/facture antérieures, et ne sont pas légalement contraignantes. Les coûts estimés sont destinés à être utilisés uniquement pour les analyses de données.

- Les informations sur les clients sont basées sur des abonnements. Les clients pour lesquels vous avez récemment créé des comptes, mais qui n’ont pas encore d’abonnement, ne sont pas inclus dans le nombre.

- Le coût estimé est basé sur la carte à tarif le plus récent, qui est basé sur la tarification du fournisseur CSP.

- Les jours sont les jours civils.

### <a name="business-insights-report"></a>Rapport Business Insights

- **Locataires client**: nombre de locataires de Azure ad distincts des clients qui ont acheté des abonnements

- **Nouveau (30 derniers jours)**: nouveaux clients achetant au moins un abonnement au cours des 30 derniers jours

- **Évolution (30 derniers jours)**: clients sans abonnement « actif », « en grâce » ou « désactivé »

- **Nouveau (dernières 24 heures)**: nouveaux clients achetant au moins un abonnement au cours des dernières 24 heures

- **Estimation du coût mensuel au cours des 12 derniers mois**: tendance du mois sur le mois du montant estimé des factures en dollars cumulés sur la période des 12 derniers mois

- **Estimation du coût par produit au cours des 12 derniers mois**: produits vendus triés par montant de facture estimée en dollars cumulé sur la période des 12 derniers mois. Cet état indique les meilleurs produits qui apportent la plupart des revenus.

- **Clients au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients et évolution des clients par mois sur la période des 12 derniers mois

- **Estimation du coût par client au cours des 12 derniers mois**: clients triés par estimation de la quantité en dollars de la facture avant impôts cumulés sur la période des 12 derniers mois. Cet état indique que les meilleurs clients apportent la plupart des revenus.

- **Nombre de clients par produit**: produits vendus triés par clients associés. Cet état indique les meilleurs produits vendus à la plupart des clients.

### <a name="subscription-insights-report"></a>Rapport sur les informations d’abonnement

- **État** de l’abonnement :

- Actif : abonnements appartenant à l’état « actif » ou « en grâce »

  - Suspendu : abonnements appartenant à l’état « désactivé »

  - Désapprovisionnés : abonnements appartenant à l’état « annulé » ou « expiré »

- **État** de l’expiration :

  - Expiré : abonnements qui ont déjà expiré (où la date de fin de l’abonnement est passée)

  - Expiration après 30 jours : abonnements qui expirent au bout de 30 jours (où la date de fin de l’abonnement est ultérieure à 30 jours)

  - Expiration dans 30 jours : abonnements arrivant à expiration dans les 30 prochains jours (où la date de fin de l’abonnement est comprise entre aujourd’hui et les 30 prochains jours)

- **Nombre total d’abonnements**: abonnements dans l’état « actif », « en délai » ou « désactivé »

- **Nouveau (30 derniers jours)**: nouveaux abonnements achetés par les clients au cours des 30 derniers jours

- **Nouveau (dernières 24 heures)**: nouveaux abonnements achetés par les clients au cours des dernières 24 heures

- **Expiration dans 30 jours**: abonnements arrivant à expiration dans les 30 prochains jours

- **Évolution (30 derniers jours)**: abonnements désapprovisionnés ou suspendus (désactivés) au cours des 30 derniers jours

- **Distribution par types d’abonnements**:% distribution du total des abonnements par licence et type d’abonnement basé sur l’utilisation

- **Nombre d’abonnements actifs par produit**: produits vendus triés par nombre d’abonnements actifs

- **Abonnements au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements et des abonnements en cours d’actualisation mensuels sur la période des 12 derniers mois

- **Détails de l’abonnement client**: vue détaillée des clients, des abonnements et des offres

### <a name="license-insights-report"></a>Rapport sur les informations de licence :

- **Licences totales**: nombre total de licences agrégées sur tous les abonnements basés sur des licences

- **Nouveau (30 derniers jours)**: ajout de licences au cours des 30 derniers jours

- **Évolution (30 derniers jours)**: réduction de la licence au cours des 30 derniers jours

- **Nouveau (dernières 24 heures)**: ajout de licences au cours des dernières 24 heures

- **Licences au** cours des 90 derniers jours : tendance du mois sur le mois des ajouts et réductions de licences agrégés tous les mois sur la période des 90 derniers jours

- **Nombre de licences actives par produit**: produits vendus triés par nombre de licences actives

- **Nombre de licences actives par client**: clients triés par nombre de licences actives

- **Détails de l’événement de licence client au** cours des 90 derniers jours : vue détaillée des clients, abonnements et événements d’abonnement, y compris la date de l’événement, le nom de l’événement, la quantité et le changement de quantité.

### <a name="licenses-usage-report"></a>Rapport d’utilisation des licences :

- **Licences attribuées par produit**: produits vendus triés par nombre d’affectations de licences

- **Licences utilisées par produit**: produits vendus triés par nombre d’utilisations de licences

- **Distribution client des licences attribuées**:% de la répartition du total des clients dans les compartiments de 20% de la plage par% d’attribution de licence

- **Distribution client des licences en cours d’utilisation**:% de la répartition du total des clients dans les compartiments de 20% de la plage par rapport à l’utilisation de la licence%

- **Licences attribuées par le client**: vue détaillée des licences vendues et des licences affectées par les clients et les produits

- **Licences utilisées par le client**: vue détaillée des licences vendues et des licences utilisées par les clients et les produits

### <a name="azure-insights-report"></a>Rapport Azure Insights :

- **Clients basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux clients basés sur l’utilisation et clients basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois

- **Abonnements basés sur l’utilisation au cours des 12 derniers mois**: tendance du mois sur le mois des nouveaux abonnements basés sur l’utilisation et abonnements basés sur l’utilisation agrégés tous les mois sur la période des 12 derniers mois

- **Estimation du coût d’utilisation par le client au** cours des 60 derniers jours : les clients basés sur l’utilisation sont triés par montant de facture estimée en euros sur la période de 60 derniers jours. Cet état indique que les meilleurs clients basés sur l’utilisation apportent la plupart des revenus

- **Estimation du coût d’utilisation par catégorie au** cours des 60 derniers jours : les catégories de compteurs d’abonnements basés sur l’utilisation sont triées en fonction du montant de la facture estimée en euros sur la période de 60 derniers jours.

- **Estimation du coût d’utilisation par abonnement au** cours des 60 derniers jours : abonnements basés sur l’utilisation par estimation de l’estimation de la quantité en dollars des factures sur la période des 60 derniers jours.

- **Coût d’utilisation estimé par le client par dépense budgétaire**: clients triés par pourcentage de leur budget de dépenses d’utilisation actuel dépassant le seuil (100%).

### <a name="azure-resource-usage-report"></a>Rapport d’utilisation des ressources Azure :

- **Utilisation des ressources Azure par jour pour la période sélectionnée**: unités de consommation quotidienne pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours.

- **Estimation du coût d’utilisation des ressources Azure pour la période sélectionnée**: coût estimé basé sur la carte de taux la plus récente pour chaque ressource limitée dans chaque abonnement basé sur l’utilisation pour la période sélectionnée au cours des 60 derniers jours. 

## <a name="next-steps"></a>Étapes suivantes

- [Présentation de l’analyse de l’espace partenaires pour Power BI application](power-bi-app-for-direct-partners.md)

- [Installer et prévisualiser l’application Analyse de l’Espace partenaires pour Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
