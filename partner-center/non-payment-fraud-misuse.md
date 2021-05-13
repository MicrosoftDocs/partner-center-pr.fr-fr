---
title: Gestion des défauts de paiement, des fraudes ou des mauvaises utilisations
description: Découvrez les différents risques impliqués dans les transactions en ligne et les meilleures pratiques pour gérer et atténuer ces risques dans l’espace partenaires.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818658"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="30c52-103">Gestion des défauts de paiement, des fraudes ou des utilisations abusives dans l’Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="30c52-103">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="30c52-104">**S’applique à**: espace partenaires | Espace partenaires pour Microsoft Cloud pour le gouvernement des États-Unis</span><span class="sxs-lookup"><span data-stu-id="30c52-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="30c52-105">**Rôles appropriés**: administrateur général | Administrateur de gestion des utilisateurs | Agent d’administration | Administrateur de facturation</span><span class="sxs-lookup"><span data-stu-id="30c52-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Billing admin</span></span>

<span data-ttu-id="30c52-106">Vous êtes financièrement responsable des achats frauduleux de vos clients et/ou du non-paiement des services achetés par les clients.</span><span class="sxs-lookup"><span data-stu-id="30c52-106">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="30c52-107">Par conséquent, *nous vous recommandons vivement de mettre en place les contrôles d’atténuation des risques de prévention et de détection des fraudes*.</span><span class="sxs-lookup"><span data-stu-id="30c52-107">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="30c52-108">Pour éviter et/ou résoudre les problèmes d’activité ou de mauvaise utilisation frauduleuses, il est important de comprendre les risques potentiels et de développer des stratégies et des pratiques qui peuvent réduire votre exposition.</span><span class="sxs-lookup"><span data-stu-id="30c52-108">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="30c52-109">Application de la stratégie d’utilisation acceptable de Microsoft</span><span class="sxs-lookup"><span data-stu-id="30c52-109">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="30c52-110">Si Microsoft détecte une activité de partenaire ou de client que nous confirmons ou soupçonnons de violer la stratégie d’utilisation acceptable, nous allons prendre des mesures d’application.</span><span class="sxs-lookup"><span data-stu-id="30c52-110">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="30c52-111">Le client peut être immédiatement suspendu.</span><span class="sxs-lookup"><span data-stu-id="30c52-111">The customer could be immediately suspended.</span></span> <span data-ttu-id="30c52-112">Vous serez averti des actions de mise en œuvre ou mises à jour sur vos demandes par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30c52-112">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="30c52-113">Abus des risques de service</span><span class="sxs-lookup"><span data-stu-id="30c52-113">Abuse of service risks</span></span>

<span data-ttu-id="30c52-114">L' **abus des risques de service** signifie que les clients utilisent des services Cloud en violation de la stratégie d’utilisation acceptable de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30c52-114">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="30c52-115">Exemples d’abus de service</span><span class="sxs-lookup"><span data-stu-id="30c52-115">Examples of abuse of service</span></span>

<span data-ttu-id="30c52-116">Voici quelques exemples de violations de la stratégie d’utilisation acceptable de Microsoft :</span><span class="sxs-lookup"><span data-stu-id="30c52-116">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="30c52-117">Courriers indésirables</span><span class="sxs-lookup"><span data-stu-id="30c52-117">Spamming</span></span>
- <span data-ttu-id="30c52-118">Piratage</span><span class="sxs-lookup"><span data-stu-id="30c52-118">Hacking</span></span>
- <span data-ttu-id="30c52-119">Attaques par déni de service distribué (DDoS)</span><span class="sxs-lookup"><span data-stu-id="30c52-119">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="30c52-120">Exploration de données Bitcoin</span><span class="sxs-lookup"><span data-stu-id="30c52-120">Bitcoin mining</span></span>
- <span data-ttu-id="30c52-121">Distribution de logiciels malveillants</span><span class="sxs-lookup"><span data-stu-id="30c52-121">Malware distribution</span></span>
- <span data-ttu-id="30c52-122">Revente d’abonnements piratés</span><span class="sxs-lookup"><span data-stu-id="30c52-122">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="30c52-123">Vol de risques de service</span><span class="sxs-lookup"><span data-stu-id="30c52-123">Theft of service risks</span></span>

<span data-ttu-id="30c52-124">Le **vol de risques de service** signifie que les clients n’ont pas l’intention de payer des services consommés.</span><span class="sxs-lookup"><span data-stu-id="30c52-124">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="30c52-125">Ce vol peut impliquer l’utilisation de moyens de paiement volés, le fait de fournir des informations de facturation erronées et/ou la valeur par défaut des soldes en suspens.</span><span class="sxs-lookup"><span data-stu-id="30c52-125">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="30c52-126">Exemples de vol de service</span><span class="sxs-lookup"><span data-stu-id="30c52-126">Examples of service theft</span></span>

<span data-ttu-id="30c52-127">Voici quelques exemples de ces risques de transactions en ligne :</span><span class="sxs-lookup"><span data-stu-id="30c52-127">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="30c52-128">Transactions qui ne se produisent pas en personne (transactions de « carte de crédit absentes »)</span><span class="sxs-lookup"><span data-stu-id="30c52-128">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="30c52-129">Identités déreprésentéees</span><span class="sxs-lookup"><span data-stu-id="30c52-129">Misrepresented identities</span></span>
- <span data-ttu-id="30c52-130">Services approvisionnés et utilisés avant la réception du paiement initial</span><span class="sxs-lookup"><span data-stu-id="30c52-130">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="30c52-131">Marchés émergents et/ou régions à risque élevé pour la fraude en ligne</span><span class="sxs-lookup"><span data-stu-id="30c52-131">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="30c52-132">Automatiser la création et l’achat de comptes par des acteurs incorrects</span><span class="sxs-lookup"><span data-stu-id="30c52-132">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="30c52-133">Gestion des risques en ligne</span><span class="sxs-lookup"><span data-stu-id="30c52-133">Managing online risk</span></span>

