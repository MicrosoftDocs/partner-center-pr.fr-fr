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
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="c0d9a-103">Ajouter et gérer plusieurs locataires dans votre compte espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c0d9a-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="c0d9a-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="c0d9a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c0d9a-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="c0d9a-105">Global admin</span></span>
- <span data-ttu-id="c0d9a-106">Administrateur des comptes</span><span class="sxs-lookup"><span data-stu-id="c0d9a-106">Account admin</span></span>

<span data-ttu-id="c0d9a-107">Cet article explique comment consolider plusieurs clients de Azure Active Directory (Azure AD) pour votre société, puis les ajouter et les gérer dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="c0d9a-108">Il y a de nombreuses raisons à cela.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-108">There are many reasons to do so.</span></span> <span data-ttu-id="c0d9a-109">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="c0d9a-109">For example:</span></span>

- <span data-ttu-id="c0d9a-110">Supposons que votre entreprise, contoso, a acquis une autre société, fabrikam.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="c0d9a-111">Vous souhaitez que les deux sociétés restent distinctes, mais que vous souhaitiez que les nouveaux employés puissent utiliser l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="c0d9a-112">Dans ce cas, vous associez le client Azure AD de la nouvelle société à votre compte global de partenaire (PGA).</span><span class="sxs-lookup"><span data-stu-id="c0d9a-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="c0d9a-113">Cette association permet aux utilisateurs des deux sociétés de travailler dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="c0d9a-114">Si vous exécutez votre activité avec plusieurs locataires (par exemple, *contoso.com*, *contoso.uk* et *contoso.in*), vous pouvez utiliser l’architecture mutualisée pour les regrouper dans le même compte d’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="c0d9a-115">Si les fusions et les instructions d’acquisition nécessitent que vous utilisiez les locataires des deux sociétés, vous devez utiliser les locataires *constoso.com* et *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="c0d9a-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="c0d9a-116">Les utilisateurs de l’un des locataires doivent être en mesure d’effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="c0d9a-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="c0d9a-117">Accédez à l’espace partenaires pour la formation, les téléchargements numériques ou l’Association MCP (Microsoft Certified Professional).</span><span class="sxs-lookup"><span data-stu-id="c0d9a-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="c0d9a-118">Être affecté à des rôles de l’espace partenaires, tels que l’administrateur Microsoft Partner Network (MPN) ou l’administrateur d’incentives.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="c0d9a-119">Ajouter un locataire Azure AD à votre compte</span><span class="sxs-lookup"><span data-stu-id="c0d9a-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="c0d9a-120">Connectez-vous en tant qu’administrateur général à [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c0d9a-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="c0d9a-121">Dans l’angle supérieur droit, sélectionnez **paramètres**, sélectionnez **paramètres du compte**, puis sélectionnez **locataires**.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Capture d’écran du bouton associer dans le volet Azure AD profil."::: 

1. <span data-ttu-id="c0d9a-123">Sélectionnez **associer**, puis indiquez le locataire que vous souhaitez associer.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="c0d9a-124">À l’invite, connectez-vous en tant qu’administrateur général au locataire que vous souhaitez associer, puis sélectionnez **confirmer**.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Capture d’écran du bouton confirmer du volet confirmer la nouvelle Azure AD Association."::: 

   <span data-ttu-id="c0d9a-126">Une fois l’Association confirmée, un message **Set All** s’affiche.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="c0d9a-127">Pour afficher le locataire qui vient d’être ajouté, sélectionnez **revenir à la gestion des locataires**.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="c0d9a-128">Vous ne pouvez pas associer un locataire à un compte s’il est déjà associé à un autre compte de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="c0d9a-129">Supprimer un locataire de votre compte</span><span class="sxs-lookup"><span data-stu-id="c0d9a-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="c0d9a-130">Connectez-vous en tant qu’administrateur général à [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c0d9a-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="c0d9a-131">Dans l’angle supérieur droit, sélectionnez l’icône des **paramètres** , puis sélectionnez **paramètres du compte**.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="c0d9a-132">Dans le volet gauche, sélectionnez **locataires**.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="c0d9a-133">Sous **gérer les locataires Azure ad**, sélectionnez l’onglet **partenaire** .</span><span class="sxs-lookup"><span data-stu-id="c0d9a-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="c0d9a-134">Sélectionnez **supprimer** en regard du locataire dont vous souhaitez supprimer l’Association.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Capture d’écran des associations de locataire actuelles et de leurs liens de suppression.":::

   <span data-ttu-id="c0d9a-136">Comme indiqué dans la capture d’écran précédente, les liens **supprimer** sont activés pour tous les locataires associés, à l’exception du locataire principal et du locataire auquel vous êtes actuellement connecté.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="c0d9a-137">Lorsque vous supprimez un locataire, les utilisateurs de ce locataire n’ont plus accès au compte de l’espace partenaires et la suppression peut avoir un impact sur vos compétences.</span><span class="sxs-lookup"><span data-stu-id="c0d9a-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c0d9a-138">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c0d9a-138">Next steps</span></span>

- [<span data-ttu-id="c0d9a-139">Créer des comptes d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c0d9a-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






