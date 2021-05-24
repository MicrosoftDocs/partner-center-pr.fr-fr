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
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855418"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="4ae42-103">Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client</span><span class="sxs-lookup"><span data-stu-id="4ae42-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="4ae42-104">**Rôles appropriés** : Administrateur général | Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="4ae42-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="4ae42-105">En tant que partenaire CSP, vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux.</span><span class="sxs-lookup"><span data-stu-id="4ae42-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="4ae42-106">Pour ce faire, vous devez disposer de privilèges d’administrateur.</span><span class="sxs-lookup"><span data-stu-id="4ae42-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="4ae42-107">Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie.</span><span class="sxs-lookup"><span data-stu-id="4ae42-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="4ae42-108">D’autres vous sont octroyés par votre client.</span><span class="sxs-lookup"><span data-stu-id="4ae42-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="4ae42-109">Privilèges d’administrateur pour Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="4ae42-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="4ae42-110">Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.</span><span class="sxs-lookup"><span data-stu-id="4ae42-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="4ae42-111">**Privilèges d’administrateur au niveau du locataire** (**privilèges d’administrateur délégués**) : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients.</span><span class="sxs-lookup"><span data-stu-id="4ae42-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="4ae42-112">Les privilèges d’administrateur délégués donnent aux partenaires CSP un accès aux locataires de leurs clients, ce qui leur permet d’effectuer des opérations d’administration telles que l’ajout ou la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4ae42-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="4ae42-113">**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients.</span><span class="sxs-lookup"><span data-stu-id="4ae42-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="4ae42-114">Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="4ae42-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="4ae42-115">Rétablir les privilèges d’administrateur des partenaires CSP</span><span class="sxs-lookup"><span data-stu-id="4ae42-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="4ae42-116">Votre client peut recréer l’attribution de rôle CSP tant que vous fournissez l’ID d’objet du groupe AdminAgents à votre client.</span><span class="sxs-lookup"><span data-stu-id="4ae42-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="4ae42-117">Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client.</span><span class="sxs-lookup"><span data-stu-id="4ae42-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="4ae42-118">Connectez-vous au tableau de bord de l’Espace partenaires, puis sélectionnez **Clients** dans le menu de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="4ae42-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="4ae42-119">Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.**</span><span class="sxs-lookup"><span data-stu-id="4ae42-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="4ae42-120">Cette action génère un lien vers le client qui dispose des droits d’administrateur de locataire.</span><span class="sxs-lookup"><span data-stu-id="4ae42-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="4ae42-121">Ce client doit sélectionner le lien et approuver la demande de relation de revendeur.</span><span class="sxs-lookup"><span data-stu-id="4ae42-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemple d’e-mail de la création d’une relation de revendeur":::

4. <span data-ttu-id="4ae42-123">Vous, le partenaire, devez vous connecter au locataire partenaire pour récupérer l’ID d’objet du groupe AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="4ae42-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="4ae42-124">Votre client, qui a le rôle **de propriétaire ou d’administrateur de l’accès utilisateur** et qui a l’autorisation de créer une attribution de rôle au niveau de l’abonnement, effectue les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="4ae42-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="4ae42-125">Se connecte au locataire où l’abonnement CSP existe.</span><span class="sxs-lookup"><span data-stu-id="4ae42-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="4ae42-126">Se connecte à l’abonnement (applicable uniquement si l’utilisateur dispose d’autorisations d’attribution de rôle sur plusieurs abonnements dans le locataire).</span><span class="sxs-lookup"><span data-stu-id="4ae42-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="4ae42-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="4ae42-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="4ae42-128">Crée l’attribution de rôle.</span><span class="sxs-lookup"><span data-stu-id="4ae42-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="4ae42-129">Si vous souhaitez accorder l’autorisation de rôle Propriétaire au niveau du groupe de ressources ou de la ressource, et non au niveau de l’abonnement, les commandes suivantes peuvent fonctionner :</span><span class="sxs-lookup"><span data-stu-id="4ae42-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="4ae42-130">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="4ae42-130">Next steps</span></span>

- [<span data-ttu-id="4ae42-131">Gérer les abonnements et les ressources dans le cadre du plan Azure</span><span class="sxs-lookup"><span data-stu-id="4ae42-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
