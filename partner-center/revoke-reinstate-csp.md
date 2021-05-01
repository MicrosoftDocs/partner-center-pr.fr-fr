---
title: Rétablir les privilèges d’administrateur pour Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment aider les clients à rétablir les privilèges d’administrateur d’un partenaire afin que ce dernier puisse aider à gérer les abonnements Azure CSP d’un client.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018185"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client  

**Rôles appropriés**

- Administrateur général
- Agent d’administration

En tant que partenaire CSP, vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux. Pour ce faire, vous devez disposer de privilèges d’administrateur. Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie. D’autres vous sont octroyés par votre client.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilèges d’administrateur pour Azure dans CSP

Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.

**Privilèges d’administrateur au niveau du locataire** (**privilèges d’administrateur délégués**) : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients. Les privilèges d’administrateur délégués donnent aux partenaires CSP un accès aux locataires de leurs clients, ce qui leur permet d’effectuer des opérations d’administration telles que l’ajout ou la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.

**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients. Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Rétablir les privilèges d’administrateur des partenaires CSP

Votre client peut recréer l’attribution de rôle CSP tant que vous fournissez l’ID d’objet du groupe AdminAgents à votre client. Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client.

1. Connectez-vous au tableau de bord de l’Espace partenaires, puis sélectionnez **Clients** dans le menu de l’Espace partenaires.

2. Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.** Cette action génère un lien vers le client qui dispose des droits d’administrateur de locataire.

3. Ce client doit sélectionner le lien et approuver la demande de relation de revendeur.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemple d’e-mail de la création d’une relation de revendeur":::

4. Vous, le partenaire, devez vous connecter au locataire partenaire pour récupérer l’ID d’objet du groupe AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Votre client, qui a le rôle **de propriétaire ou d’administrateur de l’accès utilisateur** et qui a l’autorisation de créer une attribution de rôle au niveau de l’abonnement, effectue les opérations suivantes :


    1. Se connecte au locataire où l’abonnement CSP existe.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Se connecte à l’abonnement (applicable uniquement si l’utilisateur dispose d’autorisations d’attribution de rôle sur plusieurs abonnements dans le locataire).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"`


    3. Crée l’attribution de rôle.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Si vous souhaitez accorder l’autorisation de rôle Propriétaire au niveau du groupe de ressources ou de la ressource, et non au niveau de l’abonnement, les commandes suivantes peuvent fonctionner :


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Étapes suivantes

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)
