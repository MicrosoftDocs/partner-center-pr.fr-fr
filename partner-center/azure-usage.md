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
ms.openlocfilehash: 05a041ae794270430b6e2ed7b72ff48b04018601
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453276"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="8fb8b-104">Dimensionnement des machines virtuelles Microsoft Azure pour une utilisation maximale de la réservation</span><span class="sxs-lookup"><span data-stu-id="8fb8b-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="8fb8b-105">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-105">**Applies to**</span></span>

- <span data-ttu-id="8fb8b-106">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-106">Partner Center</span></span>
- <span data-ttu-id="8fb8b-107">Portail Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-107">Azure portal</span></span>
- <span data-ttu-id="8fb8b-108">Partenaires dans CSP</span><span class="sxs-lookup"><span data-stu-id="8fb8b-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="8fb8b-109">Déterminer la taille de machine virtuelle pour la réservation Azure d’un client</span><span class="sxs-lookup"><span data-stu-id="8fb8b-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="8fb8b-110">Lorsque vous achetez Microsoft Azure réservations pour le compte de vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée pour répondre aux besoins informatiques du client.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="8fb8b-111">Vous pouvez trouver ces informations à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8fb8b-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="8fb8b-112">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-112">Azure utilization API</span></span>
- <span data-ttu-id="8fb8b-113">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-113">The Azure portal</span></span>
- <span data-ttu-id="8fb8b-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="8fb8b-114">Azure PowerShell</span></span>
- <span data-ttu-id="8fb8b-115">API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="8fb8b-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="8fb8b-116">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="8fb8b-117">Une fois que vous avez acheté une réservation, la remise de réservation est appliquée automatiquement aux machines virtuelles correspondant aux attributs et à la quantité de la réservation.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="8fb8b-118">Vous n’avez pas besoin d’affecter la réservation à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="8fb8b-119">Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="8fb8b-120">Pour identifier correctement le type et la taille de la machine virtuelle à acheter pour le compte de votre client, vous devez utiliser l’une des méthodes décrites ci-dessous, car le type de série de machines virtuelles ne s’affiche pas correctement dans les fichiers de rapprochement de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="8fb8b-121">**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API d’utilisation Azure**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="8fb8b-122">Utilisez la valeur de l’attribut ServiceType de additionalInfo dans la réponse de l’API pour identifier la taille de machine virtuelle à acheter.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="8fb8b-123">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="8fb8b-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="8fb8b-124">**Obtient les informations de dimensionnement de machine virtuelle à l’aide du Portail Microsoft Azure**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="8fb8b-125">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="8fb8b-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="8fb8b-126">Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="8fb8b-127">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="8fb8b-128">Sélectionnez **machines virtuelles** dans le menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="8fb8b-129">Sur la page de détails de la machine virtuelle, recherchez les informations relatives à la taille et à la région, comme illustré ci-dessous, et utilisez ces informations pour acheter la réservation dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    :::image type="content" source="images/usage1.png" alt-text="Informations sur la taille et la région sur la page de détails":::

<span data-ttu-id="8fb8b-131">**Récupération d’informations de dimensionnement de machine virtuelle à l’aide de Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="8fb8b-132">Utilisez les informations de l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Emplacement et taille de la machine virtuelle":::

<span data-ttu-id="8fb8b-134">**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API Azure Resource Manager (ARM)**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="8fb8b-135">À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="8fb8b-136">/subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="8fb8b-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="8fb8b-137">L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valeur vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valeur d’emplacement":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="8fb8b-140">Vérifier l’utilisation de la machine virtuelle Azure et la remise de réservation</span><span class="sxs-lookup"><span data-stu-id="8fb8b-140">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="8fb8b-141">Une fois que vous avez acheté une instance de machine virtuelle réservée Azure pour le compte d’un client, la remise pour le paiement à l’avance pour l’espace de la machine virtuelle est automatiquement appliquée aux machines virtuelles qui correspondent aux attributs et à la quantité de la réservation du client.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-141">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="8fb8b-142">Vous pouvez vérifier l’utilisation de la réservation du client et déterminer les machines virtuelles auxquelles les remises de réservation sont appliquées à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="8fb8b-142">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="8fb8b-143">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-143">The Azure portal</span></span>
- <span data-ttu-id="8fb8b-144">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-144">Azure utilization API</span></span>

