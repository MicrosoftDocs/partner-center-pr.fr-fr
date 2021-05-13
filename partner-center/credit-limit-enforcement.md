---
title: Application de la limite de crédit
ms.topic: how-to
ms.date: 05/11/2021
description: En savoir plus sur la limite de crédit et la façon dont elle est calculée. Comprend un Forum aux questions.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819207"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="4f687-104">Application de la limite de crédit (CLE)</span><span class="sxs-lookup"><span data-stu-id="4f687-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="4f687-105">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="4f687-105">**Appropriate roles**</span></span>

- <span data-ttu-id="4f687-106">Administrateur de la facturation</span><span class="sxs-lookup"><span data-stu-id="4f687-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="4f687-107">Votre limite de crédit et son fonctionnement</span><span class="sxs-lookup"><span data-stu-id="4f687-107">Your credit limit and how it works</span></span>

<span data-ttu-id="4f687-108">Votre limite de crédit est le montant maximal (en dollars américains) que vous pouvez consacrer à l’achat de produits ou d’abonnements dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="4f687-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="4f687-109">Si vous dépassez votre limite de crédit, vous ne pourrez pas effectuer de nouveaux achats tant que vous n’aurez pas effectué un paiement suffisant.</span><span class="sxs-lookup"><span data-stu-id="4f687-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="4f687-110">Vos abonnements existants vont se poursuivre sans interruption.</span><span class="sxs-lookup"><span data-stu-id="4f687-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="4f687-111">Les limites de crédit s’appliquent aux offres dans le plan Azure, les réservations Azure, les logiciels, la place de marché, les produits Azure 145 P, Office et Dynamics.</span><span class="sxs-lookup"><span data-stu-id="4f687-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="4f687-112">Les limites de crédit ne s’appliquent pas aux renouvellements et à la consommation en cours.</span><span class="sxs-lookup"><span data-stu-id="4f687-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="4f687-113">Nous attribuons votre limite de crédit au niveau du locataire durant votre période d’intégration.</span><span class="sxs-lookup"><span data-stu-id="4f687-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="4f687-114">Nous la baserons sur les revenus prévus, les prouesses en achetant et l’historique des paiements.</span><span class="sxs-lookup"><span data-stu-id="4f687-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="4f687-115">Nous utilisons ensuite la formule suivante pour calculer le solde disponible :</span><span class="sxs-lookup"><span data-stu-id="4f687-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="4f687-116">**[Limite de crédit – (achat entrant + factures non payées en attente + frais non facturés – trop-perçus)]**</span><span class="sxs-lookup"><span data-stu-id="4f687-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="4f687-117">Forum Aux Questions</span><span class="sxs-lookup"><span data-stu-id="4f687-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="4f687-118">Ma limite de crédit est-elle définie au niveau du client ou du niveau global ?</span><span class="sxs-lookup"><span data-stu-id="4f687-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="4f687-119">Niveau du locataire.</span><span class="sxs-lookup"><span data-stu-id="4f687-119">The tenant level.</span></span> <span data-ttu-id="4f687-120">Par exemple, supposons que vous travaillez à partir des États-Unis, du Canada et du Japon.</span><span class="sxs-lookup"><span data-stu-id="4f687-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="4f687-121">Si le client canadien atteint sa limite de crédit, ce locataire reçoit une notification lorsqu’il tente d’effectuer un achat dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="4f687-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="4f687-122">Les autres locataires ne seront pas affectés.</span><span class="sxs-lookup"><span data-stu-id="4f687-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="4f687-123">Si ma limite de crédit est dépassée, puis-je continuer à traiter les clients et les abonnements existants avec un accès complet ?</span><span class="sxs-lookup"><span data-stu-id="4f687-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="4f687-124">Oui.</span><span class="sxs-lookup"><span data-stu-id="4f687-124">Yes.</span></span> <span data-ttu-id="4f687-125">Les abonnements existants de vos clients continueront sans interruption.</span><span class="sxs-lookup"><span data-stu-id="4f687-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="4f687-126">Toutefois, vous ne pouvez pas acheter de nouveaux abonnements pour vos clients.</span><span class="sxs-lookup"><span data-stu-id="4f687-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="4f687-127">CLE s’applique-t-elle aux partenaires directs et aux fournisseurs indirects ?</span><span class="sxs-lookup"><span data-stu-id="4f687-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="4f687-128">Oui, il s’applique aux deux.</span><span class="sxs-lookup"><span data-stu-id="4f687-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="4f687-129">Après avoir envoyé mon paiement pour rétablir mon compte, quand puis-je acheter des abonnements supplémentaires ?</span><span class="sxs-lookup"><span data-stu-id="4f687-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="4f687-130">Vous devez être en mesure de reprendre l’achat dans les 24 heures qui suivent votre paiement, en supposant que Microsoft a reçu toutes les conditions requises pour effectuer le processus de vérification de solvabilité.</span><span class="sxs-lookup"><span data-stu-id="4f687-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="4f687-131">Comment puis-je vérifier la limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="4f687-131">How can I check my credit limit?</span></span>

<span data-ttu-id="4f687-132">Contactez [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) pour voir votre limite de crédit et obtenir des informations sur les achats récents.</span><span class="sxs-lookup"><span data-stu-id="4f687-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="4f687-133">Les factures en litige sont-elles associées à la limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="4f687-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="4f687-134">Oui.</span><span class="sxs-lookup"><span data-stu-id="4f687-134">Yes.</span></span> <span data-ttu-id="4f687-135">Toutefois, vous pouvez contacter Microsoft à [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) l’adresse pour résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="4f687-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="4f687-136">À quel moment puis-je me rappeler si j’écris ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="4f687-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="4f687-137">Vous devez avoir une réponse en moins de 24 heures.</span><span class="sxs-lookup"><span data-stu-id="4f687-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="4f687-138">Quels critères Microsoft utilise-t-il pour définir la limite de crédit d’un partenaire ?</span><span class="sxs-lookup"><span data-stu-id="4f687-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="4f687-139">Nous déterminons votre limite de crédit en fonction de vos revenus prévus, de l’acquisition des prouesses et de l’historique des paiements.</span><span class="sxs-lookup"><span data-stu-id="4f687-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="4f687-140">La limite de crédit est-elle actuellement appliquée à la nouvelle expérience de commerce ?</span><span class="sxs-lookup"><span data-stu-id="4f687-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="4f687-141">Oui.</span><span class="sxs-lookup"><span data-stu-id="4f687-141">Yes.</span></span> <span data-ttu-id="4f687-142">Les limites de crédit s’appliquent à tous les programmes et produits CSP dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="4f687-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="4f687-143">Qui recevra la notification lorsque mon organisation est proche de sa limite de crédit ?</span><span class="sxs-lookup"><span data-stu-id="4f687-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="4f687-144">Le contact financier de votre organisation doit recevoir la notification.</span><span class="sxs-lookup"><span data-stu-id="4f687-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4f687-145">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="4f687-145">Next steps</span></span>

[<span data-ttu-id="4f687-146">Notions de base de facturation</span><span class="sxs-lookup"><span data-stu-id="4f687-146">Billing basics</span></span>](./billing-basics.md)
