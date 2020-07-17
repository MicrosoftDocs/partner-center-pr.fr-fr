---
title: Vérifier l’intégrité du service pour un client
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment utiliser l’espace partenaires pour vérifier l’intégrité du service d’un client lorsqu’il rencontre un problème avec un service.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 11ec4cfcfc9326c1e9d6598dce528410c0e02542
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435478"
---
# <a name="check-service-health-for-a-customer-reporting-a-potential-service-problem-or-outage"></a><span data-ttu-id="55a4a-103">Vérifier l’état du service pour qu’un client signale un problème ou une panne de service potentiel</span><span class="sxs-lookup"><span data-stu-id="55a4a-103">Check service health for a customer reporting a potential service problem or outage</span></span>

<span data-ttu-id="55a4a-104">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="55a4a-104">**Applies to**</span></span>

- <span data-ttu-id="55a4a-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="55a4a-105">Partner Center</span></span>

<span data-ttu-id="55a4a-106">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="55a4a-106">**Appropriate roles**</span></span>

- <span data-ttu-id="55a4a-107">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="55a4a-107">Admin agent</span></span>
- <span data-ttu-id="55a4a-108">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="55a4a-108">Global admin</span></span>
- <span data-ttu-id="55a4a-109">Agent du support technique</span><span class="sxs-lookup"><span data-stu-id="55a4a-109">Helpdesk agent</span></span>
- <span data-ttu-id="55a4a-110">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="55a4a-110">Sales agent</span></span>

<span data-ttu-id="55a4a-111">L’une des premières choses que vous pouvez faire lorsqu’un client rencontre des problèmes avec un service est de vérifier l’état du service.</span><span class="sxs-lookup"><span data-stu-id="55a4a-111">One of the first things you can do when a customer is experiencing problems with a service is to check the service health.</span></span> 

## <a name="check-service-health"></a><span data-ttu-id="55a4a-112">Vérifier l’intégrité du service</span><span class="sxs-lookup"><span data-stu-id="55a4a-112">Check service health</span></span>

1. <span data-ttu-id="55a4a-113">Sélectionnez le **client** qui rencontre le problème dans la **liste des clients**.</span><span class="sxs-lookup"><span data-stu-id="55a4a-113">Select the **Customer** that is having the issue from the **Customer list**.</span></span>

2. <span data-ttu-id="55a4a-114">Dans le menu de gauche, sélectionnez **gestion des services** .</span><span class="sxs-lookup"><span data-stu-id="55a4a-114">Select **Service management** from the left menu.</span></span> <span data-ttu-id="55a4a-115">Cela permet de répertorier les services approvisionnés pour le client et l’intégrité du service pour chacun.</span><span class="sxs-lookup"><span data-stu-id="55a4a-115">This will list the services provisioned for the customer and the service health for each.</span></span> <span data-ttu-id="55a4a-116">Les partenaires peuvent cliquer sur le service qui les intéresse pour obtenir plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="55a4a-116">Partners can click the service they are interested in to get more information.</span></span> 

>[!NOTE] 
> <span data-ttu-id="55a4a-117">Les liens d’intégrité du service sur les pages de **gestion des services** prennent le partenaire pour le centre d’administration M365 ou le portail Azure en tant qu' **administrateur délégué**. Une fois que le partenaire a atteint la destination, le partenaire peut accéder aux pages d’intégrité du service dans l’un ou l’autre portail pour plus d’informations sur la panne.</span><span class="sxs-lookup"><span data-stu-id="55a4a-117">Service health links on the **Service management** pages will take the partner to either the M365 admin center or the Azure portal as **delegated admin**. Once the partner gets to either destination, the partner can navigate to the service health pages in either portal for more details about the outage.</span></span>
 
<span data-ttu-id="55a4a-118">Pendant une indisponibilité de service, Microsoft fournit des mises à jour régulières tout au long de la résolution du problème.</span><span class="sxs-lookup"><span data-stu-id="55a4a-118">During a service outage, Microsoft provides regular updates as we work to address the problem.</span></span> <span data-ttu-id="55a4a-119">Ces notifications s’affichent également sur le Portail Microsoft Azure ou le centre d’administration Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55a4a-119">These notifications are also displayed on either the Microsoft Azure portal or the Microsoft 365 admin Center.</span></span>

<span data-ttu-id="55a4a-120">Si le problème persiste après la fin de l’interruption du service, soumettez une demande de service.</span><span class="sxs-lookup"><span data-stu-id="55a4a-120">If the problem persists after the end of the service outage, submit a service request.</span></span> <span data-ttu-id="55a4a-121">Voir [Signaler des problèmes au nom d’un client](report-problems-on-behalf-of-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="55a4a-121">See [Report problems on behalf of a customer](report-problems-on-behalf-of-a-customer.md).</span></span>

<span data-ttu-id="55a4a-122">Microsoft 365 et Microsoft Azure fournissent chacun des [API que les partenaires peuvent utiliser pour récupérer l’intégrité du service en temps réel](get-automated-service-notifications-with-our-apis.md), les communications du centre de messages et les événements de maintenance planifiée.</span><span class="sxs-lookup"><span data-stu-id="55a4a-122">Microsoft 365 and Microsoft Azure each provide [APIs that partners can use to retrieve real-time service health](get-automated-service-notifications-with-our-apis.md), message center communications, and planned maintenance events.</span></span>

 

