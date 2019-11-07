---
title: Lire votre facture | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Votre facture récapitule tous les frais (sur le programme, les produits et les clients) du mois en cours. Elle est disponible dans l’espace partenaires.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: facturation d’abonnement, facturation, facturation dans l’espace partenaires, facturation espace partenaires, lire ma facture, facture, facture de l’espace partenaires, facture Fournisseur de solutions Cloud, où est ma facture ?
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652175"
---
# <a name="read-your-bill"></a>Lire votre facture

**S’applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud for US Government


Pour votre facture, accédez au menu de l' **espace partenaires** , puis sélectionnez **facturation** pour voir votre historique de facturation et vos tendances, des liens vers votre facture et votre fichier de rapprochement, et votre paiement le plus récent.

Les partenaires du programme Fournisseur de solutions Cloud qui ont choisi d’être facturés chaque mois paient Microsoft dans les 60 jours suivant la facturation des abonnements de leurs clients (basés sur la licence et sur l’utilisation).

> [!NOTE]  
> Votre facture est un résumé de tous les frais, sur le programme, les produits et les clients, pour la période de facturation en cours et est disponible dans les deux (2) jours suivant la date de facturation sélectionnée en heure UTC. Par exemple, si vous avez une date de facturation de 12 septembre, le processus de génération de facture commencera à 12:00 UTC le 13ème et sera achevé de 12:00 UTC le 14. Si vous ne voyez pas votre facture de 11:59PM UTC le 15, vous n’êtes pas dans votre Contrat de niveau de service et devez effectuer une demande de service. 

Vous recevrez une facture pour les frais basés sur une licence (Office 365) et basés sur l’utilisation (Azure) et une facture distincte pour les frais ponctuels (Azure reserved VM instances).

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
<td>Adresse d’expédition de votre facture. Pour modifier le nom ou l’adresse de la société, modifiez votre profil de facturation de l’espace partenaires. </td>
</tr>
<tr class="odd">
<td>Frais basés sur la licence</td>
<td>Frais mensuels (ou annuels) fixes des licences basées sur l’utilisation que vous avez achetées, facturés avant le service. Ce montant est la somme de tous les frais indiqués dans la colonne &quot;Subtotal&quot; du fichier de rapprochement basé sur la licence (colonne T).</td>
</tr>
<tr class="even">
<td>Frais basés sur l’utilisation</td>
<td>Utilisation d’Azure, y compris des nouvelles applications ou des nouveaux services activés et utilisés au cours du mois de facturation. Ce nombre est la somme de tous les frais indiqués dans la colonne &quot;PretaxCharges&quot; du fichier de rapprochement basé sur l’utilisation (colonne Z).</td>
</tr>
<tr class="odd">
<td>Remises</td>
<td>Par exemple, la remise que le client reçoit sur le prix normal de l’abonnement. Celle-ci apparaît comme un montant fixe, et non pas comme un prix par unité ou par licence.</td>
</tr>
<tr class="odd">
<td>Crédits</td>
<td>Crédits ou ajustements pour les modifications apportées aux abonnements (par exemple : augmentations ou baisses du nombre de sièges).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Sous-total</td>
<td>Total avant les taxes et frais et crédits hors taxes.</td>
</tr>
<td>Taxe</td>
<td>Le total des taxes des frais en cours correspond au total de la section des détails commençant à la page 2 de la facture. Ce nombre est la somme de tous les frais indiqués dans&nbsp;:
<ul>
<li>la colonne &quot;TaxAmount&quot; du fichier de rapprochement basé sur l’utilisation (colonne&nbsp;AA), et</li>
<li>la colonne &quot;Tax&quot; du fichier basé sur la licence (colonne U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Autres crédits</td>
<td>Crédits hors taxes.</td>
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
<td>Période mensuelle menant à la date de la facture. Il s’agit de la période pendant laquelle les services basés sur l’utilisation sont consommés et les services basés sur des licences sont conciliés pour les ajustements de crédit ou les modifications de nombre de licences.</td>
</tr>
<tr class="even">
<td>Date de facturation</td>
<td>Date de facturation ou date anniversaire à laquelle votre facture est générée chaque mois.</td>
</tr>
<tr class="odd">
<td>Modalités de paiement</td>
<td>Pour les achats ponctuels, le délai sera toujours de 60 jours.</td>
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
<td>Adresse où le service est utilisé. (Il s’agit de l’adresse de la société légale associée à l’aide à la société.)</td>
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
 



