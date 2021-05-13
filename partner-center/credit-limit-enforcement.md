---
title: Application de la limite de crédit
ms.topic: how-to
ms.date: 05/11/2021
description: En savoir plus sur la limite de crédit et la façon dont elle est calculée. Comprend un Forum aux questions.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819207"
---
# <a name="credit-limit-enforcement-cle"></a>Application de la limite de crédit (CLE)

**Rôles appropriés**

- Administrateur de la facturation

## <a name="your-credit-limit-and-how-it-works"></a>Votre limite de crédit et son fonctionnement

Votre limite de crédit est le montant maximal (en dollars américains) que vous pouvez consacrer à l’achat de produits ou d’abonnements dans l’espace partenaires. Si vous dépassez votre limite de crédit, vous ne pourrez pas effectuer de nouveaux achats tant que vous n’aurez pas effectué un paiement suffisant. Vos abonnements existants vont se poursuivre sans interruption.

Les limites de crédit s’appliquent aux offres dans le plan Azure, les réservations Azure, les logiciels, la place de marché, les produits Azure 145 P, Office et Dynamics. Les limites de crédit ne s’appliquent pas aux renouvellements et à la consommation en cours.

Nous attribuons votre limite de crédit au niveau du locataire durant votre période d’intégration. Nous la baserons sur les revenus prévus, les prouesses en achetant et l’historique des paiements. Nous utilisons ensuite la formule suivante pour calculer le solde disponible :

**[Limite de crédit – (achat entrant + factures non payées en attente + frais non facturés – trop-perçus)]**

## <a name="frequently-asked-questions"></a>Forum Aux Questions

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Ma limite de crédit est-elle définie au niveau du client ou du niveau global ?

Niveau du locataire. Par exemple, supposons que vous travaillez à partir des États-Unis, du Canada et du Japon. Si le client canadien atteint sa limite de crédit, ce locataire reçoit une notification lorsqu’il tente d’effectuer un achat dans l’espace partenaires. Les autres locataires ne seront pas affectés. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Si ma limite de crédit est dépassée, puis-je continuer à traiter les clients et les abonnements existants avec un accès complet ?

Oui. Les abonnements existants de vos clients continueront sans interruption. Toutefois, vous ne pouvez pas acheter de nouveaux abonnements pour vos clients.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>CLE s’applique-t-elle aux partenaires directs et aux fournisseurs indirects ?

Oui, il s’applique aux deux.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Après avoir envoyé mon paiement pour rétablir mon compte, quand puis-je acheter des abonnements supplémentaires ? 

Vous devez être en mesure de reprendre l’achat dans les 24 heures qui suivent votre paiement, en supposant que Microsoft a reçu toutes les conditions requises pour effectuer le processus de vérification de solvabilité.

### <a name="how-can-i-check-my-credit-limit"></a>Comment puis-je vérifier la limite de crédit ?

Contactez [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) pour voir votre limite de crédit et obtenir des informations sur les achats récents.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>Les factures en litige sont-elles associées à la limite de crédit ?

Oui. Toutefois, vous pouvez contacter Microsoft à [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) l’adresse pour résoudre le problème.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>À quel moment puis-je me rappeler si j’écris ucmwrcsp@microsoft.com ?

Vous devez avoir une réponse en moins de 24 heures. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Quels critères Microsoft utilise-t-il pour définir la limite de crédit d’un partenaire ?

Nous déterminons votre limite de crédit en fonction de vos revenus prévus, de l’acquisition des prouesses et de l’historique des paiements.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>La limite de crédit est-elle actuellement appliquée à la nouvelle expérience de commerce ?

Oui. Les limites de crédit s’appliquent à tous les programmes et produits CSP dans l’espace partenaires.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Qui recevra la notification lorsque mon organisation est proche de sa limite de crédit ?

Le contact financier de votre organisation doit recevoir la notification.

## <a name="next-steps"></a>Étapes suivantes

[Notions de base de facturation](./billing-basics.md)
