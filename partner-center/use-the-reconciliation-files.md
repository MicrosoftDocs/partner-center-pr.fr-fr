---
title: Utiliser vos fichiers de rapprochement
ms.topic: article
ms.date: 03/26/2021
description: En savoir plus sur les fichiers de rapprochement dans l’espace partenaires et sur l’interprétation des affichages détaillés des lignes de facturation pour un cycle de facturation donné.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730078"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Découvrez comment lire les éléments de ligne dans vos fichiers de rapprochement de l’espace partenaires

**Rôles appropriés**

- Administrateur de la facturation
- Administrateur général

Vous pouvez télécharger vos fichiers de conciliation à partir de l’espace partenaires pour obtenir une vue détaillée de chaque facture dans un cycle de facturation. Les détails des éléments de ligne incluent les frais associés aux abonnements de chaque client et les événements détaillés (par exemple, ajout de licences à mi-parcours à un abonnement).

Pour plus d’informations sur la lecture de votre facture, consultez [lire votre](read-your-bill.md) **facture**.

## <a name="understand-reconciliation-file-fields"></a>Comprendre les champs de fichier de réconciliation

- [Champs du fichier de rapprochement basé sur les licences](license-based-recon-files.md)
- [Champs du fichier de rapprochement basé sur l’utilisation](usage-based-recon-files.md)
- [Champs du fichier de rapprochement basé sur l’utilisation quotidienne estimée](daily-rated-usage-recon-files.md)
- [Champs du fichier de rapprochement des fournisseurs CSP à usage unique](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Comprendre les types de frais dans les fichiers de rapprochement

Pour comprendre les types de frais dans les fichiers de rapprochement (colonne **ChargeType** ), consultez la rubrique [types de frais de fichier de rapprochement](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Résoudre les problèmes de mise en forme

Parfois, un fichier de réconciliation peut contenir des problèmes de mise en forme. Par exemple, ce problème peut se produire si les paramètres régionaux en-US ne sont pas utilisés.

Pour résoudre les problèmes de mise en forme dans vos fichiers de rapprochement, procédez comme suit :

1. Ouvrez le fichier de réconciliation (au format. csv) dans Microsoft Excel.
2. Sélectionnez la première colonne du fichier.
3. Ouvrez l' **Assistant Conversion de texte en colonnes**. Dans le ruban, sélectionnez **données**, puis sélectionnez **texte pour les colonnes**.
4. Dans l’Assistant, sélectionnez **type de fichier délimité**. Ensuite, sélectionnez **Suivant**.
5. Dans le champ **séparateurs** , sélectionnez **virgule**. (Si l' **onglet** est déjà sélectionné, vous pouvez conserver cette option sélectionnée.) Sélectionnez ensuite **suivant**.
6. Dans le champ **format des données** de la colonne, sélectionnez **Date : mja**. Ensuite, sélectionnez **Suivant**.
7. Dans le champ **format des données** de la colonne, sélectionnez **texte** pour toutes les colonnes de montant. Ensuite, sélectionnez **Finish**.

## <a name="download-reconciliation-files-programmatically"></a>Télécharger les fichiers de rapprochement par programmation

Les fichiers de réconciliation peuvent être très volumineux et parfois difficiles à télécharger. Pour télécharger des fichiers de conciliation par programme, consultez [obtenir des lignes de facturation](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Si votre fichier dépasse la limite de lignes dans Excel

Si vous êtes en mesure de télécharger un fichier de réconciliation sans l’ouvrir dans Microsoft Excel, cela signifie probablement que le fichier contient plus de lignes qu’Excel ne l’autorise. Dans ce cas, vous pouvez utiliser l’une des procédures ci-dessous pour ouvrir le fichier.

### <a name="open-a-recon-file-in-power-bi"></a>Ouvrir un fichier de rapprochement dans Power BI

1. Téléchargez le fichier de réconciliation comme vous le feriez normalement.
2. Téléchargez, installez et ouvrez une instance de Power BI.
3. Sous **l’onglet Power bi** , sélectionnez récupérer des **données**.
4. Dans la liste des **sources de données courantes**, sélectionnez **texte/CSV**.
5. Lorsque vous y êtes invité, ouvrez votre fichier de rapprochement.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Ouvrir un fichier de rapprochement dans un tableau croisé dynamique Excel

1. Téléchargez le fichier de réconciliation comme vous le feriez normalement.
2. Ouvrez un nouveau fichier dans Microsoft Excel.
3. Sous l’onglet **données** , sélectionnez **récupérer des données**, sélectionnez **à partir d’un fichier**, puis sélectionnez **texte/CSV**.
4. Lorsque vous y êtes invité, ouvrez votre fichier de rapprochement. Vos données s’affichent.
5. Dans le menu déroulant **charger** , sélectionnez **charger sur**, puis **OK**.
6. Dans la boîte de dialogue **importer des données** , sélectionnez **rapport de tableau croisé dynamique** pour ouvrir votre fichier.

## <a name="negative-amount-displayed"></a>Montant négatif affiché

Vous pouvez voir un montant négatif dans votre fichier de réconciliation. Cela est probablement dû à l’une des raisons suivantes :

- Vous avez récemment annulé ou réduit votre nombre de licences
- Vous avez reçu un crédit pour un contrat de licence de service (SLA) ou pour la consommation Azure

Pour obtenir plus d’informations sur cette transaction, examinez son attribut de type de frais dans votre fichier de réconciliation.

## <a name="map-taxes-or-vat"></a>Taxes de carte ou TVA

Pour mapper les taxes ou la T.V.A. sur votre facture :

- Totalisez la colonne **Tax** du fichier basé sur une licence.
- Totalisez la colonne **TaxAmount** à partir du fichier d’utilisation.

## <a name="itemize-reconciliation-files-by-partner"></a>Décomposant les fichiers de rapprochement par partenaire

Les partenaires dans le **modèle indirect** peuvent utiliser ces champs supplémentaires dans des fichiers de réconciliation basés sur les licences et sur l’utilisation pour détailler les fichiers par le revendeur.

| ID MPN | Description |
| ------ | ----------- |
| ID MPN | Identificateur Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (CSP) (direct ou indirect). |
| [ID&amp;nbsp;MPN revendeur](#reseller-mpn-id) | [Identificateur MPN du revendeur de l’enregistrement pour l’abonnement](#reseller-mpn-id). Ce champ correspond à l’ID du revendeur indiqué pour l’abonnement spécifique dans l’espace partenaires. Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect. |

### <a name="reseller-mpn-id"></a>ID&nbsp;MPN revendeur

Si un partenaire CSP a vendu l’abonnement directement au client, son **ID MPN** est listé deux fois, à la fois avec l' **ID MPN** et l' **ID MPN du revendeur**.

Si un partenaire CSP a un revendeur sans **ID MPN**, cette valeur est définie sur l' **ID MPN** du partenaire à la place.

Si le partenaire CSP supprime un **ID MPN du revendeur**, cette valeur sera définie sur *-1*.

Pour afficher ou mettre à jour l' **ID MPN du revendeur**:

1. Connectez-vous à l’Espace partenaires.
2. Dans le menu de l’Espace partenaires, sélectionnez **Clients**.
3. Sélectionnez le client dans la liste.
4. Dans le menu client, sélectionnez **abonnements**.
5. Choisissez l’abonnement dans la liste.
6. Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)**.

## <a name="next-steps"></a>Étapes suivantes

- [Comment lire votre fichier de conciliation de factures &](read-your-bill.md) 