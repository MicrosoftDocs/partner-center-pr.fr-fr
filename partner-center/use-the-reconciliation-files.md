---
title: Utiliser vos fichiers de réconciliation | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Utilisez vos fichiers de rapprochement pour comprendre les affichages détaillés des lignes de l’espace partenaires.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384804"
---
# <a name="use-your-reconciliation-files"></a>Utiliser vos fichiers de rapprochement

S’applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Vous pouvez télécharger vos fichiers de conciliation à partir de l’espace partenaires pour obtenir une vue détaillée de chaque facture dans un cycle de facturation. Les détails de l’élément de ligne incluent les frais relatifs aux abonnements de chaque client et les événements détaillés (par exemple, ajout à mi-parcours de sièges à un abonnement).

Rôles appropriés :

- Administration de facturation
- Administrateur global

Pour plus d’informations sur la lecture de votre facture, consultez [lire votre](read-your-bill.md) **facture**.

## <a name="understand-reconciliation-file-fields"></a>Comprendre les champs de fichier de réconciliation

- [Champs du fichier de réconciliation basés sur les licences](license-based-recon-files.md)
- [Champs du fichier de réconciliation basés sur l’utilisation](usage-based-recon-files.md)
- [Champs de fichier de réconciliation ponctuel et périodique](one-time-recurring-recon-files.md)
- [Champs du fichier de réconciliation de l’utilisation évalué quotidiennement](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Comprendre les types de frais dans les fichiers de rapprochement

Pour comprendre les types de frais dans les fichiers de rapprochement (colonne **ChargeType** ), consultez la rubrique [types de frais de fichier de rapprochement](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Résoudre les problèmes de mise en forme

Parfois, un fichier de réconciliation peut contenir des problèmes de mise en forme. Par exemple, ce problème peut se produire si les paramètres régionaux en-US ne sont pas utilisés.

Pour résoudre les problèmes de mise en forme dans vos fichiers de rapprochement, procédez comme suit :

1. Ouvrez le fichier de réconciliation (au format. csv) dans Microsoft Excel.
2. Sélectionnez la première colonne du fichier.
3. Ouvrez l' **Assistant Conversion de texte en colonnes**. Dans le ruban, sélectionnez **données**, puis sélectionnez **texte pour les colonnes**.
4. Dans l’Assistant, sélectionnez **type de fichier délimité**. Sélectionnez ensuite **suivant**.
5. Dans le champ **séparateurs** , sélectionnez **virgule**. (Si l' **onglet** est déjà sélectionné, vous pouvez conserver cette option sélectionnée.) Sélectionnez ensuite **suivant**.
6. Dans le champ **format des données** de la colonne, sélectionnez **Date : mja**. Sélectionnez ensuite **suivant**.
7. Dans le champ **format des données** de la colonne, sélectionnez **texte** pour toutes les colonnes de montant. Ensuite, sélectionnez **Terminer**.

## <a name="download-reconciliation-files-programmatically"></a>Télécharger les fichiers de rapprochement par programmation

Les fichiers de réconciliation peuvent être très volumineux et parfois difficiles à télécharger. Pour télécharger des fichiers de conciliation par programme, consultez [obtenir des lignes de facturation](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Taxes de carte ou TVA

Pour mapper les taxes ou la T.V.A. sur votre facture :

- Totalisez la colonne **Tax** du fichier basé sur une licence.
- Totalisez la colonne **TaxAmount** à partir du fichier d’utilisation.

## <a name="itemize-reconciliation-files-by-partner"></a>Décomposant les fichiers de rapprochement par partenaire

Les partenaires dans le **modèle indirect** peuvent utiliser ces champs supplémentaires dans des fichiers de réconciliation basés sur les licences et sur l’utilisation pour détailler les fichiers par le revendeur.

| ID MPN | Description |
| ------ | ----------- |
| ID MPN | Identificateur Microsoft Partner Network (MPN) du partenaire fournisseur de solutions Cloud (CSP) (direct ou indirect). |
| [ID MPN du revendeur](#reseller-mpn-id) | [Identificateur MPN du revendeur de l’enregistrement pour l’abonnement](#reseller-mpn-id). Ce champ correspond à l’ID du revendeur indiqué pour l’abonnement spécifique dans l’espace partenaires. Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect. |

### <a name="reseller-mpn-id"></a>ID&nbsp;MPN revendeur

Si un partenaire CSP a vendu l’abonnement directement au client, son **ID MPN** est listé deux fois, à la fois avec l' **ID MPN** et l' **ID MPN du revendeur**.

Si un partenaire CSP a un revendeur sans **ID MPN**, cette valeur est définie sur l' **ID MPN** du partenaire à la place.

Si le partenaire CSP supprime un **ID MPN du revendeur**, cette valeur sera définie sur *-1*.

Pour afficher ou mettre à jour l' **ID MPN du revendeur**:

1. Connectez-vous à l’Espace partenaires.
2. Dans le menu de l’Espace partenaires, sélectionnez **Clients**.
3. Dans la liste, choisissez le client.
4. Dans le menu client, sélectionnez **abonnements**.
5. Choisissez l’abonnement dans la liste.
6. Sélectionnez **Mettre à jour** pour modifier le **Revendeur (ID&nbsp;MPN)** .
