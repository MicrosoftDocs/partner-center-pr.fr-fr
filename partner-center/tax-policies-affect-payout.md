---
title: Impact des stratégies de taxes sur le paiement pour la place de marché Azure
description: Découvrez comment les stratégies de taxes affectent le paiement pour la place de marché Azure.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758455"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="c973e-103">Impact des stratégies de taxes sur le paiement pour la place de marché Azure</span><span class="sxs-lookup"><span data-stu-id="c973e-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="c973e-104">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="c973e-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="c973e-105">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="c973e-105">Global admin</span></span>
-    <span data-ttu-id="c973e-106">Administrateur des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="c973e-106">User admin</span></span>
-    <span data-ttu-id="c973e-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="c973e-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="c973e-108">Introduction</span><span class="sxs-lookup"><span data-stu-id="c973e-108">Introduction</span></span>

<span data-ttu-id="c973e-109">La place de marché commercial Microsoft a une portée mondiale.</span><span class="sxs-lookup"><span data-stu-id="c973e-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="c973e-110">Les transactions se produisent dans les limites et selon l’emplacement de l’ISV et du client, les implications fiscales peuvent varier.</span><span class="sxs-lookup"><span data-stu-id="c973e-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="c973e-111">Microsoft AppSource et la place de marché Azure utilisent les informations de profil fiscal de l’espace partenaires pour déterminer le pays de l’ISV.</span><span class="sxs-lookup"><span data-stu-id="c973e-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="c973e-112">Pour déterminer le pays du client, utilisez les informations de facturation du client ou, si le client se trouve dans l’Union européenne, nous utilisons deux informations différentes.</span><span class="sxs-lookup"><span data-stu-id="c973e-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="c973e-113">Pour mieux comprendre les scénarios suivants, reportez-vous à la table des [Détails fiscaux](tax-details-marketplace.md) , qui indique si Microsoft collecte et paye les taxes pour le compte du serveur de publication ou si cette responsabilité appartient au serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="c973e-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="c973e-114">Tous les exemples de valeurs de vente et de taxes dans cette rubrique sont fournis à titre d’illustration uniquement, pas des chiffres exacts.</span><span class="sxs-lookup"><span data-stu-id="c973e-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="c973e-115">Le serveur de publication transagit dans le pays d’imposition géré par Microsoft</span><span class="sxs-lookup"><span data-stu-id="c973e-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="c973e-116">**Scénario A** : transactions qui ont lieu entre un serveur de publication et un client dans un [pays d’imposition géré par Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="c973e-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="c973e-117">La taxe applicable sera ajoutée à ces transactions au moment de la vente et Microsoft envoie cette taxe au pays concerné.</span><span class="sxs-lookup"><span data-stu-id="c973e-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="c973e-118">Aucun impôt n’est retenu du paiement et les calculs de paiement sont des taxes exclusives.</span><span class="sxs-lookup"><span data-stu-id="c973e-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="c973e-119">Consultez le [scénario D](#foreign-publisher-transacts-with-us-customer) pour les transactions entre un serveur de publication non US et un client américain.</span><span class="sxs-lookup"><span data-stu-id="c973e-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="c973e-121">Le serveur de publication transagit dans un pays d’imposition géré par Microsoft, où les frais relatifs au marché sont imposables</span><span class="sxs-lookup"><span data-stu-id="c973e-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="c973e-122">**Scénario B** : transactions qui ont lieu entre un serveur de publication basé aux États-Unis (tel que défini par les informations de profil d’imposition de l’espace partenaires) à un client d’un pays d’imposition géré par Microsoft, où le pays impose une taxe sur les frais de la place de marché (un service imposable).</span><span class="sxs-lookup"><span data-stu-id="c973e-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="c973e-123">Dans ce scénario, les taxes sur les frais de service du magasin sont soustraites du paiement de l’éditeur.</span><span class="sxs-lookup"><span data-stu-id="c973e-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="c973e-125">Le serveur de publication transagit dans le pays d’imposition géré par l’éditeur</span><span class="sxs-lookup"><span data-stu-id="c973e-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="c973e-126">**Scénario C** : transactions qui ont lieu entre un serveur de publication et un client d’un pays d’imposition géré par un éditeur qui n’impose pas d’impôt à la retenue sur les clients.</span><span class="sxs-lookup"><span data-stu-id="c973e-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="c973e-127">Les clients ne paient aucune taxe au point de vente et il s’agit de l’obligation de l’éditeur de payer toutes les taxes applicables.</span><span class="sxs-lookup"><span data-stu-id="c973e-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="c973e-128">Pour plus d’informations sur la tarification spécifique aux pays (par exemple, pour compenser la fiscalité à venir), consultez les [plans et la tarification des offres de la place de marché commercial](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="c973e-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Affiche le flux de travail pour le scénario de processus de paiement C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="c973e-130">Le serveur de publication étranger transagit avec le client US</span><span class="sxs-lookup"><span data-stu-id="c973e-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="c973e-131">**Scénario D** : tous les serveurs de publication étrangers (tels que définis par leurs informations de profil d’imposition de l’espace partenaires) dans les pays sans traité des États-Unis (voir le [scénario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) faisant une vente à un client basé aux États-Unis (comme défini par l’adresse de son compte client).</span><span class="sxs-lookup"><span data-stu-id="c973e-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="c973e-132">Le gouvernement des États-Unis requiert que Microsoft retenu la taxe de la part du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="c973e-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="c973e-133">Les taxes retenues du paiement au serveur de publication sont calculées en fonction du prix de l’offre.</span><span class="sxs-lookup"><span data-stu-id="c973e-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Affiche le flux de travail du scénario de processus de paiement D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="c973e-135">Un serveur de publication étranger avec un traité transagit avec le client américain</span><span class="sxs-lookup"><span data-stu-id="c973e-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="c973e-136">**Scénario E** : tous les serveurs de publication étrangers (tels que définis par leurs informations de profil d’imposition de l’espace partenaires) dans les pays avec un traité des États-Unis faisant l’acquisition d’une vente à un client basé aux États-Unis (comme défini par l’adresse de son compte client).</span><span class="sxs-lookup"><span data-stu-id="c973e-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="c973e-137">Le gouvernement des États-Unis ne demande pas à Microsoft de retenir une taxe pour le compte du serveur de publication.</span><span class="sxs-lookup"><span data-stu-id="c973e-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Affiche le flux de travail du scénario de processus de paiement E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="c973e-139">Le serveur de publication étranger vend à un client inscrit à la TVA UE dans un pays géré par Microsoft (en dehors de l’Irlande)</span><span class="sxs-lookup"><span data-stu-id="c973e-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="c973e-140">**Scénario F** : toutes les transactions entre les éditeurs étrangers et les clients inscrits à la TVA UE (en dehors de l’Irlande) dans un pays Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="c973e-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="c973e-141">Le client ne paie pas d’impôt sur la vente.</span><span class="sxs-lookup"><span data-stu-id="c973e-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Affiche le flux de travail du scénario de processus de paiement F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="c973e-143">Le serveur de publication étranger vend à un client inscrit à la TVA UE dans un pays géré par Microsoft (en Irlande)</span><span class="sxs-lookup"><span data-stu-id="c973e-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="c973e-144">**Scénario G** – toutes les transactions entre les serveurs de publication étrangers et les clients inscrits à la TVA UE (à l’Irlande) dans un Microsoft-Managed pays.</span><span class="sxs-lookup"><span data-stu-id="c973e-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="c973e-145">Le client paie la TVA irlandaise et Microsoft paie cette taxe au gouvernement irlandais.</span><span class="sxs-lookup"><span data-stu-id="c973e-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Affiche le flux de travail du scénario de processus de paiement G.":::

## <a name="next-steps"></a><span data-ttu-id="c973e-147">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c973e-147">Next steps</span></span>

- [<span data-ttu-id="c973e-148">FAQ sur l’éditeur</span><span class="sxs-lookup"><span data-stu-id="c973e-148">Publisher FAQ</span></span>](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="c973e-149">Instructions pour créer des profils de paiement et de taxes</span><span class="sxs-lookup"><span data-stu-id="c973e-149">Instructions to create payment and tax profiles</span></span>](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
