---
title: Vendre des clients Microsoft Azure des réservations
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: En tant que fournisseur de solutions Cloud, vous pouvez acheter, vendre ou gérer des réservations Azure pour les clients. Utilisez l’espace partenaires, le Portail Azure ou l’API espace partenaires.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, réservations, gérer, facturation, achat, Azure RI, instances réservées Azure
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5393e757b209de5a7df22b35a0cee0703419bef4
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198637"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="e314c-105">Vendez des Microsoft Azure des réservations aux clients à l’aide de l’espace partenaires, des Portail Azure ou des API</span><span class="sxs-lookup"><span data-stu-id="e314c-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="e314c-106">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="e314c-106">**Applies to**</span></span>

- <span data-ttu-id="e314c-107">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-107">Partner Center</span></span>
- <span data-ttu-id="e314c-108">Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e314c-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="e314c-109">Partenaires dans CSP</span><span class="sxs-lookup"><span data-stu-id="e314c-109">Partners in CSP</span></span>

<span data-ttu-id="e314c-110">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="e314c-110">**Appropriate roles**</span></span>

- <span data-ttu-id="e314c-111">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="e314c-111">Admin agent</span></span>
- <span data-ttu-id="e314c-112">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="e314c-112">Global admin</span></span>
- <span data-ttu-id="e314c-113">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="e314c-113">Helpdesk agent</span></span>
- <span data-ttu-id="e314c-114">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="e314c-114">Sales agent</span></span>
- <span data-ttu-id="e314c-115">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="e314c-115">User management admin</span></span>

<span data-ttu-id="e314c-116">Les partenaires du programme fournisseur de solutions Cloud (CSP) peuvent offrir à leurs clients Microsoft Azure des réservations.</span><span class="sxs-lookup"><span data-stu-id="e314c-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="e314c-117">Les clients peuvent gagner des économies importantes lorsqu’ils se réservent à l’avance.</span><span class="sxs-lookup"><span data-stu-id="e314c-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="e314c-118">Les réservations Azure offrent la simplicité et la flexibilité des clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="e314c-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="e314c-119">Conditions de réservation d’une ou trois ans</span><span class="sxs-lookup"><span data-stu-id="e314c-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="e314c-120">Facile à mettre en route ; installation terminée en secondes</span><span class="sxs-lookup"><span data-stu-id="e314c-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="e314c-121">Annuler ou échanger des instances réservées à tout moment pour le remboursement ajusté</span><span class="sxs-lookup"><span data-stu-id="e314c-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="e314c-122">Gérer l’utilisation des instances réservées au niveau de l’organisation ou du service individuel</span><span class="sxs-lookup"><span data-stu-id="e314c-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="e314c-123">Les réservations Azure peuvent être appelées par les clients des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="e314c-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="e314c-124">Les réservations peuvent offrir des économies considérables par rapport à la tarification du paiement à l’accès (PAYG)</span><span class="sxs-lookup"><span data-stu-id="e314c-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="e314c-125">Meilleure budgétisation et prévisions avec paiement initial pour les périodes d’un ou trois ans</span><span class="sxs-lookup"><span data-stu-id="e314c-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="e314c-126">Hiérarchisation de la capacité de calcul dans la région Azure la plus proche de ses bureaux</span><span class="sxs-lookup"><span data-stu-id="e314c-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="e314c-127">Les réservations Azure fournissent la base des solutions d’infrastructure de bout en bout lorsqu’elles sont associées à des logiciels tels que Microsoft Windows Server et Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="e314c-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="e314c-128">Vous pouvez acheter, vendre et gérer des réservations Azure dans l’espace partenaires et le Portail Azure, et à l’aide de l’API espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="e314c-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="e314c-129">Vous pouvez également accorder à vos clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement Azure que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="e314c-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="e314c-130">Suivez les liens ci-dessous pour en savoir plus.</span><span class="sxs-lookup"><span data-stu-id="e314c-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="e314c-131">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="e314c-131">Azure reservations resources</span></span>

|<span data-ttu-id="e314c-132">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="e314c-132">**For information about**</span></span>   |<span data-ttu-id="e314c-133">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="e314c-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="e314c-134">Documentation sur les réservations Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="e314c-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="e314c-135">Que sont les réservations Azure ?</span><span class="sxs-lookup"><span data-stu-id="e314c-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="e314c-136">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="e314c-137">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="e314c-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="e314c-138">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="e314c-139">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="e314c-140">Détermination de la taille de machine virtuelle correcte et vérification de l’utilisation de la machine virtuelle client</span><span class="sxs-lookup"><span data-stu-id="e314c-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="e314c-141">Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure</span><span class="sxs-lookup"><span data-stu-id="e314c-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="e314c-142">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="e314c-143">[Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="e314c-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="e314c-144">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir de votre abonnement CSP.</span><span class="sxs-lookup"><span data-stu-id="e314c-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="e314c-145">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="e314c-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
