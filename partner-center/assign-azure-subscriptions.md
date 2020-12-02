---
title: Affecter des abonnements Azure à des clients
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment affecter des abonnements Azure à vos clients dans l’espace partenaires et comment permettre aux clients de gérer leurs propres abonnements.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473949"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="fcce7-103">Affectation d’abonnements Azure à des clients dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="fcce7-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="fcce7-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="fcce7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fcce7-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="fcce7-105">Global admin</span></span>
- <span data-ttu-id="fcce7-106">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="fcce7-106">Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="fcce7-107">Affecter des abonnements Azure à vos clients</span><span class="sxs-lookup"><span data-stu-id="fcce7-107">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="fcce7-108">Sélectionnez **clients** dans le menu de l' **espace partenaires** et recherchez le client que vous souhaitez gérer.</span><span class="sxs-lookup"><span data-stu-id="fcce7-108">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="fcce7-109">Sélectionnez la flèche vers le bas à la fin de la ligne pour développer l’enregistrement du client, puis sélectionnez **portail de gestion Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="fcce7-109">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="fcce7-110">Vous serez redirigé vers le [portail Azure](https://portal.azure.com/) dans lequel vous pouvez gérer les abonnements du client.</span><span class="sxs-lookup"><span data-stu-id="fcce7-110">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="fcce7-111">Dans le Portail Azure, sélectionnez **abonnements**.</span><span class="sxs-lookup"><span data-stu-id="fcce7-111">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="fcce7-112">Sélectionnez l’abonnement que vous souhaitez affecter, puis sélectionnez **Access Control**.</span><span class="sxs-lookup"><span data-stu-id="fcce7-112">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="fcce7-113">Sélectionnez **Ajouter** pour ajouter un utilisateur à l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="fcce7-113">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="fcce7-114">Après avoir ajouté l’utilisateur à l’abonnement, vous pouvez attribuer à l’utilisateur un rôle et le compte spécifique auquel l’utilisateur aura accès.</span><span class="sxs-lookup"><span data-stu-id="fcce7-114">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="fcce7-115">Autoriser les clients à gérer leurs abonnements Windows Azure</span><span class="sxs-lookup"><span data-stu-id="fcce7-115">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="fcce7-116">Après avoir créé un abonnement Microsoft Azure pour un client, vous pouvez lui permettre de gérer son abonnement.</span><span class="sxs-lookup"><span data-stu-id="fcce7-116">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="fcce7-117">Pour ce faire, vous devez vous connecter au portail de gestion Microsoft Azure du client.</span><span class="sxs-lookup"><span data-stu-id="fcce7-117">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="fcce7-118">Pour ouvrir le Portail Azure du client, développez la liste des clients dans votre liste de clients ou sélectionnez le nom du client, puis sélectionnez **portail de gestion Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="fcce7-118">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="fcce7-119">Si vous êtes invité à vous connecter au Portail Azure, vous ne disposez peut-être pas de privilèges d’administrateur délégués.</span><span class="sxs-lookup"><span data-stu-id="fcce7-119">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="fcce7-120">Sélectionnez **Demander une relation** pour inviter le client à vous identifier comme son partenaire de référence.</span><span class="sxs-lookup"><span data-stu-id="fcce7-120">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="fcce7-121">Une fois que le client a accepté votre invitation, vous vous voyez automatiquement attribuer des privilèges d'administration délégués.</span><span class="sxs-lookup"><span data-stu-id="fcce7-121">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="fcce7-122">Dans la Portail Azure, ouvrez la liste abonnements du client et sélectionnez l’abonnement Azure du client.</span><span class="sxs-lookup"><span data-stu-id="fcce7-122">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="fcce7-123">Attribuez un rôle à l’un des utilisateurs du client afin qu’il puisse créer et gérer des ressources dans le cadre de son abonnement.</span><span class="sxs-lookup"><span data-stu-id="fcce7-123">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fcce7-124">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="fcce7-124">Next steps</span></span>

- [<span data-ttu-id="fcce7-125">Comment les partenaires CSP peuvent vendre des abonnements aux clients</span><span class="sxs-lookup"><span data-stu-id="fcce7-125">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="fcce7-126">Comment obtenir des autorisations pour gérer le service ou les abonnements d’un client</span><span class="sxs-lookup"><span data-stu-id="fcce7-126">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
