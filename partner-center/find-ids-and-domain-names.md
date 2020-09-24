---
title: Rechercher l’ID de locataire, nom de domaine, ID d’objet utilisateur
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Découvrez comment rechercher des ID dans le Portail Azure : l’ID de locataire Azure AD de l’organisation, le nom de domaine ou l’ID d’objet utilisateur spécifique. Certaines tâches ont besoin de ces informations.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/17/2020
ms.locfileid: "90740388"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="d1dc7-104">Localiser des ID importants pour un utilisateur</span><span class="sxs-lookup"><span data-stu-id="d1dc7-104">Locate important IDs for a user</span></span>

<span data-ttu-id="d1dc7-105">Cet article explique comment utiliser le [portail Azure](https://portal.azure.com/) pour localiser les informations suivantes pour un utilisateur :</span><span class="sxs-lookup"><span data-stu-id="d1dc7-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="d1dc7-106">ID de locataire Microsoft Azure Active Directory (Azure AD) de l’organisation ou de l’entreprise de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d1dc7-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="d1dc7-107">Nom de domaine principal de l’organisation ou de la société associée au locataire Azure AD</span><span class="sxs-lookup"><span data-stu-id="d1dc7-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="d1dc7-108">ID de l’objet utilisateur</span><span class="sxs-lookup"><span data-stu-id="d1dc7-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="d1dc7-109">Rechercher l’ID de locataire Microsoft Azure AD et le nom de domaine principal</span><span class="sxs-lookup"><span data-stu-id="d1dc7-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="d1dc7-110">Procédez comme suit pour Rechercher l’ID de locataire Azure AD ou le nom de domaine principal au sein du Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span>

> [!NOTE]
> <span data-ttu-id="d1dc7-111">L’ID de locataire peut être appelé des noms différents dans des applications ou des ressources différentes.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-111">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="d1dc7-112">Par exemple, l’ID de locataire peut être appelé ID de répertoire, client Azure Active Directory (Azure AD), ID Microsoft ou pour certains rapports, même *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-112">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="d1dc7-113">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d1dc7-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="d1dc7-114">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-114">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Affiche Portail Azure sélectionnant l’option Azure Active Directory dans le menu.":::

3. <span data-ttu-id="d1dc7-116">Une page de **présentation** Azure Active Directory s’affiche.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-116">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="d1dc7-117">Pour trouver l’ID de locataire Azure AD ou le nom de domaine principal, recherchez le champ **ID de locataire** et le champ **domaine principal** .</span><span class="sxs-lookup"><span data-stu-id="d1dc7-117">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="d1dc7-118">Ces champs s’affichent dans la section informations sur le locataire.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-118">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Affiche la page de vue d’ensemble avec deux champs en surbrillance, l’ID de locataire et le nom de domaine principal.":::

4. <span data-ttu-id="d1dc7-120">Vous pouvez trouver l’ID de locataire dans le Portail Azure de plusieurs façons.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-120">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="d1dc7-121">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-121">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="d1dc7-122">Recherchez ensuite la section **gérer** dans le menu et sélectionnez **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-122">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="d1dc7-123">La page Propriétés affiche également l’ID de locataire associé à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-123">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Affiche la page Propriétés avec le champ ID de locataire en surbrillance.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="d1dc7-125">Rechercher l’ID d’objet utilisateur</span><span class="sxs-lookup"><span data-stu-id="d1dc7-125">Find the user object ID</span></span>

<span data-ttu-id="d1dc7-126">Il se peut que la recherche du nom de domaine et de l’ID de locataire ne soit pas toujours suffisante.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-126">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="d1dc7-127">Vous devrez peut-être également Rechercher l’ID d’objet spécifique affecté à un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-127">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="d1dc7-128">Procédez comme suit pour Rechercher l’ID d’objet d’un utilisateur dans la Portail Azure :</span><span class="sxs-lookup"><span data-stu-id="d1dc7-128">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="d1dc7-129">Connectez-vous au [portail Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d1dc7-129">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="d1dc7-130">Dans le menu, sélectionnez **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-130">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="d1dc7-131">Recherchez la section **gérer** dans le menu, puis sélectionnez **utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-131">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Affiche Azure Active Directory menu avec l’option utilisateurs en surbrillance.":::

4. <span data-ttu-id="d1dc7-133">Dans la page utilisateurs, tapez le nom de l’utilisateur dans la zone de recherche.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-133">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Affiche la page utilisateurs avec la zone de recherche pour rechercher un utilisateur spécifique.":::

5. <span data-ttu-id="d1dc7-135">Sélectionnez le nom de l’utilisateur où il apparaît dans la liste.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-135">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Affiche la page utilisateur affichant une ligne pour l’utilisateur recherché.":::

6. <span data-ttu-id="d1dc7-137">Recherchez la section identité sur la page de profil de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-137">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="d1dc7-138">Le champ ID de l’objet s’affiche avec l’ID d’objet unique de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1dc7-138">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Affiche la page de profil utilisateur avec la section d’identité et un champ en surbrillance pour l’ID d’objet.":::

## <a name="next-steps"></a><span data-ttu-id="d1dc7-140">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="d1dc7-140">Next steps</span></span>

- [<span data-ttu-id="d1dc7-141">En savoir plus sur les profils utilisateur dans Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d1dc7-141">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="d1dc7-142">Découvrez comment les partenaires peuvent voir ou exporter les détails des clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d1dc7-142">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)