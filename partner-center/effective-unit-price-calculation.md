---
title: Calcul du prix unitaire effectif
ms.topic: how-to
ms.date: 04/02/2021
description: En savoir plus sur le prix unitaire effectif et sur la façon dont il est calculé. Cet article contient également un exemple de calcul.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147120"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="0b1b7-104">Calcul du prix unitaire effectif pour la consommation des plans Azure</span><span class="sxs-lookup"><span data-stu-id="0b1b7-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="0b1b7-105">**Rôles appropriés**: administrateur de facturation</span><span class="sxs-lookup"><span data-stu-id="0b1b7-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="0b1b7-106">Le prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="0b1b7-106">The effective unit price</span></span>

<span data-ttu-id="0b1b7-107">Le prix unitaire effectif est calculé au niveau du compteur (par opposition au niveau de la ressource) et est ajusté quotidiennement en fonction de l’utilisation du compteur.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="0b1b7-108">Nous calculons le prix unitaire effectif à l’aide des trois facteurs suivants :</span><span class="sxs-lookup"><span data-stu-id="0b1b7-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="0b1b7-109">Consommation, qui est surveillée quotidiennement tout au long du cycle de facturation</span><span class="sxs-lookup"><span data-stu-id="0b1b7-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="0b1b7-110">Coût facturable pour le compteur</span><span class="sxs-lookup"><span data-stu-id="0b1b7-110">Billable cost for the meter</span></span>
- <span data-ttu-id="0b1b7-111">Hiérarchisation (le cas échéant)</span><span class="sxs-lookup"><span data-stu-id="0b1b7-111">Tiering (if applicable)</span></span>

<span data-ttu-id="0b1b7-112">Étant donné que nous Surveillez la consommation quotidiennement tout au long du cycle de facturation, le prix unitaire effectif varie.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="0b1b7-113">Le prix final d’un cycle de facturation donné sera disponible après l’arrêt du calcul de consommation et la clôture de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="0b1b7-114">Vous verrez la plupart des modifications de la consommation après la quatrième ou la cinquième décimale.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="0b1b7-115">Déterminez si votre compteur utilise la tarification à plusieurs niveaux</span><span class="sxs-lookup"><span data-stu-id="0b1b7-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="0b1b7-116">Si vous ne savez pas si votre compteur utilise la tarification à plusieurs niveaux, utilisez la procédure ci-dessous pour le savoir.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="0b1b7-117">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0b1b7-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="0b1b7-118">Sélectionnez **vendre**, sélectionnez **tarification et offres**, puis sélectionnez **tarification du plan Azure**.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="0b1b7-119">Localisez votre compteur par ID, puis téléchargez vos données de tarification.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="0b1b7-120">Exemple de calcul</span><span class="sxs-lookup"><span data-stu-id="0b1b7-120">Sample calculation</span></span>

<span data-ttu-id="0b1b7-121">Le tableau ci-dessous donne un exemple de la façon dont nous calculons le prix unitaire effectif au cours de la période ouverte.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="0b1b7-122">Dans le tableau, les valeurs suivantes s’appliquent :</span><span class="sxs-lookup"><span data-stu-id="0b1b7-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="0b1b7-123">**Up** = prix unitaire de la ressource/heure = 0,868</span><span class="sxs-lookup"><span data-stu-id="0b1b7-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="0b1b7-124">**BCU** = unité de consommation facturable pour le compteur</span><span class="sxs-lookup"><span data-stu-id="0b1b7-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="0b1b7-125">**BC** = coût facturable pour le compteur = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="0b1b7-126">Cela reflète un ajustement de la remise de 15% du PEC.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="0b1b7-127">Nous utilisons ensuite la limite inférieure de la fonction pour limiter la valeur à deux chiffres après la virgule décimale, afin de charger la quantité minimale.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="0b1b7-128">**Prix unitaire effectif** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="0b1b7-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="0b1b7-129">Remarque : le compteur de cet exemple n’a pas de niveaux de tarification ou autres remises, c’est-à-dire les facteurs de prix unitaire effectifs dans les pourcentages de remise et autres ajustements.</span><span class="sxs-lookup"><span data-stu-id="0b1b7-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="0b1b7-130">Date</span><span class="sxs-lookup"><span data-stu-id="0b1b7-130">Date</span></span> | <span data-ttu-id="0b1b7-131">BCU (unité de consommation facturable)</span><span class="sxs-lookup"><span data-stu-id="0b1b7-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="0b1b7-132">BC (coût facturable)</span><span class="sxs-lookup"><span data-stu-id="0b1b7-132">BC (Billable cost)</span></span> | <span data-ttu-id="0b1b7-133">Prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="0b1b7-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="0b1b7-134">3-août</span><span class="sxs-lookup"><span data-stu-id="0b1b7-134">3-Aug</span></span> | <span data-ttu-id="0b1b7-135">29</span><span class="sxs-lookup"><span data-stu-id="0b1b7-135">29</span></span> | <span data-ttu-id="0b1b7-136">21,39</span><span class="sxs-lookup"><span data-stu-id="0b1b7-136">21.39</span></span> | <span data-ttu-id="0b1b7-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="0b1b7-137">0.737586206896552</span></span> |
| <span data-ttu-id="0b1b7-138">10-août</span><span class="sxs-lookup"><span data-stu-id="0b1b7-138">10-Aug</span></span> | <span data-ttu-id="0b1b7-139">210,950039</span><span class="sxs-lookup"><span data-stu-id="0b1b7-139">210.950039</span></span> | <span data-ttu-id="0b1b7-140">155,63</span><span class="sxs-lookup"><span data-stu-id="0b1b7-140">155.63</span></span> | <span data-ttu-id="0b1b7-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="0b1b7-141">0.737757626107858</span></span> |
| <span data-ttu-id="0b1b7-142">25-août</span><span class="sxs-lookup"><span data-stu-id="0b1b7-142">25-Aug</span></span> | <span data-ttu-id="0b1b7-143">555,950039</span><span class="sxs-lookup"><span data-stu-id="0b1b7-143">555.950039</span></span> | <span data-ttu-id="0b1b7-144">410,17</span><span class="sxs-lookup"><span data-stu-id="0b1b7-144">410.17</span></span> | <span data-ttu-id="0b1b7-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="0b1b7-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="0b1b7-146">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0b1b7-146">Next steps</span></span>

- [<span data-ttu-id="0b1b7-147">Facturation et taxes</span><span class="sxs-lookup"><span data-stu-id="0b1b7-147">Billing and taxes</span></span>](billing.md)
