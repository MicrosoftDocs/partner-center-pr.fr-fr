---
title: Réservations Azure & abonnements au serveur
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les opportunités de fournisseurs de solutions Cloud pour acquérir, approvisionner et gérer des réservations Azure et des abonnements de serveur pour les clients.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000203"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="fc348-103">Acquérir, approvisionner & gérer des instances de machine virtuelle réservées Azure (RI) + abonnements serveur pour les clients</span><span class="sxs-lookup"><span data-stu-id="fc348-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="fc348-104">S’applique à :</span><span class="sxs-lookup"><span data-stu-id="fc348-104">Applies to:</span></span>

- <span data-ttu-id="fc348-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="fc348-105">Partner Center</span></span>

<span data-ttu-id="fc348-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="fc348-106">**Appropriate roles**</span></span>

- <span data-ttu-id="fc348-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="fc348-107">Admin agent</span></span>
- <span data-ttu-id="fc348-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="fc348-108">Global admin</span></span>
- <span data-ttu-id="fc348-109">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="fc348-109">Helpdesk agent</span></span>
- <span data-ttu-id="fc348-110">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="fc348-110">Sales agent</span></span>
- <span data-ttu-id="fc348-111">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fc348-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="fc348-112">Cet article s’applique uniquement aux partenaires du programme fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="fc348-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="fc348-113">Les clients qui utilisent d’autres types d’abonnements (par exemple, paiement à l’utilisation, individuel, contrat de client Microsoft ou abonnements Accord Entreprise) doivent lire [cette documentation Azure reservations](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="fc348-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="fc348-114">Qu’est-ce qu’une réservation Azure ?</span><span class="sxs-lookup"><span data-stu-id="fc348-114">What are Azure Reservations?</span></span>

