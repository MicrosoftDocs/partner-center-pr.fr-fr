---
title: Définir un budget Azure pour vos clients | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Découvrez comment définir ou supprimer des budgets de dépenses Azure mensuels pour vos clients, ainsi que pour afficher les données de dépense Azure et définir des notifications relatives au budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e33a15110666bb3b4a3c76c198cde7a59d81411f
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/05/2020
ms.locfileid: "82797887"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="2b42b-103">Définir un budget Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="2b42b-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="2b42b-104">S’applique à :</span><span class="sxs-lookup"><span data-stu-id="2b42b-104">Applies to:</span></span>

- <span data-ttu-id="2b42b-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="2b42b-105">Partner Center</span></span>
- <span data-ttu-id="2b42b-106">Espace partenaires de Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="2b42b-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2b42b-107">Vous pouvez [définir un budget de dépenses Azure mensuel pour vos clients](#set-azure-spending-budget) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2b42b-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="2b42b-108">Cela permet à vos clients de gérer leurs dépenses Azure.</span><span class="sxs-lookup"><span data-stu-id="2b42b-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="2b42b-109">Cette option vous permet de comparer les dépenses Azure de vos clients au budget du mois.</span><span class="sxs-lookup"><span data-stu-id="2b42b-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="2b42b-110">Cela permet également à vos clients de budgétiser leurs dépenses Azure, de sorte que leur facture mensuelle n’est pas supérieure à celle qu’ils anticipent.</span><span class="sxs-lookup"><span data-stu-id="2b42b-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="2b42b-111">Cette fonctionnalité n’est pas disponible dans les comptes de bac à sable (sandbox) ou de test en production (TIP).</span><span class="sxs-lookup"><span data-stu-id="2b42b-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="2b42b-112">Une fois que vous avez [défini un budget de dépenses Azure pour vos clients](#set-azure-spending-budget), vous pouvez également consulter l’utilisation des clients de l’une des manières suivantes.</span><span class="sxs-lookup"><span data-stu-id="2b42b-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="2b42b-113">Ces options peuvent vous aider à identifier des services mal configurés ou des tendances inhabituelles susceptibles de suggérer des fraudes.</span><span class="sxs-lookup"><span data-stu-id="2b42b-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="2b42b-114">Vous pouvez ensuite travailler avec vos clients pour identifier la cause racine et gérer les coûts.</span><span class="sxs-lookup"><span data-stu-id="2b42b-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="2b42b-115">Si nécessaire, vous pouvez également [modifier le budget du client](#set-azure-spending-budget) sur une valeur supérieure.</span><span class="sxs-lookup"><span data-stu-id="2b42b-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="2b42b-116">Vérifier les dépenses Azure actuelles</span><span class="sxs-lookup"><span data-stu-id="2b42b-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="2b42b-117">Activer les notifications par courrier électronique lorsque la dépense d’un client est proche de sa limite budgétaire</span><span class="sxs-lookup"><span data-stu-id="2b42b-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="2b42b-118">Afficher les coûts totaux par service pour les abonnements basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="2b42b-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="2b42b-119">Vous pouvez également [supprimer un budget de dépenses Azure](#remove-azure-spending-budget) pour le ou les clients à tout moment.</span><span class="sxs-lookup"><span data-stu-id="2b42b-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="2b42b-120">Données de dépense Azure</span><span class="sxs-lookup"><span data-stu-id="2b42b-120">Azure spending data</span></span>

<span data-ttu-id="2b42b-121">Les données de dépense Azure sont une *estimation* et les *montants de facturation réels peuvent varier*.</span><span class="sxs-lookup"><span data-stu-id="2b42b-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="2b42b-122">La valeur des données *ne reflète pas* les taxes, crédits, ajustements ou autres frais qui peuvent s’appliquer.</span><span class="sxs-lookup"><span data-stu-id="2b42b-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="2b42b-123">Les données de dépense sont *actualisées une fois par jour*.</span><span class="sxs-lookup"><span data-stu-id="2b42b-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="2b42b-124">Vos clients peuvent continuer à utiliser (et être facturés pour) les services et les ressources Azure, sauf si vous modifiez leurs paramètres de compte dans le Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="2b42b-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="2b42b-125">Définir le budget des dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="2b42b-125">Set Azure spending budget</span></span>

<span data-ttu-id="2b42b-126">Vous pouvez *définir un budget de dépenses Azure mensuel* pour plusieurs clients dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="2b42b-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="2b42b-127">Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="2b42b-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="2b42b-128">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="2b42b-129">Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients pour lesquels vous souhaitez définir un budget.</span><span class="sxs-lookup"><span data-stu-id="2b42b-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="2b42b-130">Entrez une valeur pour le **Budget mensuel**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="2b42b-131">Choisissez **appliquer** pour enregistrer vos modifications.</span><span class="sxs-lookup"><span data-stu-id="2b42b-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="2b42b-132">Vous pouvez également *définir un budget pour un client individuel* dans ses paramètres d’abonnement :</span><span class="sxs-lookup"><span data-stu-id="2b42b-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="2b42b-133">Connectez-vous au tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2b42b-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="2b42b-134">Dans le menu de gauche, sous **CSP**, choisissez **clients**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="2b42b-135">Sur la page **clients** , sélectionnez le nom de la **société**du client.</span><span class="sxs-lookup"><span data-stu-id="2b42b-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="2b42b-136">Sur la page **abonnements** du client, sous **abonnement basé sur l’utilisation**, choisissez **modifier le budget**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="2b42b-137">Entrez une valeur pour le budget.</span><span class="sxs-lookup"><span data-stu-id="2b42b-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="2b42b-138">Choisissez **appliquer** pour enregistrer vos modifications.</span><span class="sxs-lookup"><span data-stu-id="2b42b-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="2b42b-139">Supprimer le budget des dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="2b42b-139">Remove Azure spending budget</span></span>

<span data-ttu-id="2b42b-140">Vous pouvez *supprimer un budget de dépenses Azure mensuel* pour vos clients dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="2b42b-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="2b42b-141">Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="2b42b-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="2b42b-142">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="2b42b-143">Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients dont vous souhaitez supprimer le budget.</span><span class="sxs-lookup"><span data-stu-id="2b42b-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="2b42b-144">Choisissez **supprimer le budget**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="2b42b-145">Vérifier les dépenses Azure actuelles</span><span class="sxs-lookup"><span data-stu-id="2b42b-145">Check current Azure spending</span></span>

<span data-ttu-id="2b42b-146">Vous pouvez à tout moment *suivre les dépenses et les budgets mensuels actuels de vos clients* :</span><span class="sxs-lookup"><span data-stu-id="2b42b-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="2b42b-147">Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="2b42b-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="2b42b-148">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="2b42b-149">Dans la page des **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, vous pouvez voir une vue d’ensemble des budgets mensuels des clients, des estimations de dépense actuelles et du pourcentage de budget utilisé.</span><span class="sxs-lookup"><span data-stu-id="2b42b-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="2b42b-150">Notifications pour les limites budgétaires</span><span class="sxs-lookup"><span data-stu-id="2b42b-150">Notifications for budget limits</span></span>

<span data-ttu-id="2b42b-151">Vous pouvez *activer les notifications par courrier électronique* lorsque la dépense mensuelle de votre client est proche de sa limite budgétaire.</span><span class="sxs-lookup"><span data-stu-id="2b42b-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="2b42b-152">Lorsque vous activez cette option, vous êtes averti lorsque les clients utilisent 80% ou plus de leur budget mensuel.</span><span class="sxs-lookup"><span data-stu-id="2b42b-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="2b42b-153">Cette option vous permet de garder un œil sur votre facture Azure.</span><span class="sxs-lookup"><span data-stu-id="2b42b-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="2b42b-154">Pour configurer les notifications par courrier électronique :</span><span class="sxs-lookup"><span data-stu-id="2b42b-154">To configure email notifications:</span></span>

1. <span data-ttu-id="2b42b-155">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2b42b-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="2b42b-156">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="2b42b-157">Dans la page **dépenses Azure** , sous **notifications par courrier électronique**, basculez le paramètre **recevoir des e-mails** **sur activé**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="2b42b-158">Choisissez **modifier l’adresse de messagerie** pour afficher l’adresse de messagerie des notifications.</span><span class="sxs-lookup"><span data-stu-id="2b42b-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="2b42b-159">Si l’adresse de messagerie *est incorrecte*, entrez l’adresse de messagerie appropriée, puis choisissez **mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="2b42b-160">Si l’adresse de messagerie *est correcte*, choisissez **Annuler**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="2b42b-161">Coûts totaux par service</span><span class="sxs-lookup"><span data-stu-id="2b42b-161">Itemized costs by service</span></span>

<span data-ttu-id="2b42b-162">Vous pouvez *afficher les coûts totaux (et l’utilisation estimée) par service pour les abonnements basés sur l’utilisation*:</span><span class="sxs-lookup"><span data-stu-id="2b42b-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="2b42b-163">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="2b42b-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="2b42b-164">Dans le menu de gauche, sous **CSP**, choisissez **clients**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="2b42b-165">Sur la page **clients** , sélectionnez le nom de la **société**du client.</span><span class="sxs-lookup"><span data-stu-id="2b42b-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="2b42b-166">Sur la page **abonnements** du client, sous **abonnements basés sur l’utilisation**, sélectionnez le nom de l' **abonnement**.</span><span class="sxs-lookup"><span data-stu-id="2b42b-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="2b42b-167">Sur la page de l’abonnement, vous pouvez passer en revue les **coûts** par service et l' **utilisation estimée** pour le mois en cours.</span><span class="sxs-lookup"><span data-stu-id="2b42b-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
