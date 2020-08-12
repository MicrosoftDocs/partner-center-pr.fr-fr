---
title: Principal de service Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter un principal de service à votre locataire Azure AD. Cela revient à ajouter une application Azure AD (principal de service) dans l’Espace partenaires.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811239"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="e6eed-104">Ajouter une application Azure AD (principal de service) dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e6eed-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="e6eed-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="e6eed-105">**Applies to**</span></span>

- <span data-ttu-id="e6eed-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e6eed-106">Partner Center</span></span>

<span data-ttu-id="e6eed-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="e6eed-107">**Appropriate roles**</span></span>

- <span data-ttu-id="e6eed-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e6eed-108">Global admin</span></span>

<span data-ttu-id="e6eed-109">Dans le programme Place de marché commerciale de l’Espace partenaires, vous pouvez désormais ajouter une application Azure AD (principal de service) en tant qu’utilisateur dans votre compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e6eed-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="e6eed-110">(Vous pouviez le faire précédemment dans votre compte Portail Cloud Partner ou CPP.</span><span class="sxs-lookup"><span data-stu-id="e6eed-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="e6eed-111">Maintenant que vous avez effectué la migration vers l’Espace partenaires, le compte CPP est en lecture seule.)</span><span class="sxs-lookup"><span data-stu-id="e6eed-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="e6eed-112">Principal du service et application Azure AD sont synonymes.</span><span class="sxs-lookup"><span data-stu-id="e6eed-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="e6eed-113">Ajouter une application Azure AD (principal de service)</span><span class="sxs-lookup"><span data-stu-id="e6eed-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="e6eed-114">Dans le tableau de bord de l’Espace partenaires, sélectionnez **Paramètres**, puis **Paramètres de développeur**.</span><span class="sxs-lookup"><span data-stu-id="e6eed-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="e6eed-115">Sélectionnez **Utilisateurs**, puis **Ajouter des applications Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="e6eed-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="e6eed-116">Sélectionnez une application Azure AD existante ou créez-en une.</span><span class="sxs-lookup"><span data-stu-id="e6eed-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="e6eed-117">Si vous créez une nouvelle application Azure AD, incluez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="e6eed-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="e6eed-118">**URL de réponse** : URL avec laquelle les utilisateurs peuvent se connecter pour utiliser votre application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6eed-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="e6eed-119">**URI d’ID d’application** : identificateur logique pour l’application Azure AD qui est présenté lors de l’envoi d’une demande d’authentification unique à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6eed-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="e6eed-120">**Rôles de sécurité** : Les rôles **Responsable** (identique au rôle « Propriétaire » dans le Portail Cloud Partner) et **Développeur** (identique au rôle « Contributeur » dans le Portail Cloud Partner) s’appliquent au programme Place de marché commerciale dans l’Espace partenaires et peuvent être associés à cette application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6eed-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e6eed-121">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e6eed-121">Next steps</span></span>

- [<span data-ttu-id="e6eed-122">Vue d’ensemble de la place de marché commerciale dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e6eed-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)