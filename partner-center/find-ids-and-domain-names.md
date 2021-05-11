---
title: Rechercher l’ID de locataire, nom de domaine, ID d’objet utilisateur
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Découvrez comment rechercher des ID dans le Portail Azure : l’ID de locataire Azure AD de l’organisation, le nom de domaine ou l’ID d’objet utilisateur spécifique. Certaines tâches ont besoin de ces informations.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740282"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="bdb14-104">Localiser des ID importants pour un utilisateur</span><span class="sxs-lookup"><span data-stu-id="bdb14-104">Locate important IDs for a user</span></span>

<span data-ttu-id="bdb14-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="bdb14-105">**Appropriate roles**</span></span>

- <span data-ttu-id="bdb14-106">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="bdb14-106">Global admin</span></span>

<span data-ttu-id="bdb14-107">Cet article explique comment utiliser le [portail Azure](https://portal.azure.com/) pour localiser les informations suivantes pour un utilisateur :</span><span class="sxs-lookup"><span data-stu-id="bdb14-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="bdb14-108">ID de locataire Microsoft Azure Active Directory (Azure AD) de l’organisation ou de l’entreprise de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="bdb14-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="bdb14-109">Nom de domaine principal de l’organisation ou de la société associée au locataire Azure AD</span><span class="sxs-lookup"><span data-stu-id="bdb14-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="bdb14-110">ID de l’objet utilisateur</span><span class="sxs-lookup"><span data-stu-id="bdb14-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="bdb14-111">Rechercher l’ID de locataire Microsoft Azure AD et le nom de domaine principal</span><span class="sxs-lookup"><span data-stu-id="bdb14-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="bdb14-112">Procédez comme suit pour Rechercher l’ID de locataire Azure AD ou le nom de domaine principal au sein du Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="bdb14-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="bdb14-113">(Si vous souhaitez rechercher un ID de locataire par programme, consultez Rechercher l' [ID de locataire avec PowerShell ou l’interface CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="bdb14-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="bdb14-114">L’ID de locataire peut être appelé des noms différents dans des applications ou des ressources différentes.</span><span class="sxs-lookup"><span data-stu-id="bdb14-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="bdb14-115">Par exemple, l’ID de locataire peut être appelé ID de répertoire, client Azure Active Directory (Azure AD), ID Microsoft ou pour certains rapports, même *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="bdb14-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="bdb14-116">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="bdb14-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="bdb14-117">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="bdb14-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Affiche Portail Azure sélectionnant l’option Azure Active Directory dans le menu.":::

3. <span data-ttu-id="bdb14-119">Une page de **présentation** Azure Active Directory s’affiche.</span><span class="sxs-lookup"><span data-stu-id="bdb14-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="bdb14-120">Pour trouver l’ID de locataire Azure AD ou le nom de domaine principal, recherchez le champ **ID de locataire** et le champ **domaine principal** .</span><span class="sxs-lookup"><span data-stu-id="bdb14-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="bdb14-121">Ces champs s’affichent dans la section informations sur le locataire.</span><span class="sxs-lookup"><span data-stu-id="bdb14-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Affiche la page de vue d’ensemble avec deux champs en surbrillance, l’ID de locataire et le nom de domaine principal.":::

4. <span data-ttu-id="bdb14-123">Vous pouvez trouver l’ID de locataire dans le Portail Azure de plusieurs façons.</span><span class="sxs-lookup"><span data-stu-id="bdb14-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="bdb14-124">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="bdb14-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="bdb14-125">Recherchez ensuite la section **gérer** dans le menu et sélectionnez **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="bdb14-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="bdb14-126">La page Propriétés affiche également l’ID de locataire associé à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bdb14-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Affiche la page Propriétés avec le champ ID de locataire en surbrillance.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="bdb14-128">Rechercher l’ID d’objet utilisateur</span><span class="sxs-lookup"><span data-stu-id="bdb14-128">Find the user object ID</span></span>

<span data-ttu-id="bdb14-129">Il se peut que la recherche du nom de domaine et de l’ID de locataire ne soit pas toujours suffisante.</span><span class="sxs-lookup"><span data-stu-id="bdb14-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="bdb14-130">Vous devrez peut-être également Rechercher l’ID d’objet spécifique affecté à un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bdb14-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="bdb14-131">Procédez comme suit pour Rechercher l’ID d’objet d’un utilisateur dans la Portail Azure :</span><span class="sxs-lookup"><span data-stu-id="bdb14-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="bdb14-132">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="bdb14-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="bdb14-133">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="bdb14-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="bdb14-134">Recherchez la section **gérer** dans le menu, puis sélectionnez **utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="bdb14-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Affiche Azure Active Directory menu avec l’option utilisateurs en surbrillance.":::

4. <span data-ttu-id="bdb14-136">Dans la page utilisateurs, tapez le nom de l’utilisateur dans la zone de recherche.</span><span class="sxs-lookup"><span data-stu-id="bdb14-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Affiche la page utilisateurs avec la zone de recherche pour rechercher un utilisateur spécifique.":::

5. <span data-ttu-id="bdb14-138">Sélectionnez le nom de l’utilisateur où il apparaît dans la liste.</span><span class="sxs-lookup"><span data-stu-id="bdb14-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Affiche la page utilisateur affichant une ligne pour l’utilisateur recherché.":::

6. <span data-ttu-id="bdb14-140">Recherchez la section identité sur la page de profil de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bdb14-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="bdb14-141">Le champ ID de l’objet s’affiche avec l’ID d’objet unique de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bdb14-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Affiche la page de profil utilisateur avec la section d’identité et un champ en surbrillance pour l’ID d’objet.":::

## <a name="next-steps"></a><span data-ttu-id="bdb14-143">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="bdb14-143">Next steps</span></span>

- [<span data-ttu-id="bdb14-144">Rechercher votre ID de locataire par programmation avec PowerShell ou l’interface CLI</span><span class="sxs-lookup"><span data-stu-id="bdb14-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="bdb14-145">En savoir plus sur les profils utilisateur dans Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bdb14-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="bdb14-146">Découvrez comment les partenaires peuvent voir ou exporter les détails des clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="bdb14-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

