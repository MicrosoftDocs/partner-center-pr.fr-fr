---
title: Obtenir le paiement dans l’espace partenaires
description: en savoir plus sur la réception de paiements pour les revenus en tant que partenaire Microsoft, par exemple via des offres de la place de marché commercial, des programmes d’incentives et le programme fournisseur de solutions Cloud. Comprend la stratégie de paiement, l’état de retenue au paiement et les instructions de paiement.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: cc01a1aada6c6665d3fd8f6efc6e5ef873736bdc
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684387"
---
# <a name="getting-paid-in-partner-center"></a>Obtenir le paiement dans l’espace partenaires

**Rôles appropriés**: administrateur de compte | Administrateur général

Cet article contient des informations importantes sur la réception de paiements pour vos offres, modules complémentaires et revenus publicitaires. Elle résume la stratégie de paiement, les étapes requises avant le paiement et la présentation des relevés de paiement.

## <a name="payout-policies-and-agreements"></a>Stratégies et contrats de paiement

L’obtention du paiement vous oblige à respecter les contrats et la politique de paiement.

- [Microsoft Azure Marketplace Publisher contrat](/legal/marketplace/msft-publisher-agreement): avant d’être payé, vous devez accepter ce contrat d’éditeur. Le présent contrat explique la relation entre vous et Microsoft en ce qui concerne les offres de vendeur dans la place de marché commercial, y compris les frais de stockage facturés par Microsoft pour chaque vente.
- La [stratégie](payout-policy-details.md) de paiement montre les stratégies de paiement de paiement, notamment le calendrier de paiement et les modes de paiement. La stratégie explique également le processus de non-paiement des clients.
- les [détails des taxes](tax-details-marketplace.md) décrivent les taxes relatives à la sélection des prix et à la responsabilité fiscale dans le cadre du contrat de [Publisher](/legal/marketplace/msft-publisher-agreement)Microsoft.
- les **frais de stockage** sont officiellement définis dans le contrat de Publisher. Les frais de stockage sont appliqués à toutes les ventes d’offres collectées par le Marketplace commercial, y compris les modules complémentaires.
- Les **paiements** sont effectués chaque mois (à condition que le seuil de paiement soit respecté). En règle générale, nous envoyons tout paiement dû pendant un mois donné, le 15 du mois. Les paiements prennent généralement entre 3 et 10 jours ouvrables supplémentaires pour atteindre votre compte de paiement. Pour plus d’informations, consultez [Seuils, modes et délais de paiement](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Étapes préalables avant le paiement

Avant d’être payé la première fois, vous devez configurer votre compte de paiement et remplir les formulaires bancaires et fiscaux nécessaires. Dans les formulaires bancaires et fiscaux, vous allez fournir vos modes de paiement préférés et les formulaires fiscaux pour la taxe à la retenue. Des formulaires bancaires et fiscaux sont nécessaires avant de pouvoir vous payer. Pour plus d’informations, consultez [configurer votre compte de paiement et vos formulaires fiscaux](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>État de paiement en attente

Par défaut, nous envoyons les paiements une fois par mois, comme décrit ci-dessus. Toutefois, vous pouvez mettre en attente vos paiements pour un programme, et Microsoft ne diffusera pas vos paiements à votre compte. Si vous choisissez de mettre vos paiements en attente, nous continuerons à enregistrer les bénéfices dans la page **versements** . Toutefois, nous n’enverrons pas de paiements à votre compte tant que vous n’aurez pas retiré la mise en attente.

pour mettre vos paiements en attente, sélectionnez l’icône d’engrenage **Paramètres** en haut à droite, puis **paramètres de compte**. Sélectionnez **paiement et taxes** dans le menu de gauche, puis dans la section **attribution du profil de paiement et** de l’impôt, localisez le programme pour lequel vous souhaitez conserver les paiements. Cochez la case **conserver mon paiement** pour conserver les paiements pour ce programme. Vous pouvez modifier votre statut de conservation de paiement à tout moment, mais votre décision aura une incidence sur le versement mensuel suivant. Par exemple, si vous souhaitez mettre le paiement d’avril en attente, veillez à définir votre état de paiement en attente sur **Activé** avant la fin du mois de mars.

Une fois que vous avez défini votre état de blocage de paiement sur **activé**, tous les versements pour ce programme sont bloqués **jusqu’à ce** que vous désactiviez la case à cocher. Dans ce cas, vous êtes inclus au cours du prochain cycle de versement mensuel (à condition que le seuil de paiement soit respecté). Si vous avez des paiements en attente, mais que vous souhaitez que le paiement ait été généré en juin, désactivez la case à cocher pour **Désactiver** avant la fin de l’opération.

>[!Note]
> l’état d’attente de paiement s’applique à chaque programme individuellement (Microsoft Store, publicité, place de marché Azure, etc.). Si vous souhaitez conserver les paiements pour tous vos programmes, conservez le paiement sur chaque programme individuellement.

## <a name="payout-statements"></a>Relevés de paiements

Le relevé de paiement affiche vos revenus des ventes de vos offres et modules complémentaires dans l’historique des transactions. Vous pouvez également afficher les détails du paiement et télécharger les rapports au format TSV ou CSV. Pour en savoir plus sur l’accès à la déclaration de paiement et les détails de l’historique des transactions et des rapports de paiement, consultez les [instructions](payout-statement.md) de paiement. En outre, vous pouvez utiliser l' [API versements partenaires](https://apidocs.microsoft.com/services/partnerpayouts) pour extraire systématiquement les rapports de paiement.

## <a name="next-steps"></a>Étapes suivantes

- [API de paiement des partenaires](https://apidocs.microsoft.com/services/partnerpayouts)
- [FAQ sur les paiements](payout-faq.yml)