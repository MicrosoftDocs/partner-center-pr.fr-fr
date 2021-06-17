---
title: Résolution des problèmes liés aux paiements et aux bénéfices
ms.topic: article
ms.date: 02/05/2021
description: Découvrez comment résoudre des problèmes tels que des revenus manquants ou incorrects, des problèmes d’éligibilité et comment concilier vos revenus d’incentives.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ad71a6e02d6472ae844c504491e5acb05d5d6426
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277859"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Résolution des problèmes liés aux paiements manquants, aux revenus incorrects et à d’autres problèmes

**Rôles appropriés**: administrateur d’incentives

Cet article vous aidera à résoudre les éventuels problèmes de paiement ou de paiement dans votre programme d’incentives. Les sujets traités incluent le minutage des paiements, la vérification de l’admissibilité de vos bénéfices et l’importance de la configuration correcte de vos profils de paiement et de taxe.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Qui peut créer ou mettre à jour les profils de paiement et de taxes pour mon organisation ?

Les utilisateurs qui ont le rôle d’administrateur d’incentives dans l’espace partenaires pour le programme d’incentives approprié et l’emplacement MPN peuvent mettre à jour et afficher les profils de paiement et de taxes de l’organisation.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Combien de temps faut-il pour que Microsoft approuve mes profils de paiement et/ou fiscaux ?

La validation peut prendre jusqu’à 48 heures. Pendant ce temps, votre profil présente l’état Inscription en cours de validation dans la page Vue d’ensemble. Une fois le processus terminé, l’État s’affiche comme **inscrit** en cas de réussite ou **action requise – mettre à jour les détails du paiement et/ou** de la taxe, si nécessaire.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Comment savoir si mon profil de paiement et fiscal est bien renseigné ?

L’état de votre inscription est indiqué dans la page Vue d’ensemble. Lorsque vous avez terminé de créer vos profils, votre statut est **validation** de l’inscription. Une fois vos informations validées, votre statut devient **inscrit**. Cet état indique que votre paiement et votre profil fiscal et que votre inscription a été effectuée avec succès.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Pourquoi je dois mettre à jour mon profil fiscal pour l’utiliser avec un nouveau programme d’incentive ?

Nous payons les incentives de différents endroits qui varient en fonction du type de d’incentive. Selon les endroits et les règles du programme d’incentive, des informations fiscales supplémentaires peuvent être nécessaires au traitement.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Comment supprimer un profil de paiement et/ou fiscal ?

Microsoft n’offre pas actuellement la possibilité de supprimer les profils de paiement et fiscaux existants.

## <a name="my-payment-is-missing-or-incorrect"></a>Mon paiement est manquant ou incorrect

La raison de paiements manquants ou incorrects est souvent l’une des suivantes :

