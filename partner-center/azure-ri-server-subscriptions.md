---
title: Réservations Azure & abonnements au serveur
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les opportunités de fournisseurs de solutions Cloud pour acquérir, approvisionner et gérer des réservations Azure et des abonnements de serveur pour les clients.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, abonnements, machine virtuelle, réservation, instance réservée
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4e5e5d88b1f629b07932d37dedb70d0309a26dce
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198627"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="5b2c8-104">Acquérir, approvisionner & gérer des instances de machine virtuelle réservées Azure (RI) + abonnements serveur pour les clients</span><span class="sxs-lookup"><span data-stu-id="5b2c8-104">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="5b2c8-105">S’applique à :</span><span class="sxs-lookup"><span data-stu-id="5b2c8-105">Applies to:</span></span>

- <span data-ttu-id="5b2c8-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="5b2c8-106">Partner Center</span></span>

<span data-ttu-id="5b2c8-107">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="5b2c8-107">**Appropriate roles**</span></span>

- <span data-ttu-id="5b2c8-108">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="5b2c8-108">Admin agent</span></span>
- <span data-ttu-id="5b2c8-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="5b2c8-109">Global admin</span></span>
- <span data-ttu-id="5b2c8-110">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="5b2c8-110">Helpdesk agent</span></span>
- <span data-ttu-id="5b2c8-111">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="5b2c8-111">Sales agent</span></span>
- <span data-ttu-id="5b2c8-112">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="5b2c8-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="5b2c8-113">Qu’est-ce qu’une réservation Azure ?</span><span class="sxs-lookup"><span data-stu-id="5b2c8-113">What are Azure Reservations?</span></span>

