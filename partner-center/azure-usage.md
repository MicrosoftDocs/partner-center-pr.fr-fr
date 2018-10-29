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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionnement d’une machine virtuelle Microsoft Azure en vue d'une utilisation optimale de la réservation 

**S'applique à**

-  Espace partenaires
-  PortailAzure
-  Partenaires fournisseurs de solutions Cloud

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Déterminer la taille de la machine virtuelle pour la réservation Azure du client 

Lorsque vous achetez des réservations MicrosoftAzure pour vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée en fonction des besoins informatiques du client. Vous pouvez trouver ces informations grâce à l'une des méthodes suivantes:

-   API d'utilisation d'Azure
-   Le portail Azure
-   Azure PowerShell
-   L’API Azure Resource Manager (ARM)

Les instructions propres à ces méthodes sont énoncées ci-dessous. Une fois que vous achetez une réservation, la remise de réservation est automatiquement appliquée aux machines virtuelles dont les attributs et la quantité correspondent à la réservation. Il n'est pas nécessaire d'attribuer la réservation à une machine virtuelle.

>[!NOTE]
>Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.

>[!IMPORTANT]
>Afin d'identifier le type et la taille corrects de la machine virtuelle à acheter pour votre client, vous devez utiliser l'une des méthodes décrites ci-dessous car le type de série de machine virtuelle ne s’affiche pas correctement dans les fichiers de rapprochement de l’Espace partenaires.


**Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de l’API d'utilisation Azure**

1.  Utilisez la valeur de l’attribut ServiceType indiquée dans additionalInfo dans la réponse de l’API pour identifier la taille de la machine virtuelle à acheter. 

2.  Pour plus d’informations, consultez [Obtenir les dossiers d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l'[API de l'Espace partenaires](https://docs.microsoft.com/partner-center/develop/). 

**Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide du portail Microsoft Azure**

1.  Dans l’espace partenaires, accédez à votre page **clients** .

2.  Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche allant vers le bas pour afficher les informations le concernant. Sélectionnez **Portail de gestion MicrosoftAzure** pour ouvrir le dossier du client dans le portail Azure. 

3.  Sélectionnez **Machines virtuelles** à partir du menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation. 

4.  Sur la page des détails de la machine virtuelle, recherchez les informations relatives à la dimension et à la région, comme illustré ci-dessous, et utilisez-les pour acheter la réservation dans l’Espace partenaires.  

    ![](images/usage1.png)

**Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de Microsoft Azure PowerShell**

Utilisez les informations indiquées dans l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation. 

![](images/usage2.png)

**Obtenir des informations sur le dimensionnement des machines virtuelles à l’aide de l'API Azure Resource Manager (ARM)**

1.  À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Vérifiez l'utilisation de la machine virtuelle Azure et la remise de réservation

Une fois que vous aurez acheté une Azure Reserved VM Instance au nom du client, la remise pour le paiement anticipé de l'espace de machine virtuelle est automatiquement appliquée aux machines virtuelles dont les attributs et la quantité correspondent à la réservation du client. 

Vous pouvez vérifier l’utilisation de la réservation du client et afficher les machines virtuelles sur lesquelles une remise de réservation a été appliquée à l'aide de l'une des méthodes suivantes:   

-   Le portail Azure
-   API d'utilisation d'Azure

Les instructions propres à ces méthodes sont énoncées ci-dessous.

>[!NOTE]
>Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Vérifier l’utilisation de la réservation du client dans le portail MicrosoftAzure

1.  Dans l’espace partenaires, accédez à votre page **clients** .

2.  Recherchez le client dont vous souhaitez vérifier la remise de réservation et l'utilisation, puis sélectionnez la flèche allant vers le bas pour afficher les informations le concernant. Sélectionnez **Portail de gestion MicrosoftAzure** pour ouvrir le dossier du client dans le portail Azure. 

3.  Sélectionnez **Réservations** à partir du menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l'utilisation. 

4.  Sur la page **Vue d’ensemble** consultez le graphique d’utilisation de la réservation, qui indique la quantité de la réservation appliquée aux machines virtuelles. 

    >[!NOTE]
    >Les données d’utilisation sont actualisées dans un délai de 8 heures maximum.
    
    a.  Si la réservation est utilisée à 100%, votre client bénéficie de tous les gains possibles découlant d'un achat de réservation. 
    
    b.  Si la réservation est utilisée à 0%, la remise n'est appliquée à aucune machine virtuelle. 
    
    c.  Si l'utilisation de la réservation se situe entre 1 et 99%, celle-ci n'est pas exploitée au maximum. 

5.  Pour éviter une telle situation, déterminez la taille appropriée de la machine virtuelle qui répondra aux besoins informatiques du client avant de procéder à l'achat.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Vérifier l’utilisation de la réservation du client avec l'API d'utilisation Azure

>[!NOTE]
>Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.  

Vous pouvez obtenir les données d’utilisation de la réservation avec l’API d'utilisation Azure pour vérifier que le client bénéficie de la remise de réservation et pour déterminer sur quelles machines virtuelles celle-ci est appliquée. Comparez l’exemple A à l'exemple B pour voir comment vérifier l’utilisation de la réservation d’un client. 

![](images\usage5.png)

-   L'identifiant reservationId identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.
-   consumptionMeter correspond à l'identifiant MeterId auquel la remise de réservation est appliquée.
-   Le ReservationMeter affiche un coût de 0$ dans la mesure où la remise de réservation a été appliquée. 

Pour plus d’informations, consultez [Obtenir les dossiers d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l'[API de l'Espace partenaires](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Les coûts associés aux logiciels, tels que MicrosoftWindows Server, ne sont pas actuellement inclus dans le prix d’une réservation de machine virtuelle et apparaîtront dans des postes distincts dans le dossier de commande et sur votre facture. Toutefois, si un client a souscrit au programme Azure Hybrid Use Benefit, les coûts de logiciel ne seront pas appliqués. Pour en savoir plus, consultez [Coûts des logiciels Windows non inclus avec les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Réservations de ressources Azure
|**Pour plus d’informations sur**   |**Lisez**    |
|:-----------------------------|:-----------------|
|Les réservation Azure dans la vue d’ensemble des fournisseurs de solutions Cloud  | [Commercialiser les MicrosoftAzure Reserved VM Instances](azure-reservations.md)
|Achat de réservations Azure pour vos clients dans l’espace partenaires   |[Acheter des réservations Azure](azure-reservations-buying.md)
| Gestion des réservations Azure dans l’espace partenaires | [Gestion des réservations Azure dans l’espace partenaires](azure-reservations-manage.md)
|Achat de réservations Azure dans le portail Azure | [Prépaiement des machines virtuelles avec Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure |
|Gestion des réservations Azure dans le portail Azure   |[Gérer les instances de machines virtuelles réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure  |
|Achat de réservations Azure à l’aide de l'API de l'Espace partenaires | [Acheter Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation pour développeurs Espace partenaires



