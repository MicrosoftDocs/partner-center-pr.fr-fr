---
title: Recevoir un paiement dans la place de marché commerciale
description: En savoir plus sur la réception de paiements pour les bénéfices sur la place de marché commerciale-place de marché Azure. Comprend la stratégie de paiement, l’état de retenue au paiement et les relevés de paiement.
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 61730eec204674d7ad095d1fffcd997f65d135ea
ms.sourcegitcommit: 7f595faf952bf2d6cdc229da38bd67ee701b2083
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/02/2020
ms.locfileid: "93189728"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>Recevoir un paiement dans la place de marché commerciale

Cet article contient des informations importantes sur la réception de paiements pour vos offres, modules complémentaires et revenus publicitaires. Elle résume la stratégie de paiement, les étapes requises avant le paiement et la présentation des relevés de paiement.

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>Contrats et stratégies de paiement de la place de marché commercial

L’obtention du paiement vous oblige à respecter les contrats et la politique de paiement.

- [Contrat](https://go.microsoft.com/fwlink/p/?LinkID=699560)de l’éditeur de place de marché Microsoft Azure : avant de payer, vous devez accepter ce contrat d’éditeur. Le présent contrat explique la relation entre vous et Microsoft en ce qui concerne les offres de vendeur dans la place de marché commercial, y compris les frais de stockage facturés par Microsoft pour chaque vente.
- La [stratégie](payout-policy-details.md) de paiement montre les stratégies de paiement de paiement, notamment le calendrier de paiement et les modes de paiement. La stratégie explique également le processus de non-paiement des clients.
- Les [Détails des taxes](tax-details-marketplace.md) décrivent les taxes relatives à la sélection des prix et à la responsabilité fiscale dans le cadre du contrat Microsoft [Publisher](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- Les **frais de stockage** sont officiellement définis dans le contrat d’éditeur. Les frais de stockage sont appliqués à toutes les ventes d’offres collectées par le Marketplace commercial, y compris les modules complémentaires.
- Les **paiements** sont effectués chaque mois (à condition que le seuil de paiement soit respecté). En général, nous envoyons tout paiement dû au cours d’un mois donné le 15 du mois. Les paiements prennent généralement entre 3 et 10 jours ouvrables supplémentaires pour atteindre votre compte de paiement. Pour plus d’informations, consultez [Seuils, modes et délais de paiement](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Étapes préalables avant le paiement

Avant d’être payé la première fois, vous devez configurer votre compte de paiement et remplir les formulaires bancaires et fiscaux nécessaires. Dans les formulaires bancaires et fiscaux, vous allez fournir vos modes de paiement préférés et les formulaires fiscaux pour la taxe à la retenue. Des formulaires bancaires et fiscaux sont nécessaires avant de pouvoir vous payer. Pour plus d’informations, consultez [configurer votre compte de paiement et vos formulaires fiscaux](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>État de paiement en attente

Par défaut, nous envoyons les paiements une fois par mois, comme décrit ci-dessus. Toutefois, vous avez la possibilité de mettre en attente vos paiements pour un programme et Microsoft ne diffusera pas vos paiements à votre compte. Si vous choisissez de mettre vos paiements en attente, nous continuerons à enregistrer les bénéfices dans la page **versements** . Toutefois, nous n’enverrons pas de paiements à votre compte tant que vous n’aurez pas retiré la mise en attente.

Pour mettre vos paiements en attente, sélectionnez l’icône d’engrenage de **paramètres** en haut à droite, puis **paramètres du développeur** . Sélectionnez **paiement et taxes** dans le menu de gauche, puis dans la section **attribution du profil de paiement et** de l’impôt, localisez le programme pour lequel vous souhaitez conserver les paiements. Cochez la case **conserver mon paiement** pour conserver les paiements pour ce programme. Vous pouvez modifier votre statut de conservation de paiement à tout moment, mais votre décision aura une incidence sur le versement mensuel suivant. Par exemple, si vous souhaitez mettre le paiement d’avril en attente, veillez à définir votre état de paiement en attente sur **Activé** avant la fin du mois de mars.

Une fois que vous avez défini votre état de blocage de paiement sur **activé** , tous les versements pour ce programme sont bloqués **jusqu’à ce** que vous désactiviez la case à cocher. Dans ce cas, vous êtes inclus au cours du prochain cycle de versement mensuel (à condition que le seuil de paiement soit respecté). Si vous avez des paiements en attente, mais que vous souhaitez que le paiement ait été généré en juin, désactivez la case à cocher pour **Désactiver** avant la fin de l’opération.

>[!Note]
> L’état d’attente de paiement s’applique à chaque programme individuellement (Microsoft Store, publicité, place de marché Azure, etc.). Si vous souhaitez conserver les paiements pour tous vos programmes, conservez le paiement sur chaque programme individuellement.

## <a name="payout-statements"></a>Relevés de paiements

Le relevé de paiement affiche vos revenus des ventes de vos offres et modules complémentaires dans l’historique des transactions. Vous pouvez également afficher les détails du paiement et télécharger les rapports au format TSV ou CSV. Pour en savoir plus sur l’accès à la déclaration de paiement et les détails de l’historique des transactions et des rapports de paiement, consultez les [instructions](payout-statement.md) de paiement. En outre, vous pouvez utiliser l' [API versements partenaires](https://apidocs.microsoft.com/services/partnerpayouts) pour extraire systématiquement les rapports de paiement.

## <a name="next-steps"></a>Étapes suivantes

- [API de paiement des partenaires](https://apidocs.microsoft.com/services/partnerpayouts)
- [FAQ sur les paiements de la Place de marché](payout-faq.md)
