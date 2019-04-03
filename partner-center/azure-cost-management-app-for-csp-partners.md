---
title: Azure Cost Management par Cloudyn pour les partenaires fournisseurs de solutions Cloud | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management par Cloudyn requiert un accès fourni à l'API de l'Espace partenaires.
author: Janet
ms.author: janet
Keywords: Application de gestion des coûts dans Azure, gérer les coûts, les applications web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: f1627727908eff9c686dd8359558e960d0fbff88
ms.sourcegitcommit: 6578eea4fe6836dad5710f8d22376ad8bba6e307
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2019
ms.locfileid: "58490341"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Application Azure Cost Management pour les partenaires fournisseurs de solutions Cloud  

**S’applique à**

-  Espace partenaires

[Obtenir plus d’informations sur Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Avant de commencer
Avant de pouvoir utiliser Azure Cost Management, veillez à ce que les conditions suivantes soient réunies :

- Vous êtes un partenaire du programme Fournisseur de solutions Cloud.
- Vous avez la possibilité de créer une application Web de l'API de l'Espace partenaires.

## <a name="overview"></a>Vue d'ensemble

Cloudyn est une application web qui permet de suivre et gérer la quantité vos clients utilisent Azure et les coûts de cette utilisation. Vous l'utilisez via l'API de l'Espace partenaires.

## <a name="register-your-web-app-in-the-partner-center"></a>Enregistrez votre application Web dans l'Espace partenaires
Lorsque vous enregistrez une application Web Azure Active Directory dans l'Espace partenaires, vous permettez l'accès à l'API de l'Espace partenaires. 
1.  Connectez-vous à l'[Espace partenaires](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) à l'aide d'un [compte d'administrateur global ou d'agent administratif](create-user-accounts-and-set-permissions.md).
2.  À partir de la **partenaires**, sélectionnez **paramètres du compte** &gt;  **[gestion des applications](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  Dans la section **Web App**, cliquez sur **Ajouter une application Web**.
<br> **Remarque**: Si vous avez déjà créé une application web, vous pouvez ignorer l’étape 3.
4.  Copiez et enregistrez le GUID **ID de commerce** et le GUID **ID d'application** de votre application Web. Vous aurez besoin des deux ID pour utiliser la version d'évaluation gratuite de 30 jours de l'application Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Ajoutez une clé secrète à votre application
1. Dans la liste déroulante en regard du bouton **Ajouter clé**, sélectionnez une durée de 1 ou 2 ans.
2. Cliquez sur **Ajouter une clé**. 
3. Copiez et enregistrez la valeur de la clé secrète. Elle vous sera demandée pour la version d'évaluation gratuite de 30 jours.<br>
   > [!NOTE]  
   > Les clés secrètes d’application sont comme les mots de passe avec des dates d’expiration plus long. Enregistrez la valeur de la clé à un emplacement sûr pour une utilisation ultérieure.

## <a name="next-steps"></a>Étapes suivantes
Démarrez une [version d'évaluation gratuite de 30 jours](https://go.microsoft.com/fwlink/?linkid=857895).
Les informations suivantes sont nécessaires pour démarrer la version d'évaluation :
- Identifiants de connexion à l'Espace partenaires
- GUID ID de commerce
- GUID ID d'application
- Valeur de la clé secrète de l'application
