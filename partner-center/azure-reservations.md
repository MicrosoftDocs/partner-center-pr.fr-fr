---
title: Vendre des clients Microsoft Azure des réservations
description: En tant que fournisseur de solutions Cloud, vous pouvez acheter, vendre ou gérer des réservations Azure pour les clients. Utilisez l’espace partenaires, le Portail Azure ou l’API espace partenaires.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534894"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="d78f3-104">Vendez des Microsoft Azure des réservations aux clients à l’aide de l’espace partenaires, des Portail Azure ou des API</span><span class="sxs-lookup"><span data-stu-id="d78f3-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="d78f3-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="d78f3-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d78f3-106">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="d78f3-106">Admin agent</span></span>
- <span data-ttu-id="d78f3-107">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="d78f3-107">Global admin</span></span>
- <span data-ttu-id="d78f3-108">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="d78f3-108">Helpdesk agent</span></span>
- <span data-ttu-id="d78f3-109">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="d78f3-109">Sales agent</span></span>
- <span data-ttu-id="d78f3-110">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d78f3-110">User management admin</span></span>

<span data-ttu-id="d78f3-111">En tant que partenaire dans le programme fournisseur de solutions Cloud (CSP), vous pouvez acheter, vendre ou gérer des réservations Azure pour les clients.</span><span class="sxs-lookup"><span data-stu-id="d78f3-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="d78f3-112">Utilisez l’espace partenaires, le Portail Azure ou l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d78f3-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="d78f3-113">Cet article s’applique uniquement aux partenaires dans CSP.</span><span class="sxs-lookup"><span data-stu-id="d78f3-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="d78f3-114">Les clients qui utilisent d’autres types d’abonnements (par exemple, paiement à l’utilisation, individuel, contrat de client Microsoft ou abonnements Accord Entreprise) doivent lire [cette documentation Azure reservations](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="d78f3-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="d78f3-115">Les partenaires du programme CSP peuvent offrir à leurs clients Microsoft Azure des réservations.</span><span class="sxs-lookup"><span data-stu-id="d78f3-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="d78f3-116">Les clients peuvent gagner des économies importantes lorsqu’ils se réservent à l’avance.</span><span class="sxs-lookup"><span data-stu-id="d78f3-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="d78f3-117">Les réservations Azure offrent la simplicité et la flexibilité des clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="d78f3-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="d78f3-118">Conditions de réservation d’une ou trois ans</span><span class="sxs-lookup"><span data-stu-id="d78f3-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="d78f3-119">Facile à mettre en route ; installation terminée en secondes</span><span class="sxs-lookup"><span data-stu-id="d78f3-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="d78f3-120">Annuler ou échanger des instances réservées à tout moment pour le remboursement ajusté</span><span class="sxs-lookup"><span data-stu-id="d78f3-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="d78f3-121">Gérer l’utilisation des instances réservées au niveau de l’organisation ou du service individuel</span><span class="sxs-lookup"><span data-stu-id="d78f3-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="d78f3-122">Les réservations Azure peuvent être appelées par les clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="d78f3-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="d78f3-123">Les réservations peuvent offrir des économies considérables par rapport à la tarification du paiement à l’accès (PAYG)</span><span class="sxs-lookup"><span data-stu-id="d78f3-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="d78f3-124">Meilleure budgétisation et prévisions avec paiement initial pour les périodes d’un ou trois ans</span><span class="sxs-lookup"><span data-stu-id="d78f3-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="d78f3-125">Hiérarchisation de la capacité de calcul dans la région Azure la plus proche de ses bureaux</span><span class="sxs-lookup"><span data-stu-id="d78f3-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="d78f3-126">Les réservations Azure fournissent la base des solutions d’infrastructure de bout en bout lorsqu’elles sont associées à des logiciels tels que Microsoft Windows Server et Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="d78f3-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="d78f3-127">Vous pouvez acheter, vendre et gérer des réservations Azure dans l’espace partenaires et le Portail Azure, et à l’aide de l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="d78f3-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="d78f3-128">Vous pouvez également accorder à vos clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement Azure que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="d78f3-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="d78f3-129">Suivez les liens ci-dessous pour en savoir plus.</span><span class="sxs-lookup"><span data-stu-id="d78f3-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="d78f3-130">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="d78f3-130">Azure reservations resources</span></span>

|<span data-ttu-id="d78f3-131">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="d78f3-131">**For information about**</span></span>   |<span data-ttu-id="d78f3-132">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="d78f3-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="d78f3-133">Documentation sur les réservations Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="d78f3-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="d78f3-134">Qu’est-ce qu’une réservation Azure ?</span><span class="sxs-lookup"><span data-stu-id="d78f3-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="d78f3-135">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d78f3-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="d78f3-136">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="d78f3-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="d78f3-137">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d78f3-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="d78f3-138">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d78f3-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="d78f3-139">Détermination de la taille de machine virtuelle correcte et vérification de l’utilisation de la machine virtuelle client</span><span class="sxs-lookup"><span data-stu-id="d78f3-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="d78f3-140">Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure</span><span class="sxs-lookup"><span data-stu-id="d78f3-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="d78f3-141">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d78f3-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="d78f3-142">[Acheter Azure reserved VM instances](/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="d78f3-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="d78f3-143">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir de votre abonnement CSP.</span><span class="sxs-lookup"><span data-stu-id="d78f3-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="d78f3-144">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="d78f3-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |