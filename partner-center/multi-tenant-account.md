---
title: Ajouter des locataires à votre compte espace partenaires
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter, consolider ou gérer plusieurs locataires Azure AD dans votre compte espace partenaires, et découvrir pourquoi vous pouvez le faire.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124803"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Ajouter et gérer plusieurs locataires dans votre compte espace partenaires


**Rôles appropriés**

- Administrateur général
- Administrateur des comptes

Cet article explique comment consolider plusieurs clients de Azure Active Directory (Azure AD) pour votre société, puis les ajouter et les gérer dans votre compte espace partenaires. Il y a de nombreuses raisons à cela. Par exemple :

- Supposons que votre entreprise, contoso, a acquis une autre société, fabrikam. Vous souhaitez que les deux sociétés restent distinctes, mais que vous souhaitiez que les nouveaux employés puissent utiliser l’espace partenaires. Dans ce cas, vous associez le client Azure AD de la nouvelle société à votre compte global de partenaire (PGA). Cette association permet aux utilisateurs des deux sociétés de travailler dans l’espace partenaires.

- Si vous exécutez votre activité avec plusieurs locataires (par exemple, *contoso.com*, *contoso.uk* et *contoso.in*), vous pouvez utiliser l’architecture mutualisée pour les regrouper dans le même compte d’ordinateur.

- Si les fusions et les instructions d’acquisition nécessitent que vous utilisiez les locataires des deux sociétés, vous devez utiliser les locataires *constoso.com* et *fabrikam.com* .

- Les utilisateurs de l’un des locataires doivent être en mesure d’effectuer les opérations suivantes :
    * Accédez à l’espace partenaires pour la formation, les téléchargements numériques ou l’Association MCP (Microsoft Certified Professional).
    * Être affecté à des rôles de l’espace partenaires, tels que l’administrateur Microsoft Partner Network (MPN) ou l’administrateur d’incentives.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Ajouter un locataire Azure AD à votre compte

1. Connectez-vous en tant qu’administrateur général à [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. Dans l’angle supérieur droit, sélectionnez **paramètres**, sélectionnez **paramètres du compte**, puis sélectionnez **locataires**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Capture d’écran du bouton associer dans le volet Azure AD profil."::: 

1. Sélectionnez **associer**, puis indiquez le locataire que vous souhaitez associer.

1. À l’invite, connectez-vous en tant qu’administrateur général au locataire que vous souhaitez associer, puis sélectionnez **confirmer**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Capture d’écran du bouton confirmer du volet confirmer la nouvelle Azure AD Association."::: 

   Une fois l’Association confirmée, un message **Set All** s’affiche. Pour afficher le locataire qui vient d’être ajouté, sélectionnez **revenir à la gestion des locataires**. 
 
>[!NOTE]
>Vous ne pouvez pas associer un locataire à un compte s’il est déjà associé à un autre compte de l’espace partenaires.


## <a name="remove-a-tenant-from-your-account"></a>Supprimer un locataire de votre compte
 
1. Connectez-vous en tant qu’administrateur général à [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. Dans l’angle supérieur droit, sélectionnez l’icône des **paramètres** , puis sélectionnez **paramètres du compte**.

1. Dans le volet gauche, sélectionnez **locataires**. Sous **gérer les locataires Azure ad**, sélectionnez l’onglet **partenaire** .
 
1. Sélectionnez **supprimer** en regard du locataire dont vous souhaitez supprimer l’Association.

   :::image type="content" source="images/disassociate.png" alt-text="Capture d’écran des associations de locataire actuelles et de leurs liens de suppression.":::

   Comme indiqué dans la capture d’écran précédente, les liens **supprimer** sont activés pour tous les locataires associés, à l’exception du locataire principal et du locataire auquel vous êtes actuellement connecté. 

   > [!NOTE]   
   > Lorsque vous supprimez un locataire, les utilisateurs de ce locataire n’ont plus accès au compte de l’espace partenaires et la suppression peut avoir un impact sur vos compétences. 

## <a name="next-steps"></a>Étapes suivantes

- [Créer des comptes d’utilisateur](create-user-accounts-and-set-permissions.md)






