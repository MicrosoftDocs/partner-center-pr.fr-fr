---
title: Ajouter des locataires supplémentaires à votre compte espace partenaires
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter, consolider ou gérer plusieurs locataires Azure AD dans votre compte espace partenaires. En savoir plus sur certaines des raisons pour lesquelles vous pourriez souhaiter le faire.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182429"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Ajouter et gérer plusieurs locataires dans votre compte espace partenaires


**Rôles appropriés**

- Administrateur général
- Administrateur des comptes

Cette fonctionnalité vous permet de gérer plusieurs locataires pour votre entreprise et de les consolider dans votre compte Espace partenaires. Il existe de nombreuses raisons pour lesquelles vous devrez peut-être gérer plusieurs Azure AD locataires dans votre compte espace partenaires. Par exemple :

- Votre entreprise peut acheter une autre société et vous souhaitez que les employés de la nouvelle société puissent utiliser l’espace partenaires. Toutefois, vous souhaitez que les deux sociétés restent séparées. Dans ce cas, vous associez le locataire Azure AD de la nouvelle société à votre compte global de partenaire (PGA). Cette association permettrait aux utilisateurs des deux entreprises de travailler dans l’espace partenaires.

- Si vous avez plusieurs locataires pour l’exécution de votre entreprise (par exemple, contoso.com, contoso.uk, contoso.in), vous pouvez utiliser une architecture mutualisée pour les relier sous le même compte d’ordinateur.

- Les fusions et les acquisitions nécessitent que vous utilisiez plusieurs locataires (par exemple, si contoso acquiert Fabrikam, vous devez être en mesure d’utiliser à la fois les locataires respectifs Constoso.com et Fabrikam.com).

- Les utilisateurs de l’un des locataires doivent être en mesure d’effectuer les opérations suivantes :
    1.  Accéder au centre des partenaires pour la formation, les téléchargements numériques, l’Association MCP
    2.  Être affecté à des rôles de l’espace partenaires comme un administrateur MPN, un administrateur d’incentives, etc.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Ajouter un autre Azure AD locataire à votre compte

1. En tant qu’administrateur général, connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.
1. À partir de l’icône **paramètres** , sélectionnez **paramètres du compte** , puis sélectionnez **locataires**.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associer des locataires"::: 

3. Sélectionnez **associer un autre locataire Active Directory** et indiquez le locataire que vous souhaitez associer.

1. En tant qu’administrateur général, connectez-vous au locataire que vous souhaitez associer et confirmez l’Association. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmer l’Association des locataires"::: 

5. Une fois que vous avez confirmé, vous verrez un avis **défini** .  Sélectionnez **revenir à la gestion des locataires pour** Voir le locataire que vous venez d’ajouter. 
 

>[!NOTE]
>Vous ne pouvez pas associer un locataire à un compte s’il est déjà associé à un autre compte de l’espace partenaires.


## <a name="remove-a-tenant-from-your-account"></a>Supprimer un locataire de votre compte
 
1. En tant qu’administrateur général, connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.

1. À partir de l’icône **paramètres** , sélectionnez **paramètres du compte** -> locataires, puis cliquez sur l’onglet **partenaire** .
 
3. Cliquez sur **supprimer** pour le locataire que vous souhaitez dissocier.

4. La dissociation d’un locataire signifie que les utilisateurs de ce locataire n’auront plus accès au compte de l’espace partenaires, ce qui peut avoir un impact sur vos compétences. 

Le bouton **supprimer** est activé pour tous les locataires associés, à l’exception du locataire principal et du locataire dans lequel vous êtes actuellement connecté.

:::image type="content" source="images/disassociate.png" alt-text="locataires avec le bouton supprimer":::
 

## <a name="next-steps"></a>Étapes suivantes

- [Ajout d'utilisateurs](create-user-accounts-and-set-permissions.md)