<span data-ttu-id="fc348-115">Azure Reservations vous aident à économiser de l’argent en prépayeant une machine virtuelle d’un an ou trois ans, SQL Database de la capacité de calcul, le débit Azure Cosmos DB ou d’autres ressources Azure.</span><span class="sxs-lookup"><span data-stu-id="fc348-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="fc348-116">Le prépaiement vous permet d’obtenir une remise sur les ressources que vous utilisez.</span><span class="sxs-lookup"><span data-stu-id="fc348-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="fc348-117">Les réservations peuvent réduire de façon significative votre machine virtuelle, votre calcul SQL Database, Azure Cosmos DB et d’autres coûts de ressources jusqu’à 72% par rapport aux tarifs du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="fc348-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="fc348-118">Des réservations permettent de bénéficier d’une remise sur la facturation et n’ont aucune incidence sur l’état de runtime de vos ressources.</span><span class="sxs-lookup"><span data-stu-id="fc348-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="fc348-119">Pour plus d’informations, voir [qu’est-ce que Azure reservations ?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="fc348-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="fc348-120">Pourquoi les clients doivent-ils acheter une réservation ?</span><span class="sxs-lookup"><span data-stu-id="fc348-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="fc348-121">Si les clients ont des machines virtuelles, des Azure Cosmos DB ou des bases de données SQL qui s’exécutent sur de longues périodes de temps, l’achat d’une réservation leur donne l’option la plus rentable.</span><span class="sxs-lookup"><span data-stu-id="fc348-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="fc348-122">Par exemple, si un client exécute continuellement quatre instances d’un service sans réservation, il est facturé au tarif du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="fc348-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="fc348-123">S’il achète une réservation pour ces ressources, il obtient immédiatement la remise de réservation.</span><span class="sxs-lookup"><span data-stu-id="fc348-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="fc348-124">Les ressources ne sont plus facturées au tarif du paiement à l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="fc348-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="fc348-125">Nouvelle offre Azure intéressante dans CSP</span><span class="sxs-lookup"><span data-stu-id="fc348-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="fc348-126">En apportant des abonnements Azure Reservations et serveur à son programme CSP, Microsoft est plus à même de permettre à ses partenaires de répondre à la demande des clients en constante évolution pour obtenir des solutions plus rentables afin de prendre en charge des charges de travail Cloud hautement prévisibles et persistantes.</span><span class="sxs-lookup"><span data-stu-id="fc348-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="fc348-127">Le programme CSP permet aux partenaires d’acquérir, de configurer et de gérer des abonnements Azure Reservations et serveur pour le compte de clients commerciaux via l’espace partenaires Microsoft et Portail Azure.</span><span class="sxs-lookup"><span data-stu-id="fc348-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="fc348-128">Nous offrons même aux partenaires dans le cadre de notre programme CSP des choix quant à la façon dont les réservations Azure peuvent être achetées.</span><span class="sxs-lookup"><span data-stu-id="fc348-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="fc348-129">Les partenaires CSP peuvent [acheter des réservations Azure pour le compte d’un client](azure-reservations-buying.md) , ou ils peuvent [autoriser le client à acheter ses propres réservations](give-customers-permission.md) à partir d’un abonnement Azure précédent que le partenaire a acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="fc348-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="fc348-130">Azure Reservations offrir aux clients la flexibilité de la virtualisation pour un large éventail de solutions informatiques, y compris le développement et les tests, l’exécution d’applications et l’extension du centre de données.</span><span class="sxs-lookup"><span data-stu-id="fc348-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="fc348-131">Avec [Azure reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) par exemple, les clients commerciaux peuvent désormais économiser jusqu’à 72% par rapport à la tarification des machines virtuelles Azure de paiement à l’utilisation en achetant ou en « reservant »-l’ordinateur virtuel pour une période de 1 ou 3 ans.</span><span class="sxs-lookup"><span data-stu-id="fc348-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="fc348-132">Les clients Windows Server avec Azure Hybrid Benefit, inclus avec Software Assurance, pourront économiser jusqu’à 80% par rapport au tarif du paiement à l’accès.</span><span class="sxs-lookup"><span data-stu-id="fc348-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="fc348-133">Avec une combinaison non appariée de tarification attrayante et une flexibilité de déploiement inégalée, les clients verront la meilleure valeur globale lorsqu’ils choisissent Azure Reservations :</span><span class="sxs-lookup"><span data-stu-id="fc348-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="fc348-134">Réservations Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-134">Azure reservations</span></span>

- <span data-ttu-id="fc348-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="fc348-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="fc348-136">Réservations SQL DB</span><span class="sxs-lookup"><span data-stu-id="fc348-136">SQL DB Reservations</span></span>
- <span data-ttu-id="fc348-137">Instance managée SQL</span><span class="sxs-lookup"><span data-stu-id="fc348-137">SQL Managed Instance</span></span>
- <span data-ttu-id="fc348-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc348-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="fc348-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="fc348-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="fc348-140">App Services</span><span class="sxs-lookup"><span data-stu-id="fc348-140">App Services</span></span>
- <span data-ttu-id="fc348-141">Azure Databricks des réservations d’unités</span><span class="sxs-lookup"><span data-stu-id="fc348-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="fc348-142">Disque managé</span><span class="sxs-lookup"><span data-stu-id="fc348-142">Managed Disk</span></span>
- <span data-ttu-id="fc348-143">Objet blob de blocs</span><span class="sxs-lookup"><span data-stu-id="fc348-143">Block blob</span></span>
- <span data-ttu-id="fc348-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="fc348-144">MySQL</span></span>
- <span data-ttu-id="fc348-145">Explorateur de données Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-145">Azure Data explorer</span></span>
- <span data-ttu-id="fc348-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="fc348-146">MariaDB</span></span>
- <span data-ttu-id="fc348-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="fc348-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="fc348-148">Abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="fc348-148">Server subscriptions</span></span>

- <span data-ttu-id="fc348-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="fc348-149">Windows Server</span></span>
- <span data-ttu-id="fc348-150">Cal Services Bureau à distance (RDS)</span><span class="sxs-lookup"><span data-stu-id="fc348-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="fc348-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="fc348-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="fc348-152">Abonnements annuels ISV Linux</span><span class="sxs-lookup"><span data-stu-id="fc348-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="fc348-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="fc348-153">SUSE Linux</span></span>
- <span data-ttu-id="fc348-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="fc348-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="fc348-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="fc348-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="fc348-156">Abonnements annuels ISV</span><span class="sxs-lookup"><span data-stu-id="fc348-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="fc348-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="fc348-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="fc348-158">Prise en main</span><span class="sxs-lookup"><span data-stu-id="fc348-158">Getting started</span></span>

<span data-ttu-id="fc348-159">Pour comprendre comment positionner Azure Reservations avec vos clients et que vous êtes opérationnel aussi rapidement que possible, nous vous recommandons l’approche suivante pour passer en revue les matériaux de préparation :</span><span class="sxs-lookup"><span data-stu-id="fc348-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="fc348-160">Passez en revue les présentations et les webinaires associés à la proposition de valeur client et au positionnement</span><span class="sxs-lookup"><span data-stu-id="fc348-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="fc348-161">Examiner et comprendre le Guide d’exploitation moderne du commerce</span><span class="sxs-lookup"><span data-stu-id="fc348-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="fc348-162">Passer en revue les questions fréquentes sur Azure RI et les abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="fc348-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="fc348-163">Comprendre les mises à jour pour les Azure Reservations et les abonnements serveur dans l' [API espace partenaires (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="fc348-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="fc348-164">Ressources</span><span class="sxs-lookup"><span data-stu-id="fc348-164">Resources</span></span>

<span data-ttu-id="fc348-165">Vous trouverez ci-dessous une liste complète des ressources qui vous aideront à intégrer rapidement Azure Reservations via l’espace partenaires :</span><span class="sxs-lookup"><span data-stu-id="fc348-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="fc348-166">Préparation des ventes</span><span class="sxs-lookup"><span data-stu-id="fc348-166">Sales readiness</span></span>

- [<span data-ttu-id="fc348-167">Vue d’ensemble des abonnements Azure Reservations et serveur avec Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="fc348-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="fc348-168">Feuille de ventes</span><span class="sxs-lookup"><span data-stu-id="fc348-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="fc348-169">FAQ sur les partenaires pour Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="fc348-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="fc348-170">FAQ sur les partenaires pour Azure Reservations et SQL DB</span><span class="sxs-lookup"><span data-stu-id="fc348-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="fc348-171">Licence d’accès client (CAL) Services Bureau à distance (RDS) (annonce)</span><span class="sxs-lookup"><span data-stu-id="fc348-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="fc348-172">Azure Reserved VM Instances (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="fc348-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="fc348-173">Abonnements serveur</span><span class="sxs-lookup"><span data-stu-id="fc348-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="fc348-174">Vue d’ensemble de SQL DB dans Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="fc348-175">Réservations SQL DB (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="fc348-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="fc348-176">Azure Cosmos DB (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="fc348-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="fc348-177">Managed Instance SQL (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="fc348-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="fc348-178">SUSE et Red Hat Enterprise Linux (Portail Azure)</span><span class="sxs-lookup"><span data-stu-id="fc348-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="fc348-179">Red Hat Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="fc348-180">SUSE Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="fc348-181">Linux sur Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="fc348-182">Présentation de la tarification Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="fc348-183">Calcul des coûts Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="fc348-184">Azure Databricks des réservations d’unités</span><span class="sxs-lookup"><span data-stu-id="fc348-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="fc348-185">Tarifs CSP : les listes de prix des **abonnements** Microsoft Azure et des **instances réservées** sont situées dans la page tarifs de l’espace partenaires [& offres](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="fc348-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="fc348-186">Formation</span><span class="sxs-lookup"><span data-stu-id="fc348-186">Training</span></span>

<span data-ttu-id="fc348-187">Inscrivez-vous pour consulter les [webinaires commerciaux](https://commercial-licensing.eventbuilder.com/FY2019_ALL) et les événements à la demande.</span><span class="sxs-lookup"><span data-stu-id="fc348-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="fc348-188">Les événements à la demande de disponibilité des licences incluent des rubriques telles que :</span><span class="sxs-lookup"><span data-stu-id="fc348-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="fc348-189">Services en ligne CSP, CSP Azure et mises à jour de licences générales, y compris Azure (novembre 2018)</span><span class="sxs-lookup"><span data-stu-id="fc348-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="fc348-190">Capacité réservée de la base de SQL SQL & flexibilité de taille d’instance (août 2018)</span><span class="sxs-lookup"><span data-stu-id="fc348-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="fc348-191">Abonnements serveur dans CSP (juillet 2018)</span><span class="sxs-lookup"><span data-stu-id="fc348-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="fc348-192">Vue d’ensemble de Azure Reservations dans CSP (mai 2018)</span><span class="sxs-lookup"><span data-stu-id="fc348-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="fc348-193">D’autres formations utiles incluent le [module de licence Azure sur l’Université partenaire](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="fc348-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="fc348-194">Operations</span><span class="sxs-lookup"><span data-stu-id="fc348-194">Operations</span></span>

- <span data-ttu-id="fc348-195">[Guide des opérations du commerce moderne](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (mis à jour) : Guide complet couvrant la stratégie clé et les aspects opérationnels, tels que les contrats, le classement via l’espace partenaires, la facture, les détails des tarifs, les incentives, le fichier de rapprochement, les API/SDK, le bac à sable et les services partagés partenaires Azure.</span><span class="sxs-lookup"><span data-stu-id="fc348-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="fc348-196">Matrice de disponibilité des pays et devise client pour les offres modernes</span><span class="sxs-lookup"><span data-stu-id="fc348-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="fc348-197">Vendre Microsoft Azure des instances réservées</span><span class="sxs-lookup"><span data-stu-id="fc348-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="fc348-198">Acheter des réservations Microsoft Azure pour vos clients</span><span class="sxs-lookup"><span data-stu-id="fc348-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="fc348-199">Gérer des réservations Azure pour le compte de vos clients</span><span class="sxs-lookup"><span data-stu-id="fc348-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="fc348-200">Facturation des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="fc348-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="fc348-201">Dimensionnement d’une machine virtuelle en vue d’une utilisation optimale de la réservation</span><span class="sxs-lookup"><span data-stu-id="fc348-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="fc348-202">API espace partenaires (API/Kit de développement logiciel)</span><span class="sxs-lookup"><span data-stu-id="fc348-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="fc348-203">Services Bureau à distance</span><span class="sxs-lookup"><span data-stu-id="fc348-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="fc348-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="fc348-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="fc348-205">Le [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) vous permet de valoriser vos licences Windows Server et d’économiser jusqu’à \* 47% sur les machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="fc348-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="fc348-206">Vous pouvez tirer parti de tels avantages avec les licences Édition Standard et Windows Server Datacenter prises en charge avec Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="fc348-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="fc348-207">Selon l’édition, vous pouvez convertir ou réutiliser vos licences pour exécuter des machines virtuelles Windows Server dans Azure et payer un taux de calcul de base inférieur (taux de machines virtuelles Linux).</span><span class="sxs-lookup"><span data-stu-id="fc348-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="fc348-208">Voir aussi [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="fc348-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="fc348-209">\* Les économies réelles peuvent varier en fonction de la région, du type d’instance ou de l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="fc348-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
