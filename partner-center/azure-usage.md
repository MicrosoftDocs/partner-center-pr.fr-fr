---
title: Dimensionnement d’une machine virtuelle Azure en vue d’une utilisation optimale de la réservation
description: Découvrez comment ajuster la taille d’une machine virtuelle aux besoins informatiques de vos clients lorsque vous achetez Microsoft Azure réservations pour eux.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149449"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="a1519-103">Dimensionnement des machines virtuelles Microsoft Azure pour une utilisation maximale de la réservation</span><span class="sxs-lookup"><span data-stu-id="a1519-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="a1519-104">**Rôles appropriés**: agent admin | Agent des ventes</span><span class="sxs-lookup"><span data-stu-id="a1519-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="a1519-105">Cet article explique comment ajuster la taille d’une machine virtuelle aux besoins informatiques de vos clients lorsque vous achetez Microsoft Azure réservations pour eux.</span><span class="sxs-lookup"><span data-stu-id="a1519-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="a1519-106">Cet article s’applique uniquement aux partenaires du programme fournisseur de solutions Cloud (CSP).</span><span class="sxs-lookup"><span data-stu-id="a1519-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="a1519-107">Les clients qui utilisent d’autres types d’abonnements (par exemple, paiement à l’utilisation, individuel, contrat de client Microsoft ou abonnements Contrat Entreprise) doivent lire [cette documentation Azure reservations](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="a1519-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="a1519-108">Déterminer la taille de machine virtuelle pour la réservation Azure d’un client</span><span class="sxs-lookup"><span data-stu-id="a1519-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="a1519-109">Lorsque vous achetez Microsoft Azure réservations pour le compte de vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée pour répondre aux besoins informatiques du client.</span><span class="sxs-lookup"><span data-stu-id="a1519-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="a1519-110">Vous pouvez trouver ces informations à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a1519-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="a1519-111">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-111">Azure utilization API</span></span>
- <span data-ttu-id="a1519-112">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-112">The Azure portal</span></span>
- <span data-ttu-id="a1519-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1519-113">Azure PowerShell</span></span>
- <span data-ttu-id="a1519-114">API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="a1519-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="a1519-115">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a1519-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="a1519-116">Une fois que vous avez acheté une réservation, la remise de réservation est appliquée automatiquement aux machines virtuelles correspondant aux attributs et à la quantité de la réservation.</span><span class="sxs-lookup"><span data-stu-id="a1519-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="a1519-117">Vous n’avez pas besoin d’affecter la réservation à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="a1519-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="a1519-118">Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.</span><span class="sxs-lookup"><span data-stu-id="a1519-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a1519-119">Pour identifier correctement le type et la taille de la machine virtuelle à acheter pour le compte de votre client, vous devez utiliser l’une des méthodes décrites ci-dessous, car le type de série de machines virtuelles ne s’affiche pas correctement dans les fichiers de rapprochement de l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a1519-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="a1519-120">Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API d’utilisation Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="a1519-121">Utilisez la valeur de l’attribut ServiceType de additionalInfo dans la réponse de l’API pour identifier la taille de machine virtuelle à acheter.</span><span class="sxs-lookup"><span data-stu-id="a1519-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="a1519-122">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="a1519-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="a1519-123">Obtient les informations de dimensionnement de machine virtuelle à l’aide du Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="a1519-124">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="a1519-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="a1519-125">Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="a1519-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a1519-126">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="a1519-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="a1519-127">Sélectionnez **machines virtuelles** dans le menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="a1519-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="a1519-128">Sur la page de détails de la machine virtuelle, recherchez les informations relatives à la taille et à la région, comme illustré ci-dessous, et utilisez ces informations pour acheter la réservation dans l’espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="a1519-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informations sur la taille et la région sur la page de détails":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="a1519-130">Récupération d’informations de dimensionnement de machine virtuelle à l’aide de Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1519-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="a1519-131">Utilisez les informations de l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="a1519-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Emplacement et taille de la machine virtuelle":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="a1519-133">Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="a1519-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="a1519-134">À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="a1519-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="a1519-135">/subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a1519-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="a1519-136">L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a1519-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valeur vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valeur d’emplacement":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="a1519-139">Vérifier l’utilisation de la machine virtuelle Azure et la remise de réservation</span><span class="sxs-lookup"><span data-stu-id="a1519-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="a1519-140">Une fois que vous avez acheté une instance de machine virtuelle réservée Azure pour le compte d’un client, la remise pour le paiement à l’avance pour l’espace de la machine virtuelle est automatiquement appliquée aux machines virtuelles qui correspondent aux attributs et à la quantité de la réservation du client.</span><span class="sxs-lookup"><span data-stu-id="a1519-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="a1519-141">Vous pouvez vérifier l’utilisation de la réservation du client et déterminer les machines virtuelles auxquelles les remises de réservation sont appliquées à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a1519-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="a1519-142">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-142">The Azure portal</span></span>
- <span data-ttu-id="a1519-143">API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-143">Azure utilization API</span></span>

