---
title: Dimensionnement d’une machine virtuelle Azure en vue d’une utilisation optimale de la réservation
ms.topic: how-to
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment ajuster la taille d’une machine virtuelle aux besoins informatiques de vos clients lorsque vous achetez Microsoft Azure réservations pour eux.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 48f7fb317d35c87eaf3d8fddc7a5da907178ef36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527445"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Dimensionnement des machines virtuelles Microsoft Azure pour une utilisation maximale de la réservation

**S’applique à**

- Espace partenaires
- Portail Azure
- Partenaires dans CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Déterminer la taille de machine virtuelle pour la réservation Azure d’un client

Lorsque vous achetez Microsoft Azure réservations pour le compte de vos clients, vous devez choisir une machine virtuelle (VM) dimensionnée pour répondre aux besoins informatiques du client. Vous pouvez trouver ces informations à l’aide de l’une des méthodes suivantes :

- API d’utilisation d’Azure
- Le portail Azure
- Azure PowerShell
- API Azure Resource Manager (ARM)

Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous. Une fois que vous avez acheté une réservation, la remise de réservation est appliquée automatiquement aux machines virtuelles correspondant aux attributs et à la quantité de la réservation. Vous n’avez pas besoin d’affecter la réservation à une machine virtuelle.

>[!NOTE]
>Les remises de réservation ne s’appliquent pas aux machines virtuelles classiques ou promotionnelles.

>[!IMPORTANT]
>Pour identifier correctement le type et la taille de la machine virtuelle à acheter pour le compte de votre client, vous devez utiliser l’une des méthodes décrites ci-dessous, car le type de série de machines virtuelles ne s’affiche pas correctement dans les fichiers de rapprochement de l’espace partenaires.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API d’utilisation Azure

1. Utilisez la valeur de l’attribut ServiceType de additionalInfo dans la réponse de l’API pour identifier la taille de machine virtuelle à acheter.

2. Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Obtient les informations de dimensionnement de machine virtuelle à l’aide du Portail Microsoft Azure

1. Dans l’espace partenaires, accédez à la page de vos **clients** .

2. Recherchez le client qui souhaite acheter des réservations de machines virtuelles Azure, puis sélectionnez la flèche vers le bas pour développer les informations du client. Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.

3. Sélectionnez **machines virtuelles** dans le menu du portail, puis sélectionnez la machine virtuelle pour laquelle vous souhaitez acheter une réservation.

4. Sur la page de détails de la machine virtuelle, recherchez les informations relatives à la taille et à la région, comme illustré ci-dessous, et utilisez ces informations pour acheter la réservation dans l’espace partenaires.  

   :::image type="content" source="images/usage1.png" alt-text="Informations sur la taille et la région sur la page de détails":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Récupération d’informations de dimensionnement de machine virtuelle à l’aide de Microsoft Azure PowerShell

Utilisez les informations de l’image ci-dessous pour obtenir l’emplacement et la taille de la machine virtuelle pour laquelle vous souhaitez acheter une réservation. 

:::image type="content" source="images/usage2.png" alt-text="Emplacement et taille de la machine virtuelle":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Récupération des informations de dimensionnement de machine virtuelle à l’aide de l’API Azure Resource Manager (ARM)

1. À l’aide des API ARMClient ou ARM, appelez le client ARM pour la machine virtuelle pour laquelle vous souhaitez acheter une réservation.

2. /subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01

3. L’appel retourne les valeurs pour **vmSize** et **location**, comme illustré ci-dessous.

    :::image type="content" source="images/usage3.png" alt-text="valeur vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valeur d’emplacement":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Vérifier l’utilisation de la machine virtuelle Azure et la remise de réservation

Une fois que vous avez acheté une instance de machine virtuelle réservée Azure pour le compte d’un client, la remise pour le paiement à l’avance pour l’espace de la machine virtuelle est automatiquement appliquée aux machines virtuelles qui correspondent aux attributs et à la quantité de la réservation du client.

Vous pouvez vérifier l’utilisation de la réservation du client et déterminer les machines virtuelles auxquelles les remises de réservation sont appliquées à l’aide de l’une des méthodes suivantes :

