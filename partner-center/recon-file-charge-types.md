---
title: Types de frais de fichier de réconciliation | Espace partenaires
ms.topic: article
ms.date: 08/26/2019
description: Types de frais (basés sur une licence, basés sur l’utilisation et exceptionnels), crédits et remises sur les fichiers de rapprochement de l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389807"
---
# <a name="understand-charge-types"></a>Présentation des types de frais

S’applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Cette rubrique décrit les mappages entre une section de facture et les types de frais associés qui peuvent se trouver dans votre fichier de rapprochement. Votre facture fournit un résumé des frais. Votre fichier de réconciliation fournit une répartition détaillée des transactions d’éléments de ligne, y compris les types de frais. Pour plus d’informations sur les fichiers de rapprochement, voir [How to use Reconciliation Files](use-the-reconciliation-files.md).

Les fichiers de [réconciliation basés sur l’utilisation](usage-based-recon-files.md) et les [fichiers de réconciliation basés sur des licences](license-based-recon-files.md) affichent uniquement les transactions et les frais liés à l’utilisation (unités consommées et frais connexes).

> [!NOTE]
> Les crédits uniques, les remises ou les remboursements qui apparaissent sur la facture en tant qu' **ajustements** ne sont pas affichés dans le fichier de réconciliation.

## <a name="map-charge-types-to-invoice-charges"></a>Mapper les types de frais aux frais de facture

Pour faire référence à des montants de frais entre votre facture et le fichier de réconciliation, utilisez les options de filtre dans Microsoft Excel. Filtrez par types de frais sur votre fichier de rapprochement pour mapper les frais de facture à un ensemble de répartitions de frais sur le fichier de rapprochement.

## <a name="license-based-charges"></a>Frais basés sur la licence

Pour mapper ces frais basés sur des licences à votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Frais d’activation | Montant facturé au client lorsqu’il utilise l’abonnement après l’achat. |
| Frais d’annulation | Frais au prorata remboursés au client lors de la modification des sièges associés. |
| Frais de cycle | Frais périodiques pour un abonnement. |
| Instance de cycle au prorata | Frais au prorata calculés par le client lors de la modification des sièges associés. |
| Frais au prorata en cas d'annulation | Remboursement calculé au prorata pour la partie inutilisée du service lors de l’annulation. |
| Frais au prorata à l’achat | Type de frais d’un abonnement lors de l’utilisation de la facturation annuelle. |
| Frais d’abonnement | Type de frais d’un abonnement lors de l’utilisation de la facturation mensuelle. |
| Frais au prorata lors du renouvellement | Frais au prorata lors du renouvellement de l’abonnement. |
| Frais de renouvellement | Frais de renouvellement d'un abonnement |
| Frais au prorata lors de l'activation | > des frais au prorata de l’activation jusqu’à la fin de la période de facturation. |

## <a name="one-time-charges"></a>Frais à usage unique

Pour mapper ces frais à la fois sur votre facture, faites la somme de la colonne **amount** du fichier basé sur une licence.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Nouveau | Utilisé lors de la création d’un nouvel achat. |
| addQuantity | Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une augmentation. |
| removeQuantity | Utilisé dans le remboursement de l’achat d’origine et la nouvelle quantité après une diminution. |
| Cancel | Utilisé lors de l’annulation d’un abonnement. |
| Convertir | Utilisé lors de la mise à niveau d’une licence, mais le nombre de sièges reste inchangé. |

## <a name="usage-charges"></a>Frais d’utilisation

Pour mapper ces frais d’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Évaluer les frais d’utilisation lors de l'annulation | Frais d’utilisation de l’accès en cas d’annulation pour une utilisation sans paiement durant la période de facturation actuelle. |
| Évaluer les frais d’utilisation pour le cycle actuel | Frais d’utilisation de l’accès pour la période de facturation actuelle. |

### <a name="credits"></a>Crédits

Pour mapper ces crédits à votre facture :

- Additionner le **TotalForCustomer** à partir du fichier basé sur une licence.
- Totalisez la colonne **PostTaxTotal** à partir du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Décalage d’un élément de ligne | Remboursement partiel ou entier à un article de ligne, y compris les taxes. |

### <a name="usage-based-discounts"></a>Remises basées sur l’utilisation

Pour mapper ces remises basées sur l’utilisation à votre facture, faites la somme de la colonne **PretaxCharges** à partir du fichier d’utilisation.

| Description des frais (colonne ChargeType dans le fichier de rapprochement) | Explication des frais |
| ------------------------------------------------------------- | ------------------ |
| Remise sur l’activation | Remise appliquée lorsque l’abonnement est activé. |
| Remise sur le cycle | Remise appliquée sur les frais périodiques. |
| Renouveler la remise | Remise appliquée lorsque l’abonnement est renouvelé. |
| Annuler la remise | Frais appliqués lors de l’annulation des remises. |

### <a name="license-based-discounts"></a>Remises basées sur la licence

Pour mapper les remises basées sur les licences à votre facture, faites la somme de la colonne **TotalOtherDiscount** du fichier basé sur une licence.

*Les remises basées sur une licence peuvent être appliquées à plusieurs types de frais.*
