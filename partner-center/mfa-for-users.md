---
title: Configurer vos utilisateurs avec l’authentification multifacteur
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Apprenez à configurer vos employés avec l’authentification multifacteur
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526001"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurer vos utilisateurs avec l’authentification multifacteur

**Rôles appropriés**

- Administrateur général

L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place. Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.

Les partenaires sont tenus d’appliquer l’authentification multifacteur (MFA) à tous les comptes d’utilisateur de leur locataire de partenaire. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Ajouter l’authentification multifacteur pour vos utilisateurs

Pour effectuer cette tâche, vous devez être l’administrateur général de votre entreprise.

Il est plus facile d’activer l’authentification multifacteur pour vos utilisateurs quand vous les ajoutez à votre locataire Azure AD.

1. Connectez-vous au [portail Azure](https://portal.azure.com), puis accédez à **Gestion des utilisateurs** .
1. Sélectionnez **Authentification multifacteur** .
1. Sélectionnez l’utilisateur que vous souhaitez activer, puis sélectionnez **Activer** .

Cette opération active l’authentification multifacteur pour cet utilisateur. Quand l’authentification est activée et que l’utilisateur se connecte pour la première fois, il est invité à configurer sa vérification MFA. Ensuite, à chaque connexion, il lui est demandé de fournir un code qui lui est envoyé par e-mail ou SMS.  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Spécifier le mode de vérification":::

Pour forcer les utilisateurs à utiliser l’authentification multifacteur, suivez les mêmes étapes que ci-dessus et choisissez l’option **Appliquer** . Pour plus d’informations, consultez [activer Azure Multi-Factor Authentication par utilisateur pour sécuriser les événements de connexion](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates). 

Tous les utilisateurs ont initialement l’état  **Désactivé** . Quand vous inscrivez des utilisateurs à Azure Multi-Factor Authentication par utilisateur, leur état passe à  **Activé** . Quand les utilisateurs activés se connectent et terminent le processus d’inscription, leur état passe à  **Appliqué** . 

## <a name="next-steps"></a>Étapes suivantes

- [Attribuer des rôles et des autorisations aux utilisateurs](permissions-overview.md)



