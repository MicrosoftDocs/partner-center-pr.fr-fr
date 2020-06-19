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
ms.openlocfilehash: 36efc58198be67181ed448d90db505889c3070d4
ms.sourcegitcommit: b81cde2d62e096e58ac3ce12fc9c35a97d10d51f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/18/2020
ms.locfileid: "85072415"
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
- [Fournisseur direct](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Fournisseur indirect](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Revendeur indirect](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Avant d’installer la version préliminaire de l’application Partner Center Analytics, vérifiez que vous remplissez les conditions suivantes.

- Vous choisissez l’application de Power BI appropriée pour votre entreprise.

- Vous disposez d’une licence Power BI Pro.

- Vous disposez des autorisations nécessaires pour installer des applications de modèle sur votre locataire.

- Vous pouvez vous connecter à Power BI.

- Vous pouvez vous connecter en tant qu’administrateur général, agent admin ou administrateur de facturation au [locataire Azure Active Directory (Azure AD) de votre entreprise](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Pour installer l’application

1. Cliquez sur le lien source de l’application donné (fournisseur direct/fournisseur indirect/revendeur indirect) dans la section ci-dessus.

2. Cliquez sur **Télécharger maintenant**. 

3. Pour accepter les conditions générales, cliquez sur **Continuer**.

4. Vous avez déjà un compte ? Sélectionnez **se connecter**.

5. Sur la page suivante, entrez votre nom d’utilisateur et votre mot de passe Power BI, puis sélectionnez se connecter.

6. Installez l’espace de travail en spécifiant le nom de l’espace de travail.

7. Vous trouverez la section modèles d’applications installés sous applications.

8. Cliquez sur applications, puis sélectionnez les applications installées.

9. L’écran prise en main de votre nouvelle application s’ouvre.

10. Pour vous connecter aux données, cliquez sur **se connecter**.

11. Dans la fenêtre contextuelle **se connecter à l’analyse de l’espace partenaires** , vérifiez que la **méthode d’authentification** est définie sur **oAuth2** ou sélectionnez **oAuth2** dans la liste, si ce n’est pas le cas. 

> [!NOTE]  
>  L’affichage de cette fenêtre peut prendre quelques minutes.

12. Sur la page connecteur de l’analyse de l' **espace partenaires** , connectez-vous avec les informations d’identification de l’administrateur général, de l’agent admin ou de facturation pour le locataire Azure AD de votre entreprise, puis sélectionnez **se connecter**.
 
13. Lorsque vous y êtes invité, sélectionnez **accepter**. 

Une fois que le Service Partner Center Analytics est connecté à Power BI, les données commencent à se charger. Selon la quantité de données, cela peut prendre jusqu’à 10 minutes. 

Une fois le chargement des données terminé, vous pouvez commencer à utiliser le tableau de bord de l’application et les rapports Partner Center Analytics dans Power BI.

## <a name="next-steps"></a>Étapes suivantes

[Afficher vos données d’entreprise avec l’application Partner Center Analytics pour Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