<span data-ttu-id="30c52-134">Vous pouvez utiliser les recommandations suivantes pour vous aider à développer des stratégies et des pratiques pour réduire votre exposition aux risques de transactions en ligne dans le cycle de vie de vos relations client.</span><span class="sxs-lookup"><span data-stu-id="30c52-134">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="30c52-135">Intégration de nouveaux clients</span><span class="sxs-lookup"><span data-stu-id="30c52-135">Onboarding new customers</span></span>

<span data-ttu-id="30c52-136">Les suggestions pour réduire les risques en ligne lors de l’intégration de nouveaux clients sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="30c52-136">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="30c52-137">Établissez des relations personnelles avec les clients lorsque cela est possible (par exemple, en contactant les clients par téléphone).</span><span class="sxs-lookup"><span data-stu-id="30c52-137">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="30c52-138">Vérifiez les informations d’identification et l’arrière-plan des clients via de meilleures méthodes (par exemple, en utilisant des bureaux de crédit ou des agences de rapports commerciaux commerciaux).</span><span class="sxs-lookup"><span data-stu-id="30c52-138">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="30c52-139">Utilisez Multi-Factor Authentication (par exemple, la vérification SMS) lors de l’inscription pour réduire l’exposition à la création et à l’achat d’un compte robotique.</span><span class="sxs-lookup"><span data-stu-id="30c52-139">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="30c52-140">Gérez et suivez les identités à l’aide de services (tels que les services d’identité numérique).</span><span class="sxs-lookup"><span data-stu-id="30c52-140">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="30c52-141">Évaluez la force financière du client par le biais de systèmes de détection des fraudes de carte de crédit rigoureux.</span><span class="sxs-lookup"><span data-stu-id="30c52-141">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="30c52-142">Établissez une stratégie effacer les regroupements.</span><span class="sxs-lookup"><span data-stu-id="30c52-142">Establish a clear collections policy.</span></span> <span data-ttu-id="30c52-143">Détaillez votre processus de collecte et lorsque l’accès aux abonnements sera affecté par un non-paiement.</span><span class="sxs-lookup"><span data-stu-id="30c52-143">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="30c52-144">(Vous pouvez désactiver l’accès ou [suspendre les abonnements d’un client](create-a-new-subscription.md#suspend-a-subscription) en cas de non-paiement.)</span><span class="sxs-lookup"><span data-stu-id="30c52-144">(You can disable access or [suspend a customer's subscriptions](create-a-new-subscription.md#suspend-a-subscription) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="30c52-145">Gestion des comptes client</span><span class="sxs-lookup"><span data-stu-id="30c52-145">Managing customer accounts</span></span>

<span data-ttu-id="30c52-146">Les suggestions relatives à la gestion des comptes clients après achat sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="30c52-146">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="30c52-147">Implémentez un processus pour recevoir, examiner, agir et répondre rapidement aux notifications Microsoft.</span><span class="sxs-lookup"><span data-stu-id="30c52-147">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="30c52-148">Collaborez avec les clients pour comprendre leurs besoins en matière d’utilisation du Cloud, tout en définissant les seuils d’analyse appropriés.</span><span class="sxs-lookup"><span data-stu-id="30c52-148">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="30c52-149">(Par exemple, vous pouvez [définir un budget de dépenses Azure mensuel](set-an-azure-spending-budget-for-your-customers.md) dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="30c52-149">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="30c52-150">Cette compréhension vous permet de surveiller l’utilisation des clients pendant le mois et de recevoir une notification lorsque les clients sont proches de leur budget.)</span><span class="sxs-lookup"><span data-stu-id="30c52-150">This understanding allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="30c52-151">Surveillez régulièrement les [journaux d’activité des clients](activity-logs.md) pour faciliter la détection des fraudes.</span><span class="sxs-lookup"><span data-stu-id="30c52-151">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="30c52-152">Effectuez une action rapide lorsque des activités suspectes sont détectées.</span><span class="sxs-lookup"><span data-stu-id="30c52-152">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="30c52-153">Évitez de fournir aux clients un accès administratif complet aux abonnements sans implémenter au préalable les contrôles d’atténuation des risques.</span><span class="sxs-lookup"><span data-stu-id="30c52-153">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="30c52-154">Gestion de la facturation client</span><span class="sxs-lookup"><span data-stu-id="30c52-154">Managing customer billing</span></span>

<span data-ttu-id="30c52-155">Les suggestions relatives à la gestion de la facturation cliente après achat sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="30c52-155">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="30c52-156">Demander des prépaiements avant les transactions initiales et la facturation.</span><span class="sxs-lookup"><span data-stu-id="30c52-156">Request prepayments prior to initial transactions and billing.</span></span>
- <span data-ttu-id="30c52-157">N’acceptez pas les instruments de paiement à haut risque (tels que les cartes prépayées ou les cartes de valeur stockées).</span><span class="sxs-lookup"><span data-stu-id="30c52-157">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="30c52-158">Surveillez les paiements des clients et les comptes chrono.</span><span class="sxs-lookup"><span data-stu-id="30c52-158">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="30c52-159">Appliquez de manière agressive des processus rappels standardisés pour des paiements tardifs ou un non-paiement.</span><span class="sxs-lookup"><span data-stu-id="30c52-159">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="30c52-160">Pour plus d’informations sur les stratégies de réduction des risques en ligne, consultez le Guide de gestion des risques pour les [transactions en ligne.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span><span class="sxs-lookup"><span data-stu-id="30c52-160">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span></span>
