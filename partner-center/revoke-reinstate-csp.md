---
title: Rétablir les privilèges d’administrateur pour Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment aider les clients à rétablir les privilèges d’administrateur d’un partenaire afin que ce dernier puisse aider à gérer les abonnements Fournisseur de solutions cloud (CSP) Azure d’un client.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510174"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client  

**Rôles appropriés** : Administrateur général | Agent d’administration

En tant que partenaire Fournisseur de solutions cloud (CSP), vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux. Pour ce faire, vous devez disposer de privilèges d’administrateur. Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie. D’autres vous sont octroyés par votre client.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilèges d’administrateur pour Azure dans CSP

Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.

- **Privilèges d’administrateur au niveau du locataire (privilèges d’administrateur délégués)**  : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients. Les privilèges d’administrateur délégués offrent aux partenaires CSP un accès aux locataires de leurs clients. Cet accès leur permet d’effectuer des fonctions d’administration telles que l’ajout/la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.
- **Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients. Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Rétablir les privilèges d’administrateur d’un partenaire CSP

Votre client peut recréer l’attribution de rôle CSP tant que vous fournissez `object ID` du groupe AdminAgents à votre client. Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client et procéder comme suit.

1. Connectez-vous au tableau de bord de l’Espace partenaires.

2. Dans le menu de l’Espace partenaires, sélectionnez **Clients**.

3. Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.** Cette action génère un lien vers le client qui dispose des droits d’administrateur de locataire.

4. Votre client doit sélectionner le lien et approuver la demande de relation de revendeur.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemple d’e-mail de la création d’une relation de revendeur.":::

5. Vous, le partenaire, devez vous connecter au locataire partenaire pour récupérer l’ID d’objet du groupe AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Votre client doit ensuite effectuer les étapes suivantes à l’aide de PowerShell ou d’Azure CLI. Votre client doit disposer des éléments suivants :

- Rôle de **propriétaire** ou **d’administrateur de l’accès utilisateur** 
- Autorisations pour créer des attributions de rôle au niveau de l’abonnement

   a. Pour PowerShell uniquement, le client doit mettre à jour le module `Az.Resources`.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Le client se connecte au locataire où l’abonnement CSP existe.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Le client se connecte à l’abonnement. Cela s’applique *uniquement* si l’utilisateur dispose d’autorisations d’attribution de rôle sur plusieurs abonnements dans le locataire.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Le client crée ensuite l’attribution de rôle.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Au lieu d’accorder des autorisations de propriétaire dans l’étendue de l’abonnement, vous pouvez les accorder au niveau du groupe de ressources ou de la ressource. 

- Au niveau du groupe de ressources

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Au niveau de la ressource

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Si les étapes ci-dessus ne fonctionnent pas ou si vous recevez des erreurs, essayez la procédure « passe-partout » suivante pour rétablir les droits d’administrateur de votre client.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Dépannage

Si le client ne peut pas effectuer l’étape 6 ci-dessus, demandez-lui d’essayer la commande suivante :

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Envoyez le fichier `newRoleAssignment.log` obtenu à Microsoft pour une analyse plus poussée.

Si la procédure « passe-partout » échoue pendant `Import-Module`, procédez comme suit :
- Si l’importation échoue parce que le module est en cours d’utilisation, redémarrez la session PowerShell en fermant et en ouvrant à nouveau toutes les fenêtres.
- Vérifiez la version de `Az.Resources` avec `Get-Module Az.Resources -ListAvailable`.
- Si la version 4.1.1 ne figure pas dans la liste, vous devez utiliser `Update-Module Az.Resources -Force`.
- Si l’erreur indique que `Az.Accounts` doit avoir une version spécifique, mettez également à jour ce module, en remplaçant `Az.Resources` par `Az.Accounts`. Vous devez ensuite redémarrer la session PowerShell.


## <a name="next-steps"></a>Étapes suivantes

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)
