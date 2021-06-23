---
title: Comment lire votre fichier de conciliation de factures &
ms.topic: article
ms.date: 06/05/2020
description: En savoir plus sur vos fichiers de conciliation de factures &. Votre facture indique les frais relatifs à l’espace partenaires dans le programme, les produits et les clients pour cette période mensuelle.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551195"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Comprendre votre facture et votre fichier de rapprochement-Découvrez comment les trouver dans l’espace partenaires


**Rôles appropriés**: administrateur général | Administrateur de facturation | Agent d’administration


Votre **facture** est un **Résumé de toutes les facturations de l’espace partenaires** (dans le programme, tous les produits et tous les clients). 

## <a name="find-your-bill-and-reconciliation-file"></a>Rechercher votre facture et votre fichier de rapprochement 

Vous pouvez trouver votre facture sur la page facturation du tableau de bord de l’espace partenaires. Vous pouvez également trouver l’historique de facturation, les tendances de dépense et les fichiers de rapprochement sur cette page. 

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/home) de l’Espace partenaires. 

2. Dans le menu de gauche, sélectionnez **facturation**. 

3. Dans la page État de facturation, sélectionnez une facture ou un fichier de rapprochement pour voir des informations plus détaillées. 

Vous pouvez trouver un lien vers votre dernière facture en haut de la page, sous solde du compte à la date de la dernière facture. 

Vous trouverez les factures précédentes dans la section historique de facturation. Choisissez l’année appropriée, puis sélectionnez la flèche déroulante en regard de la période de facturation appropriée. Sélectionnez le lien en regard de factures (.pdf) pour télécharger la facture de cette période. 

## <a name="invoice-types"></a>Types de facture

Microsoft émet une facture pour tous les frais liés à une licence (par exemple, Office 365) et les frais basés sur l’utilisation (tels qu’Azure) et une facture distincte pour les frais à usage unique (par exemple, Azure RI, Marketplace ou Azure plan).

Par exemple,  

**Scénario 1 [monnaie unique]**: le partenaire a acheté l’offre 145P et les licences Office 365,  

- Le partenaire recevra une facture PDF et deux fichiers de réconciliation couvrant les frais liés à Office 365 et Azure (145p).  

**Scénario 2 [monnaie unique]**: le partenaire a acheté pour Azure RI, Marketplace et/ou Azure plan, ainsi que des achats 145p.

- Le partenaire recevra un fichier PDF de facture et un fichier de réconciliation couvrant les frais d’Azure (145p). 

- Le partenaire recevra un autre fichier PDF de facture et un fichier de réconciliation couvrant ses frais pour l’instance réservée Azure (RI), la place de marché, le plan Azure. 

**Scénario 3 [multidevise]**: le partenaire a acheté pour Azure RIen DKK et le plan Azure en DKK, ainsi que les achats de 145P en euros.

- Le partenaire recevra un fichier PDF de facture et un fichier de réconciliation couvrant les frais relatifs à Azure RIen DKK. 

- Le partenaire recevra un fichier PDF de facture et un fichier de réconciliation couvrant les frais pour le plan Azure en EUR. 

- Le partenaire recevra un autre fichier PDF de facture et un fichier de réconciliation couvrant ses frais pour l’offre 145p en euros (ou en devise de facturation partenaire). 


## <a name="understanding-invoice-pdf"></a>Comprendre la facture PDF 

**Factures pour les frais relatifs à l’utilisation et à la licence**: les factures relatives aux frais pour les services tels que Office 365 et Azure seront disponibles dans les deux (2) jours suivant la date de facturation sélectionnée [UTC].  

**Factures pour les frais OneTime et récurrents**: les factures relatives aux frais pour les services tels qu’Azure RI, Azure plan, Marketplace seront disponibles au plus tard le huitième de chaque mois.  

Voici quelques-uns des champs clés du document PDF de facture :

**Numéro de facture**: identificateur unique du document de facture généré pour la période de facturation respective. 

**Période de facturation**: il s’agit de la période pendant laquelle vous avez des utilisations et des services basés sur une licence. 

**Date** de la facture : date de facturation ou date anniversaire à laquelle votre facture est générée chaque mois. 

**Date d’échéance du paiement**: date à laquelle votre paiement doit être reçu. 

**Frais**: montant dû dans votre devise de facturation pour la période de facturation respective. 

**Crédits**: crédits (tels que contrat de niveau de service (SLA)) ou ajustements pour les modifications apportées aux abonnements (par exemple, augmentation ou diminution de la licence). 

**Instructions de paiement**: description du paiement de votre facture, en fonction de votre région. Veillez à toujours inclure votre numéro de facture lors de l’exécution d’un paiement. 

Pour obtenir une description détaillée de tous les champs de votre fichier de facture (y compris les champs pour les frais à usage unique), consultez [champs de fichier de facture](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Comprendre les fichiers de réconciliation

 Les fichiers de rapprochement, qui fournissent des détails détaillés sur vos frais, peuvent être téléchargés en même temps que le fichier PDF de la facture. Les fichiers de réconciliation incluent des identificateurs de clients et des identificateurs d’abonnement que vous pouvez utiliser pour créer des factures client. Pour plus d’informations sur les fichiers de rapprochement, voir [How to use the Reconciliation Files](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Étapes suivantes

- [Comment utiliser les fichiers de rapprochement](use-the-reconciliation-files.md)