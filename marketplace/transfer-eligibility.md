---
title: 'Éligibilité du transfert : instructions pour le transfert d’un abonnement entre comptes de facturation, place de marché Azure'
description: Instructions pour les contrôles commerciaux avant le transfert d’un abonnement entre les comptes de facturation dans le Portail Azure.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007153"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="9a4c3-103">Éligibilité du transfert pour un abonnement entre des comptes de facturation</span><span class="sxs-lookup"><span data-stu-id="9a4c3-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="9a4c3-104">Vous pouvez [transférer un abonnement](/azure/cost-management-billing/understand/subscription-transfer) d’un compte de facturation à un autre dans la section facturation du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="9a4c3-105">Avant un transfert, l’abonnement est analysé pour rechercher les produits tiers.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="9a4c3-106">Le transfert est autorisé uniquement si *tous les* produits sont désactivés pour le transfert (voir les [critères](#criteria-for-transfer-approval-or-denial) ci-dessous).</span><span class="sxs-lookup"><span data-stu-id="9a4c3-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="9a4c3-107">Le système génère des messages d’erreur pertinents pour les applications dont l’effacement a échoué pour vous aider à déterminer les étapes suivantes.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="9a4c3-108">Cet article ne s’applique pas aux offres SaaS, car les ressources SaaS sont attachées à un locataire, et non à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="9a4c3-109">Les ressources SaaS peuvent être transférées d’un compte de facturation à un autre, mais cette opération est effectuée par ressource et par le support Azure en tant que demande de support.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="9a4c3-110">Critères d’approbation ou de refus de transfert</span><span class="sxs-lookup"><span data-stu-id="9a4c3-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="9a4c3-111">Vous ne pouvez pas transférer un abonnement si l’une de ses applications tierces répond à l’un des critères suivants :</span><span class="sxs-lookup"><span data-stu-id="9a4c3-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="9a4c3-112">Le compte cible est commercial et l’application est refusée pour être vendue via des partenaires.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="9a4c3-113">L’application est sélectionnée pour les partenaires sélectionnés et le compte cible ne figure pas dans la liste verte.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="9a4c3-114">L’offre était une offre préliminaire dans le passé pour les abonnements sélectionnés ou était une offre privée et l’abonnement ne figure plus dans la liste verte.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="9a4c3-115">Le nouveau compte de facturation est dans une région différente de celle où l’offre est vendue et l’offre ne doit pas être vendue dans cette région.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="9a4c3-116">Un transfert bloqué reste en vigueur jusqu’à ce que vous supprimiez la ressource de l’abonnement, après quoi vous pouvez réessayer le transfert.</span><span class="sxs-lookup"><span data-stu-id="9a4c3-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9a4c3-117">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="9a4c3-117">Next steps</span></span>

[<span data-ttu-id="9a4c3-118">Obtenir de l’aide pour Microsoft AppSource et la place de marché Azure</span><span class="sxs-lookup"><span data-stu-id="9a4c3-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

