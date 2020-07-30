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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389508"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="5e291-103">Ajouter et gérer plusieurs locataires dans votre compte espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5e291-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="5e291-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="5e291-104">**Applies to**</span></span>

- <span data-ttu-id="5e291-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5e291-105">Partner Center</span></span>

<span data-ttu-id="5e291-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="5e291-106">**Appropriate roles**</span></span>

- <span data-ttu-id="5e291-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="5e291-107">Global admin</span></span>

<span data-ttu-id="5e291-108">Il existe de nombreuses raisons pour lesquelles vous devrez peut-être gérer plusieurs Azure AD locataires dans votre compte espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5e291-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="5e291-109">Par exemple, votre entreprise peut acheter une autre société et vous souhaitez que les employés de la nouvelle société puissent utiliser l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5e291-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="5e291-110">Toutefois, vous souhaitez que les deux sociétés restent séparées.</span><span class="sxs-lookup"><span data-stu-id="5e291-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="5e291-111">Dans ce cas, vous associez le locataire de la nouvelle entreprise Azure AD à votre compte global de partenaire (PNG).</span><span class="sxs-lookup"><span data-stu-id="5e291-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="5e291-112">Cette association permettrait aux utilisateurs des deux entreprises de travailler dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5e291-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="5e291-113">Ajouter un autre Azure AD locataire à votre compte</span><span class="sxs-lookup"><span data-stu-id="5e291-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="5e291-114">En tant qu’administrateur général, connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="5e291-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="5e291-115">À partir de l’icône **paramètres** , sélectionnez **paramètres du compte** , puis sélectionnez **locataires**.</span><span class="sxs-lookup"><span data-stu-id="5e291-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="associer des locataires"::: 

3. <span data-ttu-id="5e291-117">Sélectionnez **associer un autre locataire Active Directory** et indiquez le locataire que vous souhaitez associer.</span><span class="sxs-lookup"><span data-stu-id="5e291-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="5e291-118">En tant qu’administrateur général, connectez-vous au locataire que vous souhaitez associer et confirmez l’Association.</span><span class="sxs-lookup"><span data-stu-id="5e291-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="confirmer l’Association des locataires"::: 

5. <span data-ttu-id="5e291-120">Une fois que vous avez confirmé, vous verrez un avis **défini** .</span><span class="sxs-lookup"><span data-stu-id="5e291-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="5e291-121">Sélectionnez **revenir à la gestion des locataires pour** Voir le locataire qui vient d’être ajouté.</span><span class="sxs-lookup"><span data-stu-id="5e291-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="5e291-122">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="5e291-122">Next steps</span></span>

- [<span data-ttu-id="5e291-123">Ajout d'utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5e291-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