<span data-ttu-id="8fb8b-145">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-145">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="8fb8b-146">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-146">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="8fb8b-147">Vérifier l’utilisation de la réservation du client dans le Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-147">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="8fb8b-148">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="8fb8b-148">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="8fb8b-149">Recherchez le client dont vous souhaitez vérifier la remise de réservation et l’utilisation, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-149">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="8fb8b-150">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-150">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="8fb8b-151">Sélectionnez **réservations** dans le menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-151">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="8fb8b-152">Sur la page **vue d’ensemble** , vérifiez le graphique d’utilisation de la réservation, qui indique la quantité de réservation appliquée aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-152">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8fb8b-153">Les données d’utilisation peuvent être retardées de 8 heures.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-153">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="8fb8b-154">a.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-154">a.</span></span> <span data-ttu-id="8fb8b-155">Si l’utilisation de la réservation est de 100%, votre client obtient toutes les économies possibles que l’achat de réservation peut fournir.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-155">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="8fb8b-156">b.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-156">b.</span></span> <span data-ttu-id="8fb8b-157">Si l’utilisation de la réservation est de 0%, la remise n’est pas appliquée à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-157">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="8fb8b-158">c.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-158">c.</span></span> <span data-ttu-id="8fb8b-159">Si l’utilisation de la réservation est comprise entre 1% et 99%, il existe des avantages inutilisés.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-159">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="8fb8b-160">Pour éviter cette situation, déterminez la taille de machine virtuelle appropriée pour prendre en charge les besoins informatiques du client avant d’effectuer l’achat.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-160">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="8fb8b-161">Vérifier l’utilisation de la réservation du client avec l’API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-161">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="8fb8b-162">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-162">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="8fb8b-163">Vous pouvez obtenir des données d’utilisation de réservation avec l’API d’utilisation d’Azure pour vérifier que le client obtient la remise de réservation et pour connaître les machines virtuelles (machines virtuelles) auxquelles la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-163">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="8fb8b-164">Comparez l’exemple A à l’exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-164">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exemples d’utilisation de la réservation":::

- <span data-ttu-id="8fb8b-166">Le réservation identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-166">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="8fb8b-167">Le compteur est le MeterId de la machine virtuelle à laquelle la remise de réservation est appliquée.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-167">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="8fb8b-168">Le ReservationMeter affiche le coût de $0, car la remise de réservation a été appliquée.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-168">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="8fb8b-169">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="8fb8b-169">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="8fb8b-170">Les coûts des logiciels, tels que Microsoft Windows Server, ne sont actuellement pas inclus dans le prix d’une réservation de machine virtuelle et apparaissent sous la forme d’éléments de ligne distincts dans l’enregistrement de commande et sur votre facture.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-170">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="8fb8b-171">Toutefois, si un client dispose de la Azure Hybrid Use Benefit, les frais liés aux logiciels ne seront pas appliqués.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-171">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="8fb8b-172">Pour plus d’informations, consultez [coûts des logiciels Windows non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="8fb8b-172">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="8fb8b-173">Ressources Azure Réservations</span><span class="sxs-lookup"><span data-stu-id="8fb8b-173">Azure reservations resources</span></span>

|<span data-ttu-id="8fb8b-174">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-174">**For information about**</span></span>   |<span data-ttu-id="8fb8b-175">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="8fb8b-175">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="8fb8b-176">Vue d’ensemble des réservations Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="8fb8b-176">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="8fb8b-177">Vendre Microsoft Azure des instances de machines virtuelles réservées</span><span class="sxs-lookup"><span data-stu-id="8fb8b-177">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="8fb8b-178">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-178">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="8fb8b-179">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-179">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="8fb8b-180">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-180">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="8fb8b-181">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-181">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="8fb8b-182">Achat de réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-182">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="8fb8b-183">[Acompte pour les machines virtuelles avec Azure reserved VM instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-183">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="8fb8b-184">Gestion des réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-184">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="8fb8b-185">[Gérer des instances de machine virtuelle réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-185">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="8fb8b-186">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-186">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="8fb8b-187">[Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="8fb8b-187">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="8fb8b-188">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="8fb8b-188">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="8fb8b-189">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="8fb8b-189">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
