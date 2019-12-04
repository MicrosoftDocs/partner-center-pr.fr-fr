---
title: Gérer des réservations Microsoft Azure pour vos clients | Espace partenaires
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Découvrez comment gérer des réservations Azure pour le compte d’un client, notamment comment annuler une réservation, échanger une réservation ou demander un remboursement.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, réservations, gérer, facturation, achat, annulation, échange, frais de résiliation précoce
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: eedfe20cea239918e5ece6f10b2b5f5988da9c50
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722282"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gérer des réservations Microsoft Azure pour vos clients

**S’applique à**

- Espace partenaires
- Portail Microsoft Azure 
- Partenaires fournisseurs de solutions Cloud

**Rôles appropriés**

- Agent d’administration
- Administrateur global
- Agent du support technique
- Commercial
- Administrateur de la gestion des utilisateurs

Pour gérer les réservations Azure de vos clients, vous devez sélectionner le client et la réservation que vous souhaitez gérer dans l’espace partenaires, puis apporter des modifications à la réservation dans le Portail Azure.

1. Pour commencer, sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les réservations. 

2. Dans le menu de la page de détails du client, sélectionnez **réservations Azure** , puis sélectionnez la réservation spécifique que vous souhaitez gérer.  

3. Sous **actions**, sélectionnez **gérer** pour accéder à l’enregistrement de réservation du client dans la portail Azure. Sur la page des détails de la réservation, suivez les étapes ci-dessous pour effectuer des tâches.  

    | **Sélectionné**   | **À**    |
    |:-----------------------------|:-----------------|
    | **Vue d’ensemble**   | Affichez les détails de la réservation d’un client, y compris la date d’expiration, l’étendue et les données d’utilisation. **REMARQUE** Sélectionnez **Remboursement** pour créer une demande de support en vue d'un remboursement calculé au prorata. Sélectionnez **Échange** pour créer une demande de support en vue de l'échange de la période de réservation non utilisée.  
    | **Access Control (IAM)**   | Gérez l’accès aux informations de réservation du client.|
    | **Configuration**   | Modifiez l’étendue de la réservation et/ou l’abonnement Azure auquel la réservation est associée.    |
    | **Propriétés**   | Affichez les propriétés de la réservation et copiez dans le presse-papiers l’ID de réservation et l’ID de commande de réservation. **REMARQUE** Le service d'assistance peut vous demander de communiquer l'identifiant de la réservation et l'identifiant de commande si vous demandez une assistance au nom d'un client.    |
    | **Nouvelle demande de support**    | Demander de l’aide au support Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annuler ou échanger une réservation 

Si, à tout moment, les besoins de l’entreprise d’un client changent, ils peuvent souhaiter annuler une réservation et obtenir un remboursement ou échanger le montant du remboursement calculé au prorata de la réservation à utiliser pour le prix d’une nouvelle réservation.

Dans ces deux scénarios, Microsoft vous refinance le montant pour vous permettre de gérer les transactions financières résultantes avec vos clients. Microsoft ne contacte pas directement les clients sur la facturation, les annulations ou les remboursements.


**Fonctionnement des annulations**

Les clients peuvent demander l’annulation d’une réservation à tout moment (montant de remboursement plafonné à $50 000 par an). L’annulation d’une réservation permet au client de retourner le montant des mois restants d’une réservation Azure pour un droit de résiliation précoce. Le solde calculé au prorata, moins les frais de résiliation précoce, est remboursé sur votre compte afin que vous puissiez rembourser le compte du client. 

Voir ci-dessous pour obtenir des détails et des frais d’annulation.


|**Date d’annulation**<br> précédant   |**Syntaxe**    |**Créancière**  |**Fin précoce**<br> frais    |**Plafond de remboursement** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|au moins 5                         | non          | 100%       | non                              | $50 000 USD   |
|au moins 5                         | Oui         | Pro-évalué  | non                              | $50 000 USD   |
|Plus de 5                        | non          | Pro-évalué  | douze                             | $50 000 USD   |
|Plus de 5                        | Oui         | Pro-évalué  | douze                             | $50 000 USD   |


**Fonctionnement des échanges** 

Si un client souhaite acheter une réservation différente de celle qu’il a achetée à l’origine, il peut demander un échange. L’échange d’une réservation peut être une alternative intéressante à l’annulation d’une réservation, car elle permet au client d’utiliser le montant du remboursement calculé au prorata du prix de la nouvelle réservation. 

Le montant du remboursement calculé au prorata est crédité sur votre compte afin que vous puissiez offrir un échange au client.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Demander un remboursement ou un échange pour le compte d’un client 

Pour traiter une demande de support pour un remboursement ou un échange pour le compte de vos clients, sélectionnez le client et la réservation dans l’espace partenaires, puis créez la demande de support dans le Portail Azure. 

>[!NOTE]
>Les agents du support Microsoft peuvent vous demander de fournir l’identifiant de réservation et l’identifiant de commande de la réservation. Vous pouvez trouver ces informations dans la page de **Propriétés** de la réservation dans la portail Azure. 

1. Pour commencer, sélectionnez **clients** dans le menu de l’espace partenaires, puis sélectionnez le client qui souhaite obtenir un remboursement. 

2. Sur la page de détails du client, sélectionnez **réservations Azure** , puis sélectionnez la réservation spécifique que le client souhaite rembourser.  

3. Sous **actions**, sélectionnez **remboursement** pour accéder à l’enregistrement de réservation du client dans la portail Azure et lancez une demande de support.  

4. Sur la page **Nouvelle demande de support**, suivez les étapes ci-dessous pour demander un remboursement. Sélectionnez **Suivant** après chaque étape. 

    |**Première**                    |**Souhaité**    |
    |:---------------------------|:-----------------|
    |**1 notions de base**                |Type de problème : facturation  |
    |**2 problème**               |Type de problème : gestion de la réservation. Catégorie : Échanges et remboursements. |
    |**3 informations de contact**   |Sélectionnez vos préférences et entrez les informations requises. 

5.  Sélectionnez **Créer** lorsque vous avez terminé.

## <a name="azure-reservations-resources"></a>Ressources des réservations Azure
|**Pour plus d’informations sur**   |**Lisez cela**    |
|:-----------------------------|:-----------------|
|Réservations Azure dans la vue d’ensemble des fournisseurs de solutions Cloud  | [Vendre Microsoft Azure des instances réservées](azure-reservations.md) |
|Achat de réservations Azure pour vos clients dans l’espace partenaires   |[Acheter des réservations Azure](azure-reservations-buying.md) |
|Déterminer la taille appropriée de la machine virtuelle et vérifier l’utilisation des machines virtuelles par le client   |[Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure](azure-usage.md)   |
|Achat de réservations Azure à l’aide de l'API de l'Espace partenaires | [Acheter Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation pour développeurs Espace partenaires

