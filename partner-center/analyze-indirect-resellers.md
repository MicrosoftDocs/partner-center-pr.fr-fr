---
title: Analyser les performances des revendeurs indirects
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Utilisez Analytics pour savoir comment fonctionnent vos revendeurs indirects, à la fois leurs succès et les zones qui peuvent nécessiter plus d’attention.
author: LauraBrenner
ms.author: labrenne
ms.assetid: 4D7DAD9D-4B69-4741-8E80-44256320982E
ms.topic: article
keywords: données métiers
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 72064e3847d30b3049649269618256638b2fe4d8
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83794946"
---
# <a name="use-analytics-to-analyze-performance-of-your-indirect-resellers"></a><span data-ttu-id="0c50f-104">Utiliser Analytics pour analyser les performances de vos revendeurs indirects</span><span class="sxs-lookup"><span data-stu-id="0c50f-104">Use analytics to analyze performance of your indirect resellers</span></span>

<span data-ttu-id="0c50f-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="0c50f-105">**Applies to**</span></span>

- <span data-ttu-id="0c50f-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="0c50f-106">Partner Center</span></span>
- <span data-ttu-id="0c50f-107">Partenaires du programme Fournisseur de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="0c50f-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="0c50f-108">**Rôles appropriés**</span><span class="sxs-lookup"><span data-stu-id="0c50f-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0c50f-109">Administrateur général</span><span class="sxs-lookup"><span data-stu-id="0c50f-109">Global admin</span></span>
- <span data-ttu-id="0c50f-110">Administrateur de la gestion des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0c50f-110">User management admin</span></span>
- <span data-ttu-id="0c50f-111">Agent d’administration</span><span class="sxs-lookup"><span data-stu-id="0c50f-111">Admin agent</span></span>
- <span data-ttu-id="0c50f-112">Agent commercial</span><span class="sxs-lookup"><span data-stu-id="0c50f-112">Sales agent</span></span>

<span data-ttu-id="0c50f-113">Les données prennent des décisions commerciales.</span><span class="sxs-lookup"><span data-stu-id="0c50f-113">Data drives business decisions.</span></span> <span data-ttu-id="0c50f-114">Utilisez les mesures de la page **Reseller Analytics** pour identifier vos réussites, les réussites des revendeurs indirects et les zones qui nécessitent une attention particulière.</span><span class="sxs-lookup"><span data-stu-id="0c50f-114">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="0c50f-115">Utilisez ces informations lorsque vous planifiez de nouveaux objectifs commerciaux.</span><span class="sxs-lookup"><span data-stu-id="0c50f-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="0c50f-116">L’analytique des revendeurs indirects est disponible uniquement pour les partenaires du programme fournisseur de solutions Cloud.</span><span class="sxs-lookup"><span data-stu-id="0c50f-116">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="0c50f-117">Nous effectuons le suivi des mesures suivantes :</span><span class="sxs-lookup"><span data-stu-id="0c50f-117">We are tracking the following metrics:</span></span>

<span data-ttu-id="0c50f-118">**Résumé**</span><span class="sxs-lookup"><span data-stu-id="0c50f-118">**Summary**</span></span>  
 - <span data-ttu-id="0c50f-119">**Total revendeurs**: nombre de revendeurs actifs le dernier jour de l’abonnement</span><span class="sxs-lookup"><span data-stu-id="0c50f-119">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="0c50f-120">**Nouveaux revendeurs**: nombre de nouveaux revendeurs indirects pour la période spécifiée</span><span class="sxs-lookup"><span data-stu-id="0c50f-120">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="0c50f-121">**Revendeurs actifs**: nombre de revendeurs indirects où le MPNID est d’au moins 1 abonnement et où l’état de l’abonnement n’est pas annulé.</span><span class="sxs-lookup"><span data-stu-id="0c50f-121">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="0c50f-122">**Revendeurs**transmettant : nombre de revendeurs indirects avec un abonnement vendu au cours de la période spécifiée</span><span class="sxs-lookup"><span data-stu-id="0c50f-122">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="0c50f-123">**Revendeurs par marché**</span><span class="sxs-lookup"><span data-stu-id="0c50f-123">**Resellers by market**</span></span>  
 - <span data-ttu-id="0c50f-124">Total des revendeurs par emplacement géographique</span><span class="sxs-lookup"><span data-stu-id="0c50f-124">Total resellers by geographic location</span></span>  

<span data-ttu-id="0c50f-125">**Top des revendeurs par abonnements vendus**</span><span class="sxs-lookup"><span data-stu-id="0c50f-125">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="0c50f-126">Liste des revendeurs, triée selon le nombre d’abonnements qu’ils ont vendus</span><span class="sxs-lookup"><span data-stu-id="0c50f-126">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="0c50f-127">**Principaux produits par nombre d’abonnements**</span><span class="sxs-lookup"><span data-stu-id="0c50f-127">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="0c50f-128">**Dynamics 365**: produits Dynamics 365 triés par abonnements vendus</span><span class="sxs-lookup"><span data-stu-id="0c50f-128">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="0c50f-129">**EMS**: nombre d’abonnements aux services de gestion d’entreprise vendus</span><span class="sxs-lookup"><span data-stu-id="0c50f-129">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="0c50f-130">**Microsoft 365**: nombre d’abonnements Microsoft 365 vendus</span><span class="sxs-lookup"><span data-stu-id="0c50f-130">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="0c50f-131">**Office 365**: produits Office 365 triés par abonnements vendus</span><span class="sxs-lookup"><span data-stu-id="0c50f-131">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="0c50f-132">**Nouveaux abonnements**</span><span class="sxs-lookup"><span data-stu-id="0c50f-132">**New subscriptions**</span></span>  
 - <span data-ttu-id="0c50f-133">Nombre de nouveaux abonnements ajoutés par date</span><span class="sxs-lookup"><span data-stu-id="0c50f-133">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="0c50f-134">**Évolution de l’abonnement**</span><span class="sxs-lookup"><span data-stu-id="0c50f-134">**Subscription churn**</span></span>  
 - <span data-ttu-id="0c50f-135">**Nouveaux abonnements**: nombre de nouveaux abonnements ajoutés par date</span><span class="sxs-lookup"><span data-stu-id="0c50f-135">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="0c50f-136">**Abonnements déconfigurés**: nombre d’abonnements annulés ou suspendus par date</span><span class="sxs-lookup"><span data-stu-id="0c50f-136">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="0c50f-137">**Nouveaux détails du revendeur**</span><span class="sxs-lookup"><span data-stu-id="0c50f-137">**New reseller details**</span></span>  
 - <span data-ttu-id="0c50f-138">**Nom du revendeur**: noms des revendeurs indirects</span><span class="sxs-lookup"><span data-stu-id="0c50f-138">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="0c50f-139">**Emplacement**: marchés où les revendeurs indirects fonctionnent</span><span class="sxs-lookup"><span data-stu-id="0c50f-139">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="0c50f-140">**Abonnements**: nombre d’abonnements vendus par le revendeur</span><span class="sxs-lookup"><span data-stu-id="0c50f-140">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="0c50f-141">**Licences**: nombre total de licences vendues par le revendeur pour l’ensemble des abonnements</span><span class="sxs-lookup"><span data-stu-id="0c50f-141">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
  