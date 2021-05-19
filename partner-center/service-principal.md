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
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854925"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="1e314-104">Ajouter une application Azure AD (principal de service) dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e314-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="1e314-105">**Rôles appropriés** : administrateur général</span><span class="sxs-lookup"><span data-stu-id="1e314-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="1e314-106">Dans le programme Place de marché commerciale de l’Espace partenaires, vous pouvez désormais ajouter une application Azure AD (principal de service) en tant qu’utilisateur dans votre compte Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="1e314-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="1e314-107">(Vous pouviez le faire précédemment dans votre compte Portail Cloud Partner ou CPP.</span><span class="sxs-lookup"><span data-stu-id="1e314-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="1e314-108">Maintenant que vous avez effectué la migration vers l’Espace partenaires, le compte CPP est en lecture seule.)</span><span class="sxs-lookup"><span data-stu-id="1e314-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="1e314-109">Principal du service et application Azure AD sont synonymes.</span><span class="sxs-lookup"><span data-stu-id="1e314-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="1e314-110">Ajouter une application Azure AD (principal de service)</span><span class="sxs-lookup"><span data-stu-id="1e314-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="1e314-111">Dans le tableau de bord de l’Espace partenaires, sélectionnez **Paramètres**, puis **Paramètres de développeur**.</span><span class="sxs-lookup"><span data-stu-id="1e314-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="1e314-112">Sélectionnez **Utilisateurs**, puis **Ajouter des applications Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="1e314-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="1e314-113">Sélectionnez une application Azure AD existante ou créez-en une.</span><span class="sxs-lookup"><span data-stu-id="1e314-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="1e314-114">Si vous créez une nouvelle application Azure AD, incluez les informations suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e314-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="1e314-115">**URL de réponse** : URL avec laquelle les utilisateurs peuvent se connecter pour utiliser votre application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e314-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="1e314-116">**URI d’ID d’application** : identificateur logique pour l’application Azure AD qui est présenté lors de l’envoi d’une demande d’authentification unique à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e314-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="1e314-117">**Rôles de sécurité** : Les rôles **Responsable** (identique au rôle « Propriétaire » dans le Portail Cloud Partner) et **Développeur** (identique au rôle « Contributeur » dans le Portail Cloud Partner) s’appliquent au programme Place de marché commerciale dans l’Espace partenaires et peuvent être associés à cette application Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e314-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="1e314-118">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1e314-118">Next steps</span></span>

- [<span data-ttu-id="1e314-119">Vue d’ensemble de la place de marché commerciale dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="1e314-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)