<span data-ttu-id="a1519-144">Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="a1519-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="a1519-145">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="a1519-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="a1519-146">Vérifier l’utilisation de la réservation du client dans le Portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="a1519-147">Dans l’espace partenaires, accédez à la page de vos **clients** .</span><span class="sxs-lookup"><span data-stu-id="a1519-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="a1519-148">Recherchez le client dont vous souhaitez vérifier la remise de réservation et l’utilisation, puis sélectionnez la flèche vers le bas pour développer les informations du client.</span><span class="sxs-lookup"><span data-stu-id="a1519-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a1519-149">Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="a1519-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="a1519-150">Sélectionnez **réservations** dans le menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l’utilisation.</span><span class="sxs-lookup"><span data-stu-id="a1519-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="a1519-151">Sur la page **vue d’ensemble** , vérifiez le graphique d’utilisation de la réservation, qui indique la quantité de réservation appliquée aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="a1519-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a1519-152">Les données d’utilisation peuvent être retardées de 8 heures.</span><span class="sxs-lookup"><span data-stu-id="a1519-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="a1519-153">a.</span><span class="sxs-lookup"><span data-stu-id="a1519-153">a.</span></span> <span data-ttu-id="a1519-154">Si l’utilisation de la réservation est de 100%, votre client obtient toutes les économies possibles que l’achat de réservation peut fournir.</span><span class="sxs-lookup"><span data-stu-id="a1519-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="a1519-155">b.</span><span class="sxs-lookup"><span data-stu-id="a1519-155">b.</span></span> <span data-ttu-id="a1519-156">Si l’utilisation de la réservation est de 0%, la remise n’est pas appliquée à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="a1519-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="a1519-157">c.</span><span class="sxs-lookup"><span data-stu-id="a1519-157">c.</span></span> <span data-ttu-id="a1519-158">Si l’utilisation de la réservation est comprise entre 1% et 99%, il existe des avantages inutilisés.</span><span class="sxs-lookup"><span data-stu-id="a1519-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="a1519-159">Pour éviter cette situation, déterminez la taille de machine virtuelle appropriée pour prendre en charge les besoins informatiques du client avant d’effectuer l’achat.</span><span class="sxs-lookup"><span data-stu-id="a1519-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="a1519-160">Vérifier l’utilisation de la réservation du client avec l’API d’utilisation d’Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="a1519-161">Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="a1519-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="a1519-162">Vous pouvez obtenir des données d’utilisation de réservation avec l’API d’utilisation d’Azure pour vérifier que le client obtient la remise de réservation et pour connaître les machines virtuelles (machines virtuelles) auxquelles la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="a1519-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="a1519-163">Comparez l’exemple A à l’exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.</span><span class="sxs-lookup"><span data-stu-id="a1519-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Exemples d’utilisation de la réservation":::

- <span data-ttu-id="a1519-165">Le réservation identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="a1519-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="a1519-166">Le compteur est le MeterId de la machine virtuelle à laquelle la remise de réservation est appliquée.</span><span class="sxs-lookup"><span data-stu-id="a1519-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="a1519-167">Le ReservationMeter affiche le coût de $0, car la remise de réservation a été appliquée.</span><span class="sxs-lookup"><span data-stu-id="a1519-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="a1519-168">Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="a1519-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="a1519-169">Les coûts des logiciels, tels que Microsoft Windows Server, ne sont actuellement pas inclus dans le prix d’une réservation de machine virtuelle et apparaissent sous la forme d’éléments de ligne distincts dans l’enregistrement de commande et sur votre facture.</span><span class="sxs-lookup"><span data-stu-id="a1519-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="a1519-170">Toutefois, si un client dispose de la Azure Hybrid Use Benefit, les frais liés aux logiciels ne seront pas appliqués.</span><span class="sxs-lookup"><span data-stu-id="a1519-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="a1519-171">Pour plus d’informations, consultez [coûts des logiciels Windows non inclus dans les instances réservées](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="a1519-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="a1519-172">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a1519-172">Next steps</span></span>

|<span data-ttu-id="a1519-173">**Pour obtenir des informations sur**</span><span class="sxs-lookup"><span data-stu-id="a1519-173">**For information about**</span></span>   |<span data-ttu-id="a1519-174">**Lisez cela**</span><span class="sxs-lookup"><span data-stu-id="a1519-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="a1519-175">Vue d’ensemble des réservations Azure dans CSP</span><span class="sxs-lookup"><span data-stu-id="a1519-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="a1519-176">Vendre Microsoft Azure des instances de machines virtuelles réservées</span><span class="sxs-lookup"><span data-stu-id="a1519-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="a1519-177">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a1519-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="a1519-178">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a1519-179">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a1519-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a1519-180">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a1519-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a1519-181">Achat de réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="a1519-182">[Acompte pour les machines virtuelles avec Azure reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="a1519-183">Gestion des réservations Azure dans le Portail Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="a1519-184">[Gérer des instances de machine virtuelle réservées](/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="a1519-185">Achat de réservations Azure à l’aide de l’API espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a1519-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a1519-186">[Acheter Azure reserved VM instances](/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="a1519-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="a1519-187">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement que vous avez acheté pour eux.</span><span class="sxs-lookup"><span data-stu-id="a1519-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="a1519-188">Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure</span><span class="sxs-lookup"><span data-stu-id="a1519-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |