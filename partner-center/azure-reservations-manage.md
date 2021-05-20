---
title: Gérer les réservations Azure pour les clients
description: Découvrez comment gérer des réservations Azure pour un client, notamment comment annuler une réservation, échanger une réservation ou demander un remboursement.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149483"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Gérez, annulez, échangez ou remboursez Microsoft Azure réservations pour les clients

**Rôles appropriés**: agent admin | Administrateur général | Agent du support technique | Agent commercial | Administrateur de gestion des utilisateurs

Cet article explique comment gérer des réservations Azure pour un client, notamment comment annuler une réservation, échanger une réservation ou demander un remboursement.

> [!NOTE]
> Cet article s’applique uniquement aux partenaires du programme fournisseur de solutions Cloud (CSP). Les clients qui utilisent d’autres types d’abonnements (par exemple, paiement à l’utilisation, individuel, contrat de client Microsoft ou abonnements Contrat Entreprise) doivent lire [cette documentation Azure reservations](/azure/cost-management-billing/reservations).

Pour gérer les réservations Azure de vos clients, vous devez sélectionner le client et la réservation que vous souhaitez gérer dans l’espace partenaires, puis apporter des modifications à la réservation dans le Portail Azure.

1. Pour commencer, sélectionnez **clients** dans le menu espace partenaires, puis sélectionnez le client dont vous souhaitez gérer les réservations. 

2. Dans le menu de la page de détails du client, sélectionnez **réservations Azure** , puis sélectionnez la réservation spécifique que vous souhaitez gérer.  

3. Sous **actions**, sélectionnez **gérer** pour accéder à l’enregistrement de réservation du client dans la portail Azure. Sur la page Détails de la réservation, suivez les étapes ci-dessous pour terminer les tâches.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Vue d'ensemble**   | Affichez les détails de la réservation d’un client, y compris la date d’expiration, l’étendue et les données d’utilisation. **Remarque** Sélectionnez **remboursement** pour créer une demande de support pour un remboursement au prorata. Sélectionnez **Exchange** pour créer une demande de support afin d’échanger la partie inutilisée de votre terme de réservation.  
    | **Contrôle d’accès (IAM)**   | Gérez l’accès aux informations de réservation du client.|
    | **Configuration**   | Modifiez l’étendue de la réservation et/ou l’abonnement Azure auquel la réservation est associée.    |
    | **Propriétés**   | Affichez les propriétés de la réservation et copiez dans le presse-papiers l’ID de réservation et l’ID de commande de réservation. **Remarque** La prise en charge peut vous demander l’ID de réservation et l’ID de commande de réservation lorsque vous demandez un support pour le compte d’un client.    |
    | **Nouvelle demande de support**    | Demandez de l’aide à partir de Support Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annuler ou échanger une réservation

Si, à tout moment, les besoins de l’entreprise d’un client changent, ils peuvent souhaiter annuler une réservation et obtenir un remboursement ou échanger le montant du remboursement calculé au prorata de la réservation à utiliser pour le prix d’une nouvelle réservation.

Dans ces deux scénarios, Microsoft vous refinance le montant pour vous permettre de gérer les transactions financières résultantes avec vos clients. Microsoft ne contacte pas directement les clients sur la facturation, les annulations ou les remboursements.

### <a name="how-cancellations-work"></a>Fonctionnement des annulations

Les clients peuvent demander l’annulation d’une réservation à tout moment (montant de remboursement plafonné à $50 000 par an). L’annulation d’une réservation permet au client de retourner le montant des mois restants d’une réservation Azure pour un droit de résiliation précoce. Le solde calculé au prorata, moins les frais de résiliation précoce, est remboursé sur votre compte afin que vous puissiez rembourser le compte du client. 

Voir ci-dessous pour obtenir des détails et des frais d’annulation.


|**Date d’annulation**<br> précédant   |**Utilisation**    |**Crédit**  |**Fin précoce**<br> frais    |**Plafond de remboursement** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|au moins 5                         | Non          | 100 %       | Non                              | $50 000 USD   |
|au moins 5                         | Oui         | Pro-évalué  | Non                              | $50 000 USD   |
|Plus de 5                        | Non          | Pro-évalué  | 12 %                             | $50 000 USD   |
|Plus de 5                        | Oui         | Pro-évalué  | 12 %                             | $50 000 USD   |

### <a name="how-exchanges-work"></a>Fonctionnement des échanges 

Si un client souhaite acheter une réservation différente de celle qu’il a achetée à l’origine, il peut demander un échange. L’échange d’une réservation peut être une alternative intéressante à l’annulation d’une réservation, car elle permet au client d’utiliser le montant du remboursement au prorata vers le prix de la nouvelle réservation. 

Le montant du remboursement calculé au prorata est crédité sur votre compte afin que vous puissiez offrir un échange au client.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Demander un remboursement ou un échange pour le compte d’un client

Pour traiter une demande de support pour un remboursement ou un échange pour le compte de vos clients, sélectionnez le client et la réservation dans l’espace partenaires, puis créez la demande de support dans le Portail Azure. 

>[!NOTE]
>Support Microsoft agents peuvent vous demander de fournir l’ID de réservation et l’ID de commande de réservation. Vous pouvez trouver ces informations dans la page de **Propriétés** de la réservation dans la portail Azure.

1. Pour commencer, sélectionnez **clients** dans le menu de l’espace partenaires, puis sélectionnez le client qui souhaite obtenir un remboursement. 

2. Sur la page de détails du client, sélectionnez **réservations Azure** , puis sélectionnez la réservation spécifique que le client souhaite rembourser.  

3. Sous **actions**, sélectionnez **remboursement** pour accéder à l’enregistrement de réservation du client dans la portail Azure et lancez une demande de support.  

4. Dans la page **nouvelle demande de support** , suivez les étapes ci-dessous pour demander un remboursement. Sélectionnez **suivant** après chaque étape. 

   |**Étape**                    |**Souhaité**    |
   |:---------------------------|:-----------------|
   |**1 notions de base**                |Type de problème : facturation.  |
   |**2 problème**               |Type de problème : gestion des réservations. Catégorie : échanges et remboursements. |
   |**3 informations de contact**   |Sélectionnez vos préférences, puis entrez les informations requises. 

5. Sélectionnez **Créer** lorsque vous avez terminé.

## <a name="azure-reservations-resources"></a>Ressources Azure Réservations

|**Pour obtenir des informations sur**   |**Lisez cela**    |
|:-----------------------------|:-----------------|
|Vue d’ensemble des réservations Azure dans CSP  | [Vendre Microsoft Azure des instances réservées](azure-reservations.md) |
|Achat de réservations Azure pour vos clients dans l’espace partenaires   | [Acheter des réservations Azure](azure-reservations-buying.md) |
|Déterminer la taille de machine virtuelle correcte et vérifier l’utilisation de la machine virtuelle client   | [Dimensionnement des machines virtuelles pour l’utilisation maximale de la réservation Azure](azure-usage.md)   |
|Achat de réservations Azure à l’aide de l’API espace partenaires | [Acheter Azure reserved VM instances](/partner-center/develop/purchase-azure-reservations) dans la documentation du développeur de l’espace partenaires   |
|Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure à partir d’un abonnement que vous avez acheté pour eux. | [Accorder aux clients l’autorisation d’acheter leurs propres réservations Azure](give-customers-permission.md)   |