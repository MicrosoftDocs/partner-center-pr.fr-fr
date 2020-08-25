---
title: Ajouter des locataires supplémentaires à votre compte espace partenaires
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gérer plusieurs locataires via votre compte espace partenaires
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846955"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="0ada5-103">Ajouter et gérer plusieurs locataires dans votre compte espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0ada5-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="0ada5-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="0ada5-104">**Applies to**</span></span>

- <span data-ttu-id="0ada5-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0ada5-105">Partner Center</span></span>

<span data-ttu-id="0ada5-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="0ada5-106">**Appropriate roles**</span></span>

- <span data-ttu-id="0ada5-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="0ada5-107">Global admin</span></span>

<span data-ttu-id="0ada5-108">Cette fonctionnalité vous permet de gérer plusieurs locataires pour votre entreprise et de les consolider dans votre compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="0ada5-109">Il existe de nombreuses raisons pour lesquelles vous devrez peut-être gérer plusieurs Azure AD locataires dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="0ada5-110">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="0ada5-110">For example:</span></span>

- <span data-ttu-id="0ada5-111">Votre entreprise peut acheter une autre société et vous souhaitez que les employés de la nouvelle société puissent utiliser l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="0ada5-112">Toutefois, vous souhaitez que les deux sociétés restent séparées.</span><span class="sxs-lookup"><span data-stu-id="0ada5-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="0ada5-113">Dans ce cas, vous associez le locataire Azure AD de la nouvelle société à votre compte global de partenaire (PGA).</span><span class="sxs-lookup"><span data-stu-id="0ada5-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="0ada5-114">Cette association permettrait aux utilisateurs des deux entreprises de travailler dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="0ada5-115">Si vous avez plusieurs locataires pour l’exécution de votre entreprise (par exemple, contoso.com, contoso.uk, contoso.in), vous pouvez utiliser une architecture mutualisée pour les relier sous le même compte d’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="0ada5-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="0ada5-116">Les fusions et les acquisitions nécessitent que vous utilisiez plusieurs locataires (par exemple, si contoso acquiert Fabrikam, vous devez être en mesure d’utiliser à la fois les locataires respectifs Constoso.com et Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="0ada5-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="0ada5-117">Les utilisateurs de l’un des locataires doivent être en mesure d’effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="0ada5-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="0ada5-118">Accéder au centre des partenaires pour la formation, les téléchargements numériques, l’Association MCP</span><span class="sxs-lookup"><span data-stu-id="0ada5-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="0ada5-119">Être affecté à des rôles de l’espace partenaires comme un administrateur MPN, un administrateur d’incentives, etc.</span><span class="sxs-lookup"><span data-stu-id="0ada5-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="0ada5-120">Ajouter un autre Azure AD locataire à votre compte</span><span class="sxs-lookup"><span data-stu-id="0ada5-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="0ada5-121">En tant qu’administrateur général, connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="0ada5-122">À partir de l’icône **paramètres** , sélectionnez **paramètres du compte** , puis sélectionnez **locataires**.</span><span class="sxs-lookup"><span data-stu-id="0ada5-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associer des locataires"::: 

3. <span data-ttu-id="0ada5-124">Sélectionnez **associer un autre locataire Active Directory** et indiquez le locataire que vous souhaitez associer.</span><span class="sxs-lookup"><span data-stu-id="0ada5-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="0ada5-125">En tant qu’administrateur général, connectez-vous au locataire que vous souhaitez associer et confirmez l’Association.</span><span class="sxs-lookup"><span data-stu-id="0ada5-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmer l’Association des locataires"::: 

5. <span data-ttu-id="0ada5-127">Une fois que vous avez confirmé, vous verrez un avis **défini** .</span><span class="sxs-lookup"><span data-stu-id="0ada5-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="0ada5-128">Sélectionnez **revenir à la gestion des locataires pour** Voir le locataire qui vient d’être ajouté.</span><span class="sxs-lookup"><span data-stu-id="0ada5-128">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="0ada5-129">Vous ne pouvez pas associer un locataire à un compte s’il est déjà associé à un autre compte de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0ada5-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="0ada5-130">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0ada5-130">Next steps</span></span>

- [<span data-ttu-id="0ada5-131">Ajout d'utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0ada5-131">Add users</span></span>](create-user-accounts-and-set-permissions.md)
