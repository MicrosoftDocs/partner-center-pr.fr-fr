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
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315845"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="b176b-103">Rétablir les privilèges d’administrateur pour les abonnements Azure CSP d’un client</span><span class="sxs-lookup"><span data-stu-id="b176b-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="b176b-104">**Rôles applicables**</span><span class="sxs-lookup"><span data-stu-id="b176b-104">**Applicable roles**</span></span>

- <span data-ttu-id="b176b-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="b176b-105">Global admin</span></span>
- <span data-ttu-id="b176b-106">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="b176b-106">Admin agent</span></span>

<span data-ttu-id="b176b-107">En tant que partenaire CSP, vos clients pensent souvent que vous allez gérer leur utilisation d’Azure et leurs systèmes pour eux.</span><span class="sxs-lookup"><span data-stu-id="b176b-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="b176b-108">Pour ce faire, vous devez disposer de privilèges d’administrateur.</span><span class="sxs-lookup"><span data-stu-id="b176b-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="b176b-109">Certains privilèges sont accordés quand votre relation de revendeur avec le client est établie.</span><span class="sxs-lookup"><span data-stu-id="b176b-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="b176b-110">D’autres vous sont octroyés par votre client.</span><span class="sxs-lookup"><span data-stu-id="b176b-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="b176b-111">Privilèges d’administrateur pour Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="b176b-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="b176b-112">Il existe deux niveaux de privilèges d’administrateur pour Azure dans CSP.</span><span class="sxs-lookup"><span data-stu-id="b176b-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="b176b-113">**Privilèges d’administrateur au niveau du locataire** (**privilèges d’administrateur délégués**) : les partenaires CSP obtiennent ces privilèges quand une relation est établie entre le revendeur CSP et les clients.</span><span class="sxs-lookup"><span data-stu-id="b176b-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="b176b-114">Les privilèges d’administrateur délégués donnent aux partenaires CSP un accès aux locataires de leurs clients, ce qui leur permet d’effectuer des fonctions d’administration telles que l’ajout/la gestion d’utilisateurs, la réinitialisation des mots de passe et la gestion des licences utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b176b-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="b176b-115">**Privilèges d’administrateur au niveau de l’abonnement** : les partenaires CSP obtiennent ces privilèges durant la création d’abonnements Azure CSP pour leurs clients.</span><span class="sxs-lookup"><span data-stu-id="b176b-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="b176b-116">Avec ces privilèges, les partenaires CSP ont un accès complet à ces abonnements, ce qui leur permet de provisionner et de gérer des ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="b176b-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="b176b-117">Rétablir les privilèges d’administrateur des partenaires CSP</span><span class="sxs-lookup"><span data-stu-id="b176b-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="b176b-118">Votre client peut recréer l’attribution de rôle CSP tant que vous fournissez l’ID d’objet du groupe AdminAgents à votre client.</span><span class="sxs-lookup"><span data-stu-id="b176b-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="b176b-119">Pour récupérer des privilèges d’administrateur délégués, vous devez travailler avec votre client.</span><span class="sxs-lookup"><span data-stu-id="b176b-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="b176b-120">Connectez-vous au tableau de bord de l’Espace partenaires, puis sélectionnez **Clients** dans le menu de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="b176b-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="b176b-121">Sélectionnez le client avec lequel vous travaillez et **demandez une relation de revendeur.**</span><span class="sxs-lookup"><span data-stu-id="b176b-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="b176b-122">Cela génère un lien vers le client disposant des droits d’administrateur de locataire.</span><span class="sxs-lookup"><span data-stu-id="b176b-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="b176b-123">Ce client doit sélectionner le lien et approuver la demande de relation de revendeur.</span><span class="sxs-lookup"><span data-stu-id="b176b-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemple d’e-mail de la création d’une relation de revendeur":::

4. <span data-ttu-id="b176b-125">Vous, le partenaire, devez vous connecter au locataire partenaire pour récupérer l’ID d’objet du groupe AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="b176b-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="b176b-126">Votre client, qui a le rôle **de propriétaire ou d’administrateur de l’accès utilisateur** et qui a l’autorisation de créer une attribution de rôle au niveau de l’abonnement, effectue les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="b176b-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="b176b-127">Se connecte au locataire où l’abonnement CSP existe.</span><span class="sxs-lookup"><span data-stu-id="b176b-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="b176b-128">Se connecte à l’abonnement (applicable uniquement si l’utilisateur dispose d’autorisations d’attribution de rôle sur plusieurs abonnements dans le locataire).</span><span class="sxs-lookup"><span data-stu-id="b176b-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="b176b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="b176b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="b176b-130">Crée l’attribution de rôle.</span><span class="sxs-lookup"><span data-stu-id="b176b-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="b176b-131">Si vous souhaitez accorder l’autorisation de rôle propriétaire au niveau du groupe de ressources ou de la ressource et non au niveau de l’étendue de l’abonnement, les commandes suivantes peuvent fonctionner :</span><span class="sxs-lookup"><span data-stu-id="b176b-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="b176b-132">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="b176b-132">Next steps</span></span>

- [<span data-ttu-id="b176b-133">Gérer les abonnements et les ressources dans le cadre du plan Azure</span><span class="sxs-lookup"><span data-stu-id="b176b-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
