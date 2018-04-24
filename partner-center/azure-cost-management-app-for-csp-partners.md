---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espacepartenaires
description: Azure Cost Management par Cloudyn requiert un accès fourni à l'API de l'Espace partenaires.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.openlocfilehash: 01553b850d5839d721de5406c3f1c63094f76bd6
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/08/2018
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud  

**S'applique à**

-  Espace partenaires

[Obtenez davantage d'informations sur Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Avant de commencer
Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies:
- Vous êtes un partenaire du programme Fournisseur de solutions Cloud.
- Vous avez la possibilité de créer une application Web de l'API du Tableau de bord du partenaire.

## <a name="overview"></a>Vue d'ensemble

Azure Cost Management by Cloudyn est une application Web qui vous permet de suivre et de gérer le degré d'utilisation d'Azure par vos clients et les coûts de cette utilisation. Vous l'utilisez via l'API du Tableau de bord du partenaire.

## <a name="register-your-web-app-in-the-partner-dashboard"></a>Enregistrez votre application Web dans le Tableau de bord du partenaire
Lorsque vous enregistrez une application Web Azure ActiveDirectory dans le Tableau de bord du partenaire, vous permettez l'accès à l'API du Tableau de bord du partenaire. 
1.  Connectez-vous au [Tableau de bord du partenaire](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).
2.  Dans le **Tableau de bord**, sélectionnez **Paramètres du compte** &gt; **[Gestion des utilisateurs](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Dans la section **Web App**, cliquez sur **Ajouter une application Web**.
<br> **Remarque**: si vous avez déjà créé une application Web, vous pouvez ignorer l'étape3.
4.  Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web. Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30jours de l'application Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Ajoutez une clé secrète à votre application
1.  Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2ans.
2.  Cliquez sur **Ajouter une clé**. 
3.  Copiez et enregistrez la valeur de la clé secrète. Elle vous sera demandée pour la version d'évaluation gratuite de 30jours.
<br>**Remarque**: les clés secrètes d'application sont semblables à des mots de passe avec des dates d'expiration plus longues. Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.

## <a name="next-steps"></a>Étapes suivantes
Démarrez une [version d'évaluation gratuite de 30jours](https://go.microsoft.com/fwlink/?linkid=857895).
Les informations suivantes sont nécessaires pour démarrer la version d'évaluation:
- Identifiants de connexion au Tableau de bord du partenaire
- GUID ID de commerce
- GUID ID d'application
- Valeur de la clé secrète de l'application
