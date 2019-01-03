---
title: Lire votre facture | Espace partenaires
ms.topic: article
ms.date: 10/29/2018
description: Votre facture récapitule tous les frais (sur le programme, les produits et les clients) du mois en cours. Il est disponible dans l’espace partenaires.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: facturation d’abonnement, facturation, facturation dans l’espace partenaires, facturation espace partenaires, lire ma facture, facture, facture de l’espace partenaires, facture Fournisseur de solutions Cloud, où est ma facture?
ms.localizationpriority: medium
ms.openlocfilehash: a6c4ef705e7f66d2e40bd117e3d674d2f06acb76
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990931"
---
# <a name="read-your-bill"></a>Lire votre facture

**S'applique à**

-  Espace partenaires
-  Espace partenaires de MicrosoftCloud pour le gouvernement des États-Unis


Pour consulter votre facture, accédez au menu **Espace partenaires** , puis sélectionnez la **facturation** pour afficher votre historique de facturation et les tendances, des liens vers votre facture et fichier de rapprochement et votre dernier paiement.

Les partenaires du programme Fournisseur de solutions Cloud qui ont choisi d’être facturés chaque mois paient Microsoft dans les 60jours suivant la facturation des abonnements de leurs clients (basés sur la licence et sur l’utilisation).

> [!NOTE]  
> Votre facture récapitule tous les frais (sur le programme, les produits et les clients) de la période de facturation en cours et est disponible dans les quatre (4) jours suivant la date de facturation sélectionnée.

Vous recevrez une facture pour basée sur la licence (Office 365) et sur l’utilisation des frais (Azure) et une facture distincte à usage unique (Azure reserved VM instances) frais.

Pour plus d’informations sur les frais par élément, utilisez les fichiers de rapprochement joints. Les fichiers de rapprochement comprennent les ID de clients et d’abonnements que vous utiliserez pour créer des factures client. Pour plus d’informations, voir [Utilisation des fichiers de rapprochement](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Définitions des fichiers de factures


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Champ</strong></td>
<td><strong>Description</strong></td>
</tr>
<tr class="even">
<td>Numéro d’identification américain FEIN</td>
<td>Votre numéro fiscal fédéral.</td>
</tr>
<tr class="odd">
<td>Numéro de client</td>
<td>Votre numéro de client.</td>
</tr>
<tr class="even">
<td>Adresse de facturation</td>
<td>Adresse d’expédition de votre facture. Pour modifier le nom de la société ou l’adresse, modifiez votre profil de facturation de l’espace partenaires. </td>
</tr>
<tr class="odd">
<td>Frais basé sur les licences</td>
<td>Frais mensuels (ou annuels) fixes des licences basées sur l’utilisation que vous avez achetées, facturés avant le service. Ce montant est la somme de tous les frais indiqués dans la colonne &quot;Subtotal&quot; du fichier de rapprochement basé sur la licence (colonneT).</td>
</tr>
<tr class="even">
<td>Frais basés sur l’utilisation</td>
<td>Utilisation d’Azure, y compris des nouveaux services ou des nouvelles applications activés et utilisés au cours du mois de facturation. Ce nombre est la somme de tous les frais indiqués dans la colonne &quot;PretaxCharges&quot; du fichier de rapprochement basé sur l’utilisation (colonne&nbsp;Z).</td>
</tr>
<tr class="odd">
<td>Remises</td>
<td>Par exemple, la remise que le client reçoit sur le prix normal de l’abonnement. Celle-ci apparaît comme un montant fixe, et non pas comme un prix par unité ou par licence.</td>
</tr>
<tr class="odd">
<td>Crédits</td>
<td>Crédits ou ajustements pour les modifications apportées aux abonnements (par exemple : augmentations ou baisses du nombre d’emplacements).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Sous-total</td>
<td>Total avant taxes et frais de taxe et les crédits.</td>
</tr>
<td>Taxe</td>
<td>Total des taxes des frais en cours correspond au total de la section des détails commençant à la page&nbsp;2 de la facture. Ce nombre est la somme de tous les frais indiqués dans&nbsp;:
<ul>
<li>la colonne &quot;TaxAmount&quot; du fichier de rapprochement basé sur l’utilisation (colonne&nbsp;AA), et</li>
<li>la colonne &quot;Tax&quot; du fichier basé sur la licence (colonne&nbsp;U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Autres crédits</td>
<td>Crédits de taxe.</td>
</tr>
<tr class="even">
<td>Total des frais en cours</td>
<td>Montant dû dans votre devise de facturation pour la période de facturation, à payer à la date d’échéance.</td>
</tr>
<tr class="odd">
<td>Instructions pour le paiement</td>
<td>Explique comment payer votre facture en fonction de votre région. Indiquez toujours votre numéro de facture lors du paiement.</td>
</tr>
<tr class="even">
<td>Numéro de facture</td>
<td>Numéro de votre facture.</td>
</tr>
<tr class="odd">
<td>Période de facturation</td>
<td>Du mois en conduisant à la date de facturation. Il s’agit de la période pendant laquelle basés sur l’utilisation des services sont utilisés et les services basés sur la licence sont rapprochées pour des ajustements de crédit ou des modifications dans le nombre de licences.</td>
</tr>
<tr class="even">
<td>Date de facturation</td>
<td>Votre date de facturation ou la date anniversaire sur lequel votre facture est généré chaque mois.</td>
</tr>
<tr class="odd">
<td>Modalités de paiement</td>
<td>Pour les achats ponctuels, le délai sera toujours de 60jours.</td>
</tr>
<tr class="even">
<td>Date d’échéance du paiement</td>
<td>Votre paiement doit être reçu au plus tard à cette date.</td>
</tr>
<tr class="odd">
<td>Numéro du bon de commande du client</td>
<td>Numéro de votre bon de commande.</td>
</tr>
<tr class="even">
<td>Service client</td>
<td>Adresse du site web pour accéder au service client.</td>
</tr>
<tr class="odd">
<td>Bénéficiaire du service</td>
<td>Adresse où le service est utilisé. (C’est l’adresse officielle de société).</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Liste détaillée des frais ponctuels

|**Champ** |**Définition**|
|:----------------|:-----------------------------|
|Date |Date d’achat. |
|Description |Nom du produit. |
|Quantité |Le nombre de produits (réservations, par exemple) achetés. |
|Prix unitaire |Prix par produit (par exemple, réservation). |
|Remises |Toutes les remises applicables. |
|Montant hors taxe |Sous-total des achats avant impôts. |
|Taxe de vente |Montant des taxes. |
|Total |Total à payer. |
 



