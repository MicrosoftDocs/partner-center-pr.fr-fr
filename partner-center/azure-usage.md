---
title: Microsoft Azure le dimensionnement de la machine virtuelle pour une utilisation maximale de la réservation | Espace partenaires
ms.topic: article
ms.date: 04/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment ajuster la taille d’une machine virtuelle aux besoins informatiques de vos clients lorsque vous achetez Microsoft Azure réservations pour eux.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, réservations, machine virtuelle, gérer, utilisation, dimensionnement
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: f214a3dd507370f37347d4e014059367f13c5669
ms.sourcegitcommit: 53476b7837192fa4d60470bd5b99e5355e7e48c0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/28/2020
ms.locfileid: "82205777"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="69aa3-104">Dimensionnement des machines virtuelles Microsoft Azure pour une utilisation maximale de la réservation</span><span class="sxs-lookup"><span data-stu-id="69aa3-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="69aa3-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="69aa3-105">**Applies to**</span></span>

- <span data-ttu-id="69aa3-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-106">Partner Center</span></span>
- <span data-ttu-id="69aa3-107">Portail Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-107">Azure portal</span></span>
- <span data-ttu-id="69aa3-108">Partenaires dans CSP</span><span class="sxs-lookup"><span data-stu-id="69aa3-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="69aa3-109">Déterminer la taille de machine virtuelle pour la réservation Azure d’un client</span><span class="sxs-lookup"><span data-stu-id="69aa3-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="69aa3-110">Lorsque vous achetez Microsoft Azure réservations pour le compte de vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée pour répondre aux besoins informatiques du client.</span><span class="sxs-lookup"><span data-stu-id="69aa3-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="69aa3-111">Vous pouvez trouver ces informations à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69aa3-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="69aa3-112">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-112">Azure utilization API</span></span>
- <span data-ttu-id="69aa3-113">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-113">The Azure portal</span></span>
- <span data-ttu-id="69aa3-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="69aa3-114">Azure PowerShell</span></span>
- <span data-ttu-id="69aa3-115">API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="69aa3-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="69aa3-116">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="69aa3-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="69aa3-117">Une fois que vous avez acheté une réservation, la remise de réservation est appliquée automatiquement aux machines virtuelles correspondant aux attributs et à la quantité de la réservation.</span><span class="sxs-lookup"><span data-stu-id="69aa3-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="69aa3-118">Vous n’avez pas besoin d’affecter la réservation à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="69aa3-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="69aa3-119">Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.</span><span class="sxs-lookup"><span data-stu-id="69aa3-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="69aa3-120">Pour identifier correctement le type et la taille de la machine virtuelle à acheter pour le compte de votre client, vous devez utiliser l’une des méthodes décrites ci-dessous, car le type de série de machines virtuelles ne s’affiche pas correctement dans les fichiers de rapprochement de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="69aa3-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="69aa3-121">**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API d’utilisation Azure**</span><span class="sxs-lookup"><span data-stu-id="69aa3-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="69aa3-122">Utilisez la valeur de l’attribut ServiceType de additionalInfo dans la réponse de l’API pour identifier la taille de machine virtuelle à acheter.</span><span class="sxs-lookup"><span data-stu-id="69aa3-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="69aa3-123">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="69aa3-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="69aa3-124">**Obtient les informations de dimensionnement de machine virtuelle à l’aide du Portail Microsoft Azure**</span><span class="sxs-lookup"><span data-stu-id="69aa3-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="69aa3-125">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="69aa3-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="69aa3-126">Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="69aa3-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="69aa3-127">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="69aa3-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="69aa3-128">Sélectionnez **machines virtuelles** dans le menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="69aa3-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="69aa3-129">Sur la page de détails de la machine virtuelle, recherchez les informations relatives à la taille et à la région, comme illustré ci-dessous, et utilisez ces informations pour acheter la réservation dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="69aa3-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Informations sur la taille et la région sur la page de détails](images/usage1.png)

<span data-ttu-id="69aa3-131">**Récupération d’informations de dimensionnement de machine virtuelle à l’aide de Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="69aa3-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="69aa3-132">Utilisez les informations de l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="69aa3-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Emplacement et taille de la machine virtuelle](images/usage2.png)

<span data-ttu-id="69aa3-134">**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API Azure Resource Manager (ARM)**</span><span class="sxs-lookup"><span data-stu-id="69aa3-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="69aa3-135">À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="69aa3-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="69aa3-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/Providers/Microsoft.Compute/virtualMachines/<VM Instance Name>? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="69aa3-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="69aa3-137">L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="69aa3-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="69aa3-138">![valeur de](images/usage3.png) ![l’emplacement de la valeur vmSize](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="69aa3-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span></span>

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="69aa3-139">Vérifier l’utilisation de la machine virtuelle Azure et la remise de réservation</span><span class="sxs-lookup"><span data-stu-id="69aa3-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="69aa3-140">Une fois que vous avez acheté une instance de machine virtuelle réservée Azure pour le compte d’un client, la remise pour le paiement à l’avance pour l’espace de la machine virtuelle est automatiquement appliquée aux machines virtuelles qui correspondent aux attributs et à la quantité de la réservation du client.</span><span class="sxs-lookup"><span data-stu-id="69aa3-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="69aa3-141">Vous pouvez vérifier l’utilisation de la réservation du client et déterminer les machines virtuelles auxquelles les remises de réservation sont appliquées à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="69aa3-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="69aa3-142">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-142">The Azure portal</span></span>
- <span data-ttu-id="69aa3-143">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-143">Azure utilization API</span></span>

