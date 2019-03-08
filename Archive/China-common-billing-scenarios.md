---
title: Scénarios de facturation courantes (Partner Center géré par 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586332"
---
# <a name="common-billing-scenarios"></a><span data-ttu-id="f1e41-103">Exemples de facturation courants</span><span class="sxs-lookup"><span data-stu-id="f1e41-103">Common billing scenarios</span></span>

<span data-ttu-id="f1e41-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="f1e41-104">**Applies to**</span></span>

-   <span data-ttu-id="f1e41-105">Espace partenaires géré par 21Vianet</span><span class="sxs-lookup"><span data-stu-id="f1e41-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="f1e41-106">Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement.</span><span class="sxs-lookup"><span data-stu-id="f1e41-106">This topic explains what you should expect to see on your bill after you add new subscriptions, adjust the number of seats in a subscription, or cancel a subscription.</span></span> 


## <a name="licence-based-billing"></a><span data-ttu-id="f1e41-107">Facturation basée sur la licence</span><span class="sxs-lookup"><span data-stu-id="f1e41-107">Licence-based billing</span></span>


<span data-ttu-id="f1e41-108">Pour les mois sans modification des abonnements basés sur le certificat, vous verrez un seul élément de ligne pour chaque abonnement sur votre fichier de rapprochement et la facture des frais d’avance pour le mois prochain.</span><span class="sxs-lookup"><span data-stu-id="f1e41-108">For months without changes to licence-based subscriptions, you'll see a single line item for each subscription on your reconciliation file and invoice for the advance charge for the coming month.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f1e41-109">Scénario</span><span class="sxs-lookup"><span data-stu-id="f1e41-109">Scenario</span></span></td>
<td><span data-ttu-id="f1e41-110">Description</span><span class="sxs-lookup"><span data-stu-id="f1e41-110">Description</span></span></td>
<td><span data-ttu-id="f1e41-111">Exemple</span><span class="sxs-lookup"><span data-stu-id="f1e41-111">Example</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f1e41-112">Nouvel abonnement</span><span class="sxs-lookup"><span data-stu-id="f1e41-112">New subscription</span></span></td>
<td><p><span data-ttu-id="f1e41-113">La période entre la date de début de l’abonnement et la première date de facturation est GRATUITE.</span><span class="sxs-lookup"><span data-stu-id="f1e41-113">The period between the start date of the subscription and the first billing date is FREE.</span></span></p>
<p><span data-ttu-id="f1e41-114">Votre fichier de rapprochement contient un seul élément :</span><span class="sxs-lookup"><span data-stu-id="f1e41-114">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-115">l’avance de frais pour le mois suivant</span><span class="sxs-lookup"><span data-stu-id="f1e41-115">next month's advance charge</span></span></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f1e41-116">Nouvel abonnement : annulé avant la fin de la période de facturation</span><span class="sxs-lookup"><span data-stu-id="f1e41-116">New subscription: cancelled before the billing cut</span></span></td>
<td><span data-ttu-id="f1e41-117">Les frais ne seront pas être appliqués au compte.</span><span class="sxs-lookup"><span data-stu-id="f1e41-117">Charges will not be applied to the account.</span></span> <span data-ttu-id="f1e41-118">L’abonnement n’apparaîtra pas dans le fichier de rapprochement.</span><span class="sxs-lookup"><span data-stu-id="f1e41-118">The subscription won't appear in the reconciliation file.</span></span> <span data-ttu-id="f1e41-119">Ceci est utile si vous voulez effectuer des tests sans que cela implique des frais d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="f1e41-119">This is useful if you want to perform testing without incurring subscription charges.</span></span></td>
<td></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f1e41-120">Nouvel abonnement : avec ajustement de la quantité de licences pendant la période gratuite.</span><span class="sxs-lookup"><span data-stu-id="f1e41-120">New subscription: with licence quantity adjustments during the free period</span></span></td>
<td><p><span data-ttu-id="f1e41-121">Votre fichier de rapprochement contient plusieurs éléments :</span><span class="sxs-lookup"><span data-stu-id="f1e41-121">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-122">modification du nombre de licences, facturées au prix unitaire 0.</span><span class="sxs-lookup"><span data-stu-id="f1e41-122">license quantity changes, charged at 0 Unit Price.</span></span> <span data-ttu-id="f1e41-123">(la modification du nombre de sièges ne génère aucun frais pendant la période gratuite)</span><span class="sxs-lookup"><span data-stu-id="f1e41-123">(There is no cost for seat changes during the free period)</span></span></li>
<li><span data-ttu-id="f1e41-124">l’avance de frais pour le mois suivant, reflétant la nouvelle quantité.</span><span class="sxs-lookup"><span data-stu-id="f1e41-124">advance charge for the next month, reflecting the new quantity.</span></span></li>
</ul></td>
<td><span data-ttu-id="f1e41-125">Utilisation au prorata :</span><span class="sxs-lookup"><span data-stu-id="f1e41-125">Prorated usage:</span></span>
<ul>
<li><span data-ttu-id="f1e41-126">Du 3 au 7 juin pour 10 sièges = ZÉRO frais</span><span class="sxs-lookup"><span data-stu-id="f1e41-126">June 3rd to June 7th for 10 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="f1e41-127">Du 8 au 11 juin pour 20 sièges = ZÉRO frais</span><span class="sxs-lookup"><span data-stu-id="f1e41-127">June 8th to June 11th for 20 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="f1e41-128">Du 12 au 14 juin pour 15 sièges = ZÉRO frais</span><span class="sxs-lookup"><span data-stu-id="f1e41-128">June 12th to June 14th for 15 seats = ZERO charge</span></span></li>
</ul>
<p><span data-ttu-id="f1e41-129">Couper de facturation : Passez gratuit pendant la période de mois complet à partir du 15 juin au 14 juillet pour les 15 sièges.</span><span class="sxs-lookup"><span data-stu-id="f1e41-129">Billing cut: Advance charge for the whole month period from June 15th to July 14th for 15 seats.</span></span> <span data-ttu-id="f1e41-130">À supposer que les frais par abonnement et par mois soient de 10 USD, ils se monteront à 10 USD x 15 sièges = 150 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-130">Assuming the charge per subscription per month is 10 USD, the charge would be 10 USD x 15 seats = 150 USD.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f1e41-131">Abonnement existant : Augmentation ou diminution de la quantité de licence</span><span class="sxs-lookup"><span data-stu-id="f1e41-131">Existing subscription: Increase or decrease in licence quantity</span></span></td>
<td><p><span data-ttu-id="f1e41-132">Votre fichier de rapprochement contient plusieurs éléments :</span><span class="sxs-lookup"><span data-stu-id="f1e41-132">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-133">l’extourne de l’avance de frais</span><span class="sxs-lookup"><span data-stu-id="f1e41-133">the advance charge reversal</span></span></li>
<li><span data-ttu-id="f1e41-134">les frais d’utilisation au prorata</span><span class="sxs-lookup"><span data-stu-id="f1e41-134">prorated usage charges</span></span></li>
<li><span data-ttu-id="f1e41-135">l’avance de frais pour le mois suivant</span><span class="sxs-lookup"><span data-stu-id="f1e41-135">next month's advance charge</span></span></li>
</ul></td>
<td><p><span data-ttu-id="f1e41-136">Utilisation au prorata :</span><span class="sxs-lookup"><span data-stu-id="f1e41-136">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-137">Du 15 au 19 juillet pour 15 sièges = 26,61 USD</span><span class="sxs-lookup"><span data-stu-id="f1e41-137">July 15th to July 19th for 15 seats = 26.61 USD</span></span></li>
<li><span data-ttu-id="f1e41-138">Du 20 au 30 juillet pour 12 sièges = 46,84 USD</span><span class="sxs-lookup"><span data-stu-id="f1e41-138">July 20th to July 30th for 12 seats = 46.84 USD</span></span></li>
<li><span data-ttu-id="f1e41-139">Du 31 juillet au 9 août pour 18 sièges = 63,87 USD</span><span class="sxs-lookup"><span data-stu-id="f1e41-139">July 31st to August 9th for 18 seats = 63.87 USD</span></span></li>
<li><span data-ttu-id="f1e41-140">Du 10 au 14 août pour 10 sièges = 17,74 USD</span><span class="sxs-lookup"><span data-stu-id="f1e41-140">August 10th to August 14th for 10 seats = 17.74 USD</span></span></li>
</ul>
<span data-ttu-id="f1e41-141">Extourne de l’avance de frais pour l’intégralité du mois du 15 juillet au 14 août = -165 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-141">Reversal of the advance charge for the whole month period from July 15th to August 14th = -165 USD.</span></span>
<p><span data-ttu-id="f1e41-142">Couper de facturation : Passez des frais pour la période de mois complet à partir du 15 août au 14 septembre pour les 10 sièges = 110 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-142">Billing cut: Advance charge for the whole month period from August 15th to September 14th for 10 seats = 110 USD.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f1e41-143">Annulation : aucune modification préalable du nombre de sièges</span><span class="sxs-lookup"><span data-stu-id="f1e41-143">Cancellation: no prior seat changes</span></span></td>
<td><p><span data-ttu-id="f1e41-144">Votre fichier de rapprochement contient un seul élément :</span><span class="sxs-lookup"><span data-stu-id="f1e41-144">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-145">Un crédit pour les jours non utilisés, l’intégralité de la période ayant été facturée d’avance dans le document de facturation précédent.</span><span class="sxs-lookup"><span data-stu-id="f1e41-145">A credit for unused days, because the whole period was billed in advance in the previous billing statement.</span></span> <span data-ttu-id="f1e41-146">Cette valeur est calculée en fonction de la date de fin de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="f1e41-146">This is calculated based on the Subscription End date.</span></span></li>
</ul></td>
<td><span data-ttu-id="f1e41-147">Précédemment facturés des frais d’avance : Le 15 août à 14 septembre pour 10 sièges = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-147">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="f1e41-148">Part utilisée de l’avance de frais du 15 août au 24 août.</span><span class="sxs-lookup"><span data-stu-id="f1e41-148">Consumed portion of the advance charge from August 15th to August 24th.</span></span></p>
<p><span data-ttu-id="f1e41-149">Crédit inutilisé jours : Le 25 août à 14 septembre pour 10 sièges =-74.51.</span><span class="sxs-lookup"><span data-stu-id="f1e41-149">Credit for unused days: August 25th to September 14th for 10 seats = -74.51.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f1e41-150">Annulation : avec modification préalable du nombre de sièges</span><span class="sxs-lookup"><span data-stu-id="f1e41-150">Cancellation: with prior seat changes</span></span></td>
<td><p><span data-ttu-id="f1e41-151">Votre fichier de rapprochement contient plusieurs éléments :</span><span class="sxs-lookup"><span data-stu-id="f1e41-151">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-152">l’extourne de l’avance de frais</span><span class="sxs-lookup"><span data-stu-id="f1e41-152">the advance charge reversal</span></span></li>
<li><span data-ttu-id="f1e41-153">les frais d’utilisation au prorata</span><span class="sxs-lookup"><span data-stu-id="f1e41-153">prorated usage charges</span></span></li>
<li><span data-ttu-id="f1e41-154">un crédit pour les jours non utilisés</span><span class="sxs-lookup"><span data-stu-id="f1e41-154">a credit for any unused days</span></span></li>
</ul></td>
<td><span data-ttu-id="f1e41-155">Précédemment facturés des frais d’avance : Le 15 août à 14 septembre pour 10 sièges = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-155">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="f1e41-156">Utilisation au prorata :</span><span class="sxs-lookup"><span data-stu-id="f1e41-156">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="f1e41-157">Du 15 au 24 août pour 10 sièges</span><span class="sxs-lookup"><span data-stu-id="f1e41-157">August 15th to August 24th for 10 seats</span></span></li>
<li><span data-ttu-id="f1e41-158">Du 25 août au 14 septembre pour 5 sièges</span><span class="sxs-lookup"><span data-stu-id="f1e41-158">August 25th to September 14th for 5 seats</span></span></li>
</ul>
<p><span data-ttu-id="f1e41-159">Crédit inutilisé jours : Le 1er septembre à 14 septembre pour 5 utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="f1e41-159">Credit for unused days: September 1st to September 14th for 5 seats.</span></span></p>
<p><span data-ttu-id="f1e41-160">Extourne de l’avance de frais pour l’intégralité du mois du 15 août au 14 septembre = -100 USD.</span><span class="sxs-lookup"><span data-stu-id="f1e41-160">Reversal of the advance charge for the whole month period from August 15th to September 14th = -100 USD.</span></span></p></td>
</tr>
</tbody>
</table>
