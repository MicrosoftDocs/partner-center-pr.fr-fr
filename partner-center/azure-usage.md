---
title: Dimensionnement d’une machine virtuelle Microsoft Azure pour utilisation maximale de réservation | L’espace partenaires
ms.topic: article
ms.date: 10/29/2018
Description: Information on purchasing and managing Azure reservations
author: v-petand
ms.author: v-petand
keywords: azure, réservations, machines virtuelles, gérer, utilisation, dimensionnement
ms.localizationpriority: medium
ms.openlocfilehash: 00978e8e000dded2e4f7bb5d5d6506711e521c86
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795922"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="c17ce-103">Dimensionnement d’une machine virtuelle Microsoft Azure en vue d'une utilisation optimale de la réservation</span><span class="sxs-lookup"><span data-stu-id="c17ce-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="c17ce-104">S'applique à</span><span class="sxs-lookup"><span data-stu-id="c17ce-104">Applies to</span></span>**

-  <span data-ttu-id="c17ce-105">Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-105">Partner Center</span></span>
-  <span data-ttu-id="c17ce-106">PortailAzure</span><span class="sxs-lookup"><span data-stu-id="c17ce-106">Azure portal</span></span>
-  <span data-ttu-id="c17ce-107">Partenaires fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="c17ce-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="c17ce-108">Déterminer la taille de la machine virtuelle pour la réservation Azure du client</span><span class="sxs-lookup"><span data-stu-id="c17ce-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="c17ce-109">Lorsque vous achetez des réservations MicrosoftAzure pour vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée en fonction des besoins informatiques du client.</span><span class="sxs-lookup"><span data-stu-id="c17ce-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="c17ce-110">Vous pouvez trouver ces informations grâce à l'une des méthodes suivantes:</span><span class="sxs-lookup"><span data-stu-id="c17ce-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="c17ce-111">API d'utilisation d'Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-111">Azure utilization API</span></span>
-   <span data-ttu-id="c17ce-112">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-112">The Azure portal</span></span>
-   <span data-ttu-id="c17ce-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c17ce-113">Azure PowerShell</span></span>
-   <span data-ttu-id="c17ce-114">L’API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="c17ce-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="c17ce-115">Les instructions propres à ces méthodes sont énoncées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="c17ce-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="c17ce-116">Une fois que vous achetez une réservation, la remise de réservation est automatiquement appliquée aux machines virtuelles dont les attributs et la quantité correspondent à la réservation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="c17ce-117">Il n'est pas nécessaire d'attribuer la réservation à une machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="c17ce-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="c17ce-118">Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.</span><span class="sxs-lookup"><span data-stu-id="c17ce-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="c17ce-119">Afin d'identifier le type et la taille corrects de la machine virtuelle à acheter pour votre client, vous devez utiliser l'une des méthodes décrites ci-dessous car le type de série de machine virtuelle ne s’affiche pas correctement dans les fichiers de rapprochement de l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c17ce-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="c17ce-120">Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de l’API d'utilisation Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="c17ce-121">Utilisez la valeur de l’attribut ServiceType indiquée dans additionalInfo dans la réponse de l’API pour identifier la taille de la machine virtuelle à acheter.</span><span class="sxs-lookup"><span data-stu-id="c17ce-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="c17ce-122">Pour plus d’informations, consultez [Obtenir les dossiers d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l'[API de l'Espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="c17ce-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="c17ce-123">Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide du portail Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="c17ce-124">Dans l’espace partenaires, accédez à votre page **clients** .</span><span class="sxs-lookup"><span data-stu-id="c17ce-124">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="c17ce-125">Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche allant vers le bas pour afficher les informations le concernant.</span><span class="sxs-lookup"><span data-stu-id="c17ce-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="c17ce-126">Sélectionnez **Portail de gestion MicrosoftAzure** pour ouvrir le dossier du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="c17ce-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="c17ce-127">Sélectionnez **Machines virtuelles** à partir du menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="c17ce-128">Sur la page des détails de la machine virtuelle, recherchez les informations relatives à la dimension et à la région, comme illustré ci-dessous, et utilisez-les pour acheter la réservation dans l’Espace partenaires.</span><span class="sxs-lookup"><span data-stu-id="c17ce-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="c17ce-129">Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="c17ce-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="c17ce-130">Utilisez les informations indiquées dans l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="c17ce-131">Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de l'API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="c17ce-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="c17ce-132">À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="c17ce-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="c17ce-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="c17ce-134">L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="c17ce-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="c17ce-135">Vérifiez l'utilisation de la machine virtuelle Azure et la remise de réservation</span><span class="sxs-lookup"><span data-stu-id="c17ce-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="c17ce-136">Une fois que vous aurez acheté une Azure Reserved VM Instance au nom du client, la remise pour le paiement anticipé de l'espace de machine virtuelle est automatiquement appliquée aux machines virtuelles dont les attributs et la quantité correspondent à la réservation du client.</span><span class="sxs-lookup"><span data-stu-id="c17ce-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="c17ce-137">Vous pouvez vérifier l’utilisation de la réservation du client et afficher les machines virtuelles sur lesquelles une remise de réservation a été appliquée à l'aide de l'une des méthodes suivantes:</span><span class="sxs-lookup"><span data-stu-id="c17ce-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="c17ce-138">Le portail Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-138">The Azure portal</span></span>
-   <span data-ttu-id="c17ce-139">API d'utilisation d'Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-139">Azure utilization API</span></span>

<span data-ttu-id="c17ce-140">Les instructions propres à ces méthodes sont énoncées ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="c17ce-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="c17ce-141">Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="c17ce-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="c17ce-142">Vérifier l’utilisation de la réservation du client dans le portail MicrosoftAzure</span><span class="sxs-lookup"><span data-stu-id="c17ce-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="c17ce-143">Dans l’espace partenaires, accédez à votre page **clients** .</span><span class="sxs-lookup"><span data-stu-id="c17ce-143">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="c17ce-144">Recherchez le client dont vous souhaitez vérifier la remise de réservation et l'utilisation, puis sélectionnez la flèche allant vers le bas pour afficher les informations le concernant.</span><span class="sxs-lookup"><span data-stu-id="c17ce-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="c17ce-145">Sélectionnez **Portail de gestion MicrosoftAzure** pour ouvrir le dossier du client dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="c17ce-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="c17ce-146">Sélectionnez **Réservations** à partir du menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l'utilisation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="c17ce-147">Sur la page **Vue d’ensemble** consultez le graphique d’utilisation de la réservation, qui indique la quantité de la réservation appliquée aux machines virtuelles.</span><span class="sxs-lookup"><span data-stu-id="c17ce-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="c17ce-148">Les données d’utilisation sont actualisées dans un délai de 8 heures maximum.</span><span class="sxs-lookup"><span data-stu-id="c17ce-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="c17ce-149">a.</span><span class="sxs-lookup"><span data-stu-id="c17ce-149">a.</span></span>  <span data-ttu-id="c17ce-150">Si la réservation est utilisée à 100%, votre client bénéficie de tous les gains possibles découlant d'un achat de réservation.</span><span class="sxs-lookup"><span data-stu-id="c17ce-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="c17ce-151">b.</span><span class="sxs-lookup"><span data-stu-id="c17ce-151">b.</span></span>  <span data-ttu-id="c17ce-152">Si la réservation est utilisée à 0%, la remise n'est appliquée à aucune machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="c17ce-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="c17ce-153">c.</span><span class="sxs-lookup"><span data-stu-id="c17ce-153">c.</span></span>  <span data-ttu-id="c17ce-154">Si l'utilisation de la réservation se situe entre 1 et 99%, celle-ci n'est pas exploitée au maximum.</span><span class="sxs-lookup"><span data-stu-id="c17ce-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="c17ce-155">Pour éviter une telle situation, déterminez la taille appropriée de la machine virtuelle qui répondra aux besoins informatiques du client avant de procéder à l'achat.</span><span class="sxs-lookup"><span data-stu-id="c17ce-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="c17ce-156">Vérifier l’utilisation de la réservation du client avec l'API d'utilisation Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="c17ce-157">Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.</span><span class="sxs-lookup"><span data-stu-id="c17ce-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="c17ce-158">Vous pouvez obtenir les données d’utilisation de la réservation avec l’API d'utilisation Azure pour vérifier que le client bénéficie de la remise de réservation et pour déterminer sur quelles machines virtuelles celle-ci est appliquée.</span><span class="sxs-lookup"><span data-stu-id="c17ce-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="c17ce-159">Comparez l’exemple A à l'exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.</span><span class="sxs-lookup"><span data-stu-id="c17ce-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="c17ce-160">L'identifiant reservationId identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.</span><span class="sxs-lookup"><span data-stu-id="c17ce-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="c17ce-161">consumptionMeter correspond à l'identifiant MeterId auquel la remise de réservation est appliquée.</span><span class="sxs-lookup"><span data-stu-id="c17ce-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="c17ce-162">Le ReservationMeter affiche un coût de 0$ dans la mesure où la remise de réservation a été appliquée.</span><span class="sxs-lookup"><span data-stu-id="c17ce-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="c17ce-163">Pour plus d’informations, consultez [Obtenir les dossiers d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l'[API de l'Espace partenaires](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="c17ce-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="c17ce-164">Les coûts associés aux logiciels, tels que MicrosoftWindows Server, ne sont pas actuellement inclus dans le prix d’une réservation de machine virtuelle et apparaîtront dans des postes distincts dans le dossier de commande et sur votre facture.</span><span class="sxs-lookup"><span data-stu-id="c17ce-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="c17ce-165">Toutefois, si un client a souscrit au programme Azure Hybrid Use Benefit, les coûts de logiciel ne seront pas appliqués.</span><span class="sxs-lookup"><span data-stu-id="c17ce-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="c17ce-166">Pour en savoir plus, consultez [Coûts des logiciels Windows non inclus avec les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="c17ce-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="c17ce-167">Réservations de ressources Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-167">Azure reservations resources</span></span>
|**<span data-ttu-id="c17ce-168">Pour plus d’informations sur</span><span class="sxs-lookup"><span data-stu-id="c17ce-168">For information about</span></span>**   |**<span data-ttu-id="c17ce-169">Lisez</span><span class="sxs-lookup"><span data-stu-id="c17ce-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="c17ce-170">Les réservation Azure dans la vue d’ensemble des fournisseurs de solutions Cloud</span><span class="sxs-lookup"><span data-stu-id="c17ce-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="c17ce-171">Commercialiser les MicrosoftAzure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="c17ce-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="c17ce-172">Achat de réservations Azure pour vos clients dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-172">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="c17ce-173">Acheter des réservations Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
| <span data-ttu-id="c17ce-174">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-174">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="c17ce-175">Gestion des réservations Azure dans l’espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-175">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="c17ce-176">Achat de réservations Azure dans le portail Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-176">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="c17ce-177">[Prépaiement des machines virtuelles avec Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-177">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="c17ce-178">Gestion des réservations Azure dans le portail Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-178">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="c17ce-179">[Gérer les instances de machines virtuelles réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure</span><span class="sxs-lookup"><span data-stu-id="c17ce-179">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="c17ce-180">Achat de réservations Azure à l’aide de l'API de l'Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-180">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="c17ce-181">[Acheter Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation pour développeurs Espace partenaires</span><span class="sxs-lookup"><span data-stu-id="c17ce-181">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



