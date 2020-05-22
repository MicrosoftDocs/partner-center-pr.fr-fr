---
title: Installer l’analyse de l’espace partenaires pour Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Suivez les étapes décrites dans cet article pour installer et afficher un aperçu de l’application Partner Center Analytics pour Power BI (pour les partenaires directs dans CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795872"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installer et prévisualiser l’application Analyse de l’Espace partenaires pour Microsoft Power BI

**S’applique à**

- Espace partenaires

**Rôles appropriés**
-   Administrateur général
-   Administrateur des utilisateurs
-   Agent commercial
-   Agent d’administration

## <a name="before-you-begin"></a>Avant de commencer

Sélectionnez l’application la plus pertinente pour votre entreprise dans la liste suivante d’applications Power BI disponibles :
- [Partenaire direct](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Partenaire indirect](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Revendeur indirect](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Avant d’installer la version préliminaire de l’application Partner Center Analytics, vérifiez que vous remplissez les conditions suivantes.

- Vous choisissez l’application de Power BI appropriée pour votre entreprise.

- Vous disposez d’un abonnement actif à Microsoft Power BI Professional ou Microsoft Power BI Premium.

- Vous pouvez vous connecter à Power BI.

- Vous pouvez vous connecter en tant qu’administrateur général, agent admin ou administrateur de facturation au [locataire Azure Active Directory (Azure AD) de votre entreprise](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Pour installer l’application

1. Lancer [le processus d’installation](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. Sous **déjà un compte ?** , sélectionnez **se connecter**. 

3. Sur la page suivante, entrez votre nom d’utilisateur et votre mot de passe Power BI, puis sélectionnez **se connecter**. 

4. Dans la fenêtre contextuelle **se connecter à l’analyse de l’espace partenaires** , vérifiez que la **méthode d’authentification** est définie sur **oAuth2** ou sélectionnez **oAuth2** dans la liste, si ce n’est pas le cas. 

> [!NOTE]  
>  L’affichage de cette fenêtre peut prendre quelques minutes.

5. Sur la page connecteur de l’analyse de l' **espace partenaires** , connectez-vous avec les informations d’identification de l’administrateur général, de l’agent admin ou de facturation pour le locataire Azure AD de votre entreprise, puis sélectionnez **se connecter**.
 
6. Lorsque vous y êtes invité, sélectionnez **accepter**. 

Une fois que le Service Partner Center Analytics est connecté à Power BI, les données commencent à se charger. Selon la quantité de données, cela peut prendre jusqu’à 10 minutes. 

Une fois le chargement des données terminé, vous pouvez commencer à utiliser le tableau de bord de l’application et les rapports Partner Center Analytics dans Power BI.

## <a name="next-steps"></a>Étapes suivantes

[Afficher vos données d’entreprise avec l’application Partner Center Analytics pour Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
