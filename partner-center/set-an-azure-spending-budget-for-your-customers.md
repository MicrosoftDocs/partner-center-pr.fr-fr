---
title: Définir un budget de dépenses Azure pour les clients
ms.topic: how-to
ms.date: 03/17/2021
description: Découvrez comment définir ou supprimer des budgets de dépenses Azure mensuels pour vos clients, ainsi que pour afficher les données de dépense Azure et définir des notifications relatives au budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855350"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="0da1d-103">Définir, vérifier ou supprimer des budgets de dépenses Azure mensuels pour les clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0da1d-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="0da1d-104">**Rôles appropriés**: agent d’administration</span><span class="sxs-lookup"><span data-stu-id="0da1d-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="0da1d-105">Vous pouvez [définir un budget de dépenses Azure mensuel pour vos clients](#set-azure-spending-budget) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0da1d-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="0da1d-106">Cela permet à vos clients de gérer leurs dépenses Azure.</span><span class="sxs-lookup"><span data-stu-id="0da1d-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="0da1d-107">Cette option vous permet de comparer les dépenses Azure de vos clients au budget du mois.</span><span class="sxs-lookup"><span data-stu-id="0da1d-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="0da1d-108">Il permet également à vos clients de budgétiser leurs dépenses Azure, de sorte que leur facture mensuelle n’est pas supérieure à celle qu’ils anticipent.</span><span class="sxs-lookup"><span data-stu-id="0da1d-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="0da1d-109">Cette fonctionnalité n’est pas disponible dans les comptes de bac à sable (sandbox) ou de test en production (TIP).</span><span class="sxs-lookup"><span data-stu-id="0da1d-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="0da1d-110">Une fois que vous avez [défini un budget de dépenses Azure pour vos clients](#set-azure-spending-budget), vous pouvez également consulter l’utilisation des clients de l’une des manières suivantes.</span><span class="sxs-lookup"><span data-stu-id="0da1d-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="0da1d-111">Ces options peuvent vous aider à identifier des services mal configurés ou des tendances inhabituelles susceptibles de suggérer des fraudes.</span><span class="sxs-lookup"><span data-stu-id="0da1d-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="0da1d-112">Vous pouvez ensuite travailler avec vos clients pour identifier la cause racine et gérer les coûts.</span><span class="sxs-lookup"><span data-stu-id="0da1d-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="0da1d-113">Si nécessaire, vous pouvez également [modifier le budget du client](#set-azure-spending-budget) sur une valeur supérieure.</span><span class="sxs-lookup"><span data-stu-id="0da1d-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="0da1d-114">Vérifier les dépenses Azure actuelles</span><span class="sxs-lookup"><span data-stu-id="0da1d-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="0da1d-115">Activer les notifications par courrier électronique lorsque la dépense d’un client est proche de sa limite budgétaire</span><span class="sxs-lookup"><span data-stu-id="0da1d-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="0da1d-116">Afficher les coûts totaux par service pour les abonnements basés sur l’utilisation</span><span class="sxs-lookup"><span data-stu-id="0da1d-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="0da1d-117">Vous pouvez également [supprimer un budget de dépenses Azure](#remove-azure-spending-budget) pour le ou les clients à tout moment.</span><span class="sxs-lookup"><span data-stu-id="0da1d-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="0da1d-118">Données de dépense Azure</span><span class="sxs-lookup"><span data-stu-id="0da1d-118">Azure spending data</span></span>

<span data-ttu-id="0da1d-119">Les données de dépense Azure sont une *estimation* et les *montants de facturation réels peuvent varier*.</span><span class="sxs-lookup"><span data-stu-id="0da1d-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="0da1d-120">La valeur des données *ne reflète pas* les taxes, crédits, ajustements ou autres frais qui peuvent s’appliquer.</span><span class="sxs-lookup"><span data-stu-id="0da1d-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="0da1d-121">Les données de dépense sont *actualisées une fois par jour*.</span><span class="sxs-lookup"><span data-stu-id="0da1d-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="0da1d-122">Vos clients peuvent continuer à utiliser (et être facturés pour) les services et les ressources Azure, sauf si vous modifiez leurs paramètres de compte dans le Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="0da1d-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="0da1d-123">Définir le budget des dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="0da1d-123">Set Azure spending budget</span></span>

<span data-ttu-id="0da1d-124">Vous pouvez *définir un budget de dépenses Azure mensuel* pour plusieurs clients dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="0da1d-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="0da1d-125">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0da1d-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0da1d-126">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0da1d-127">Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients pour lesquels vous souhaitez définir un budget.</span><span class="sxs-lookup"><span data-stu-id="0da1d-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="0da1d-128">Entrez une valeur pour le **Budget mensuel**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="0da1d-129">Choisissez **appliquer** pour enregistrer vos modifications.</span><span class="sxs-lookup"><span data-stu-id="0da1d-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="0da1d-130">Vous pouvez également *définir un budget pour un client individuel* dans ses paramètres d’abonnement :</span><span class="sxs-lookup"><span data-stu-id="0da1d-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="0da1d-131">Connectez-vous au tableau de bord de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0da1d-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="0da1d-132">Dans le menu de gauche, sous **CSP**, choisissez **clients**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0da1d-133">Sur la page **clients** , sélectionnez le nom de la **société** du client.</span><span class="sxs-lookup"><span data-stu-id="0da1d-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0da1d-134">Sur la page **abonnements** du client, sous **abonnement basé sur l’utilisation**, choisissez **modifier le budget**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="0da1d-135">Entrez une valeur pour le budget.</span><span class="sxs-lookup"><span data-stu-id="0da1d-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="0da1d-136">Choisissez **appliquer** pour enregistrer vos modifications.</span><span class="sxs-lookup"><span data-stu-id="0da1d-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="0da1d-137">Supprimer le budget des dépenses Azure</span><span class="sxs-lookup"><span data-stu-id="0da1d-137">Remove Azure spending budget</span></span>

<span data-ttu-id="0da1d-138">Vous pouvez *supprimer un budget de dépenses Azure mensuel* pour vos clients dans l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="0da1d-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="0da1d-139">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0da1d-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0da1d-140">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0da1d-141">Dans la page **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, sélectionnez le ou les clients dont vous souhaitez supprimer le budget.</span><span class="sxs-lookup"><span data-stu-id="0da1d-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="0da1d-142">Choisissez **supprimer le budget**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="0da1d-143">Vérifier les dépenses Azure actuelles</span><span class="sxs-lookup"><span data-stu-id="0da1d-143">Check current Azure spending</span></span>

<span data-ttu-id="0da1d-144">Vous pouvez à tout moment *suivre les dépenses et les budgets mensuels actuels de vos clients* :</span><span class="sxs-lookup"><span data-stu-id="0da1d-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="0da1d-145">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0da1d-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="0da1d-146">Dans le menu de gauche, sous **CSP**, choisissez **dépenses Azure**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="0da1d-147">Dans la page des **dépenses Azure** , sous **clients avec Microsoft Azure abonnements**, vous pouvez voir une vue d’ensemble des budgets mensuels des clients, des estimations de dépense actuelles et du pourcentage de budget utilisé.</span><span class="sxs-lookup"><span data-stu-id="0da1d-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="0da1d-148">Notifications pour les limites budgétaires</span><span class="sxs-lookup"><span data-stu-id="0da1d-148">Notifications for budget limits</span></span>

<span data-ttu-id="0da1d-149">Vous pouvez *activer les notifications par courrier électronique* lorsque la dépense mensuelle de votre client est proche de sa limite budgétaire.</span><span class="sxs-lookup"><span data-stu-id="0da1d-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="0da1d-150">Lorsque vous activez cette option, vous êtes averti lorsque les clients utilisent 80% ou plus de leur budget mensuel.</span><span class="sxs-lookup"><span data-stu-id="0da1d-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="0da1d-151">Cette option vous permet de garder un œil sur votre facture Azure.</span><span class="sxs-lookup"><span data-stu-id="0da1d-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="0da1d-152">Pour configurer les notifications par courrier électronique :</span><span class="sxs-lookup"><span data-stu-id="0da1d-152">To configure email notifications:</span></span>

1. <span data-ttu-id="0da1d-153">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0da1d-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0da1d-154">Accédez à **Settings**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="0da1d-155">Sélectionnez **Mes préférences**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="0da1d-156">Si ce n’est pas le cas, configurez une adresse de messagerie préférée.</span><span class="sxs-lookup"><span data-stu-id="0da1d-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="0da1d-157">Configurez la langue par défaut pour la notification.</span><span class="sxs-lookup"><span data-stu-id="0da1d-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="0da1d-158">Sélectionnez l’onglet **CSP** sous la section **Préférences de notification** .</span><span class="sxs-lookup"><span data-stu-id="0da1d-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="0da1d-159">Vérifiez l’option E-mail pour la notification de **dépenses Azure** , puis **Enregistrez**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="0da1d-160">Coûts totaux par service</span><span class="sxs-lookup"><span data-stu-id="0da1d-160">Itemized costs by service</span></span>

<span data-ttu-id="0da1d-161">Vous pouvez *afficher les coûts totaux (et l’utilisation estimée) par service pour les abonnements basés sur l’utilisation*:</span><span class="sxs-lookup"><span data-stu-id="0da1d-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="0da1d-162">Connectez-vous à l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="0da1d-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="0da1d-163">Dans le menu de gauche, sous **CSP**, choisissez **clients**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="0da1d-164">Sur la page **clients** , sélectionnez le nom de la **société** du client.</span><span class="sxs-lookup"><span data-stu-id="0da1d-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="0da1d-165">Sur la page **abonnements** du client, sous **abonnements basés sur l’utilisation**, sélectionnez le nom de l' **abonnement**.</span><span class="sxs-lookup"><span data-stu-id="0da1d-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="0da1d-166">Sur la page de l’abonnement, vous pouvez passer en revue les **coûts** par service et l' **utilisation estimée** pour le mois en cours.</span><span class="sxs-lookup"><span data-stu-id="0da1d-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="0da1d-167">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0da1d-167">Next steps</span></span>

- [<span data-ttu-id="0da1d-168">Nouvelle expérience de commerce pour les CSP - Facturation Azure</span><span class="sxs-lookup"><span data-stu-id="0da1d-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
