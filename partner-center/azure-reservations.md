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
ms.openlocfilehash: 7f6ca7aa7dddbd9e32690928ee8d48afa5071b14
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/02/2020
ms.locfileid: "89367033"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="878a4-104">Vendez des Microsoft Azure des réservations aux clients à l’aide de l’espace partenaires, des Portail Azure ou des API</span><span class="sxs-lookup"><span data-stu-id="878a4-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="878a4-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="878a4-105">**Applies to**</span></span>

- <span data-ttu-id="878a4-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-106">Partner Center</span></span>
- <span data-ttu-id="878a4-107">Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="878a4-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="878a4-108">Partenaires du programme Fournisseur de solutions Microsoft Cloud</span><span class="sxs-lookup"><span data-stu-id="878a4-108">Partners in the CSP program</span></span>

<span data-ttu-id="878a4-109">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="878a4-109">**Appropriate roles**</span></span>

- <span data-ttu-id="878a4-110">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="878a4-110">Admin agent</span></span>
- <span data-ttu-id="878a4-111">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="878a4-111">Global admin</span></span>
- <span data-ttu-id="878a4-112">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="878a4-112">Helpdesk agent</span></span>
- <span data-ttu-id="878a4-113">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="878a4-113">Sales agent</span></span>
- <span data-ttu-id="878a4-114">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="878a4-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="878a4-115">Cet article s’applique uniquement aux partenaires du programme fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="878a4-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="878a4-116">Les clients qui utilisent d’autres types d’abonnements (par exemple, paiement à l’utilisation, individuel, contrat de client Microsoft ou abonnements Accord Entreprise) doivent lire [cette documentation Azure reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="878a4-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="878a4-117">Les partenaires du programme CSP peuvent offrir à leurs clients Microsoft Azure des réservations.</span><span class="sxs-lookup"><span data-stu-id="878a4-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="878a4-118">Les clients peuvent gagner des économies importantes lorsqu’ils se réservent à l’avance.</span><span class="sxs-lookup"><span data-stu-id="878a4-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="878a4-119">Les réservations Azure offrent la simplicité et la flexibilité des clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="878a4-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="878a4-120">Conditions de réservation d’une ou trois ans</span><span class="sxs-lookup"><span data-stu-id="878a4-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="878a4-121">Facile à mettre en route ; installation terminée en secondes</span><span class="sxs-lookup"><span data-stu-id="878a4-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="878a4-122">Annuler ou échanger des instances réservées à tout moment pour le remboursement ajusté</span><span class="sxs-lookup"><span data-stu-id="878a4-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="878a4-123">Gérer l’utilisation des instances réservées au niveau de l’organisation ou du service individuel</span><span class="sxs-lookup"><span data-stu-id="878a4-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="878a4-124">Les réservations Azure peuvent être appelées par les clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="878a4-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="878a4-125">Les réservations peuvent offrir des économies considérables par rapport à la tarification du paiement à l’accès (PAYG)</span><span class="sxs-lookup"><span data-stu-id="878a4-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="878a4-126">Meilleure budgétisation et prévisions avec paiement initial pour les périodes d’un ou trois ans</span><span class="sxs-lookup"><span data-stu-id="878a4-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="878a4-127">Hiérarchisation de la capacité de calcul dans la région Azure la plus proche de ses bureaux</span><span class="sxs-lookup"><span data-stu-id="878a4-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="878a4-128">Les réservations Azure fournissent la base des solutions d’infrastructure de bout en bout lorsqu’elles sont associées à des logiciels tels que Microsoft Windows Server et Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="878a4-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="878a4-129">Vous pouvez acheter, vendre et gérer des réservations Azure dans l’espace partenaires et le Portail Azure, et à l’aide de l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="878a4-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="878a4-130">Vous pouvez également accorder à vos clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement Azure que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="878a4-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="878a4-131">Suivez les liens ci-dessous pour en savoir plus.</span><span class="sxs-lookup"><span data-stu-id="878a4-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="878a4-132">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="878a4-132">Azure reservations resources</span></span>

|<span data-ttu-id="878a4-133">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="878a4-133">**For information about**</span></span>   |<span data-ttu-id="878a4-134">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="878a4-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="878a4-135">Documentation sur les réservations Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="878a4-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="878a4-136">Qu’est-ce qu’une réservation Azure ?</span><span class="sxs-lookup"><span data-stu-id="878a4-136">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="878a4-137">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="878a4-138">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="878a4-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="878a4-139">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="878a4-140">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="878a4-141">Détermination de la taille de machine virtuelle correcte et vérification de l’utilisation de la machine virtuelle client</span><span class="sxs-lookup"><span data-stu-id="878a4-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="878a4-142">Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure</span><span class="sxs-lookup"><span data-stu-id="878a4-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="878a4-143">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="878a4-144">[Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="878a4-144">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="878a4-145">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir de votre abonnement CSP.</span><span class="sxs-lookup"><span data-stu-id="878a4-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="878a4-146">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="878a4-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
