---
title: Facturation du plan Azure – Fichiers de facturation et de rapprochement
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment accéder à la structure des fichiers de facturation et de rapprochement liée à la facturation pour le plan Azure et comment la comprendre.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658431"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nouvelle expérience de commerce pour les fournisseurs de solutions Cloud - Facturation Azure 

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général

Cet article explique comment accéder à la structure des fichiers de facturation et de rapprochement liée à la facturation pour le plan Azure et comment la comprendre. La facturation dans le plan Azure est une expérience simplifiée qui utilise une date de facturation unique et une période de facturation par mois civil.

## <a name="summary-of-billing-essentials"></a>Résumé des fondamentaux de la facturation

- **Date de la facture** : La facture et le fichier de rapprochement sont disponibles dans le tableau de bord/l’API de l’Espace partenaires au plus tard le 8 du mois (minuit UTC).

- **Période de facturation de la facture** : La période de facturation de la facture s’aligne sur le mois civil, par exemple, elle court du 1er au 31 octobre ou du 1er au 30 novembre.

- **Périodes de frais de service** : Les frais s’alignent sur le mois civil. Par exemple, si le partenaire facturé ajoute des services Azure par le biais d’un plan Azure le 15 octobre et que le client commence à consommer les services Azure le 15 octobre, alors le partenaire facturé reçoit la facture/le rapprochement le 8 novembre pour la consommation effectuée par le client pendant la période de service allant du 15 au 31 octobre. La facture du mois suivant qui va être générée le 08/12 contient tous les frais relatifs à la période de service 01/11 au 31/11.

- **Conditions de paiement de la facture**  : 60 jours nets.

- **Devise de la facture** : Les partenaires continuent à être facturés dans la devise officielle du pays du client. Par exemple, si le partenaire facturé est en Irlande avec des clients au Royaume-Uni, en Norvège et en Allemagne, alors le partenaire facturé reçoit une facture/un rapprochement en GBP, NOK et EUR.

- **Primes incitatives des partenaires** : Payées à 45 jours fin de mois.

## <a name="access-your-invoices-and-reconciliation-files"></a>Accéder à vos factures et à vos fichiers de rapprochement

L’administrateur général ou l’administrateur de facturation de votre entreprise reçoit un e-mail dès qu’une facture est consultable.

Pour accéder à la facture et au fichier de rapprochement :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/) de l’Espace partenaires.

2. Dans le menu de l’Espace partenaires, sélectionnez **Facturation**.

3. Sélectionnez l’onglet correspondant à **Recurring** (Périodique) et **One-time** (Ponctuelle) ainsi qu’à la devise qui vous intéresse.

   :::image type="content" source="images/azure/billing3.png" alt-text="facturation":::

4. Sélectionnez **Facture** ou **Fichier de rapprochement**.  

   Pour voir l’historique des factures et des fichiers de rapprochement, développez la ligne d’historique de facturation située en dessous.

## <a name="understanding-usage-data"></a>Fonctionnement des données d’utilisation 

1. Le plan Azure est le conteneur racine ou de niveau supérieur pour l’utilisation. Toute utilisation est liée à un seul plan Azure.

2. Dans un plan, il y aura un ou plusieurs abonnements Azure. Il s’agit de conteneurs utilisés pour la gestion et le déploiement des ressources. 

3. Dans un abonnement, les groupes de ressources s’ajoutent aux ressources de groupe. Chaque ressource est déployée sur un groupe de ressources. 

4. Les machines virtuelles et les comptes de stockage sont des exemples de ressources. 

5. Les ressources émettent des compteurs : Les compteurs sont des mesures de consommation d’une ressource et une ressource peut émettre l’utilisation de plusieurs compteurs. Les compteurs sont identifiés par un ProductId, un SKUId et un AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hiérarchie des groupes de ressources et du contrôle des abonnements

**Compte Azure (locataire)**

- Abonnement A
    - Groupe de ressources 1
        - Machine virtuelle (ressource)
            - Compteur de calcul
        - Réseau virtuel (ressource)
            - Aucun compteur de facturation

    - Groupe de ressources 2
        - Machine virtuelle (ressource)
            - Compteur de calcul
        - Disque managé SSD Premium (ressource)
            - Compteur de capacité de stockage
            - Compteur des opérations de stockage

- Abonnement B   -Groupe de ressources 1       - Azure SQL (ressource)           - Compteur DTU       - Passerelle VPN (ressource)           - Compteur de passerelle VPN

    - Groupe de ressources 2
        - Interface réseau virtuelle (ressource)
            - Aucun compteur de facturation

## <a name="read-the-invoice"></a>Lire la facture

1. La facture est disponible au plus tard le huit de chaque mois.

