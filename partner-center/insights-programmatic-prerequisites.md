---
title: Conditions préalables à l’accès programmatique aux données d’analyse
description: Conditions préalables à l’accès programmatique aux données d’analyse
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375068"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Conditions préalables à l’accès programmatique aux données d’analyse

**Rôles appropriés :** Administrateur général | Administrateur MPN

Avant de pouvoir accéder par programme aux données analytiques de Partner Insights, vous devez remplir les conditions suivantes.

## <a name="mpn-program-enrollment"></a>Inscription au programme MPN

Pour accéder par programme à des données analytiques d’analyse partenaire, vous devez être inscrit au programme MPN et disposer d’un compte espace partenaires. Pour en savoir plus, consultez [créer un compte MPN dans l’espace partenaires](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>créer une application Azure Active Directory (AAD)

les informations d’identification de l’utilisateur standard ne peuvent pas être utilisées pour l’accès par programme aux données du partenaire Informations Analytics. une application Azure Active Directory (AAD) doit être créée avec un secret (application + accès utilisateur) pour accéder aux api d’accès par programme. pour savoir comment créer une application AAD et une clé secrète, consultez [démarrage rapide : inscrire une application avec le Plateforme d’identités Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Une autorisation est requise pour accéder à l’API partenaire Microsoft. Pour savoir comment ajouter une autorisation, consultez [Partner API Authentication-Partner](/partner/develop/api-authentication#application-and-user-access) .

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Attribuer le rôle ERV (Executive Report Viewer) à l’utilisateur

Pour accéder par programme à des données analytiques d’analyse partenaire, vous devez disposer d’une visionneuse de rapports (ERV). pour savoir comment attribuer le rôle ERV à l’utilisateur, consultez [espace partenaires Informations accès en fonction du rôle-espace partenaires](insights-roles.md)

## <a name="generate-an-aad-token"></a>Générer un jeton AAD

Vous devez générer un jeton AAD à l’aide de l’ID d’application (client), de la clé secrète client, de votre ID d’utilisateur et de votre mot de passe. Pour savoir comment générer un jeton AAD, cliquez   [ici](insights-programmatic-first-api-call.md#token-generation) .

> [!Note]
> Ce jeton est valide une heure.

## <a name="next-steps"></a>Étapes suivantes
[Paradigme de l’accès programmatique](insights-programmatic-access-paradigm.md)