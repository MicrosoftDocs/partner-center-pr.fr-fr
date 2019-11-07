---
title: Calcul du crédit gagné par le partenaire | Espace partenaires
ms.topic: article
ms.date: 09/17/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Calcul du calcul de l’aspect du crédit gagné du partenaire Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 402ee0e2084191c7d4f592dd91480be8e1bd0341
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653721"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="bd820-103">Mode de calcul du crédit gagné (PEC) du partenaire</span><span class="sxs-lookup"><span data-stu-id="bd820-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="bd820-104">Les partenaires qui possèdent la gestion des opérations informatiques 24/24 h des pièces ou la totalité de l’environnement Azure de leurs clients dans CSP sont récompensés avec PEC.</span><span class="sxs-lookup"><span data-stu-id="bd820-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="bd820-105">Le PEC est fourni dans le cadre de la facture au partenaire qui a une relation de facturation directe avec Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bd820-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="bd820-106">Le crédit est calculé quotidiennement et reflété dans la facture mensuelle.</span><span class="sxs-lookup"><span data-stu-id="bd820-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="bd820-107">Par défaut, dans CSP, les partenaires reçoivent les droits d’accès nécessaires à l’abonnement du client, ce qui leur permet d’avoir une gestion et un contrôle des opérations 24h/24 et 7j/7 des ressources sur l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="bd820-107">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="bd820-108">Les autres façons dont le client peut configurer l’accès pour un partenaire de transaction sont décrites dans la section suivante.</span><span class="sxs-lookup"><span data-stu-id="bd820-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="bd820-109">Exigences importantes en matière de calcul et d’éligibilité :</span><span class="sxs-lookup"><span data-stu-id="bd820-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="bd820-110">Un partenaire doit avoir un accord MPN actif et un rôle de compte basé sur les règles C (RBAC) valide pour recevoir le crédit des ressources Azure qu’il gère.</span><span class="sxs-lookup"><span data-stu-id="bd820-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="bd820-111">En savoir plus sur les [rôles RBAC valides]</span><span class="sxs-lookup"><span data-stu-id="bd820-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="bd820-112">Le fournisseur indirect est éligible pour PEC s’il ou son revendeur indirect, ou les deux, disposent d’un contrôle opérationnel et d’une gestion opérationnelles 24/24 h des ressources Azure du client dans CSP.</span><span class="sxs-lookup"><span data-stu-id="bd820-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="bd820-113">Le PEC est associé à la consommation facturée de l’espace Azure du client dans le CSP géré par le partenaire.</span><span class="sxs-lookup"><span data-stu-id="bd820-113">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="bd820-114">PEC est disponible uniquement pour les partenaires du CSP qui sont facturés par Microsoft (fournisseur indirect et partenaire direct Bill).</span><span class="sxs-lookup"><span data-stu-id="bd820-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="bd820-115">Services éligibles : le crédit gagné par le partenaire s’applique à toute la consommation Azure 1PP Azure indiquée dans la liste de prix.</span><span class="sxs-lookup"><span data-stu-id="bd820-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="bd820-116">Il existe des exceptions, notamment, 3PP et Azure Reservations.</span><span class="sxs-lookup"><span data-stu-id="bd820-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="bd820-117">Le PEC est calculé quotidiennement et peut être affiché dans le fichier de rapprochement quotidien.</span><span class="sxs-lookup"><span data-stu-id="bd820-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="bd820-118">Un partenaire (fournisseur ou revendeur (par le biais de son fournisseur) doit avoir accès à la journée entière (24h/24, 7j/7) pour s’assurer qu’il gagne du PEC.</span><span class="sxs-lookup"><span data-stu-id="bd820-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="bd820-119">Le PEC est réalisé au niveau de la ressource Azure.</span><span class="sxs-lookup"><span data-stu-id="bd820-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="bd820-120">Si le partenaire dispose d’un accès valide au niveau de l’abonnement ou du groupe de ressources, chaque ressource dont le rôle est supérieur à l’entité supérieure gagnera le PEC.</span><span class="sxs-lookup"><span data-stu-id="bd820-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="bd820-121">Le PEC sera inclus sur la facture mensuelle du partenaire.</span><span class="sxs-lookup"><span data-stu-id="bd820-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="bd820-122">La facture est nette de frais.</span><span class="sxs-lookup"><span data-stu-id="bd820-122">The invoice is net of charges.</span></span> <span data-ttu-id="bd820-123">Les détails sont affichés dans le fichier de rapprochement des factures.</span><span class="sxs-lookup"><span data-stu-id="bd820-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="bd820-124">Pour plus d’informations sur l’accès à la gestion des abonnements Azure et sur la liaison de votre ID MPN aux rôles RBAC, consultez [gérer les abonnements et les ressources sous le plan Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="bd820-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="bd820-125">Pour plus d’informations</span><span class="sxs-lookup"><span data-stu-id="bd820-125">For more information</span></span>

- [<span data-ttu-id="bd820-126">Plan Azure-facturation</span><span class="sxs-lookup"><span data-stu-id="bd820-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="bd820-127">Tarifs de la nouvelle expérience de commerce pour les fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="bd820-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)