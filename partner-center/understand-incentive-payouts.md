---
title: Afficher les détails de votre incentive et de votre programme
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Utilisez ces pages pour afficher et gérer l’état du programme d’incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 3d163271329e2f2a117d7df3abcf9b31f2c4979f
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755866"
---
# <a name="view-your-incentives-program-details"></a>Afficher les détails de votre programme d’incentives

**Rôles appropriés**

- Administrateur d’incentives
- Utilisateur de l’incentive
- Visionneuse en lecture seule incitative
- Administrateur général
- Administrateur de partenaire MPN

Cet article explique comment accéder à la page **vue d’ensemble de mes incentives** , qui indique l’état global de vos programmes d’incentives, ainsi que l’état de chaque programme à chaque emplacement. Il fournit également les différents États d’inscription. 

>[!NOTE]
>Pour plus d’informations sur les incentives et les incentives de l’espace partenaires, consultez [investissements et incentives](https://partner.microsoft.com/membership/partner-incentives) pour les partenaires (connexion requise).

## <a name="access-the-incentives-overview-page"></a>Accéder à la page de présentation des incentives

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard).
1. Sélectionnez **incentives**, puis **vue d’ensemble** dans le menu.
1. Vous pouvez voir le récapitulatif des gains et des paiements en haut de la page, ainsi que des informations supplémentaires dans le tableau ci-dessous. Vous pouvez également trier, regrouper et développer la table qui l’accompagne :

   - Pour trier par colonne, sélectionnez le nom de la colonne.
   - Pour regrouper par programme, sélectionnez l’onglet **par programme** au-dessus du tableau.
   - Pour regrouper par emplacement, sélectionnez l’onglet **par emplacement** au-dessus du tableau.
   - Pour afficher plus de détails sur les inscriptions au sein d’un groupe spécifique, sélectionnez le symbole représentant un Chevron à la fin d’une ligne donnée. Ce Chevron développe votre vue.
1. Si une action supplémentaire est nécessaire pour s’inscrire à un programme, ces informations s’afficheront dans la colonne **Status** (État). Dans ce cas, sélectionnez le symbole représentant un chevron pour connaître les étapes à suivre.

## <a name="enrollment-status"></a>État de l'inscription

Le tableau suivant décrit les différents États d’inscription indiqués dans la colonne **État** .

| **Statut**         | **Visible quand** |
|:------------------------------------|:------------------|
| Action requise  | Le partenaire a accepté une invitation à s’inscrire à un programme d’incentives, mais il peut avoir besoin de mettre à jour les informations bancaires ou fiscales. Consultez la colonne **actions requises** pour les étapes suivantes ou les liens pour mettre à jour vos informations bancaires ou fiscales dans l’espace partenaires. |
| Abandonné  | Le programme d’incentives spécifique n’est plus proposé dans le système d’incentives. |
| Inscrit  | Toutes les informations fiscales et bancaires ont été validées. Aucune autre action d’inscription n’est requise par le partenaire. |
| Inscription  | L’utilisateur n’est pas un administrateur d’incentives et l’inscription est dans l' **action requise** ou la validation des États d' **inscription** .|
| Inactif/inéligible | Le programme d’incentives n’est peut-être pas ouvert à l’inscription pour le moment ou le partenaire ne répond pas aux conditions d’inscription ou de réinscription. <br><br> Si l’État n’est pas **éligible**, le partenaire ne répond pas aux conditions d’éligibilité actuelles pour le programme ; Si vous sélectionnez le lien **voir les conditions d’éligibilité** sous l’état de l’inscription, vous verrez les conditions requises pour l’éligibilité et celles qui ont été respectées. <br><br> Vous pouvez également voir un état **inactif** pour les inscriptions d’organisation virtuelle (VORG) ou de compte global de partenaire (PGA) qui ne sont plus actives dans le programme d’incentives.  |
| Invité  | Une nouvelle invitation d’inscription au programme d’incentives a été envoyée au partenaire, mais le partenaire n’a pas encore démarré le processus d’inscription. La colonne adjacente **actions requises** affiche les étapes suivantes et les liens associés.  |
| Validation de l’inscription  | Le partenaire a déjà effectué ou mis à jour des informations bancaires et fiscales pour une inscription nouvelle ou existante et attend que Microsoft valide ces informations. Pendant le processus de validation, la validation de l' **inscription** peut s’afficher pendant jusqu’à 48 heures.  |

## <a name="see-your-payment-information"></a>Voir vos informations de paiement

Sélectionnez l’icône paiement dans le coin supérieur droit de l’écran pour accéder à ces différents résumés :

- Historique des transactions
- Paiements
- Exporter des données

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustre l’icône de paiement dans le coin supérieur droit du portail espace partenaires":::

Ces informations incluent le montant total des gains et des paiements d’incentives depuis que vous vous êtes inscrit aux programmes d’incentives. Cette page contient également les gains et les paiements par site ou par programme, ainsi que des actions supplémentaires que vous devrez peut-être effectuer pour vous inscrire à un programme dans un site en particulier. 

Vous pouvez également utiliser l' [API](https://apidocs.microsoft.com/services/partnerpayouts) de paiement de partenaire pour vous connecter et obtenir directement les données de paiement et de transaction de paiement. Pour en savoir plus, consultez les [instructions de paiement](payout-statement.md) .

## <a name="next-steps"></a>Étapes suivantes

- [Relevés de paiements](payout-statement.md)
