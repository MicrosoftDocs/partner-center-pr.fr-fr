---
title: Taxes et frais de service de RTPC régionaux
description: En tant que partenaire Office 365 qui transforme Microsoft 365 produits vocaux, vous pouvez être soumis à des taxes régionales, des frais ou des exigences réglementaires pour les services RTPC.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854721"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Taxes régionales, réglementations relatives aux services de réseau public commuté (PTSN)

**Rôles appropriés**: administrateur général | Administrateur d’utilisateur | Agent d’administration

Dans certaines juridictions, les services de réseau public commuté (RTPC) peuvent être soumis à des exigences légales et fiscales qui peuvent affecter l’ordre et la facturation des partenaires. Dans le États-Unis, y compris Porto Rico, les services RTPC, qui incluent la conférence audio, les plans d’appel et les crédits de communication, sont soumis à des obligations réglementaires et fiscales particulières. Dans le États-Unis et à Porto Rico, les tarifs de Microsoft sont les services RTPC comme taxes incluses.  Des taxes et réglementations uniques sur les RTPC affectent les partenaires Office 365 qui transportent des produits Microsoft 365 Voice.  Si un partenaire affiche le prix d’un service&nbsp;RTC Microsoft, il peut avoir à calculer et restituer des taxes et frais&nbsp;RTC.

## <a name="partner-recommendations"></a>Recommandations pour les partenaires

Demandez à vos conseillers juridiques de comprendre la responsabilité de votre organisation en ce qui concerne la réglementation, les taxes et les frais des services RTPC, ainsi que d’autres inconvénients potentiels.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Présentation des factures et fichier de rapprochement des partenaires

Les factures CSP et les fichiers de conciliation CSP dans le États-Unis, Porto Rico et Canada, qui incluent Skype for Business RTPC et Microsoft 365 Voice services, fournissent des éléments de ligne distincts pour les composants RTPC et non-RTC.

En outre, les factures CSP affichent la note de bas de page suivante :

* Le prix affiché est facturé pour les services de plan de conférence audio et d’appel.  Toutes les taxes transactionnelles applicables sont facturées exclusivement au montant indiqué, à l’exception des ventes effectuées au sein de la États-Unis.  Aux États-Unis, le prix affiché est taxes inclusives, car il inclut des frais pour le plan d’appel et les services de conférence audio, ainsi que des frais pour les taxes et les frais que nous sommes tenus de payer.  Les services de plan de conférence audio et d’appel sont servis par l’affilié Microsoft autorisé à les fournir.  Pour plus d’informations, consultez [Licences en volume Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Exemple de fichier de réconciliation

Office 365 Enterprise E5 présente le fichier de rapprochement sous la forme de deux Articles de ligne avec des noms identiques et des ID identiques, mais chaque article a un prix unitaire unique (par exemple : $28,40 et $2,00). Cette séparation du composant Skype Entreprise Conférence&nbsp;RTC de l’offre Office&nbsp;365 vous permet d’appliquer correctement les taxes.

**#1 de l’exemple de rapprochement des partenaires (sélectionner des colonnes) :**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office&nbsp;365 Enterprise&nbsp;E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Frais de cycle   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office&nbsp;365 Enterprise&nbsp;E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Frais de cycle   |2,00   |

**Exemple de #2 de rapprochement des partenaires**

Microsoft 365 Business Voice disponible dans le Canada possède des composants de passerelle RTPC supplémentaires qui sont consolidés sur une facture CSP (similaire à Office 365 E5, deux éléments de ligne sont présentés, l’un pour les composants RTPC et l’autre pour les composants non-RTPC).  Le fichier de rapprochement des fournisseurs de services Cloud pour Microsoft 365 Business Voice affiche tous les composants de RTPC taxables individuellement (les composants RTPC individuels ne sont pas consolidés dans. CSV ou l’outil API).  La somme des détails de la commande et des montants facturés pour les clients qui se trouvent dans le fichier de rapprochement correspond à la facture du fournisseur de services Cloud.

## <a name="additional-resources"></a>Ressources supplémentaires
Pour plus d’informations, visitez le site [Microsoft 365 pour les partenaires](https://www.microsoft.com/microsoft-365/partners/) .