- Le portail Azure
- API d’utilisation d’Azure

Les instructions d’utilisation de chacune de ces méthodes sont présentées ci-dessous.

>[!NOTE]
>Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Vérifier l’utilisation de la réservation du client dans le Portail Microsoft Azure

1. Dans l’espace partenaires, accédez à la page de vos **clients** .

2. Recherchez le client dont vous souhaitez vérifier la remise de réservation et l’utilisation, puis sélectionnez la flèche vers le bas pour développer les informations du client. Sélectionnez **portail de gestion Microsoft Azure** pour ouvrir l’enregistrement du client dans le portail Azure.
3. Sélectionnez **réservations** dans le menu du portail, puis sélectionnez la réservation pour laquelle vous souhaitez vérifier l’utilisation.
4. Sur la page **vue d’ensemble** , vérifiez le graphique d’utilisation de la réservation, qui indique la quantité de réservation appliquée aux machines virtuelles.

    >[!NOTE]
    >Les données d’utilisation peuvent être retardées de 8 heures.

    a. Si l’utilisation de la réservation est de 100%, votre client obtient toutes les économies possibles que l’achat de réservation peut fournir.
    b. Si l’utilisation de la réservation est de 0%, la remise n’est pas appliquée à une machine virtuelle.
    c. Si l’utilisation de la réservation est comprise entre 1% et 99%, il existe des avantages inutilisés.

5. Pour éviter cette situation, déterminez la taille de machine virtuelle appropriée pour prendre en charge les besoins informatiques du client avant d’effectuer l’achat.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Vérifier l’utilisation de la réservation du client avec l’API d’utilisation d’Azure

>[!NOTE]
>Seule l’API d’utilisation Azure indique à quelle machine virtuelle la remise est appliquée.  

Vous pouvez obtenir des données d’utilisation de réservation avec l’API d’utilisation d’Azure pour vérifier que le client obtient la remise de réservation et pour connaître les machines virtuelles (machines virtuelles) auxquelles la remise est appliquée. Comparez l’exemple A à l’exemple B pour voir comment vérifier l’utilisation de la réservation d’un client.

:::image type="content" source="images/usage5.png" alt-text="Exemples d’utilisation de la réservation":::

- Le réservation identifie la réservation Azure qui a été utilisée pour appliquer la remise à la machine virtuelle.
- Le compteur est le MeterId de la machine virtuelle à laquelle la remise de réservation est appliquée.
- Le ReservationMeter affiche le coût de $0, car la remise de réservation a été appliquée.

Pour plus d’informations, consultez [obtenir les enregistrements d’utilisation d’un client pour Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) dans l' [API espace partenaires](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Les coûts des logiciels, tels que Microsoft Windows Server, ne sont actuellement pas inclus dans le prix d’une réservation de machine virtuelle et apparaissent sous la forme d’éléments de ligne distincts dans l’enregistrement de commande et sur votre facture. Toutefois, si un client dispose de la Azure Hybrid Use Benefit, les frais liés aux logiciels ne seront pas appliqués. Pour plus d’informations, consultez [coûts des logiciels Windows non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Ressources Azure Réservations

|**Pour obtenir des informations sur**   |**Lisez cela**    |
|:-----------------------------|:-----------------|
|Vue d’ensemble des réservations Azure dans CSP  | [Vendre Microsoft Azure des instances de machines virtuelles réservées](azure-reservations.md)
|Achat de réservations Azure pour vos clients dans l’espace partenaires   | [Acheter des réservations Azure](azure-reservations-buying.md)
|Gestion des réservations Azure dans l’espace partenaires | [Gestion des réservations Azure dans l’espace partenaires](azure-reservations-manage.md)
|Achat de réservations Azure dans le Portail Azure | [Acompte pour les machines virtuelles avec Azure reserved VM instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure |
|Gestion des réservations Azure dans le Portail Azure   | [Gérer des instances de machine virtuelle réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure  |
|Achat de réservations Azure à l’aide de l’API espace partenaires | [Acheter Azure reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires   |
|Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement que vous avez acheté pour eux. | [Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure](give-customers-permission.md)   |
