---
title: Configurer vos utilisateurs avec l’authentification multifacteur
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Apprenez à configurer vos employés avec l’authentification multifacteur
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182373"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="1a9df-103">Configurer vos utilisateurs avec l’authentification multifacteur</span><span class="sxs-lookup"><span data-stu-id="1a9df-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="1a9df-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="1a9df-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1a9df-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="1a9df-105">Global admin</span></span>

<span data-ttu-id="1a9df-106">L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités.</span><span class="sxs-lookup"><span data-stu-id="1a9df-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="1a9df-107">Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible.</span><span class="sxs-lookup"><span data-stu-id="1a9df-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="1a9df-108">C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place.</span><span class="sxs-lookup"><span data-stu-id="1a9df-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="1a9df-109">Nous recommandons vivement à tous les partenaires d’activer l’authentification multifacteur (MFA) pour les utilisateurs de leur locataire partenaire.</span><span class="sxs-lookup"><span data-stu-id="1a9df-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="1a9df-110">Ajouter l’authentification multifacteur pour vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1a9df-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="1a9df-111">Pour effectuer cette tâche, vous devez être l’administrateur général de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="1a9df-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="1a9df-112">Il est plus facile d’activer l’authentification multifacteur pour vos utilisateurs quand vous les ajoutez à votre locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1a9df-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="1a9df-113">Connectez-vous au [portail Azure](https://portal.azure.com), puis accédez à **Gestion des utilisateurs**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="1a9df-114">Sélectionnez **Authentification multifacteur**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="1a9df-115">Sélectionnez l’utilisateur que vous souhaitez activer, puis sélectionnez **Activer**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="1a9df-116">Cette opération active l’authentification multifacteur pour cet utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1a9df-116">This will enable MFA for this user.</span></span> <span data-ttu-id="1a9df-117">Quand l’authentification est activée et que l’utilisateur se connecte pour la première fois, il est invité à configurer sa vérification MFA.</span><span class="sxs-lookup"><span data-stu-id="1a9df-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="1a9df-118">Ensuite, à chaque connexion, il lui est demandé de fournir un code qui lui est envoyé par e-mail ou SMS (selon l’option configurée).</span><span class="sxs-lookup"><span data-stu-id="1a9df-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Spécifier le mode de vérification":::

>[!NOTE]
><span data-ttu-id="1a9df-120">Vous pouvez **contraindre** les utilisateurs à utiliser l’authentification multifacteur en suivant les mêmes étapes que celles ci-dessus et en sélectionnant **Appliquer**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="1a9df-121">Pour plus d’informations, consultez [Activer l’authentification multifacteur Azure par utilisateur pour sécuriser les événements de connexion](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="1a9df-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="1a9df-122">Tous les utilisateurs ont initialement l’état  **Désactivé**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-122">All users start out **Disabled**.</span></span> <span data-ttu-id="1a9df-123">Quand vous inscrivez des utilisateurs à Azure Multi-Factor Authentication par utilisateur, leur état passe à  **Activé**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="1a9df-124">Quand les utilisateurs activés se connectent et terminent le processus d’inscription, leur état passe à  **Appliqué**.</span><span class="sxs-lookup"><span data-stu-id="1a9df-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1a9df-125">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="1a9df-125">Next steps</span></span>

- [<span data-ttu-id="1a9df-126">Attribuer des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="1a9df-126">Assign roles and permissions to users</span></span>](permissions-overview.md)