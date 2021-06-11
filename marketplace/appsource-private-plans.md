---
title: Plans privés dans Microsoft AppSource
description: Configuration de plans privés dans Microsoft AppSource (place de marché Azure).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008531"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="b2af7-103">Plans privés dans Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="b2af7-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="b2af7-104">Les plans privés sont la manière dont les éditeurs fournissent des plans personnalisés à des clients spécifiques.</span><span class="sxs-lookup"><span data-stu-id="b2af7-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="b2af7-105">Cette option est désormais disponible dans Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="b2af7-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="b2af7-106">Les plans privés peuvent être vendus sur des offres SaaS (AppSource for software as a service) avec l’appel à l’action **obtenir maintenant** .</span><span class="sxs-lookup"><span data-stu-id="b2af7-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="b2af7-107">Demander à votre éditeur de logiciels indépendant un plan privé</span><span class="sxs-lookup"><span data-stu-id="b2af7-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="b2af7-108">Pour qu’un plan privé soit à votre disposition dans AppSource, vous devez contacter l’éditeur de logiciels indépendant directement et négocier un tarif personnalisé et des spécifications techniques.</span><span class="sxs-lookup"><span data-stu-id="b2af7-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="b2af7-109">Une fois les conditions du plan privé accordées, l’ISV crée un plan pour vous et l’attribue à l’ID de locataire de votre organisation, que vous devez fournir.</span><span class="sxs-lookup"><span data-stu-id="b2af7-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="b2af7-110">Recherche de votre ID de locataire</span><span class="sxs-lookup"><span data-stu-id="b2af7-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="b2af7-111">Dans AppSource, dans le coin supérieur droit, sélectionnez l’icône de votre profil de compte, puis **afficher le locataire**.</span><span class="sxs-lookup"><span data-stu-id="b2af7-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="b2af7-112">Copiez l’ID de locataire et fournissez-le à l’ISV.</span><span class="sxs-lookup"><span data-stu-id="b2af7-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Montre comment rechercher votre ID de locataire.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="b2af7-114">Rechercher un plan privé dans AppSource</span><span class="sxs-lookup"><span data-stu-id="b2af7-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="b2af7-115">Il peut falloir jusqu’à 48 heures après que l’ISV ait publié le nouveau plan privé avant de le voir dans AppSource.</span><span class="sxs-lookup"><span data-stu-id="b2af7-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="b2af7-116">Pour rechercher les plans privés associés à votre ID de locataire, sélectionnez **plans privés** (icône de verrou) en haut à droite de AppSource.</span><span class="sxs-lookup"><span data-stu-id="b2af7-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Affiche l’icône de verrou (cadenas) dans la barre d’outils supérieure.":::

<span data-ttu-id="b2af7-118">Si vous n’êtes pas connecté, un message vous invite à le faire.</span><span class="sxs-lookup"><span data-stu-id="b2af7-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="b2af7-119">Vous pouvez ensuite acheter les plans privés associés à votre ID de locataire sous l’onglet **plans + tarification** .</span><span class="sxs-lookup"><span data-stu-id="b2af7-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Affiche les offres privées sous l’onglet plan et tarification.":::

<span data-ttu-id="b2af7-121">Si des plans privés ne sont pas disponibles pour votre locataire, un message indique que vous n’avez pas de plans ou d’offres privés.</span><span class="sxs-lookup"><span data-stu-id="b2af7-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="b2af7-122">Acheter un plan privé</span><span class="sxs-lookup"><span data-stu-id="b2af7-122">Purchase a private plan</span></span>

<span data-ttu-id="b2af7-123">Un ISV peut inclure un ou plusieurs plans privés au sein d’une offre.</span><span class="sxs-lookup"><span data-stu-id="b2af7-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="b2af7-124">Chaque offre peut avoir des plans publics et privés, mais les plans privés s’affichent sous une page de liste d’offres distincte accessible à partir de l’icône d’offre privée (cadenas) en haut à droite de la page.</span><span class="sxs-lookup"><span data-stu-id="b2af7-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="b2af7-125">Les plans privés disponibles sont affichés sous l’onglet **plans + tarification** . Les plans privés ont un badge bleu distinctif.</span><span class="sxs-lookup"><span data-stu-id="b2af7-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Affiche le badge d’offre privée bleue en regard des offres privées.":::

<span data-ttu-id="b2af7-127">Pour acheter un plan sélectionné, sélectionnez **obtenir maintenant** et suivez les étapes indiquées.</span><span class="sxs-lookup"><span data-stu-id="b2af7-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b2af7-128">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="b2af7-128">Next steps</span></span>

- [<span data-ttu-id="b2af7-129">Qu’est-ce que Microsoft AppSource ?</span><span class="sxs-lookup"><span data-stu-id="b2af7-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
