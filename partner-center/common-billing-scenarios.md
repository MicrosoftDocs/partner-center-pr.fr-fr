---
title: "Scénarios de facturation courants | Espace partenaires"
description: "Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et les abonnements basés sur la licence sont affectés différemment."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 92805672975e319b53c2cd89063442df2feb1267
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2017
---
# <a name="common-billing-scenarios"></a>Scénarios de facturation courants

**S'applique à**

-  Espace partenaires
-  Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis
-  Espace partenaires de MicrosoftCloud Allemagne

Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, modifiez le nombre de licences dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et ceux basés sur la licence sont affectés différemment.

## <a name="in-this-section"></a>Dans cette section


-   [Facturation basée sur l’utilisation](#usagebased)

-   [Facturation basée sur la licence](#licensebased)

## <a href="" id="usagebased"></a>Facturation basée sur l’utilisation


Seuls les services utilisés dans la période de facturation précédente vous sont facturés. Les services et applications Azure qui sont activés et utilisés pendant la période de facturation apparaissent sur la facture.

-   Les barèmes des services peuvent changer au cours du cycle de facturation.
    -   Augmentation de prix: préavis de 30jours.
    -   Les réductions de prix s’appliquent à compter du jour où elles prennent effet.
    -   Les abonnements existants sont facturés au taux en vigueur au début du cycle de facturation.
    -   Les nouveaux abonnements (créés au cours du cycle de facturation) sont facturés au taux en vigueur lorsque vous les avez ajoutés.
-   Si vous annulez un abonnement au cours du premier cycle de facturation, les frais d’utilisation apparaissent dans le fichier de rapprochement de la période pendant laquelle l’abonnement était actif.

## <a href="" id="licensebased"></a>Facturation basée sur la licence

Pour les mois durant lesquels aucune modification n’a été apportée aux abonnements basés sur la licence, un seul élément par abonnement apparaît sur votre facture. Il s’agit de l’avance de frais pour le mois suivant.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Scénario</td>
<td>Description</td>
<td>Exemple</td>
</tr>
<tr class="even">
<td>Nouvel abonnement ajouté</td>
<td><p>La période entre la date de début de l’abonnement et la première date de facturation est GRATUITE.</p>
<p>Votre fichier de rapprochement contient un seul élément:</p>
<ul>
<li>L’avance de frais pour le mois suivant</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nouvel abonnement: annulé avant la fin de la période de facturation</td>
<td>Les frais ne seront pas appliqués au compte. L’abonnement n’apparaîtra pas dans le fichier de rapprochement. Ceci est utile si vous voulez effectuer des tests sans que cela implique des frais d’abonnement.</td>
<td></td>
</tr>
<tr class="even">
<td>Nouvel abonnement: avec modification du nombre de licences pendant la période gratuite</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments:</p>
<ul>
<li>la modification du nombre de licences, facturée au prix unitaire0. (la modification du nombre de licences ne génère aucun frais pendant la période gratuite)</li>
<li>l’avance de frais pour le mois suivant, reflétant la nouvelle quantité.</li>
</ul></td>
<td>Utilisation au prorata:
<ul>
<li>Du 3au7juin pour 10licences = ZÉRO frais</li>
<li>Du 8au11juin pour 20licences = ZÉRO frais</li>
<li>Du 12au14 juin pour 15licences = ZÉRO frais</li>
</ul>
<p>Échéance de facturation: avance de frais pour l’intégralité du mois du 15juin au 14juillet pour 15licences. À supposer que les frais par abonnement et par mois soient de 10USD, ils se monteront à 10USD x 15licences = 150USD.</p></td>
</tr>
<tr class="odd">
<td>Abonnement existant: augmenter ou réduire le nombre de licences</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments:</p>
<ul>
<li>l’extourne de l’avance de frais</li>
<li>les frais d’utilisation au prorata</li>
<li>l’avance de frais pour le mois suivant</li>
</ul></td>
<td><p>Utilisation au prorata:</p>
<ul>
<li>Du 15au19juillet pour 15licences = 26,61USD</li>
<li>Du 20au30juillet pour 12licences = 46,84USD</li>
<li>Du 31juillet au9août pour 18licences = 63,87USD</li>
<li>Du 10au14août pour 10licences = 17,74USD</li>
</ul>
Extourne de l’avance de frais pour l’intégralité du mois du 15juillet au 14août = -165USD.
<p>Limite de facturation: l’avance de frais pour le mois complet entre le 15août et le 14septembre pour 10licences = 110USD.</p></td>
</tr>
<tr class="even">
<td>Annulation: aucune modification préalable du nombre de licences</td>
<td><p>Votre fichier de rapprochement contient un seul élément:</p>
<ul>
<li>Un crédit pour les jours non utilisés, l’intégralité de la période ayant été facturée d’avance dans le document de facturation précédent. Cette valeur est calculée en fonction de la date de fin de l’abonnement.</li>
</ul></td>
<td>Avance de frais déjà facturée: du 15août au 14septembre pour 10licences = 100USD.
<p>Part utilisée de l’avance de frais du 15août au 24août.</p>
<p>Crédit pour les jours non utilisés: du 25août au 14septembre pour 10licences = -74,51.</p></td>
</tr>
<tr class="odd">
<td>Annulation: avec modification préalable du nombre de licences</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments:</p>
<ul>
<li>l’extourne de l’avance de frais</li>
<li>les frais d’utilisation au prorata</li>
<li>un crédit pour les jours non utilisés</li>
</ul></td>
<td>Avance de frais déjà facturée: du 15août au 14septembre pour 10licences = 100USD.
<p>Utilisation au prorata:</p>
<ul>
<li>Du 15au 24août pour 10licences</li>
<li>Du 25août au 14septembre pour 5licences</li>
</ul>
<p>Crédit pour les jours non utilisés: du 1er au 14septembre pour 5licences.</p>
<p>Extourne de l’avance de frais pour l’intégralité du mois du 15août au 14septembre = -100USD.</p></td>
</tr>
</tbody>
</table>




 



