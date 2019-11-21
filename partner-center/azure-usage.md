---
title: Microsoft Azure le dimensionnement de la machine virtuelle pour une utilisation maximale de la réservation | Espace partenaires
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment ajuster la taille d’une machine virtuelle aux besoins informatiques de vos clients lorsque vous achetez Microsoft Azure réservations pour eux.
author: LauraBrenner
ms.author: labrenne
keywords: azure, réservations, machines virtuelles, gérer, utilisation, dimensionnement
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253250"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionnement d’une machine virtuelle Microsoft Azure en vue d'une utilisation optimale de la réservation

**S’applique à**

- Espace partenaires
- Portail Azure
- Partenaires fournisseurs de solutions Cloud

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Déterminer la taille de machine virtuelle pour la réservation Azure d’un client 

Lorsque vous achetez Microsoft Azure réservations pour le compte de vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée pour répondre aux besoins informatiques du client. Vous pouvez trouver ces informations grâce à l'une des méthodes suivantes :

- API d'utilisation d'Azure
- Le portail Azure
- Azure PowerShell
- L’API Azure Resource Manager (ARM)

Les instructions propres à ces méthodes sont énoncées ci-dessous. Une fois que vous achetez une réservation, la remise de réservation est automatiquement appliquée aux machines virtuelles dont les attributs et la quantité correspondent à la réservation. Vous n’avez pas besoin d’affecter la réservation à une machine virtuelle.

>[!NOTE]
>Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.

>[!IMPORTANT]
>Afin d'identifier le type et la taille corrects de la machine virtuelle à acheter pour votre client, vous devez utiliser l'une des méthodes décrites ci-dessous car le type de série de machine virtuelle ne s’affiche pas correctement dans les fichiers de rapprochement de l’Espace partenaires.

**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API d’utilisation Azure**

1. Utilisez la valeur de l’attribut ServiceType indiquée dans additionalInfo dans la réponse de l’API pour identifier la taille de la machine virtuelle à acheter.
2. Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).

**Obtient les informations de dimensionnement de machine virtuelle à l’aide du Portail Microsoft Azure**

1. Dans l’espace partenaires, accédez à la page de vos **clients** .
2. Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche vers le bas pour développer les informations du client. Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.
3. Sélectionnez **Machines virtuelles** à partir du menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.
4. Sur la page de détails de la machine virtuelle, recherchez les informations relatives à la taille et à la région, comme illustré ci-dessous, et utilisez ces informations pour acheter la réservation dans l’espace partenaires.  

    ![Informations sur la taille et la région sur la page de détails](images/usage1.png)

**Récupération d’informations de dimensionnement de machine virtuelle à l’aide de Microsoft Azure PowerShell**

Utilisez les informations indiquées dans l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation. 

![Emplacement et taille de la machine virtuelle](images/usage2.png)

**Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API Azure Resource Manager (ARM)**

1. À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.

    ![valeur vmSize](images/usage3.png) valeur d’emplacement ![](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Vérifiez l'utilisation de la machine virtuelle Azure et la remise de réservation

Une fois que vous avez acheté une instance de machine virtuelle réservée Azure pour le compte d’un client, la remise pour le paiement à l’avance pour l’espace de la machine virtuelle est automatiquement appliquée aux machines virtuelles qui correspondent aux attributs et à la quantité de la réservation du client.

Vous pouvez vérifier l’utilisation de la réservation du client et déterminer les machines virtuelles auxquelles les remises de réservation sont appliquées à l’aide de l’une des méthodes suivantes :

- Le portail Azure
- API d'utilisation d'Azure

Les instructions propres à ces méthodes sont énoncées ci-dessous.

>[!NOTE]
>Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Vérifier l’utilisation de la réservation du client dans le Portail Microsoft Azure

1. Dans l’espace partenaires, accédez à la page de vos **clients** .

2. Recherchez le client dont vous souhaitez vérifier la remise de réservation et l’utilisation, puis sélectionnez la flèche vers le bas pour développer les informations du client. Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.
3. Sélectionnez **Réservations** à partir du menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l'utilisation.
4. Sur la page **vue d’ensemble** , vérifiez le graphique d’utilisation de la réservation, qui indique la quantité de réservation appliquée aux machines virtuelles.

    >[!NOTE]
    >Les données d’utilisation sont actualisées dans un délai de 8 heures maximum.

    a. Si l’utilisation de la réservation est de 100%, votre client obtient toutes les économies possibles que l’achat de réservation peut fournir.
    b. Si l’utilisation de la réservation est de 0%, la remise n’est pas appliquée à une machine virtuelle.
    c. Si l’utilisation de la réservation est comprise entre 1% et 99%, il existe des avantages inutilisés.

5. Pour éviter cette situation, déterminez la taille de machine virtuelle appropriée pour prendre en charge les besoins informatiques du client avant d’effectuer l’achat.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Vérifier l’utilisation de la réservation du client avec l’API d’utilisation d’Azure

>[!NOTE]
>Seule l'API d’utilisation Azure indique les machines virtuelles sur lesquelles la remise est appliquée.  

Vous pouvez obtenir les données d’utilisation de la réservation avec l’API d'utilisation Azure pour vérifier que le client bénéficie de la remise de réservation et pour déterminer sur quelles machines virtuelles celle-ci est appliquée. Comparez l’exemple A à l’exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.

![Exemples d’utilisation de la réservation](images/usage5.png)

- L'identifiant reservationId identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.
- consumptionMeter correspond à l'identifiant MeterId auquel la remise de réservation est appliquée.
- Le ReservationMeter affiche un coût de 0 $ dans la mesure où la remise de réservation a été appliquée.

Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Les coûts associés aux logiciels, tels que Microsoft Windows Server, ne sont pas actuellement inclus dans le prix d’une réservation de machine virtuelle et apparaîtront dans des postes distincts dans le dossier de commande et sur votre facture. Toutefois, si un client a souscrit au programme Azure Hybrid Use Benefit, les coûts de logiciel ne seront pas appliqués. Pour en savoir plus, consultez [Coûts des logiciels Windows non inclus avec les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ressources des réservations Azure

|**Pour plus d’informations sur**   |**Lisez cela**    |
|:-----------------------------|:-----------------|
|Réservations Azure dans la vue d’ensemble des fournisseurs de solutions Cloud  | [Vendre Microsoft Azure des instances de machines virtuelles réservées](azure-reservations.md)
|Achat de réservations Azure pour vos clients dans l’espace partenaires   |[Acheter des réservations Azure](azure-reservations-buying.md)
|Gestion des réservations Azure dans l’espace partenaires | [Gestion des réservations Azure dans l’espace partenaires](azure-reservations-manage.md)
|Achat de réservations Azure dans le portail Azure | [Prépaiement des machines virtuelles avec Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure |
|Gestion des réservations Azure dans le portail Azure   |[Gérer les instances de machines virtuelles réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure  |
|Achat de réservations Azure à l’aide de l'API de l'Espace partenaires | [Acheter Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation pour développeurs Espace partenaires
