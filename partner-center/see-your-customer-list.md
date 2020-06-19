---
title: Gérer la liste de vos clients
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Les enregistrements de clients font partie des ressources d’informations les plus importantes. Découvrez comment afficher, Rechercher, mettre à jour & exporter des informations dans votre liste de clients de l’espace partenaires.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b248a5614bc071068ee2e7a70906795c12f24a14
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992160"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gérer votre liste de clients-Rechercher, mettre à jour ou exporter des clients dans l’espace partenaires

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Les enregistrements de client comptent parmi vos ressources information les plus importantes dans l’Espace partenaires. Vous pouvez rechercher des comptes client dans votre base de données et exporter la base de données des clients totalement ou en partie dans un fichier&nbsp;CSV compatible avec Excel. Vous pouvez également exporter les informations sur les abonnements d’un client dans un fichier&nbsp;CSV.

Les journaux d’activité fournissent des données exportables sur les transactions et les actions de gestion des clients. Pour plus d’informations, consultez [Afficher les journaux d’activité des clients](activity-logs.md).

## <a name="search-for-a-customer"></a>Rechercher un client

1.  Dans le menu **espace partenaires** , sélectionnez **clients**.
2.  Pour rechercher un client, entrez le nom du client ou le nom de domaine dans la zone de recherche.
3.  Sélectionnez la **flèche vers le bas** à la fin de la ligne d’un client pour voir son ID&nbsp;Microsoft, ainsi que les liens rapides vers ses services et ses abonnements.

## <a name="update-a-customers-company-name"></a>Mettre à jour le nom de la société du client

Dans le menu **espace partenaires** , sélectionnez **clients**.
2.  Pour rechercher un client, entrez le nom du client ou le nom de domaine dans la zone de recherche.
3.  Sélectionnez la **flèche vers le bas** à la fin de la ligne d’un client pour voir son ID&nbsp;Microsoft, ainsi que les liens rapides vers ses services et ses abonnements.
4.  Sous les informations de **facturation** du client, mettez à jour le nom de la société. Lorsque vous enregistrez la nouvelle valeur, elle apparaîtra dans la liste des clients. Cela modifiera uniquement le nom de la société à facturer et la valeur de liste de clients. Cette opération ne modifiera aucune autre entrée.
<sup>1</sup>
## <a name="export-your-customer-list"></a>Exporter votre liste de clients

1. Dans le menu **espace partenaires** , sélectionnez **clients**.
2. Sélectionnez **Exporter clients**.

   L’Espace partenaires convertit votre liste de clients en un fichier&nbsp;CSV et le télécharge dans le dossier de téléchargement par défaut de votre ordinateur. Vous pouvez également exporter des sous-ensembles de données client. Les colonnes contiennent les données suivantes&nbsp;:

   - **ID Microsoft**;
   - **Nom**de la société ;
   - **Nom de domaine principal**;
   - **Relation**&nbsp;: relation commerciale du partenaire avec chaque client répertorié.

    Par défaut, l’Espace partenaires exporte la liste des clients, quelle que soit sa longueur. Vous pouvez également effectuer des recherches par nom de société ou de domaine dans la liste des clients et exporter ce sous-ensemble de données.

3. Si vous êtes un fournisseur indirect, vous pouvez filtrer votre liste de clients par revendeur indirect. Sélectionnez **Filtrer par revendeur indirect** dans la liste, puis choisissez un revendeur.
<sup>1</sup>

## <a name="export-customer-subscription-information"></a>Exporter les informations d’abonnement client

1. Dans le menu **espace partenaires** , sélectionnez **clients**.

2. Sélectionnez le **nom de société** d’un client. La page **Abonnements** d’un client affiche la liste complète de ses abonnements à des produits.

3. Sélectionnez **Exporter des abonnements**. L’Espace partenaires convertit les données de l’abonnement du client en un fichier&nbsp;CSV et le télécharge dans le dossier de téléchargement par défaut de votre ordinateur. Les colonnes contiennent les données suivantes&nbsp;:
   - **ID d’abonnement**;
   - **Abonnement**&nbsp;: nom du produit correspondant à l’abonnement
   - **Quantité**&nbsp;: nombre de licences achetées
   - **État**;
   - **Revendeur**&nbsp;: ID du revendeur qui possède et gère l’abonnement.

> [!NOTE]  
> Pour plus d’informations sur la gestion des abonnements, consultez [abonnements client](customer-subscriptions.md).
