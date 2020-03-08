---
title: Découvrez les offres sur la place de marché commerciale | Espace partenaires
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment les partenaires CSP peuvent utiliser l’espace partenaires pour afficher ou rechercher les offres SaaS ou la tarification des éditeurs de logiciels indépendants dans la place de marché.
author: MicheleHope
ms.author: v-mihope
keywords: abonnements, Marketplace, Marketplace commerciale, tiers, ISV, offres SaaS, programme fournisseur de solutions Cloud, programme CSP, partenaires CSP
ms.localizationpriority: medium
ms.openlocfilehash: 23a31646165576842b625ec4f05a8da404fae01d
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340145"
---
# <a name="discover-offers-and-pricing-in-the-commercial-marketplace"></a>Découvrir les offres et la tarification dans la place de marché commerciale

**S’applique à**

- Centre pour partenaires
- Partenaires du programme Fournisseur de solutions Microsoft Cloud

**Rôles appropriés**

- Administrateur global
- Agent d’administration

Lorsque des éditeurs de logiciels indépendants choisissent de publier une offre dans la place de marché commercial, ils peuvent également décider s’ils souhaitent que l’offre soit disponible dans le programme CSP. S’ils choisissent de vendre l’offre par le biais du programme CSP, les partenaires CSP doivent voir l’offre dans la place de marché de l’espace partenaires. 

Si une offre ISV n’apparaît pas comme prévu dans l’espace partenaires, cela peut être dû à ce qui suit :

- L’ISV a décidé de ne pas vendre l’offre par le biais du programme CSP. Par exemple, certains produits ISV peuvent avoir été mis à disposition dans d’autres zones de la place de marché commerciale (par exemple, dans [Microsoft AppSource](https://appsource.microsoft.com/) et la place de [marché Azure](https://azuremarketplace.microsoft.com/)), mais ils peuvent ne pas apparaître pour les fournisseurs de services de domaine dans la place de marché de l’espace partenaires.

- L’ISV a décidé de rendre l’offre exclusive à un nombre sélectionné de partenaires CSP. Pour plus d’informations sur les offres exclusives, consultez plus loin dans cette rubrique d’aide.

- Le type d’offre peut ne pas être possible via l’espace partenaires ou Portail Azure (par exemple, des conteneurs ou des offres basées sur l’utilisation).

- Le pays de facturation de vos clients associés peut ne pas être pris en charge pour cette offre ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Afficher les offres de la place de marché dans l’espace partenaires

Pour afficher les offres de la place de marché commercial disponibles dans le programme CSP : 

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires, puis sélectionnez **CSP** dans le menu de navigation de gauche.

2. Sélectionnez **vendre**, puis **Marketplace**. Par défaut, vous verrez des produits de tous types et catégories.

3. Sélectionnez un filtre par type ou catégorie. Vous pouvez également utiliser la **recherche** pour rechercher des mots clés spécifiques, des noms d’offres ou des noms d’éditeurs ISV.

4. Sélectionnez une offre de produit spécifique dans la liste. Cela vous permet d’obtenir un onglet de vue d’ensemble du produit, dans lequel vous pouvez en savoir plus sur l’offre. Les informations de cet onglet peuvent inclure : 

    - Description du produit ou de l’offre

    - Plus d’informations sur l’éditeur ISV

    - Liens vers la documentation ou les documents marketing téléchargés par l’éditeur ISV

    - Autres contacts ISV possibles pour le support technique, l’ingénierie ou un contact pour le programme CSP

5. Pour obtenir plus d’informations sur les plans, les références SKU ou les tarifs disponibles pour une offre, sélectionnez l’onglet **plans + tarification** . Cet onglet vous indiquera les éléments suivants :

    - Les marchés où cette offre est disponible

    - Liste des références (SKU) ou plans disponibles pour l’offre

    - Tarification pour chaque référence ou plan disponible

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Afficher les offres de la place de marché via les API de l’espace partenaires

Les partenaires du programme CSP peuvent également utiliser des API pour retourner une liste d’offres éligibles. Les offres éligibles seront uniquement celles proposées par le partenaire pour vendre via la place de marché de l’espace partenaires. Pour les partenaires qui utilisent des API pour identifier les offres dans le catalogue, reportez-vous à l’aide pour [obtenir une liste des offres pour un marché](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Afficher les dernières offres de la place de marché dans l’espace partenaires

Suivez les étapes ci-dessous pour connaître les dernières informations sur la tarification associées à une offre :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires, puis sélectionnez **CSP** dans le menu de navigation de gauche.

2. Sélectionnez **vendre**, puis **Marketplace**. Une liste des offres de la place de marché s’affiche.

3. Faites défiler vers le bas jusqu’à la section **Marketplace** (en dessous de la **tarification du plan Azure**) et sélectionnez **Exporter la liste des prix** dans l’angle supérieur droit. Cela génère une feuille de calcul avec les données de tarification les plus récentes pour les offres SaaS basées sur une licence et disponibles auprès des éditeurs ISV. Certaines tarifs d’application Azure peuvent également apparaître ici. Ces informations sont mises à jour quotidiennement, ce qui vous permet de vérifier les prix actuels aussi souvent que vous le souhaitez.

4. Si un produit ISV comprend une période d’essai gratuite, la feuille de calcul affiche deux lignes pour ce produit :

    - Une ligne affiche le prix de l’essai gratuit de zéro. Cela signifie qu’une période d’essai gratuite est disponible.

    - L’autre ligne affiche le prix et les conditions qui s’appliquent après la fin de la période d’évaluation gratuite.

En tant que partenaire du programme CSP, vous pouvez être éligible à d’autres incentives associés à certaines offres de la place de marché commercial. Pour plus d’informations sur les autres incentives, consultez le [Guide d’incentives du fournisseur](https://aka.ms/partnerincentives) de solutions Cloud (nécessite une connexion CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>En savoir plus sur les offres exclusives Marketplace

Les éditeurs de logiciels indépendants ont la possibilité de rendre leurs offres disponibles uniquement pour des partenaires spécifiques dans le programme CSP. C’est ce qu’on appelle une offre exclusive. Tous les partenaires du programme CSP peuvent toujours afficher toutes les offres ISV dans la place de marché commerciale de l’espace partenaires, y compris celles marquées comme exclusives.

Si une offre n’est **pas** marquée comme exclusive, tous les partenaires peuvent acheter cette offre (en supposant que le pays de facturation du client sélectionné correspond à la disponibilité du pays de l’offre de l’ISV).

Toutefois, pour toute offre marquée comme exclusive, seuls les partenaires sélectionnés par l’ISV pourront acheter cette offre.

> [!NOTE]
> Si vous voyez une offre marquée comme exclusive que vous souhaitez vendre à vos clients, contactez directement l’ISV et demandez l’autorisation de vendre l’offre exclusive. Lorsque vous affichez les détails d’une offre exclusive, vous pouvez voir un lien **ISV de contact** que vous pouvez sélectionner.

Pour en savoir plus sur l’expérience ISV dans le Marketplace commercial, consultez [fournisseurs de solutions Cloud](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers).

Pour plus d’informations sur l’expérience du fournisseur de services Cloud sur la place de marché, consultez [Présentation du marché commercial](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Étapes suivantes :

- [Acheter des offres de la place de marché commercial](csp-commercial-marketplace-purchase.md)