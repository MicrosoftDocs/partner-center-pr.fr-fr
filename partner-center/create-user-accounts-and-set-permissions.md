---
title: Créer des comptes d’utilisateur et attribuer des rôles
description: Un rôle doit être attribué à chaque employé pour lui permettre d’accéder à l’Espace partenaires. Découvrez comment créer des comptes d’utilisateur, attribuer des rôles et définir des autorisations.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
Keywords: rôles, autorisations, ajouter un utilisateur, attribuer un rôle, administrateur, admin, agent
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 9ec8e98f77d49e34b6747b0f580502e9df25a950
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265193"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a>Créer des comptes d’utilisateur et attribuer des rôles et des autorisations

**Rôles appropriés**

- Administrateur des comptes
- Administrateur général
- Administrateur de la gestion des utilisateurs

Créez des comptes d’utilisateur pour les employés qui doivent accéder à l’Espace partenaires. Ces tâches doivent être effectuées par l’administrateur de la gestion des utilisateurs, l’administrateur des comptes ou l’administrateur général. L’utilisateur qui effectue ces tâches doit aussi se voir attribuer les rôles Administrateur d’utilisateurs ou Administrateur général d’Azure Active Directory (AAD). Pour plus d’informations sur les rôles d’AAD, consultez [Autorisations des rôles d’administrateur dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Ajouter un nouvel utilisateur

1. À partir de l’icône **Paramètres** en haut à droite de l’Espace partenaires, sélectionnez **Gestion des utilisateurs**.

2. Sélectionnez **Ajouter un utilisateur**.

3. Entrez le nom complet et l’adresse e-mail unique de l’utilisateur.

4. Sélectionnez le type d’agent et/ou le type d’administrateur que vous souhaitez attribuer à l’utilisateur. Comme l’accès à l'Espace partenaires dépend des rôles, vous pouvez affecter des autorisations pour personnaliser l’affichage de l’utilisateur de manière à ne montrer que les fonctionnalités dont l’utilisateur a besoin pour effectuer des tâches spécifiques.  Si des utilisateurs souhaitent se voir attribuer un rôle, ils peuvent trouver des administrateurs généraux à contacter en accédant à **Gestion des utilisateurs** et en filtrant sur Administrateur général.

5. Sélectionnez **Ajouter** pour créer le compte d’utilisateur. Confirmez les détails de l’utilisateur sur la page suivante.

> [!IMPORTANT]  
> Prenez note des informations de connexion du nouvel utilisateur affichées sur cette page. Veillez à copier et à envoyer ces informations au nouvel utilisateur car vous ne pourrez pas y accéder ultérieurement. 


L’utilisateur devra se connecter à l’Espace partenaires avec son nom d’utilisateur et un mot de passe temporaire. Lorsque l’utilisateur se connecte à l’Espace partenaires pour la première fois, il est invité à modifier son mot de passe. 


### <a name="find-your-global-admin"></a>Rechercher votre administrateur général

Parfois, un utilisateur peut être amené à changer de rôle ou un nouvel utilisateur peut souhaiter se voir attribuer un rôle spécifique.  
Pour trouver un administrateur général capable de changer des rôles ou d’attribuer des rôles à un nouvel utilisateur, à partir de l’icône **Paramètres** en haut à droite de l’Espace partenaires, sélectionnez **Gestion des utilisateurs** et filtrez sur Administrateur général. 


### <a name="new-global-admin"></a>Nouvel administrateur général

Si votre administrateur général quitte l’organisation et qu’une autre personne doit endosser ce rôle, vous pouvez envoyer un ticket à l’équipe Azure ou Office 365. Pour plus d’informations sur la façon de procéder, sélectionnez l’une des options ci-dessous.

[Nouvel administrateur général pour Azure](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Nouvel administrateur général pour Office 365](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>Attribuer des rôles d’utilisateur

Pour travailler dans l’Espace partenaires, un rôle doit vous être attribué.  Vous avez actuellement le choix entre des rôles de locataire Azure Active Directory, des rôles Fournisseur de solutions Cloud (CSP) et des rôles d’entreprise non-AAD. Une entreprise individuelle peut avoir besoin de tous ces rôles.

>[!Important]
>Les individus doivent être listés dans votre locataire pour pouvoir accéder à l’Espace partenaires. Les attributions de rôles fournissent un accès supplémentaire.


**Parmi les rôles de locataire AAD, citons :**
- Administrateur général
- Administrateur des utilisateurs

**Parmi les rôles CSP, citons :**
- Agent d’administration
- Administrateur de la facturation
- Agent commercial
- Agent du support technique

**Rôles qui gèrent l’adhésion au MPN et l’entreprise (non-AAD)**
- Administrateur partenaire MPN
- Administrateur des comptes
- Administrateur des références
- Administrateur de profils métier
- Utilisateur et administrateur d’incentives

**Le fournisseur de panneau de contrôle est un rôle CSP et non-AAD**.
- Administrateur général

L’**utilisateur invité** doit faire partie du locataire AAD et peut avoir n’importe quel rôle non-AAD.

Pour obtenir des informations spécifiques sur les rôles et ce qu’ils peuvent faire, consultez [Attribuer des autorisations aux utilisateurs](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Associer le compte Microsoft Learn d’un utilisateur dans l’Espace Partenaires

Pour que vous puissiez voir les parcours d’apprentissage et de formation suivis par vos utilisateurs pour acquérir des compétences, ils doivent associer leur ID MCP à leur compte Espace partenaires. En tant qu’administrateur général, quand vous ajoutez de nouveaux utilisateurs, veillez à leur rappeler d’associer leur ID MCP à leur compte. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Comment associer votre ID MCP à votre compte Espace partenaires

1. Dans le tableau de bord de l’Espace partenaires, sélectionnez l'icône **Votre compte** située dans le coin supérieur droit, puis **Mon profil**.

2. Sous **Votre formation**, vous pouvez associer votre compte Microsoft Learning et connecter votre compte Microsoft à l’Université des partenaires.
