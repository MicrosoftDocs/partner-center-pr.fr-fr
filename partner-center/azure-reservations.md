---
title: Vendre des clients Microsoft Azure des réservations
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: En tant que fournisseur de solutions Cloud, vous pouvez acheter, vendre ou gérer des réservations Azure pour les clients. Utilisez l’espace partenaires, le Portail Azure ou l’API espace partenaires.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4524d810a036953e45fb94a72241734e02a2798f
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435728"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="3d1c6-104">Vendez des Microsoft Azure des réservations aux clients à l’aide de l’espace partenaires, des Portail Azure ou des API</span><span class="sxs-lookup"><span data-stu-id="3d1c6-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="3d1c6-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="3d1c6-105">**Applies to**</span></span>

- <span data-ttu-id="3d1c6-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-106">Partner Center</span></span>
- <span data-ttu-id="3d1c6-107">Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3d1c6-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="3d1c6-108">Partenaires dans CSP</span><span class="sxs-lookup"><span data-stu-id="3d1c6-108">Partners in CSP</span></span>

<span data-ttu-id="3d1c6-109">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="3d1c6-109">**Appropriate roles**</span></span>

- <span data-ttu-id="3d1c6-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="3d1c6-110">Admin agent</span></span>
- <span data-ttu-id="3d1c6-111">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="3d1c6-111">Global admin</span></span>
- <span data-ttu-id="3d1c6-112">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="3d1c6-112">Helpdesk agent</span></span>
- <span data-ttu-id="3d1c6-113">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="3d1c6-113">Sales agent</span></span>
- <span data-ttu-id="3d1c6-114">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3d1c6-114">User management admin</span></span>

<span data-ttu-id="3d1c6-115">Les partenaires du programme fournisseur de solutions Cloud (CSP) peuvent offrir à leurs clients Microsoft Azure des réservations.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-115">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="3d1c6-116">Les clients peuvent gagner des économies importantes lorsqu’ils se réservent à l’avance.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="3d1c6-117">Les réservations Azure offrent la simplicité et la flexibilité des clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="3d1c6-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="3d1c6-118">Conditions de réservation d’une ou trois ans</span><span class="sxs-lookup"><span data-stu-id="3d1c6-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="3d1c6-119">Facile à mettre en route ; installation terminée en secondes</span><span class="sxs-lookup"><span data-stu-id="3d1c6-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="3d1c6-120">Annuler ou échanger des instances réservées à tout moment pour le remboursement ajusté</span><span class="sxs-lookup"><span data-stu-id="3d1c6-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="3d1c6-121">Gérer l’utilisation des instances réservées au niveau de l’organisation ou du service individuel</span><span class="sxs-lookup"><span data-stu-id="3d1c6-121">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="3d1c6-122">Les réservations Azure peuvent être appelées par les clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="3d1c6-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="3d1c6-123">Les réservations peuvent offrir des économies considérables par rapport à la tarification du paiement à l’accès (PAYG)</span><span class="sxs-lookup"><span data-stu-id="3d1c6-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="3d1c6-124">Meilleure budgétisation et prévisions avec paiement initial pour les périodes d’un ou trois ans</span><span class="sxs-lookup"><span data-stu-id="3d1c6-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="3d1c6-125">Hiérarchisation de la capacité de calcul dans la région Azure la plus proche de ses bureaux</span><span class="sxs-lookup"><span data-stu-id="3d1c6-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="3d1c6-126">Les réservations Azure fournissent la base des solutions d’infrastructure de bout en bout lorsqu’elles sont associées à des logiciels tels que Microsoft Windows Server et Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="3d1c6-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="3d1c6-127">Vous pouvez acheter, vendre et gérer des réservations Azure dans l’espace partenaires et le Portail Azure, et à l’aide de l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="3d1c6-128">Vous pouvez également accorder à vos clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement Azure que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="3d1c6-129">Suivez les liens ci-dessous pour en savoir plus.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="3d1c6-130">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="3d1c6-130">Azure reservations resources</span></span>

|<span data-ttu-id="3d1c6-131">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="3d1c6-131">**For information about**</span></span>   |<span data-ttu-id="3d1c6-132">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="3d1c6-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="3d1c6-133">Documentation sur les réservations Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="3d1c6-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="3d1c6-134">Qu’est-ce qu’une réservation Azure ?</span><span class="sxs-lookup"><span data-stu-id="3d1c6-134">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="3d1c6-135">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="3d1c6-136">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="3d1c6-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3d1c6-137">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="3d1c6-138">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3d1c6-139">Détermination de la taille de machine virtuelle correcte et vérification de l’utilisation de la machine virtuelle client</span><span class="sxs-lookup"><span data-stu-id="3d1c6-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="3d1c6-140">Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure</span><span class="sxs-lookup"><span data-stu-id="3d1c6-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="3d1c6-141">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3d1c6-142">[Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="3d1c6-142">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="3d1c6-143">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir de votre abonnement CSP.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="3d1c6-144">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="3d1c6-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