- **Vous n’êtes peut-être pas éligible.**  Les gains seront disponibles uniquement si vous respectez les conditions d’éligibilité opérationnelle, c’est-à-dire que vous êtes inscrit à la période de rémunération du programme correspondante.
- **Vous n’avez peut-être pas respecté les exigences.**  Vérifiez que vous répondez aux critères d’éligibilité et aux règles de revenus éligibles pour l’incentive recherché.

  **Pour vérifier votre éligibilité**

  1. Connectez-vous à [incentives partenaires](https://partner.microsoft.com/membership/partner-incentives).

  2. Faites défiler jusqu’à la liste des documents de votre programme.
  
  3. Sélectionnez le lien de document souhaité, puis passez en revue les sections 

L' **éligibilité des partenaires** et les règles de **revenus éligibles**.

- **Votre profil de paiement est peut-être incomplet.** La date de début de vos gains d’incentives sera le premier jour du mois où vous avez rempli toutes les conditions d’éligibilité, notamment l’intégration des détails fiscaux et de paiement. Les gains ne seront pas disponibles pour les mois antérieurs à la finalisation du paiement et des taxes. Par exemple, si vous répondez à toutes les conditions au cours du mois d’avril 2020, la date de début de vos gains sera le 1er avril 2020.
- **Vous avez peut-être une action en suspens**.  Il est possible que vos primes incitatives ne soient pas traitées car que vous ayez mis une action en attente.

  **Pour afficher vos actions en suspens**

  1. Connectez-vous à [incentives partenaires](https://partner.microsoft.com/membership/partner-incentives).
  2. Ouvrez la page **historique des transactions** . Passez en revue les champs de cette page pour connaître les actions en suspens à effectuer, comme le **profil d’impôt en** attente, le **profil de paiement en** attente ou l’envoi d’un **facture d’impôt en attente**.

Si ces actions ne sont pas utiles et que vos paiements sont toujours manquants ou incorrects, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>Comment puis-je concilier mes ajustements ?

Vous pouvez localiser et concilier vos ajustements en téléchargeant les détails de votre transaction et de vos revenus.

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard/).
2. Dans la barre de navigation supérieure, sélectionnez l’icône Money, puis sélectionnez **historique des transactions**.
3. Appliquez les filtres appropriés. (Voir la Remarque **importante** ci-dessous.)
4. Une fois que vous avez filtré vos données, sélectionnez **Démarrer le téléchargement**, puis **Exporter les données**. Vos données s’ouvrent dans un fichier CSV.
5. Dans le fichier CSV, accédez à la colonne P, **type** acquis.
6. Filtrez cette colonne pour l' **ajustement-remise**. Vous pouvez voir le mois de chaque ajustement dans la colonne S.

>[!IMPORTANT]
>Les ajustements appliqués aux périodes de paie précédentes ne seront pas visibles dans le bénéfice du mois au cours duquel l’ajustement a été appliqué. Les ajustements seront toujours reflétés dans le rapport des bénéfices pour le mois auquel l’ajustement a été appliqué.
>
>Par exemple, un ajustement du salaire de janvier 2019 qui a été traité en septembre 2019 ne reflète pas le montant des bénéfices pour le 2019 septembre. Toutefois, lorsque le paiement pour le 2019 septembre est reçu, il inclut l’ajustement du 2019 du 1er janvier qui a été appliqué en septembre. Dans ce scénario, vous devez télécharger les détails de la transaction du 2019 janvier pour voir l’ajustement qui a été appliqué.
>
>Gardez cela à l’esprit lorsque vous définissez vos filtres de date. Comme indiqué ci-dessus, les ajustements pour les périodes précédentes ne sont visibles que dans le mois auquel l’ajustement a été appliqué. Vérifiez que la plage de dates sélectionnée correspond au mois de l’ajustement que vous tentez de localiser. Vous devrez peut-être sélectionner **Effacer tout** pour supprimer vos filtres, puis en appliquer de nouveaux.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Pourquoi les paiements au titre de ma demande de coopération sont-ils effectués dans deux monnaies différentes ?

Quand les fonds de coopération proviennent de différentes entités Microsoft, les paiements sont effectués dans la monnaie locale de chaque entité.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Pourquoi ai-je été payé dans une autre monnaie que celle de ma demande de financement ?

À chaque programme d’incentive correspond un profil bancaire qui a été créé pendant la configuration. La monnaie spécifiée dans ce profil correspond à la monnaie dans laquelle vous êtes payé.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Je ne vois pas les bénéfices pour une période donnée

Si vous ne voyez pas les bénéfices pour une période dans laquelle ils sont attendus, cela est généralement dû à l’un des problèmes suivants :

- **Vous n’êtes peut-être pas éligible.**  Les gains seront disponibles uniquement si vous respectez les conditions d’éligibilité opérationnelle, c’est-à-dire que vous êtes inscrit à la période de rémunération du programme correspondante.

- **Votre profil de paiement est peut-être incomplet.**  La date de début de vos gains d’incentives sera le premier jour du mois où vous avez rempli toutes les conditions d’éligibilité, notamment l’intégration des détails fiscaux et de paiement. Les gains ne seront pas disponibles pour les mois antérieurs à la finalisation du paiement et des taxes. Par exemple, si vous répondez à toutes les conditions au cours du mois d’avril 2020, la date de début de vos gains sera le 1er avril 2020.

Si vous avez rempli les conditions d’éligibilité, y compris l’intégration avec le paiement et les détails fiscaux, et que les revenus sont toujours manquants, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="my-earnings-are-missing-or-incorrect"></a>Mes revenus sont manquants ou incorrects

Des gains manquants ou incorrects peuvent être le résultat de l’un des problèmes suivants :

- **Vous n’avez peut-être pas respecté les conditions.**  Vérifiez que vous répondez aux critères d’[éligibilité](#my-payment-is-missing-or-incorrect) et aux règles de revenus éligibles pour l’incentive recherché.

- **Il peut y avoir des écarts.**  Si vous remplissez les conditions d’éligibilité et [de bénéfice du](incentives-confirm-your-earnings-eligibility.md) [programme](incentives-determined-your-program-eligibility.md) et que vos revenus semblent toujours incorrects, les informations suivantes peuvent vous aider à récupérer vos données.

Les bénéfices s’affichent dans la page **historique des transactions** et dans la page **paiements** . Vous pouvez accéder aux deux pages en sélectionnant l’icône **paiement** dans la barre de navigation de l’espace partenaires.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Informations de transaction.":::

Les montants de gain mensuels dans la vue historique des transactions peuvent ne pas s’aligner sur le montant de paiement reçu pour un mois spécifique. Cela est dû à des recalculs et des ajustements pour les périodes d’approvisionnement antérieurs qui sont appliquées aux paiements futurs.

Par exemple, un ajustement du salaire de janvier 2019 qui a été traité en septembre 2019 ne sera pas reflété dans le montant des bénéfices pour le 2019 septembre. Toutefois, lorsque le paiement pour le 2019 septembre est reçu, il inclut l’ajustement du 2019 du 1er janvier qui a été appliqué en septembre.

Dans ce scénario, vous devez télécharger les détails de la transaction pour obtenir une vue complète de tous les bénéfices inclus dans votre paiement.  En outre, vous pouvez accéder à la vue paiements pour télécharger des transactions pour chaque paiement.

### <a name="transaction-history"></a>Historique des transactions

Cette vue affiche les tendances de paiement et de paiement par mois, les bénéfices par État et les détails de la transaction, ainsi que l’état du paiement pour chaque transaction. Les données ne sont visibles que pour les programmes et ID MPN pour lesquels vous êtes un utilisateur ou un administrateur d’incentives.

### <a name="payments"></a>Paiements

Cette vue vous permet d’afficher les paiements pour tous les programmes et ID MPN. Les données ne sont visibles que pour les programmes et ID MPN pour lesquels vous êtes un utilisateur ou un administrateur d’incentives. À partir de cette vue, vous pouvez télécharger la remise ou afficher les détails de la transaction par paiement.

| Pour | Accédez ici |
| ------ | :----------- | 
| Affichez vos informations de paiement par ligne, y compris les montants de versement et de paiement en devise locale  | Afficher le champ **liste des paiements**   |
| Télécharger une lettre de remise   |  Sélectionner la **remise de paiement**  |
| Afficher les détails de niveau transaction pour un paiement spécifique |  Sélectionner une **vue**  |
| Exporter les détails d’une transaction vers Excel  |  Sélectionnez **Démarrer le téléchargement**, puis **Exporter les données**. Tous les filtres sélectionnés seront appliqués aux données exportées. Une fois que l’État est passé à terminé, sélectionnez **Télécharger** et suivez les invites pour exporter le rapport détaillé des transactions. Actualisez la page si l’État n’est pas mis à jour dans un délai de cinq minutes.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Revenus et paiements manquants ou incorrects

Si vous ne parvenez pas à localiser les détails d’un paiement ou d’une transaction, vérifiez si vous avez appliqué les filtres appropriés. Dans la mesure où certains noms de programme ont changé (par exemple, le fournisseur CSP 1T direct Partner est désormais un partenaire de facturation directe), vous devrez peut-être utiliser plusieurs sélections.

Si vous ne trouvez toujours pas vos revenus ou si vous pensez que les bénéfices affichés sont incorrects, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Comment faire concilier mes revenus ?

Si vous constatez des écarts dans vos revenus, effectuez les étapes suivantes :

1. **Vérifiez que vous êtes éligible aux gains**.  Les bénéfices seront disponibles uniquement si vous remplissez les conditions d’éligibilité [et de bénéfice du](incentives-confirm-your-earnings-eligibility.md) [programme](incentives-determined-your-program-eligibility.md) .

2. **Vérifiez que votre profil de paiement est complet.**  La date de début de vos gains d’incentives sera le premier jour du mois où vous avez rempli toutes les conditions d’éligibilité, notamment l’intégration des détails fiscaux et de paiement. Les gains ne seront pas disponibles pour les mois antérieurs à la finalisation du paiement et des taxes. Par exemple, si vous répondez à toutes les conditions au cours du mois d’avril 2020, la date de début de vos gains sera le 1er avril 2020. 

3. **Vérifiez que vous remplissez toutes les conditions**.  Vérifiez que vous avez respecté les règles d' [éligibilité](#my-payment-is-missing-or-incorrect) et de chiffre d’affaires éligible pour votre programme d’incentives.

Si ces actions ne sont pas utiles et que vos revenus ne sont toujours pas conciliés, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>Où puis-je trouver mes tarifs ?

1. Connectez-vous à [incentives partenaires](https://partner.microsoft.com/membership/partner-incentives).

2. Faites défiler la liste pour accéder aux documents de votre programme.

3. Sélectionnez le lien du document pour le programme correspondant.

4. Dans le document, reportez-vous à la section **structure et tarifs du programme**.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les demandes de coopération](incentives-managing-co-op-claims.md)