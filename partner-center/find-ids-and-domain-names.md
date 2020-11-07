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
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360069"
---
# <a name="locate-important-ids-for-a-user"></a>Localiser des ID importants pour un utilisateur

Cet article explique comment utiliser le [portail Azure](https://portal.azure.com/) pour localiser les informations suivantes pour un utilisateur :

- ID de locataire Microsoft Azure Active Directory (Azure AD) de l’organisation ou de l’entreprise de l’utilisateur

- Nom de domaine principal de l’organisation ou de la société associée au locataire Azure AD

- ID de l’objet utilisateur

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Rechercher l’ID de locataire Microsoft Azure AD et le nom de domaine principal

Procédez comme suit pour Rechercher l’ID de locataire Azure AD ou le nom de domaine principal au sein du Portail Azure. (Si vous souhaitez rechercher un ID de locataire par programme, consultez Rechercher l' [ID de locataire avec PowerShell ou l’interface CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)

> [!NOTE]
> L’ID de locataire peut être appelé des noms différents dans des applications ou des ressources différentes. Par exemple, l’ID de locataire peut être appelé ID de répertoire, client Azure Active Directory (Azure AD), ID Microsoft ou pour certains rapports, même *tenantguid*.

1. Connectez-vous au [portail Azure](https://portal.azure.com/).

2. Dans le menu, sélectionnez **Azure Active Directory**.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Affiche Portail Azure sélectionnant l’option Azure Active Directory dans le menu.":::

3. Une page de **présentation** Azure Active Directory s’affiche. Pour trouver l’ID de locataire Azure AD ou le nom de domaine principal, recherchez le champ **ID de locataire** et le champ **domaine principal** . Ces champs s’affichent dans la section informations sur le locataire.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Affiche la page de vue d’ensemble avec deux champs en surbrillance, l’ID de locataire et le nom de domaine principal.":::

4. Vous pouvez trouver l’ID de locataire dans le Portail Azure de plusieurs façons. Dans le menu, sélectionnez **Azure Active Directory**. Recherchez ensuite la section **gérer** dans le menu et sélectionnez **Propriétés**.

   La page Propriétés affiche également l’ID de locataire associé à l’utilisateur.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Affiche la page Propriétés avec le champ ID de locataire en surbrillance.":::

## <a name="find-the-user-object-id"></a>Rechercher l’ID d’objet utilisateur

Il se peut que la recherche du nom de domaine et de l’ID de locataire ne soit pas toujours suffisante. Vous devrez peut-être également Rechercher l’ID d’objet spécifique affecté à un utilisateur. Procédez comme suit pour Rechercher l’ID d’objet d’un utilisateur dans la Portail Azure :

1. Connectez-vous au [portail Azure](https://portal.azure.com/).

2. Dans le menu, sélectionnez **Azure Active Directory**.

3. Recherchez la section **gérer** dans le menu, puis sélectionnez **utilisateurs**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Affiche Azure Active Directory menu avec l’option utilisateurs en surbrillance.":::

4. Dans la page utilisateurs, tapez le nom de l’utilisateur dans la zone de recherche.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Affiche la page utilisateurs avec la zone de recherche pour rechercher un utilisateur spécifique.":::

5. Sélectionnez le nom de l’utilisateur où il apparaît dans la liste.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Affiche la page utilisateur affichant une ligne pour l’utilisateur recherché.":::

6. Recherchez la section identité sur la page de profil de l’utilisateur. Le champ ID de l’objet s’affiche avec l’ID d’objet unique de l’utilisateur.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Affiche la page de profil utilisateur avec la section d’identité et un champ en surbrillance pour l’ID d’objet.":::

## <a name="next-steps"></a>Étapes suivantes

- [Rechercher votre ID de locataire par programmation avec PowerShell ou l’interface CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [En savoir plus sur les profils utilisateur dans Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Découvrez comment les partenaires peuvent voir ou exporter les détails des clients dans l’espace partenaires](see-your-customer-list.md)
