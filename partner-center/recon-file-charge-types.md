---
title: Types de frais de fichier de réconciliation
ms.topic: article
ms.date: 06/05/2020
description: Découvrez les types de frais (par exemple, basés sur une licence, basés sur l’utilisation et une fois), les crédits et les remises dans les fichiers de rapprochement de l’espace partenaires.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ec4f4a483ecfd106f7ec41b85372e136524a046
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909107"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Comprendre les différents types de frais dans les fichiers de rapprochement de l’espace partenaires

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Administrateur général

Cette rubrique décrit les mappages entre une section de facture et les types de frais associés qui peuvent se trouver dans votre fichier de rapprochement. Votre facture fournit un résumé des frais. Votre fichier de réconciliation fournit une répartition détaillée des transactions d’éléments de ligne, y compris les types de frais. Pour plus d’informations sur les fichiers de rapprochement, voir [How to use Reconciliation Files](use-the-reconciliation-files.md).

Les fichiers de [réconciliation basés sur l’utilisation](usage-based-recon-files.md) et les [fichiers de réconciliation basés sur des licences](license-based-recon-files.md) affichent uniquement les transactions et les frais liés à l’utilisation (unités consommées et frais connexes).

> [!NOTE]
> Les crédits uniques, les remises ou les remboursements qui apparaissent sur la facture en tant qu' **ajustements** ne sont pas affichés dans le fichier de réconciliation.

## <a name="map-charge-types-to-invoice-charges"></a>Mapper les types de frais aux frais de facture

Pour faire référence à des montants de frais entre votre facture et le fichier de réconciliation, utilisez les options de filtre dans Microsoft Excel. Filtrez par types de frais sur votre fichier de rapprochement pour mapper les frais de facture à un ensemble de répartitions de frais sur le fichier de rapprochement.

## <a name="license-based-charges"></a>Frais basés sur les licences

Pour mapper ces frais basés sur des licences à votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Frais d’activation | Montant facturé au client lorsqu’il utilise l’abonnement après l’achat. |
| Frais d’annulation | Frais au prorata remboursés au client lors de la modification des sièges associés. |
| Annuler le taux d’instance | Frais au prorata annulés lorsque l’abonnement du client avec abonnement mensuel est suspendu et que les sièges associés ont été modifiés au cours du même mois. |
| Frais de cycle | Frais périodiques pour un abonnement. |
| Instance de cycle au prorata | Frais au prorata calculés par le client lors de la modification des sièges associés. |
| Frais liés au prorata en cas d’annulation | Remboursement calculé au prorata pour la partie inutilisée du service lors de l’annulation. |
| Frais liés au prorata en cas de conversion hors de l’offre actuelle | Frais facturés au prorata après la conversion de l’abonnement mensuel actuel en abonnement annuel. |
| Frais liés au prorata lors de la conversion vers une nouvelle offre | Frais au prorata après conversion d’un abonnement mensuel en nouvel abonnement annuel. |
| Frais au prorata à l’achat | Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle. |
| Frais d’achat | Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle. |
| Frais liés au prorata lors du renouvellement | Frais au prorata lors du renouvellement de l’abonnement. |
| Frais de renouvellement | Facturation pour le renouvellement d’un abonnement |
| Frais de prorata lors de l’activation | Frais au prorata de l’activation jusqu’à la fin de la période de facturation. |

## <a name="one-time-charges"></a>Frais à usage unique

Pour mapper ces frais à la fois sur votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Nouveau | Utilisé lors de la création d’un nouvel achat. |
| addQuantity | Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une augmentation. |
| removeQuantity | Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une diminution. |
| Annuler | Utilisé lorsqu’un abonnement est annulé. |
| Convertir | Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé. |

## <a name="usage-charges"></a>Frais d'utilisation

Pour mapper ces frais d’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Évaluer les frais d’utilisation lors de l’annulation | Frais d’utilisation de l’accès en cas d’annulation pour utilisation impayée au cours de la période de facturation actuelle. |
| Évaluer les frais d’utilisation pour le cycle actuel | Frais d’utilisation de l’accès pour la période de facturation en cours. |

### <a name="credits"></a>Crédits

Pour mapper ces crédits à votre facture :

- Additionner le **TotalForCustomer** à partir du fichier basé sur une licence.
- Totalisez la colonne **PostTaxTotal** à partir du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Décalage d’un élément de ligne | Remboursement partiel ou entier sur un élément de ligne, y compris les taxes. |

### <a name="usage-based-discounts"></a>Remises basées sur l’utilisation

Pour mapper ces remises basées sur l’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** à partir du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Remise d’activation | Remise appliquée lorsque l’abonnement est activé. |
| Remise au cycle | Remise appliquée sur les frais périodiques. |
| Remise de renouvellement | Remise appliquée lorsque l’abonnement est renouvelé. |
| Annuler la remise | Frais appliqués lorsque les remises sont annulées. |

### <a name="license-based-discounts"></a>Remises basées sur une licence

Pour mapper les remises basées sur les licences à votre facture, faites la somme de la colonne **TotalOtherDiscount** du fichier basé sur une licence.

*Les remises basées sur une licence peuvent être appliquées à plusieurs types de frais.*
