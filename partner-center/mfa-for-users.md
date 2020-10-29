---
title: Configurer vos utilisateurs avec l’authentification multifacteur
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Apprenez à configurer vos employés avec l’authentification multifacteur
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526001"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="e7a50-103">Configurer vos utilisateurs avec l’authentification multifacteur</span><span class="sxs-lookup"><span data-stu-id="e7a50-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="e7a50-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="e7a50-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e7a50-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e7a50-105">Global admin</span></span>

<span data-ttu-id="e7a50-106">L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités.</span><span class="sxs-lookup"><span data-stu-id="e7a50-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="e7a50-107">Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible.</span><span class="sxs-lookup"><span data-stu-id="e7a50-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="e7a50-108">C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place.</span><span class="sxs-lookup"><span data-stu-id="e7a50-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="e7a50-109">Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="e7a50-109">To help safeguard partners and customers, we are introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="e7a50-110">Les partenaires sont tenus d’appliquer l’authentification multifacteur (MFA) à tous les comptes d’utilisateur de leur locataire de partenaire.</span><span class="sxs-lookup"><span data-stu-id="e7a50-110">Partners are required to enforce multi-factor authentication (MFA) for all user accounts in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="e7a50-111">Ajouter l’authentification multifacteur pour vos utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e7a50-111">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="e7a50-112">Pour effectuer cette tâche, vous devez être l’administrateur général de votre entreprise.</span><span class="sxs-lookup"><span data-stu-id="e7a50-112">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="e7a50-113">Il est plus facile d’activer l’authentification multifacteur pour vos utilisateurs quand vous les ajoutez à votre locataire Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e7a50-113">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="e7a50-114">Connectez-vous au [portail Azure](https://portal.azure.com), puis accédez à **Gestion des utilisateurs** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-114">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management** .</span></span>
1. <span data-ttu-id="e7a50-115">Sélectionnez **Authentification multifacteur** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-115">Select **Multi-factor authentication** .</span></span>
1. <span data-ttu-id="e7a50-116">Sélectionnez l’utilisateur que vous souhaitez activer, puis sélectionnez **Activer** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-116">Select the user you want to enable and then select **Enable** .</span></span>

<span data-ttu-id="e7a50-117">Cette opération active l’authentification multifacteur pour cet utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e7a50-117">This will enable MFA for this user.</span></span> <span data-ttu-id="e7a50-118">Quand l’authentification est activée et que l’utilisateur se connecte pour la première fois, il est invité à configurer sa vérification MFA.</span><span class="sxs-lookup"><span data-stu-id="e7a50-118">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="e7a50-119">Ensuite, à chaque connexion, il lui est demandé de fournir un code qui lui est envoyé par e-mail ou SMS.</span><span class="sxs-lookup"><span data-stu-id="e7a50-119">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message.</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Spécifier le mode de vérification":::

<span data-ttu-id="e7a50-121">Pour forcer les utilisateurs à utiliser l’authentification multifacteur, suivez les mêmes étapes que ci-dessus et choisissez l’option **Appliquer** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-121">To force users to use MFA, you can **Enforce** using same steps as above and selecting **Enforce** .</span></span> <span data-ttu-id="e7a50-122">Pour plus d’informations, consultez [activer Azure Multi-Factor Authentication par utilisateur pour sécuriser les événements de connexion](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="e7a50-122">Learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="e7a50-123">Tous les utilisateurs ont initialement l’état  **Désactivé** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-123">All users start out **Disabled** .</span></span> <span data-ttu-id="e7a50-124">Quand vous inscrivez des utilisateurs à Azure Multi-Factor Authentication par utilisateur, leur état passe à  **Activé** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-124">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled** .</span></span> <span data-ttu-id="e7a50-125">Quand les utilisateurs activés se connectent et terminent le processus d’inscription, leur état passe à  **Appliqué** .</span><span class="sxs-lookup"><span data-stu-id="e7a50-125">When enabled users sign in and complete the registration process, their state changes to **Enforced** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e7a50-126">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="e7a50-126">Next steps</span></span>

- [<span data-ttu-id="e7a50-127">Attribuer des rôles et des autorisations aux utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e7a50-127">Assign roles and permissions to users</span></span>](permissions-overview.md)



