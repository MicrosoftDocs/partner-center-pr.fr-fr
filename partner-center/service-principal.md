---
title: Principal de service Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment ajouter un principal de service à votre locataire Azure AD. Cela revient à ajouter une application Azure AD (principal de service) dans l’Espace partenaires.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, plan Azure, principal de service, application Azure AD
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 76a65cd824c7c1af5242bea3af6069a466c9fa1c
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425998"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="f8c9f-105">Ajouter une application Azure AD (principal de service) dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="f8c9f-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="f8c9f-106">Dans le programme Place de marché commerciale de l’Espace partenaires, vous pouvez désormais ajouter une application Azure AD (principal de service) en tant qu’utilisateur dans votre compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="f8c9f-107">(Vous pouviez le faire précédemment dans votre compte Portail Cloud Partner ou CPP.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="f8c9f-108">Maintenant que vous avez effectué la migration vers l’Espace partenaires, le compte CPP est en lecture seule.) Notez que principal de service et application Azure AD sont synonymes.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-108">Now that you have migrated to Partner Center, the CPP account is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="f8c9f-109">Ajouter une application Azure AD (principal de service)</span><span class="sxs-lookup"><span data-stu-id="f8c9f-109">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="f8c9f-110">Dans le tableau de bord de l’Espace partenaires, sélectionnez **Paramètres**, puis **Paramètres de développeur**.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-110">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="f8c9f-111">Sélectionnez **Utilisateurs**, puis **Ajouter des applications Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-111">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="f8c9f-112">Sélectionnez une application Azure AD existante ou créez-en une.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-112">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="f8c9f-113">Si vous créez une nouvelle application Azure AD, incluez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="f8c9f-113">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="f8c9f-114">**URL de réponse** : URL avec laquelle les utilisateurs peuvent se connecter pour utiliser votre application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-114">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="f8c9f-115">**URI d’ID d’application** : identificateur logique pour l’application Azure AD qui est présenté lors de l’envoi d’une demande d’authentification unique à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-115">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="f8c9f-116">**Rôles de sécurité** : Les rôles **Responsable** (identique au rôle « Propriétaire » dans le Portail Cloud Partner) et **Développeur** (identique au rôle « Contributeur » dans le Portail Cloud Partner) s’appliquent au programme Place de marché commerciale dans l’Espace partenaires et peuvent être associés à cette application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f8c9f-116">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
