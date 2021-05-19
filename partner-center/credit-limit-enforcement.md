---
title: Application d’une limite de crédit
ms.topic: how-to
ms.date: 05/11/2021
description: En savoir plus sur la limite de crédit et la façon dont elle est calculée. Comprend un Forum aux questions.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148106"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="48305-104">Application de la limite de crédit (CLE)</span><span class="sxs-lookup"><span data-stu-id="48305-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="48305-105">**Rôles appropriés**: administrateur de facturation</span><span class="sxs-lookup"><span data-stu-id="48305-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="48305-106">Votre limite de crédit et son fonctionnement</span><span class="sxs-lookup"><span data-stu-id="48305-106">Your credit limit and how it works</span></span>

<span data-ttu-id="48305-107">Votre limite de crédit est le montant maximal (en dollars américains) que vous pouvez consacrer à l’achat de produits ou d’abonnements dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="48305-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="48305-108">Si vous dépassez votre limite de crédit, vous ne pourrez pas effectuer de nouveaux achats tant que vous n’aurez pas effectué un paiement suffisant.</span><span class="sxs-lookup"><span data-stu-id="48305-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="48305-109">Vos abonnements existants vont se poursuivre sans interruption.</span><span class="sxs-lookup"><span data-stu-id="48305-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="48305-110">Les limites de crédit s’appliquent aux offres dans le plan Azure, les réservations Azure, les logiciels, la place de marché, les produits Azure 145 P, Office et Dynamics.</span><span class="sxs-lookup"><span data-stu-id="48305-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="48305-111">Les limites de crédit ne s’appliquent pas aux renouvellements et à la consommation en cours.</span><span class="sxs-lookup"><span data-stu-id="48305-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="48305-112">Nous attribuons votre limite de crédit au niveau du locataire durant votre période d’intégration.</span><span class="sxs-lookup"><span data-stu-id="48305-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="48305-113">Nous la baserons sur les revenus prévus, les prouesses en achetant et l’historique des paiements.</span><span class="sxs-lookup"><span data-stu-id="48305-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="48305-114">Nous utilisons ensuite la formule suivante pour calculer le solde disponible :</span><span class="sxs-lookup"><span data-stu-id="48305-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="48305-115">**[Limite de crédit – (achat entrant + factures non payées en attente + frais non facturés – trop-perçus)]**</span><span class="sxs-lookup"><span data-stu-id="48305-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="48305-116">Forum Aux Questions</span><span class="sxs-lookup"><span data-stu-id="48305-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="48305-117">Ma limite de crédit est-elle définie au niveau du client ou du niveau global ?</span><span class="sxs-lookup"><span data-stu-id="48305-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="48305-118">Niveau du locataire.</span><span class="sxs-lookup"><span data-stu-id="48305-118">The tenant level.</span></span> <span data-ttu-id="48305-119">Par exemple, supposons que vous travaillez à partir des États-Unis, du Canada et du Japon.</span><span class="sxs-lookup"><span data-stu-id="48305-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="48305-120">Si le client canadien atteint sa limite de crédit, ce locataire reçoit une notification lorsqu’il tente d’effectuer un achat dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="48305-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="48305-121">Les autres locataires ne seront pas affectés.</span><span class="sxs-lookup"><span data-stu-id="48305-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="48305-122">Si ma limite de crédit est dépassée, puis-je continuer à traiter les clients et les abonnements existants avec un accès complet ?</span><span class="sxs-lookup"><span data-stu-id="48305-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="48305-123">Oui.</span><span class="sxs-lookup"><span data-stu-id="48305-123">Yes.</span></span> <span data-ttu-id="48305-124">Les abonnements existants de vos clients continueront sans interruption.</span><span class="sxs-lookup"><span data-stu-id="48305-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="48305-125">Toutefois, vous ne pouvez pas acheter de nouveaux abonnements pour vos clients.</span><span class="sxs-lookup"><span data-stu-id="48305-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="48305-126">CLE s’applique-t-elle aux partenaires directs et aux fournisseurs indirects ?</span><span class="sxs-lookup"><span data-stu-id="48305-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="48305-127">Oui, il s’applique aux deux.</span><span class="sxs-lookup"><span data-stu-id="48305-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="48305-128">Après avoir envoyé mon paiement pour rétablir mon compte, quand puis-je acheter des abonnements supplémentaires ?</span><span class="sxs-lookup"><span data-stu-id="48305-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="48305-129">Vous devez être en mesure de reprendre l’achat dans les 24 heures qui suivent votre paiement, en supposant que Microsoft a reçu toutes les conditions requises pour effectuer le processus de vérification de solvabilité.</span><span class="sxs-lookup"><span data-stu-id="48305-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="48305-130">Comment puis-je vérifier la limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="48305-130">How can I check my credit limit?</span></span>

<span data-ttu-id="48305-131">Contactez [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) pour voir votre limite de crédit et obtenir des informations sur les achats récents.</span><span class="sxs-lookup"><span data-stu-id="48305-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="48305-132">Les factures en litige sont-elles associées à la limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="48305-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="48305-133">Oui.</span><span class="sxs-lookup"><span data-stu-id="48305-133">Yes.</span></span> <span data-ttu-id="48305-134">Toutefois, vous pouvez contacter Microsoft à [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) l’adresse pour résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="48305-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="48305-135">À quel moment puis-je me rappeler si j’écris ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="48305-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="48305-136">Vous devez avoir une réponse en moins de 24 heures.</span><span class="sxs-lookup"><span data-stu-id="48305-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="48305-137">Quels critères Microsoft utilise-t-il pour définir la limite de crédit d’un partenaire ?</span><span class="sxs-lookup"><span data-stu-id="48305-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="48305-138">Nous déterminons votre limite de crédit en fonction de vos revenus prévus, de l’acquisition des prouesses et de l’historique des paiements.</span><span class="sxs-lookup"><span data-stu-id="48305-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="48305-139">La limite de crédit est-elle actuellement appliquée à la nouvelle expérience de commerce ?</span><span class="sxs-lookup"><span data-stu-id="48305-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="48305-140">Oui.</span><span class="sxs-lookup"><span data-stu-id="48305-140">Yes.</span></span> <span data-ttu-id="48305-141">Les limites de crédit s’appliquent à tous les programmes et produits CSP dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="48305-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="48305-142">Qui recevra la notification lorsque mon organisation est proche de sa limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="48305-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="48305-143">Le contact financier de votre organisation doit recevoir la notification.</span><span class="sxs-lookup"><span data-stu-id="48305-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="48305-144">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="48305-144">Next steps</span></span>

[<span data-ttu-id="48305-145">Notions de base de facturation</span><span class="sxs-lookup"><span data-stu-id="48305-145">Billing basics</span></span>](./billing-basics.md)