<span data-ttu-id="5b2c8-114">Azure Reservations vous aident à économiser de l’argent en prépayeant une machine virtuelle d’un an ou trois ans, SQL Database de la capacité de calcul, le débit Azure Cosmos DB ou d’autres ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="5b2c8-115">Le prépaiement vous permet d’obtenir une remise sur les ressources que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="5b2c8-116">Les réservations peuvent réduire de façon significative votre machine virtuelle, votre calcul SQL Database, Azure Cosmos DB et d’autres coûts de ressources jusqu’à 72% par rapport aux tarifs du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="5b2c8-117">Des réservations permettent de bénéficier d’une remise sur la facturation et n’ont aucune incidence sur l’état de runtime de vos ressources.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="5b2c8-118">Pour plus d’informations, voir [qu’est-ce que Azure reservations ?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-118">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="5b2c8-119">Pourquoi les clients doivent-ils acheter une réservation ?</span><span class="sxs-lookup"><span data-stu-id="5b2c8-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="5b2c8-120">Si les clients ont des machines virtuelles, des Azure Cosmos DB ou des bases de données SQL qui s’exécutent sur de longues périodes de temps, l’achat d’une réservation leur donne l’option la plus rentable.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="5b2c8-121">Par exemple, si un client exécute continuellement quatre instances d’un service sans réservation, il est facturé au tarif du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="5b2c8-122">S’il achète une réservation pour ces ressources, il obtient immédiatement la remise de réservation.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="5b2c8-123">Les ressources ne sont plus facturées au tarif du paiement à l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="5b2c8-124">Nouvelle offre Azure intéressante dans CSP</span><span class="sxs-lookup"><span data-stu-id="5b2c8-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="5b2c8-125">En apportant des abonnements Azure Reservations et serveur à son programme CSP, Microsoft est plus à même de permettre à ses partenaires de répondre à la demande des clients en constante évolution pour obtenir des solutions plus rentables afin de prendre en charge des charges de travail Cloud hautement prévisibles et persistantes.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="5b2c8-126">Le programme CSP permet aux partenaires d’acquérir, de configurer et de gérer des abonnements Azure Reservations et serveur pour le compte de clients commerciaux via l’espace partenaires Microsoft et Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-126">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="5b2c8-127">Nous offrons même aux partenaires dans le cadre de notre programme CSP des choix quant à la façon dont les réservations Azure peuvent être achetées.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-127">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="5b2c8-128">Les partenaires CSP peuvent [acheter des réservations Azure pour le compte d’un client](azure-reservations-buying.md) , ou ils peuvent [autoriser le client à acheter ses propres réservations](give-customers-permission.md) à partir d’un abonnement Azure précédent que le partenaire a acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-128">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="5b2c8-129">Azure Reservations offrir aux clients la flexibilité de la virtualisation pour un large éventail de solutions informatiques, y compris le développement et les tests, l’exécution d’applications et l’extension du centre de données.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="5b2c8-130">Avec [Azure reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) par exemple, les clients commerciaux peuvent désormais économiser jusqu’à 72% par rapport à la tarification des machines virtuelles Azure de paiement à l’utilisation en achetant ou en « reservant »-l’ordinateur virtuel pour une période de 1 ou 3 ans.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-130">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="5b2c8-131">Les clients Windows Server avec Azure Hybrid Benefit, inclus avec Software Assurance, pourront économiser jusqu’à 80% par rapport au tarif du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-131">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="5b2c8-132">Avec une combinaison non appariée de tarification attrayante et une flexibilité de déploiement inégalée, les clients verront la meilleure valeur globale lorsqu’ils choisissent Azure Reservations :</span><span class="sxs-lookup"><span data-stu-id="5b2c8-132">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="5b2c8-133">Réservations Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-133">Azure reservations</span></span>

- <span data-ttu-id="5b2c8-134">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="5b2c8-134">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="5b2c8-135">Réservations SQL DB</span><span class="sxs-lookup"><span data-stu-id="5b2c8-135">SQL DB Reservations</span></span>
- <span data-ttu-id="5b2c8-136">Instance managée SQL</span><span class="sxs-lookup"><span data-stu-id="5b2c8-136">SQL Managed Instance</span></span>
- <span data-ttu-id="5b2c8-137">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5b2c8-137">Azure Cosmos DB</span></span>
- <span data-ttu-id="5b2c8-138">Azure SQL Data Warehouse.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-138">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="5b2c8-139">App Services</span><span class="sxs-lookup"><span data-stu-id="5b2c8-139">App Services</span></span>
- <span data-ttu-id="5b2c8-140">Azure Databricks des réservations d’unités</span><span class="sxs-lookup"><span data-stu-id="5b2c8-140">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="5b2c8-141">Disque managé</span><span class="sxs-lookup"><span data-stu-id="5b2c8-141">Managed Disk</span></span>
- <span data-ttu-id="5b2c8-142">Objet blob de blocs</span><span class="sxs-lookup"><span data-stu-id="5b2c8-142">Block blob</span></span>
- <span data-ttu-id="5b2c8-143">MySQL</span><span class="sxs-lookup"><span data-stu-id="5b2c8-143">MySQL</span></span>
- <span data-ttu-id="5b2c8-144">Explorateur de données Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-144">Azure Data explorer</span></span>
- <span data-ttu-id="5b2c8-145">MariaDB</span><span class="sxs-lookup"><span data-stu-id="5b2c8-145">MariaDB</span></span>
- <span data-ttu-id="5b2c8-146">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="5b2c8-146">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="5b2c8-147">Abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="5b2c8-147">Server subscriptions</span></span>

- <span data-ttu-id="5b2c8-148">Windows Server</span><span class="sxs-lookup"><span data-stu-id="5b2c8-148">Windows Server</span></span>
- <span data-ttu-id="5b2c8-149">Cal Services Bureau à distance (RDS)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-149">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="5b2c8-150">SQL Server</span><span class="sxs-lookup"><span data-stu-id="5b2c8-150">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="5b2c8-151">Abonnements annuels ISV Linux</span><span class="sxs-lookup"><span data-stu-id="5b2c8-151">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="5b2c8-152">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="5b2c8-152">SUSE Linux</span></span>
- <span data-ttu-id="5b2c8-153">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="5b2c8-153">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="5b2c8-154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="5b2c8-154">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="5b2c8-155">Abonnements annuels ISV</span><span class="sxs-lookup"><span data-stu-id="5b2c8-155">ISV annual subscriptions</span></span>

- <span data-ttu-id="5b2c8-156">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="5b2c8-156">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="5b2c8-157">Mise en route</span><span class="sxs-lookup"><span data-stu-id="5b2c8-157">Getting started</span></span>

<span data-ttu-id="5b2c8-158">Pour comprendre comment positionner Azure Reservations avec vos clients et que vous êtes opérationnel aussi rapidement que possible, nous vous recommandons l’approche suivante pour passer en revue les matériaux de préparation :</span><span class="sxs-lookup"><span data-stu-id="5b2c8-158">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="5b2c8-159">Passez en revue les présentations et les webinaires associés à la proposition de valeur client et au positionnement</span><span class="sxs-lookup"><span data-stu-id="5b2c8-159">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="5b2c8-160">Examiner et comprendre le Guide d’exploitation moderne du commerce</span><span class="sxs-lookup"><span data-stu-id="5b2c8-160">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="5b2c8-161">Passer en revue les questions fréquentes sur Azure RI et les abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="5b2c8-161">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="5b2c8-162">Comprendre les mises à jour pour les Azure Reservations et les abonnements serveur dans l' [API espace partenaires (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-162">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="5b2c8-163">Ressources</span><span class="sxs-lookup"><span data-stu-id="5b2c8-163">Resources</span></span>

<span data-ttu-id="5b2c8-164">Vous trouverez ci-dessous une liste complète des ressources qui vous aideront à intégrer rapidement Azure Reservations via l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="5b2c8-164">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="5b2c8-165">Préparation des ventes</span><span class="sxs-lookup"><span data-stu-id="5b2c8-165">Sales readiness</span></span>

- [<span data-ttu-id="5b2c8-166">Vue d’ensemble des abonnements Azure Reservations et serveur avec Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="5b2c8-166">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="5b2c8-167">Feuille de ventes</span><span class="sxs-lookup"><span data-stu-id="5b2c8-167">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="5b2c8-168">FAQ sur les partenaires pour Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="5b2c8-168">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="5b2c8-169">FAQ sur les partenaires pour Azure Reservations et SQL DB</span><span class="sxs-lookup"><span data-stu-id="5b2c8-169">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="5b2c8-170">Licence d’accès client (CAL) Services Bureau à distance (RDS) (annonce)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-170">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="5b2c8-171">Azure Reserved VM Instances (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-171">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="5b2c8-172">Abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="5b2c8-172">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="5b2c8-173">Vue d’ensemble de SQL DB dans Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-173">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="5b2c8-174">Réservations SQL DB (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-174">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="5b2c8-175">Azure Cosmos DB (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-175">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="5b2c8-176">Managed Instance SQL (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-176">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="5b2c8-177">SUSE et Red Hat Enterprise Linux (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-177">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="5b2c8-178">Red Hat Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-178">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="5b2c8-179">SUSE Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-179">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="5b2c8-180">Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-180">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="5b2c8-181">Présentation de la tarification Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-181">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="5b2c8-182">Calcul des coûts Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-182">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="5b2c8-183">Azure Databricks des réservations d’unités</span><span class="sxs-lookup"><span data-stu-id="5b2c8-183">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="5b2c8-184">Tarifs CSP : les listes de prix des **abonnements** Microsoft Azure et des **instances réservées** sont situées dans la page tarifs de l’espace partenaires [& offres](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="5b2c8-184">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="5b2c8-185">Entrainement</span><span class="sxs-lookup"><span data-stu-id="5b2c8-185">Training</span></span>

<span data-ttu-id="5b2c8-186">Inscrivez-vous pour consulter les [webinaires commerciaux](https://commercial-licensing.eventbuilder.com/FY2019_ALL) et les événements à la demande.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-186">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="5b2c8-187">Les événements à la demande de disponibilité des licences incluent des rubriques telles que :</span><span class="sxs-lookup"><span data-stu-id="5b2c8-187">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="5b2c8-188">Services en ligne CSP, CSP Azure et mises à jour de licences générales, y compris Azure (novembre 2018)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-188">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="5b2c8-189">Capacité réservée de la base de SQL SQL & flexibilité de taille d’instance (août 2018)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-189">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="5b2c8-190">Abonnements serveur dans CSP (juillet 2018)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-190">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="5b2c8-191">Vue d’ensemble de Azure Reservations dans CSP (mai 2018)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-191">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="5b2c8-192">D’autres formations utiles incluent le [module de licence Azure sur l’Université partenaire](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="5b2c8-192">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="5b2c8-193">Operations</span><span class="sxs-lookup"><span data-stu-id="5b2c8-193">Operations</span></span>

- <span data-ttu-id="5b2c8-194">[Guide des opérations du commerce moderne](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (mis à jour) : Guide complet couvrant la stratégie clé et les aspects opérationnels, tels que les contrats, le classement via l’espace partenaires, la facture, les détails des tarifs, les incentives, le fichier de rapprochement, les API/SDK, le bac à sable et les services partagés partenaires Azure.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-194">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="5b2c8-195">Matrice de disponibilité des pays et devise client pour les offres modernes</span><span class="sxs-lookup"><span data-stu-id="5b2c8-195">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="5b2c8-196">Vendre Microsoft Azure des instances réservées</span><span class="sxs-lookup"><span data-stu-id="5b2c8-196">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="5b2c8-197">Acheter des réservations Microsoft Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="5b2c8-197">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="5b2c8-198">Gérer des réservations Azure pour le compte de vos clients</span><span class="sxs-lookup"><span data-stu-id="5b2c8-198">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="5b2c8-199">Facturation des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="5b2c8-199">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="5b2c8-200">Dimensionnement d’une machine virtuelle en vue d’une utilisation optimale de la réservation</span><span class="sxs-lookup"><span data-stu-id="5b2c8-200">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="5b2c8-201">API espace partenaires (API/Kit de développement logiciel)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-201">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="5b2c8-202">Services Bureau à distance</span><span class="sxs-lookup"><span data-stu-id="5b2c8-202">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="5b2c8-203">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="5b2c8-203">Azure Hybrid Benefit</span></span>

<span data-ttu-id="5b2c8-204">Le [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) vous permet de valoriser vos licences Windows Server et d’économiser jusqu’à \* 47% sur les machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-204">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="5b2c8-205">Vous pouvez tirer parti de tels avantages avec les licences Édition Standard et Windows Server Datacenter prises en charge avec Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-205">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="5b2c8-206">Selon l’édition, vous pouvez convertir ou réutiliser vos licences pour exécuter des machines virtuelles Windows Server dans Azure et payer un taux de calcul de base inférieur (taux de machines virtuelles Linux).</span><span class="sxs-lookup"><span data-stu-id="5b2c8-206">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="5b2c8-207">Voir aussi [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="5b2c8-207">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="5b2c8-208">\* Les économies réelles peuvent varier en fonction de la région, du type d’instance ou de l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="5b2c8-208">\*Actual savings may vary based on region, instance type, or usage.</span></span>
