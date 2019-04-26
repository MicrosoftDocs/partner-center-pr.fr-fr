---
title: Scénarios de facturation courantes (Partner Center géré par 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132339"
---
# <a name="common-billing-scenarios"></a>Exemples de facturation courants

**S’applique à**

-   Espace partenaires géré par 21Vianet


Cette rubrique explique ce que vous pouvez voir sur votre facture lorsque vous ajoutez de nouveaux abonnements, réglez le nombre de sièges dans un abonnement ou annulez un abonnement. 


## <a name="licence-based-billing"></a>Facturation basée sur la licence


Pour les mois sans modification des abonnements basés sur le certificat, vous verrez un seul élément de ligne pour chaque abonnement sur votre fichier de rapprochement et la facture des frais d’avance pour le mois prochain.

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
<p>Couper de facturation : Passez gratuit pendant la période de mois complet à partir du 15 juin au 14 juillet pour les 15 sièges. À supposer que les frais par abonnement et par mois soient de 10 USD, ils se monteront à 10 USD x 15 sièges = 150 USD.</p></td>
</tr>
<tr class="odd">
<td>Abonnement existant : Augmentation ou diminution de la quantité de licence</td>
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
<p>Couper de facturation : Passez des frais pour la période de mois complet à partir du 15 août au 14 septembre pour les 10 sièges = 110 USD.</p></td>
</tr>
<tr class="even">
<td>Annulation : aucune modification préalable du nombre de sièges</td>
<td><p>Votre fichier de rapprochement contient un seul élément :</p>
<ul>
<li>Un crédit pour les jours non utilisés, l’intégralité de la période ayant été facturée d’avance dans le document de facturation précédent. Cette valeur est calculée en fonction de la date de fin de l’abonnement.</li>
</ul></td>
<td>Précédemment facturés des frais d’avance : Le 15 août à 14 septembre pour 10 sièges = 100 USD.
<p>Part utilisée de l’avance de frais du 15 août au 24 août.</p>
<p>Crédit inutilisé jours : Le 25 août à 14 septembre pour 10 sièges =-74.51.</p></td>
</tr>
<tr class="odd">
<td>Annulation : avec modification préalable du nombre de sièges</td>
<td><p>Votre fichier de rapprochement contient plusieurs éléments :</p>
<ul>
<li>l’extourne de l’avance de frais</li>
<li>les frais d’utilisation au prorata</li>
<li>un crédit pour les jours non utilisés</li>
</ul></td>
<td>Précédemment facturés des frais d’avance : Le 15 août à 14 septembre pour 10 sièges = 100 USD.
<p>Utilisation au prorata :</p>
<ul>
<li>Du 15 au 24 août pour 10 sièges</li>
<li>Du 25 août au 14 septembre pour 5 sièges</li>
</ul>
<p>Crédit inutilisé jours : Le 1er septembre à 14 septembre pour 5 utilisateurs.</p>
<p>Extourne de l’avance de frais pour l’intégralité du mois du 15 août au 14 septembre = -100 USD.</p></td>
</tr>
</tbody>
</table>
