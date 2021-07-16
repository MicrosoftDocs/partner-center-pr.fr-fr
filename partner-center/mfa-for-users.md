---
title: Configurer vos utilisateurs avec l’authentification multifacteur
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Apprenez à configurer vos employés avec l’authentification multifacteur
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450801"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurer vos utilisateurs avec l’authentification multifacteur

**Rôles appropriés** : administrateur général

L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place. Nous recommandons vivement à tous les partenaires d’activer l’authentification multifacteur (MFA) pour les utilisateurs de leur locataire partenaire. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Ajouter l’authentification multifacteur pour vos utilisateurs

Pour effectuer cette tâche, vous devez être l’administrateur général de votre entreprise.

Il est plus facile d’activer l’authentification multifacteur pour vos utilisateurs quand vous les ajoutez à votre locataire Azure AD.

1. Connectez-vous au [portail Azure](https://portal.azure.com), puis accédez à **Gestion des utilisateurs**.
1. Sélectionnez **Authentification multifacteur**.
1. Sélectionnez l’utilisateur que vous souhaitez activer, puis sélectionnez **Activer**.

Cette opération active l’authentification multifacteur pour cet utilisateur. Quand l’authentification est activée et que l’utilisateur se connecte pour la première fois, il est invité à configurer sa vérification MFA. Ensuite, à chaque connexion, il lui est demandé de fournir un code qui lui est envoyé par e-mail ou SMS (selon l’option configurée).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Spécifiez le mode de vérification.":::

>[!NOTE]
>Vous pouvez **contraindre** les utilisateurs à utiliser l’authentification multifacteur en suivant les mêmes étapes que celles ci-dessus et en sélectionnant **Appliquer**. Pour plus d’informations, consultez [Activer l’authentification multifacteur Azure par utilisateur pour sécuriser les événements de connexion](/azure/active-directory/authentication/howto-mfa-userstates). 

Tous les utilisateurs ont initialement l’état  **Désactivé**. Quand vous inscrivez des utilisateurs à Azure Active Directory Multi-Factor Authentication par utilisateur, leur état passe à  **Activé**. Quand les utilisateurs activés se connectent et terminent le processus d’inscription, leur état passe à  **Appliqué**. 

## <a name="next-steps"></a>Étapes suivantes

- [Attribuer des rôles et des autorisations aux utilisateurs](permissions-overview.md)