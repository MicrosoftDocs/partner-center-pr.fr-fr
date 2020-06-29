---
title: Implémenter les exigences de sécurité des partenaires
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment implémenter les exigences de sécurité nécessaires pour vos utilisateurs
author: LauraBrenner
ms.author: labrenne
keywords: sécurité
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133264"
---
# <a name="implement-the-partner-security-requirements"></a>Implémenter les exigences de sécurité des partenaires

**Rôles appropriés**

- Administrateur général

La sécurité et la confidentialité des clients et des partenaires sont des priorités absolues pour Microsoft. Nous observons un nombre croissant d'atteintes à la sécurité toujours plus sophistiquées, principalement liées à des identités compromises. Dans la mesure où les contrôles préventifs jouent un rôle clé dans une stratégie de défense globale visant à contrer les attaques de sécurité, nous allons commencer à mettre en œuvre un ensemble d’exigences de sécurité obligatoires pour améliorer la protection des partenaires et de leurs clients.

Ce didacticiel vous apprendra à identifier les exigences de sécurité des partenaires, à les satisfaire et à évaluer leur impact pour les utilisateurs de votre annuaire de partenaires.

Tous les partenaires qui participent au programme des fournisseurs de solutions Cloud, de même que les fournisseurs de panneau de contrôle (CPV) et les partenaires-conseillers, sont tenus d'imposer l'authentification multifacteur (MFA) à chacun des utilisateurs de leur locataire partenaire. Pour ce faire, deux [stratégies Azure Active Directory de référence](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) doivent être activées. Les stratégies de référence sont un ensemble de stratégies prédéfinies qui contribuent à protéger les organisations contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure la pulvérisation de mot de passe, le rejeu et le hameçonnage. Les stratégies de base de référence sont disponibles dans toutes les éditions d’Azure Active Directory. Microsoft met ces stratégies de protection de base de référence à la disposition de tous, car les attaques basées sur l’identité ont augmenté ces dernières années.

Les procédures ci-dessous décrivent le processus d’activation des deux stratégies de base de référence nécessaires :

- **Exiger l’authentification multifacteur pour les administrateurs** : L’activation de la stratégie Exiger l’authentification multifacteur pour les administrateurs nécessite que les utilisateurs ayant un rôle d’administrateur s’inscrivent pour  l’authentification MFA avec l’application d’authentification. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.

- **Protection de l’utilisateur final** : La protection de l’utilisateur final est une stratégie de protection de base de référence MFA basée sur les risques qui protège tous les utilisateurs d’un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent à l’authentification MFA à l’aide de l’application d’authentification. Les utilisateurs peuvent ignorer l’invite d’inscription à l’authentification MFA pendant 14 jours, après quoi il leur est impossible de se connecter tant qu’ils ne s’inscrivent pas à l’authentification MFA. Une fois inscrits à l’authentification multifacteur, les utilisateurs sont invités à utiliser l’authentification multifacteur uniquement pendant les tentatives de connexion risquées. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que leur mot de passe soit réinitialisé et que les événements à risque soient ignorés.

Une fois ces stratégies activées, chaque utilisateur peut utiliser Azure MFA sans frais supplémentaires. Si vous utilisez une solution tierce, vous devez imposer l'authentification MFA à chacun des utilisateurs qui accèdent aux services cloud commerciaux de Microsoft.

>[!NOTE]
>Étant donné que l'authentification MFA sera imposée à chacun des utilisateurs de l'annuaire de partenaires, elle aura un impact sur toutes les automatisations ou intégrations qui utilisent les informations d'identification de l'utilisateur. Pour y remédier, vous devrez modifier la façon dont votre automatisation ou votre intégration se connecte aux services cloud commerciaux de Microsoft. Si le service auquel vous vous connectez prend en charge l’authentification par jeton, nous vous recommandons d'implémenter le framework [Modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Étape 1 : Bloquer tous les protocoles d’authentification hérités existants

Avant d’activer les stratégies Exiger l’authentification MFA pour les administrateurs et Protection de l’utilisateur final, vérifiez que vos utilisateurs n’utilisent pas des protocoles d’authentification hérités. Pour plus d'informations, consultez l'article [Procédure : Bloquer l'authentification héritée auprès d'Azure AD à l'aide de l'accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use).

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Étape 2 : Activer la stratégie de base de référence Exiger l’authentification multifacteur pour les administrateurs

La stratégie de base de référence Exiger l’authentification multifacteur pour les administrateurs nécessite l’authentification MFA pour les rôles d’annuaire suivants, considérés comme les rôles Azure AD les plus privilégiés :

- Administrateur général
- Administrateur SharePoint
- Administrateur Exchange
- Administrateur de l’accès conditionnel
- Administrateur de sécurité
- Administrateur du support technique/administrateur de mots de passe
- Administrateur de facturation
- Administrateur utilisateur

Lors de l’activation de la stratégie Exiger l’authentification multifacteur pour les administrateurs, les neuf rôles d’administrateur ci-dessus doivent s’inscrire à l’authentification MFA à l’aide de l’application d’authentification. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.

Si votre organisation utilise ces comptes dans des scripts ou du code, envisagez de les remplacer par des  [identités managées](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Pour activer cette stratégie et protéger vos administrateurs :

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.

2. Accédez à **Azure Active Directory** > **Accès conditionnel**.

3. Dans la liste des stratégies, sélectionnez **Stratégie de référence : exiger l’authentification multifacteur pour les administrateurs**.

4. Définissez **Activer la stratégie** sur **Utiliser la stratégie immédiatement**.

5. Sélectionnez **Enregistrer**.

Une fois que vous avez activé cette stratégie, les utilisateurs dans les rôles d’administrateur ci-dessus sont invités à se connecter pour fournir des informations de sécurité supplémentaires et configurer l’application mobile. Une fois cette opération terminée, ils peuvent se connecter au service cloud approprié.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Étape 3 : Activer la stratégie de base de référence Protection de l’utilisateur final

La stratégie de référence de protection de l’utilisateur final protège tous les utilisateurs dans un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent à l’authentification Azure MFA dans un délai de 14 jours. Une fois inscrits, les utilisateurs ne seront invités à utiliser l'authentification MFA que lors des tentatives de connexion risquées. À l'avenir, ce comportement changera pour les locataires partenaires. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que le mot de passe soit réinitialisé et les risques ignorés.

La stratégie Stratégie de base de référence : La protection de l’utilisateur final est préconfigurée et apparaît en haut quand vous accédez au panneau Accès conditionnel dans le portail Azure.

Pour activer cette stratégie et protéger vos utilisateurs :

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.

2. Accédez à **Azure Active Directory** > **Accès conditionnel**.

3. Dans la liste des stratégies, sélectionnez **Stratégie de référence : Protection de l’utilisateur final (préversion)** .

4. Définissez **Activer la stratégie** sur **Utiliser la stratégie immédiatement**.

5. Sélectionnez **Enregistrer**.

Une fois que vous avez activé cette stratégie, tous les utilisateurs sont invités à se connecter pour fournir des informations de sécurité supplémentaires et configurer l’application mobile. Une fois cette opération terminée, ils peuvent se connecter au service cloud approprié.

>[!NOTE]
>Tant que les exigences de sécurité des partenaires ne sont pas appliquées, les utilisateurs qui ne sont pas couverts par la stratégie de base de référence Exiger l’authentification multifacteur pour les administrateurs sont soumis seulement à l’authentification MFA en fonction du risque.