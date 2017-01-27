---
title: "Scénarios de facturation courants | Espace partenaires"
description: "Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et les abonnements basés sur la licence sont affectés différemment."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: e1825890f208a90b9b5694f4000ac06687ac87ab
ms.openlocfilehash: 5ac69f33ca78be1eca2af439a48d6d0904a4cfc5

---

# Scénarios de facturation courants

**S'applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud Germany

Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement. Les abonnements basés sur l’utilisation et les abonnements basés sur la licence sont affectés différemment.

## Dans cette section


-   [Facturation basée sur l’utilisation](#usagebased)

-   [Facturation basée sur la licence](#licensebased)

## <a href="" id="usagebased"></a>Facturation basée sur l’utilisation


Seuls les services utilisés dans la période de facturation précédente vous sont facturés. Les services et applications Azure qui sont activés et utilisés pendant la période de facturation apparaissent sur la facture.

-   La première facture indique la période initiale entre la date de début de l’abonnement et la date de la première facture.
-   Les barèmes des services peuvent changer au cours du cycle de facturation.
    -   Augmentation de prix&nbsp;: préavis de 30&nbsp;jours.
    -   Réduction de prix&nbsp;: jour d’application de la modification.
    -   Les abonnements existants utilisent le taux en vigueur au début du cycle de facturation.
    -   Les nouveaux abonnements (créés au cours du cycle de facturation) utilisent le taux en vigueur à la date de création.
-   Si vous annulez un abonnement avant la fin de sa première période de facturation ou à un moment donné pendant le cycle de facturation, les frais d’utilisation apparaissent dans le fichier de rapprochement de la période pendant laquelle l’abonnement était actif.

## <a href="" id="licensebased"></a>Facturation basée sur la licence


Pour les mois durant lesquels aucune modification n’a été apportée aux abonnements basés sur la licence, un seul élément par abonnement apparaît sur votre fichier de rapprochement et sur votre facture&nbsp;: l’avance de frais pour le mois suivant.

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
<td>Nouvel abonnement</td>
<td><p>La période entre la date de début de l’abonnement et la première date de facturation est GRATUITE.</p>
<p>Votre fichier de rapprochement contient un seul élément :</p>
<ul>
<li>l’avance de frais pour le mois suivant</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nouvel abonnement : annulé avant la fin de la période de facturation</td>
<td>Les frais ne seront pas être appliqués au compte. L’abonnement n’apparaîtra pas dans le fichier de rapprochement. Ceci est utile si vous voulez effectuer des tests sans que cela implique des frais d’abonnement.</td>
<td></td>
</tr>
<tr class="even">
<td>Nouvel abonnement : avec ajustement de la quantité de licences pendant la période gratuite.</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments :</p>
<ul>
<li>modification du nombre de licences, facturées au prix unitaire 0. (la modification du nombre de sièges ne génère aucun frais pendant la période gratuite)</li>
<li>l’avance de frais pour le mois suivant, reflétant la nouvelle quantité.</li>
</ul></td>
<td>Utilisation au prorata :
<ul>
<li>Du 3 au 7 juin pour 10 sièges = ZÉRO frais</li>
<li>Du 8 au 11 juin pour 20 sièges = ZÉRO frais</li>
<li>Du 12 au 14 juin pour 15 sièges = ZÉRO frais</li>
</ul>
<p>Échéance de facturation : avance de frais pour l’intégralité du mois du 15 juin au 14 juillet pour 15 sièges. À supposer que les frais par abonnement et par mois soient de 10 USD, ils se monteront à 10 USD x 15 sièges = 150 USD.</p></td>
</tr>
<tr class="odd">
<td>Abonnement existant : augmenter ou diminuer la quantité de licences</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments :</p>
<ul>
<li>l’extourne de l’avance de frais</li>
<li>les frais d’utilisation au prorata</li>
<li>l’avance de frais pour le mois suivant</li>
</ul></td>
<td><p>Utilisation au prorata :</p>
<ul>
<li>Du 15 au 19 juillet pour 15 sièges = 26,61 USD</li>
<li>Du 20 au 30 juillet pour 12 sièges = 46,84 USD</li>
<li>Du 31 juillet au 9 août pour 18 sièges = 63,87 USD</li>
<li>Du 10 au 14 août pour 10 sièges = 17,74 USD</li>
</ul>
Extourne de l’avance de frais pour l’intégralité du mois du 15 juillet au 14 août = -165 USD.
<p>Limite de facturation : l’avance de frais pour le mois complet entre le 15 août et le 14 septembre pour 10 sièges = 110 USD.</p></td>
</tr>
<tr class="even">
<td>Annulation : aucune modification préalable du nombre de sièges</td>
<td><p>Votre fichier de rapprochement contient un seul élément :</p>
<ul>
<li>Un crédit pour les jours non utilisés, l’intégralité de la période ayant été facturée d’avance dans le document de facturation précédent. Cette valeur est calculée en fonction de la date de fin de l’abonnement.</li>
</ul></td>
<td>Avance de frais déjà facturée : du 15 août au 14 septembre pour 10 sièges = 100 USD.
<p>Part utilisée de l’avance de frais du 15 août au 24 août.</p>
<p>Crédit pour les jours non utilisés : du 25 août au 14 septembre pour 10 sièges = -74,51.</p></td>
</tr>
<tr class="odd">
<td>Annulation : avec modification préalable du nombre de sièges</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments :</p>
<ul>
<li>l’extourne de l’avance de frais</li>
<li>les frais d’utilisation au prorata</li>
<li>un crédit pour les jours non utilisés</li>
</ul></td>
<td>Avance de frais déjà facturée : du 15 août au 14 septembre pour 10 sièges = 100 USD.
<p>Utilisation au prorata :</p>
<ul>
<li>Du 15 au 24 août pour 10 sièges</li>
<li>Du 25 août au 14 septembre pour 5 sièges</li>
</ul>
<p>Crédit pour les jours non utilisés : du 1er au 14 septembre pour 5 sièges.</p>
<p>Extourne de l’avance de frais pour l’intégralité du mois du 15 août au 14 septembre = -100 USD.</p></td>
</tr>
</tbody>
</table>

 

 

 






<!--HONumber=Jan17_HO2-->


