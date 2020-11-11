---
title: Calcul du prix unitaire effectif
ms.topic: how-to
ms.date: 11/10/2020
description: En savoir plus sur l’unité de prix effective et sur la manière dont elle est calculée. Comprend un exemple de calcul.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498570"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="c50ec-104">Calcul du prix unitaire effectif pour la consommation des plans Azure</span><span class="sxs-lookup"><span data-stu-id="c50ec-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="c50ec-105">Le prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="c50ec-105">The effective unit price</span></span>

<span data-ttu-id="c50ec-106">Le prix unitaire effectif est calculé au niveau du compteur (par opposition au niveau de la ressource) et est ajusté quotidiennement en fonction de l’utilisation du compteur.</span><span class="sxs-lookup"><span data-stu-id="c50ec-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="c50ec-107">Nous calculons le prix unitaire effectif à l’aide des trois facteurs suivants :</span><span class="sxs-lookup"><span data-stu-id="c50ec-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="c50ec-108">Consommation, qui est surveillée quotidiennement tout au long du cycle de facturation</span><span class="sxs-lookup"><span data-stu-id="c50ec-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="c50ec-109">Coût facturable pour le compteur</span><span class="sxs-lookup"><span data-stu-id="c50ec-109">Billable cost for the meter</span></span>
- <span data-ttu-id="c50ec-110">Hiérarchisation (le cas échéant)</span><span class="sxs-lookup"><span data-stu-id="c50ec-110">Tiering (if applicable)</span></span>

<span data-ttu-id="c50ec-111">Étant donné que nous Surveillez la consommation quotidiennement tout au long du cycle de facturation, le prix unitaire effectif varie.</span><span class="sxs-lookup"><span data-stu-id="c50ec-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="c50ec-112">Le prix final d’un cycle de facturation donné sera disponible après l’arrêt du calcul de consommation et la clôture de la période de facturation.</span><span class="sxs-lookup"><span data-stu-id="c50ec-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="c50ec-113">Vous verrez la plupart des modifications de la consommation après la quatrième ou la cinquième décimale.</span><span class="sxs-lookup"><span data-stu-id="c50ec-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="c50ec-114">Déterminez si votre compteur utilise la tarification à plusieurs niveaux</span><span class="sxs-lookup"><span data-stu-id="c50ec-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="c50ec-115">Si vous ne savez pas si votre compteur utilise la tarification à plusieurs niveaux, utilisez la procédure ci-dessous pour le savoir.</span><span class="sxs-lookup"><span data-stu-id="c50ec-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="c50ec-116">Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c50ec-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c50ec-117">Sélectionnez **vendre** , sélectionnez **tarification et offres** , puis sélectionnez **tarification du plan Azure**.</span><span class="sxs-lookup"><span data-stu-id="c50ec-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="c50ec-118">Localisez votre compteur par ID, puis téléchargez vos données de tarification.</span><span class="sxs-lookup"><span data-stu-id="c50ec-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="c50ec-119">Exemple de calcul</span><span class="sxs-lookup"><span data-stu-id="c50ec-119">Sample calculation</span></span>

<span data-ttu-id="c50ec-120">Le tableau ci-dessous donne un exemple de la façon dont nous calculons le prix unitaire effectif au cours de la période ouverte.</span><span class="sxs-lookup"><span data-stu-id="c50ec-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="c50ec-121">Dans le tableau, les valeurs suivantes s’appliquent :</span><span class="sxs-lookup"><span data-stu-id="c50ec-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="c50ec-122">**Up** = prix unitaire de la ressource/heure = 0,868</span><span class="sxs-lookup"><span data-stu-id="c50ec-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="c50ec-123">**BCU** = unité de consommation facturable pour le compteur</span><span class="sxs-lookup"><span data-stu-id="c50ec-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="c50ec-124">**BC** = coût facturable pour le compteur = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="c50ec-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="c50ec-125">Cela reflète un ajustement de la remise de 15% du PEC.</span><span class="sxs-lookup"><span data-stu-id="c50ec-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="c50ec-126">Nous utilisons ensuite la limite inférieure de la fonction pour limiter la valeur à deux chiffres après la virgule décimale, afin de charger la quantité minimale.</span><span class="sxs-lookup"><span data-stu-id="c50ec-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="c50ec-127">**Prix unitaire effectif** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="c50ec-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="c50ec-128">Remarque : le compteur de cet exemple n’a pas de niveaux de tarification.</span><span class="sxs-lookup"><span data-stu-id="c50ec-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="c50ec-129">Date</span><span class="sxs-lookup"><span data-stu-id="c50ec-129">Date</span></span> | <span data-ttu-id="c50ec-130">BCU (unité de consommation facturable)</span><span class="sxs-lookup"><span data-stu-id="c50ec-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="c50ec-131">BC (coût facturable)</span><span class="sxs-lookup"><span data-stu-id="c50ec-131">BC (Billable cost)</span></span> | <span data-ttu-id="c50ec-132">Prix unitaire effectif</span><span class="sxs-lookup"><span data-stu-id="c50ec-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="c50ec-133">3-août</span><span class="sxs-lookup"><span data-stu-id="c50ec-133">3-Aug</span></span> | <span data-ttu-id="c50ec-134">29</span><span class="sxs-lookup"><span data-stu-id="c50ec-134">29</span></span> | <span data-ttu-id="c50ec-135">21,39</span><span class="sxs-lookup"><span data-stu-id="c50ec-135">21.39</span></span> | <span data-ttu-id="c50ec-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="c50ec-136">0.737586206896552</span></span> |
| <span data-ttu-id="c50ec-137">10-août</span><span class="sxs-lookup"><span data-stu-id="c50ec-137">10-Aug</span></span> | <span data-ttu-id="c50ec-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="c50ec-138">210.950039</span></span> | <span data-ttu-id="c50ec-139">155,63</span><span class="sxs-lookup"><span data-stu-id="c50ec-139">155.63</span></span> | <span data-ttu-id="c50ec-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="c50ec-140">0.737757626107858</span></span> |
| <span data-ttu-id="c50ec-141">25-août</span><span class="sxs-lookup"><span data-stu-id="c50ec-141">25-Aug</span></span> | <span data-ttu-id="c50ec-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="c50ec-142">555.950039</span></span> | <span data-ttu-id="c50ec-143">410,17</span><span class="sxs-lookup"><span data-stu-id="c50ec-143">410.17</span></span> | <span data-ttu-id="c50ec-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="c50ec-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="c50ec-145">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c50ec-145">Next steps</span></span>

- [<span data-ttu-id="c50ec-146">Facturation et taxes</span><span class="sxs-lookup"><span data-stu-id="c50ec-146">Billing and taxes</span></span>](billing.md)