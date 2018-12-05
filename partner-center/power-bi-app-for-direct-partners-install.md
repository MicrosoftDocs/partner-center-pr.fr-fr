---
title: Installer et prévisualiser l’application Analyse de l’Espace partenaires pour MicrosoftPowerBI | Espacepartenaires
ms.topic: article
ms.date: 10/29/2018
description: Suivez les étapes ci-dessous pour obtenir un aperçu de l’application Analyse de l’Espace partenaires pour MicrosoftPowerBI (pour les partenaires directs dans le programme Fournisseur de solutions cloud).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e4eaecc151f8cc4e5e45bbfa7d02236fb1444a24
ms.sourcegitcommit: 3eb069edf36bdb61518c0c7cc2ccaf2d8dde4adb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2018
ms.locfileid: "6131698"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installer et prévisualiser l’application Analyse de l’Espace partenaires pour MicrosoftPowerBI

**S’applique à**

- Espace partenaires

## <a name="before-you-begin"></a>Avant de commencer

Sélectionnez l’application qui correspond le mieux à votre entreprise à partir de la liste des applications de Power BI disponibles à la suivante:
- [Partenaire direct](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Partenaire indirect](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Revendeur indirect](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Avant d’installer la version préliminaire de l'application Analyse de l’Espace partenaires pour MicrosoftPowerBI, veillez à satisfaire les conditions suivantes.

- Vous choisissez l’application de Power BI appropriée pour votre entreprise.

- Vous avez un abonnement actif à MicrosoftPower BI Professionnel ou MicrosoftPower BI Premium.

- Vous pouvez vous connecter à Power BI.

- Vous pouvez vous connecter en tant qu’administrateur général, agent administrateur ou administrateur de facturation au [client Azure ActiveDirectory (AD Azure) de votre société](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Pour installer l'application

1. Lancez le [processus d’installation](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. Sous **Vous disposez déjà d'un compte?**, sélectionnez **Se connecter**. 

3.  Sur la page suivante, entrez le nom d'utilisateur et le mot de passe pour votre Power BI, puis sélectionnez **Se connecter**. 

4.  Sur la fenêtre contextuelle **Se connecter à Analyse de l’Espace partenaires**, vérifiez que la **méthode d’authentification** est définie sur **oAuth2**, sinon, sélectionnez **oAuth2** dans la liste. 

    > [!NOTE]  
>  L’affichage de cette fenêtre peut prendre quelques minutes.

5.  Sur la page **Connecteur d'Analyse de l’Espace partenaires**, connectez-vous en utilisant les informations d’identification d'administrateur général, d’agent administrateur ou d'administrateur de facturation pour le client Azure AD de votre société, puis sélectionnez **Se connecter**.
 
6.  Lorsque vous êtes invité à accéder, sélectionnez **Accepter**. 

Une fois que le service Analyse de l’Espace partenaires est connecté à Power BI, les données commencent à se charger. Selon la quantité de données, cela peut prendre jusqu'à 10minutes. 

Après le chargement des données, vous pouvez commencer à utiliser les rapports et le tableau de bord de l'application Analyse de l’Espace partenaires dans Power BI.

## <a name="next-steps"></a>Étapes suivantes

[Afficher les données de votre entreprise avec l’application Analyse de l’Espace partenaires pour MicrosoftPowerBI](power-bi-app-for-direct-partners-use.md)
