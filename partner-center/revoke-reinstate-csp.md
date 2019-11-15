---
title: Rétablir les privilèges d’administrateur pour les abonnements Azure CSP | Espace partenaires
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ce document explique comment aider les clients à rétablir les privilèges d’administrateur d’un partenaire
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 1bcbcf32e3b3f4513ed3e55984b49b090da4a734
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651702"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Rétablir les privilèges d’administrateur pour les abonnements Azure CSP  

**Rôles applicables**

- Administrateur global
- Agent d’administration

En tant que partenaire CSP, vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux. Pour ce faire, vous devez disposer de privilèges d’administrateur. Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie. D’autres vous sont octroyés par votre client.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilèges d’administrateur pour Azure dans CSP 

Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP. 

**Privilèges d’administrateur au niveau du locataire** (**privilèges d’administrateur délégués**) : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients. Cela donne aux partenaires CSP un accès aux locataires de leurs clients, ce qui leur permet d’effectuer des fonctions d’administration telles que l’ajout/la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur. 

**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients. Cela donne aux partenaires CSP un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure. 


## <a name="reinstate-csp-partners-admin-privileges"></a>Rétablir les privilèges d’administrateur des partenaires CSP

Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client.
 
 1. Connectez-vous au tableau de bord de l’Espace partenaires, puis sélectionnez **Clients** dans le menu de l’Espace partenaires.

 2. Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.** Cela génère un lien vers le client disposant des droits d’administrateur de locataire.

 3. Cet utilisateur doit sélectionner le lien et approuver la demande de relation de revendeur.
 
![relation de revendeur](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Ajout du groupe d’agents d’administration en tant que propriétaire de l’abonnement Azure CSP

 Votre client devra ajouter votre groupe d’agents d’administration en tant que propriétaire de l’abonnement Azure CSP.

1. Utilisez la console PowerShell ou l’environnement d’écriture de scripts intégré (ISE) de PowerShell. Vérifiez que les modules AzureRM et AzureAD sont installés. 

2.  Connectez-vous à votre locataire Azure AD.
Applet de commande PowerShell : Connect-AzureAD

3.  Obtenez l’ObjectId des groupes d’agents d’administration.
Applet de commande PowerShell : Get-AzureADGroup`1nn

![groupe d’agents d’administration](images/azure/revoke5.png)

Les étapes suivantes sont effectuées par l’utilisatrice de la société de votre client qui dispose d’un accès propriétaire à l’abonnement Azure CSP.

4. L’utilisatrice disposant d’un accès propriétaire à l’abonnement Azure CSP se connecte à Azure Resource Manager à l’aide de ses informations d’identification.

    Applet de commande PowerShell : Login-AzureRMAccount

5.  Elle peut ensuite ajouter votre groupe d’agents d’administration en tant que propriétaire à l’abonnement Azure CSP.

    Applet de commande PowerShell : New-AzureRMRoleAssignment -ObjectId <ID d’objet que vous avez obtenu à l’étape 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![propriétaires d’agents d’administration](images/azure/revoke6.png)    

**Pour plus d’informations**

[Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)
