---
title: Azure Cost Management par Cloudyn pour les fournisseurs de services de chiffrement
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment inscrire l’application Web Cloudyn et utiliser une clé secrète pour celle-ci dans l’espace partenaires afin de pouvoir utiliser l’application pour suivre l’utilisation et les coûts d’Azure du client.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435908"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Suivre l’utilisation et les coûts d’Azure des clients avec l’application Azure Cost Management pour les partenaires CSP  

**S’applique à**

- Espace partenaires
- Partenaires du programme Fournisseur de solutions Cloud

**Rôles appropriés**

- Administrateur général
- Agent d’administration

[Obtenir plus d’informations sur Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Avant de commencer
Avant de pouvoir utiliser Azure Cost Management, assurez-vous que vous remplissez les conditions suivantes :

- Vous êtes un partenaire dans le programme du fournisseur de solutions Cloud.
- Vous avez la possibilité de créer une application Web d’API de l’espace partenaires.

## <a name="overview"></a>Vue d’ensemble

Cloudyn est une application Web qui vous permet de suivre et de gérer l’utilisation d’Azure par vos clients, ainsi que les coûts de cette utilisation. Vous l’utilisez par le biais de l’API espace partenaires.

## <a name="register-your-web-app-in-the-partner-center"></a>Inscrire votre application Web dans l’espace partenaires
Lorsque vous inscrivez une application Web Azure Active Directory dans l’espace partenaires, vous activez l’accès à l’API espace partenaires. 
1.  Connectez-vous à [l’espace partenaires](https://partnercenter.microsoft.com/pcv/dashboard/overview) à l’aide d’un [compte d’administrateur général ou d’agent d’administration](create-user-accounts-and-set-permissions.md).
2.  Dans l' **espace partenaires**, sélectionnez **paramètres du compte** &gt; **[gestion des applications](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  Dans la section **application Web** , cliquez sur **Ajouter une nouvelle application Web**.
<br> **Remarque**: Si vous avez déjà créé une application Web, vous pouvez ignorer l’étape 3.
4.  Copiez et enregistrez le GUID de l' **ID de commerce** et le GUID de l' **ID d’application** pour votre application Web. Vous aurez besoin des deux ID pour utiliser la version d’évaluation gratuite de 30 jours de l’application Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Ajouter une clé secrète à votre application
1. Dans la liste déroulante en regard du bouton **Ajouter une clé** , sélectionnez une durée de 1 ou 2 ans.
2. Cliquez sur **Ajouter une clé**. 
3. Copiez et enregistrez la valeur de la clé secrète. Vous en aurez besoin pour la version d’évaluation gratuite de 30 jours.<br>
   > [!NOTE]  
   > Les clés secrètes de l’application sont semblables aux mots de passe avec des dates d’expiration plus longues. Enregistrez la valeur de clé dans un emplacement sécurisé pour une utilisation ultérieure.

## <a name="next-steps"></a>Étapes suivantes
Démarrez une [version d’évaluation gratuite de 30 jours](https://go.microsoft.com/fwlink/?linkid=857895).
Vous avez besoin des informations suivantes pour commencer la version d’évaluation :
- Informations d’identification de connexion de l’espace partenaires
- GUID de l’ID de commerce
- GUID de l’ID d’application
- Valeur de clé secrète d’application
