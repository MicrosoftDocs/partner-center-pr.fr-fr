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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="322d7-103">Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client</span><span class="sxs-lookup"><span data-stu-id="322d7-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="322d7-104">**Rôles appropriés** : Administrateur général | Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="322d7-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="322d7-105">En tant que partenaire Fournisseur de solutions cloud (CSP), vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux.</span><span class="sxs-lookup"><span data-stu-id="322d7-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="322d7-106">Pour ce faire, vous devez disposer de privilèges d’administrateur.</span><span class="sxs-lookup"><span data-stu-id="322d7-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="322d7-107">Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie.</span><span class="sxs-lookup"><span data-stu-id="322d7-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="322d7-108">D’autres vous sont octroyés par votre client.</span><span class="sxs-lookup"><span data-stu-id="322d7-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="322d7-109">Privilèges d’administrateur pour Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="322d7-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="322d7-110">Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.</span><span class="sxs-lookup"><span data-stu-id="322d7-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="322d7-111">**Privilèges d’administrateur au niveau du locataire (privilèges d’administrateur délégués)**  : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients.</span><span class="sxs-lookup"><span data-stu-id="322d7-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="322d7-112">Les privilèges d’administrateur délégués offrent aux partenaires CSP un accès aux locataires de leurs clients.</span><span class="sxs-lookup"><span data-stu-id="322d7-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="322d7-113">Cet accès leur permet d’effectuer des fonctions d’administration telles que l’ajout/la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.</span><span class="sxs-lookup"><span data-stu-id="322d7-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="322d7-114">**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients.</span><span class="sxs-lookup"><span data-stu-id="322d7-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="322d7-115">Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="322d7-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="322d7-116">Rétablir les privilèges d’administrateur d’un partenaire CSP</span><span class="sxs-lookup"><span data-stu-id="322d7-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="322d7-117">Votre client peut recréer l’attribution de rôle CSP tant que vous fournissez `object ID` du groupe AdminAgents à votre client.</span><span class="sxs-lookup"><span data-stu-id="322d7-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="322d7-118">Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client et procéder comme suit.</span><span class="sxs-lookup"><span data-stu-id="322d7-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="322d7-119">Connectez-vous au tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="322d7-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="322d7-120">Dans le menu de l’Espace partenaires, sélectionnez **Clients**.</span><span class="sxs-lookup"><span data-stu-id="322d7-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="322d7-121">Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.**</span><span class="sxs-lookup"><span data-stu-id="322d7-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="322d7-122">Cette action génère un lien vers le client qui dispose des droits d’administrateur de locataire.</span><span class="sxs-lookup"><span data-stu-id="322d7-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="322d7-123">Votre client doit sélectionner le lien et approuver la demande de relation de revendeur.</span><span class="sxs-lookup"><span data-stu-id="322d7-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemple d’e-mail de la création d’une relation de revendeur.":::

5. <span data-ttu-id="322d7-125">Vous, le partenaire, devez vous connecter au locataire partenaire pour récupérer l’ID d’objet du groupe AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="322d7-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="322d7-126">Votre client doit ensuite effectuer les étapes suivantes à l’aide de PowerShell ou d’Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="322d7-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="322d7-127">Votre client doit disposer des éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="322d7-127">Your customer must have:</span></span>

- <span data-ttu-id="322d7-128">Rôle de **propriétaire** ou **d’administrateur de l’accès utilisateur**</span><span class="sxs-lookup"><span data-stu-id="322d7-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="322d7-129">Autorisations pour créer des attributions de rôle au niveau de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="322d7-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="322d7-130">a.</span><span class="sxs-lookup"><span data-stu-id="322d7-130">a.</span></span> <span data-ttu-id="322d7-131">Pour PowerShell uniquement, le client doit mettre à jour le module `Az.Resources`.</span><span class="sxs-lookup"><span data-stu-id="322d7-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="322d7-132">b.</span><span class="sxs-lookup"><span data-stu-id="322d7-132">b.</span></span> <span data-ttu-id="322d7-133">Le client se connecte au locataire où l’abonnement CSP existe.</span><span class="sxs-lookup"><span data-stu-id="322d7-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="322d7-134">c.</span><span class="sxs-lookup"><span data-stu-id="322d7-134">c.</span></span> <span data-ttu-id="322d7-135">Le client se connecte à l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="322d7-135">The customer connects to the subscription.</span></span> <span data-ttu-id="322d7-136">Cela s’applique *uniquement* si l’utilisateur dispose d’autorisations d’attribution de rôle sur plusieurs abonnements dans le locataire.</span><span class="sxs-lookup"><span data-stu-id="322d7-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="322d7-137">d.</span><span class="sxs-lookup"><span data-stu-id="322d7-137">d.</span></span> <span data-ttu-id="322d7-138">Le client crée ensuite l’attribution de rôle.</span><span class="sxs-lookup"><span data-stu-id="322d7-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="322d7-139">Au lieu d’accorder des autorisations de propriétaire dans l’étendue de l’abonnement, vous pouvez les accorder au niveau du groupe de ressources ou de la ressource.</span><span class="sxs-lookup"><span data-stu-id="322d7-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="322d7-140">Au niveau du groupe de ressources</span><span class="sxs-lookup"><span data-stu-id="322d7-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="322d7-141">Au niveau de la ressource</span><span class="sxs-lookup"><span data-stu-id="322d7-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="322d7-142">Si les étapes ci-dessus ne fonctionnent pas ou si vous recevez des erreurs, essayez la procédure « passe-partout » suivante pour rétablir les droits d’administrateur de votre client.</span><span class="sxs-lookup"><span data-stu-id="322d7-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="322d7-143">Dépannage</span><span class="sxs-lookup"><span data-stu-id="322d7-143">Troubleshooting</span></span>

<span data-ttu-id="322d7-144">Si le client ne peut pas effectuer l’étape 6 ci-dessus, demandez-lui d’essayer la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="322d7-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="322d7-145">Envoyez le fichier `newRoleAssignment.log` obtenu à Microsoft pour une analyse plus poussée.</span><span class="sxs-lookup"><span data-stu-id="322d7-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="322d7-146">Si la procédure « passe-partout » échoue pendant `Import-Module`, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="322d7-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="322d7-147">Si l’importation échoue parce que le module est en cours d’utilisation, redémarrez la session PowerShell en fermant et en ouvrant à nouveau toutes les fenêtres.</span><span class="sxs-lookup"><span data-stu-id="322d7-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="322d7-148">Vérifiez la version de `Az.Resources` avec `Get-Module Az.Resources -ListAvailable`.</span><span class="sxs-lookup"><span data-stu-id="322d7-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="322d7-149">Si la version 4.1.1 ne figure pas dans la liste, vous devez utiliser `Update-Module Az.Resources -Force`.</span><span class="sxs-lookup"><span data-stu-id="322d7-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="322d7-150">Si l’erreur indique que `Az.Accounts` doit avoir une version spécifique, mettez également à jour ce module, en remplaçant `Az.Resources` par `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="322d7-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="322d7-151">Vous devez ensuite redémarrer la session PowerShell.</span><span class="sxs-lookup"><span data-stu-id="322d7-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="322d7-152">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="322d7-152">Next steps</span></span>

- [<span data-ttu-id="322d7-153">Gérer les abonnements et les ressources dans le cadre du plan Azure</span><span class="sxs-lookup"><span data-stu-id="322d7-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
