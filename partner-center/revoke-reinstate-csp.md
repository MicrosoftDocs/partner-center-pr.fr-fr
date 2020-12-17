---
title: Rétablir les privilèges d’administrateur pour Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment aider les clients à rétablir les privilèges d’administrateur d’un partenaire afin que ce dernier puisse aider à gérer les abonnements Azure CSP d’un client.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011500"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client  

**Rôles applicables**

- Administrateur général
- Agent d’administration

En tant que partenaire CSP, vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux. Pour ce faire, vous devez disposer de privilèges d’administrateur. Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie. D’autres vous sont octroyés par votre client.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilèges d’administrateur pour Azure dans CSP

Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.

**Privilèges d’administrateur au niveau du locataire** (**privilèges d’administrateur délégués**) : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients. Cela donne aux partenaires CSP un accès aux locataires de leurs clients, ce qui leur permet d’effectuer des fonctions d’administration telles que l’ajout/la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.

**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients. Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Rétablir les privilèges d’administrateur des partenaires CSP

Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client.

1. Connectez-vous au tableau de bord de l’Espace partenaires, puis sélectionnez **Clients** dans le menu de l’Espace partenaires.

2. Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.** Cela génère un lien vers le client disposant des droits d’administrateur de locataire.

3. Cet utilisateur doit sélectionner le lien et approuver la demande de relation de revendeur.

   :::image type="content" source="images/azure/revoke4.png" alt-text="relation de revendeur":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Ajout du groupe d’agents d’administration en tant que propriétaire de l’abonnement Azure CSP

Votre client devra ajouter votre groupe d’agents d’administration en tant que propriétaire d’un abonnement Azure CSP, d’un groupe de ressources ou d’une ressource. 

1. Utilisez la console PowerShell ou l’environnement d’écriture de scripts intégré (ISE) de PowerShell. Vérifiez que les modules AzureAD sont installés.

2. Connectez-vous à votre locataire Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Obtenez l’ObjectId des groupes d’agents d’administration.

   ```powershell
   Get-AzureADGroup
   ```
   Les étapes suivantes sont effectuées par l’utilisatrice de la société de votre client qui dispose d’un accès propriétaire à l’abonnement Azure CSP.

4. L’utilisatrice disposant d’un accès propriétaire à l’abonnement Azure CSP se connecte à Azure en utilisant ses informations d’identification.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Elle pourra ensuite ajouter votre groupe d’agents d’administration en tant que propriétaire d’un abonnement Azure CSP, d’un groupe de ressources ou d’une ressource en appliquant un URI de ressource approprié dans le paramètre d’étendue. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Étapes suivantes

[Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)
