---
title: Fichiers de réconciliation ponctuels et périodiques
ms.topic: article
ms.date: 05/26/2020
description: Comprendre la signification de chaque champ ou colonne dans les fichiers de rapprochement ponctuels et périodiques de l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84bed4fac8984b3fc8757b8185da514c5d8212d6
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749197"
---
# <a name="one-time-and-recurring-reconciliation-files-in-partner-center"></a>Fichiers de réconciliation ponctuels et périodiques dans l’espace partenaires

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Administrateur général
- Administrateur des utilisateurs
- Administrateur de la facturation
- Agent d’administration
- Agent commercial

Cette rubrique explique comment lire des fichiers de réconciliation ponctuels et périodiques dans l’espace partenaires.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Champs dans les fichiers de réconciliation ponctuels et périodiques

| Colonne | Description |
| ------ | ----------- |
| PartnerId | Identificateur de locataire unique Azure Active Directory (Azure AD) pour une entité de facturation spécifique, au format GUID. Non requis pour le rapprochement. Identique dans toutes les lignes. |
| CustomerId | Identificateur unique du locataire Azure AD, au format GUID. Identifie le client. |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’espace Partenaires. |
| CustomerDomainName | Nom de domaine du client. Ce champ peut apparaître vide jusqu’au deuxième cycle de facturation. *N’utilisez pas ce champ comme identificateur unique pour le client. Le client/partenaire peut mettre à jour le personnel ou le domaine par défaut par le biais du portail Office 365.* |
| CustomerCountry | Pays dans lequel se trouve le client. |
| InvoiceNumber | Numéro de facture sur lequel figure la transaction spécifiée. |
| MpnId | Identificateur MPN du partenaire CSP. |
| OrderId | Identificateur unique d’une commande dans la plateforme Microsoft Commerce. Non utilisé pour le rapprochement. |
| OrderDate | Date à laquelle la commande a été placée. |
| ProductId | Identificateur du produit. |
| SkuId | Identificateur d’une référence (SKU) particulière. |
| AvailabilityId | Identificateur pour la disponibilité d’une référence (SKU) particulière. Cela indique si la référence (SKU) est disponible à l’achat dans le pays, la devise, le secteur d’activité, etc. |
| SkuName | Titre d’une référence (SKU) particulière. |
| ProductName | Nom du produit. |
| ChargeType | Type de frais ou d’ajustement. |
| UnitPrice | Prix unitaire publié dans la liste de prix au moment de l’achat. *Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement.* |
| Quantité | Nombre d’unités. *Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement.* |
| SubTotal | Total avant impôt. Vérifie si votre sous-total correspond au total attendu, en cas de remise. |
| TaxTotal | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. |
| Total | Total après impôts. Vérifie si les impôts sont retenus sur la facture. |
| Devise | Type de devise. Chaque entité de facturation n’a qu’une seule devise. Assurez-vous que cela correspond à votre première facture, puis vérifiez à nouveau après toute mise à jour de la plateforme de facturation majeure. |
| PriceAdjustmentDescription | Une explication de toute remise applicable. |
| PublisherName | Nom de l’éditeur du produit.
| PublisherId | Identificateur unique d’un serveur de publication particulier. |
| SubscriptionDescription | Nom convivial d’un abonnement. |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme Microsoft Commerce. Non utilisé pour le rapprochement. *Cet identificateur n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* |
| ChargeStartDate | Date de début des frais. L’heure est toujours définie sur le début de la journée, 0:00. |
| ChargeEndDate | Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59. |
| TermAndBillingcycle | La durée et le cycle de facturation de l’achat (par exemple, *1 an, mensuel*). |
| EffectiveUnitPrice | Le prix unitaire après ajustements a été effectué. |
| Unité | Type d’unité achetée. |
| AlternateId | Identificateur alternatif à un ID de **commande**. |
| BillableQuantity | Représente le nombre total d’unités achetées ou consommées. |
| BillingFrequency | Décrit si la ligne est une fréquence mensuelle ou ponctuelle. *Cela est actuellement pris en charge pour Azure RI uniquement, avec des valeurs prises en charge mensuelles. Si l’RI est acheté avec une fréquence de facturation unique, ce champ dans le fichier de rapprochement s’affiche vide.* |
| PricingCurrency | Tarif de la ressource ou de l’offre. |
| PCToBCExchangeRate | Taux de change appliqué pour la devise de tarification à la devise de facturation. |
| PCToBCExchangeRateDate | Date à laquelle la devise de tarification pour la devise de facturation est déterminée. |
| MeterDescription | Description du compteur pour la ligne de consommation. |