<span data-ttu-id="69aa3-144">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="69aa3-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="69aa3-145">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="69aa3-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="69aa3-146">Vérifier l’utilisation de la réservation du client dans le Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="69aa3-147">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="69aa3-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="69aa3-148">Recherchez le client dont vous souhaitez vérifier la remise de réservation et l’utilisation, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="69aa3-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="69aa3-149">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="69aa3-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="69aa3-150">Sélectionnez **réservations** dans le menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="69aa3-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="69aa3-151">Sur la page **vue d’ensemble** , vérifiez le graphique d’utilisation de la réservation, qui indique la quantité de réservation appliquée aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="69aa3-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="69aa3-152">Les données d’utilisation peuvent être retardées de 8 heures.</span><span class="sxs-lookup"><span data-stu-id="69aa3-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="69aa3-153">a.</span><span class="sxs-lookup"><span data-stu-id="69aa3-153">a.</span></span> <span data-ttu-id="69aa3-154">Si l’utilisation de la réservation est de 100%, votre client obtient toutes les économies possibles que l’achat de réservation peut fournir.</span><span class="sxs-lookup"><span data-stu-id="69aa3-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="69aa3-155">b.</span><span class="sxs-lookup"><span data-stu-id="69aa3-155">b.</span></span> <span data-ttu-id="69aa3-156">Si l’utilisation de la réservation est de 0%, la remise n’est pas appliquée à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="69aa3-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="69aa3-157">c.</span><span class="sxs-lookup"><span data-stu-id="69aa3-157">c.</span></span> <span data-ttu-id="69aa3-158">Si l’utilisation de la réservation est comprise entre 1% et 99%, il existe des avantages inutilisés.</span><span class="sxs-lookup"><span data-stu-id="69aa3-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="69aa3-159">Pour éviter cette situation, déterminez la taille de machine virtuelle appropriée pour prendre en charge les besoins informatiques du client avant d’effectuer l’achat.</span><span class="sxs-lookup"><span data-stu-id="69aa3-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="69aa3-160">Vérifier l’utilisation de la réservation du client avec l’API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="69aa3-161">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="69aa3-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="69aa3-162">Vous pouvez obtenir des données d’utilisation de réservation avec l’API d’utilisation d’Azure pour vérifier que le client obtient la remise de réservation et pour connaître les machines virtuelles (machines virtuelles) auxquelles la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="69aa3-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="69aa3-163">Comparez l’exemple A à l’exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.</span><span class="sxs-lookup"><span data-stu-id="69aa3-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

![Exemples d’utilisation de la réservation](images/usage5.png)

- <span data-ttu-id="69aa3-165">Le réservation identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="69aa3-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="69aa3-166">Le compteur est le MeterId de la machine virtuelle à laquelle la remise de réservation est appliquée.</span><span class="sxs-lookup"><span data-stu-id="69aa3-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="69aa3-167">Le ReservationMeter affiche le coût de $0, car la remise de réservation a été appliquée.</span><span class="sxs-lookup"><span data-stu-id="69aa3-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="69aa3-168">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="69aa3-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="69aa3-169">Les coûts des logiciels, tels que Microsoft Windows Server, ne sont actuellement pas inclus dans le prix d’une réservation de machine virtuelle et apparaissent sous la forme d’éléments de ligne distincts dans l’enregistrement de commande et sur votre facture.</span><span class="sxs-lookup"><span data-stu-id="69aa3-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="69aa3-170">Toutefois, si un client dispose de la Azure Hybrid Use Benefit, les frais liés aux logiciels ne seront pas appliqués.</span><span class="sxs-lookup"><span data-stu-id="69aa3-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="69aa3-171">Pour plus d’informations, consultez [coûts des logiciels Windows non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="69aa3-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="69aa3-172">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="69aa3-172">Azure reservations resources</span></span>

|<span data-ttu-id="69aa3-173">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="69aa3-173">**For information about**</span></span>   |<span data-ttu-id="69aa3-174">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="69aa3-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="69aa3-175">Vue d’ensemble des réservations Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="69aa3-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="69aa3-176">Vendre Microsoft Azure des instances de machines virtuelles réservées</span><span class="sxs-lookup"><span data-stu-id="69aa3-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="69aa3-177">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="69aa3-178">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="69aa3-179">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="69aa3-180">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="69aa3-181">Achat de réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="69aa3-182">[Acompte pour les machines virtuelles avec Azure reserved VM instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="69aa3-183">Gestion des réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="69aa3-184">[Gérer des instances de machine virtuelle réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="69aa3-185">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="69aa3-186">[Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="69aa3-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="69aa3-187">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="69aa3-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="69aa3-188">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="69aa3-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