2. Les partenaires ont 60 jours pour effectuer le paiement.

3. La période de facturation couvre un mois civil donné, par exemple, du 1er au 31 octobre.

4. Les frais sont nets d’ajustements (le montant est net de « crédit Partenaires pour les services managés »).

5. Consultez le fichier de rapprochement et le fichier d’utilisation quotidienne estimée pour obtenir d’autres informations sur la facturation.

   :::image type="content" source="images/azure/invoice1.png" alt-text="facture":::

## <a name="read-the-invoice-reconciliation-file"></a>Lire le fichier de rapprochement des factures

1. Chaque combinaison de compteur et de plan Azure peut avoir jusqu’à deux lignes de facturation sur le fichier de rapprochement.

2. Si le compteur est éligible à un type de remise ou crédit (par exemple, des remises différenciées ou le crédit Partenaires pour les services managés) pendant tout le mois civil, le fichier de rapprochement ne contient qu’une seule ligne de facturation. La colonne **PriceAdjusmentDescription** référencera la remise ou le crédit Partenaires.

3. Si aucune ressource d’un compteur particulier n’est éligible à une remise ou au crédit Partenaires, le fichier de rapprochement ne contient qu’une seule ligne de facturation et le prix unitaire effectif correspond au prix de vente au détail (à savoir, le prix unitaire).

4. Si le compteur, ou n’importe quelle ressource émettant ce compteur, est éligible au **crédit Partenaires pour les services managés** pendant une partie du mois, le fichier de rapprochement contient deux lignes de facturation. Une ligne représente les jours pendant lesquels le compteur est éligible et la seconde ligne représente les jours où il n’est pas éligible.

## <a name="read-the-daily-usage-file"></a>Lire le fichier d’utilisation quotidienne

- Les compteurs d’abonnement dans le cadre d’un plan Azure sont évalués et cumulés quotidiennement.

- Le **crédit Partenaires pour les services managés** est déterminé et appliqué quotidiennement.

- Chaque compteur d’abonnement a une ligne pour chaque jour du mois où une consommation a eu lieu.

- Dans l’exemple ci-dessous :

  - Le compteur est éligible au **crédit Partenaires pour les services managés** du 01/07 au 03/07. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.

  - Le compteur n’est pas éligible au **crédit Partenaires pour les services managés** du 04/07 au 07/07. Notez que le prix unitaire effectif est le prix de vente au détail.

  - Le compteur est éligible au **crédit Partenaires pour les services managés** du 08/07 au 31/07. Notez que le prix unitaire effectif correspond au prix de vente au détail moins le crédit Partenaires.

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Facture dans la devise du client

Les services Azure fournis par l’intermédiaire d’un plan Azure sont facturés en USD et facturés dans la devise officielle du pays du client. Si la devise de facturation n’est pas USD, le taux de change utilisé est indiqué à la dernière page de la facture. Les taux de change sont déterminés tous les mois et appliqués à la facture suivante. Pour obtenir la liste complète des devises des pays, consultez la [grille des devises client et la disponibilité des offres de nouveau commerce par pays](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft suit les cours de la Bourse de Londres pour la conversion. Nous utilisons le taux de change, qui est le taux de change capturé à la dernière seconde du dernier jour ouvrable du mois à la Bourse de Londres. Les taux de change sont actualisés et disponibles le jour précédant le premier jour du mois auquel ils s’appliquent.

## <a name="azure-reservations"></a>Réservations Azure


Si vous achetez des [réservations Azure](azure-reservations.md) par le biais d’un plan Azure, vous pouvez choisir une facturation mensuelle ou ponctuelle.


## <a name="azure-spending"></a>Dépenses Azure

L’expérience des dépenses Azure existante est mise à jour pour prendre en charge la facturation du nouveau plan Azure dans l’Espace partenaires. Cela permet aux partenaires d’effectuer les opérations suivantes :

- Voir, gérer et recevoir des alertes pour le budget défini au niveau d’un client 

- Voir les dépenses totales estimées sur un plan Azure (ventilées par niveau de ressource et de compteur)

Étant donné que le modèle de facturation des services Azure par le biais d’un plan Azure correspond à une consommation après paiement, pour éviter une facture plus importante que prévu, les partenaires peuvent appliquer un budget mensuel et suivre le pourcentage d’utilisation. Un budget peut être appliqué à un seul client ou à plusieurs clients à la fois. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Dépenses Azure":::

## <a name="next-steps"></a>Étapes suivantes

- Découvrez le calcul du crédit Partenaires (PEC). Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/) de l’Espace partenaires et recherchez la liste de prix disponible.

- Découvrez l’[achat du plan Azure](purchase-azure-plan.md).

- Consultez les [tarifs de la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud](azure-plan-price-list.md).
