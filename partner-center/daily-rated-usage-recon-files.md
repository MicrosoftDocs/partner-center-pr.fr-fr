---
title: Fichiers de rapprochement d’utilisation évalués quotidiennement
ms.topic: article
ms.date: 05/15/2020
description: Découvrez comment lire les fichiers de rapprochement d’utilisation évalués quotidiennement dans l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3536b1b71dd8378e88ac14726adcca7fa0e08530
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795594"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Découvrez comment lire les fichiers de rapprochement d’utilisation évalués quotidiennement dans l’espace partenaires

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Agent d’administration
- Administrateur de la facturation
- Agent commercial
- Agent du support technique

Cette rubrique explique comment lire les fichiers de réconciliation d’utilisation évalués quotidiennement.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Champs dans les fichiers de rapprochement d’utilisation évalués quotidiennement

| Colonne | Description |
| ------ | ----------- |
| PartnerId | Identificateur de partenaire au format GUID. |
| PartnerName | Nom du partenaire. |
| CustomerId | Identificateur Microsoft unique du client au format GUID. |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’Espace partenaires. *Cette colonne est très importante pour rapprocher la facture de vos informations système.* |
| CustomerDomainName | Nom de domaine du client. |
| CustomerCountry | Pays dans lequel se trouve le client. |
| MpnId | Identificateur MPN du partenaire CSP. |
| Tier2MpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. |
| InvoiceNumber | Numéro de facture sur lequel figure la transaction spécifiée. |
| ProductId | Identificateur du produit. |
| SkuId | Identificateur d’une référence (SKU) particulière. |
| AvailabilityId | Identificateur pour la disponibilité d’une référence (SKU) particulière. Cela indique si la référence (SKU) est disponible à l’achat dans le pays, la devise, le secteur d’activité, etc. |
| SkuName | Titre d’une référence (SKU) particulière. |
| ProductName | Nom du produit. |
| PublisherName | Nom de l'éditeur. |
| PublisherId | Identificateur du serveur de publication au format GUID. |
| SubscriptionDescription | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s’agit d’un champ identique à **OfferName**). |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme de facturation Microsoft. Non utilisé pour le rapprochement. *Cet identificateur n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* |
| ChargeStartDate | Date de début du cycle de facturation (sauf lors de la présentation de dates de données d’utilisation latentes précédemment non facturées du cycle de facturation précédent). L’heure est toujours définie sur le début de la journée, 0:00. |
| ChargeEndDate | Date de fin du cycle de facturation (sauf lors de la présentation de dates de données d’utilisation latentes précédemment non facturées du cycle bilingue précédent). L’heure indique toujours la fin de la journée, 23:59. |
| UsageDate | Date d’utilisation du service. |
| MeterType | Type de compteur. |
| MeterCategory | Service de niveau supérieur pour l’utilisation. |
| MeterId | Identificateur du compteur utilisé. |
| MeterSubCategory | Le type de service Azure, qui peut affecter la vitesse. |
| MeterName | Unité de mesure du compteur consommé. |
| MeterRegion | Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant). |
| Unité | Unité du **nom**de la ressource. |
| ResourceLocation | Centre de données dans lequel le compteur est en cours d’exécution. |
| ConsumedService | Service de plateforme Azure que vous avez utilisé. |
| ResourceGroup | Représente un conteneur qui contient les ressources associées pour une solution Azure. |
| ResourceURI | URI de la ressource en cours d’utilisation. |
| ChargeType | Type de frais ou d’ajustement.  |
| UnitPrice | Prix par licence, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que ce prix correspond aux informations stockées dans votre système de facturation au cours du rapprochement. |
| Quantité | Nombre de licences. Assurez-vous que ce prix correspond aux informations stockées dans votre système de facturation au cours du rapprochement. |
| Unité | Type d’unité dans lequel le compteur est facturé.  |
| BillingPreTaxTotal | Montant total de la facturation avant taxes. |
| BillingCurrency | Devise dans la région géographique du client. |
| PricingPreTaxTotal | La tarification avant les taxes est ajoutée. |
| PricingCurrency | Devise utilisée dans la liste de prix. |
| ServiceInfo1 | Nombre de connexions Service Bus qui ont été approvisionnées et utilisées pour un jour donné. |
| ServiceInfo2 | Champ hérité qui capture les métadonnées facultatives propres au service. |
| Balises | Représente une organisation logique des ressources Azure définies par l’utilisateur. |
| AdditionalInfo | Toutes les informations supplémentaires non couvertes sont dans les autres colonnes. |
| EffectiveUnitPrice | Valeur réelle facturée par unité, y compris les remises, les crédits acquis, etc. |
| PCToBCExchangeRate | Taux de change appliqué pour la devise de tarification à la devise de facturation. |
| PCToBCExchangeRateDate | Date à laquelle la devise de tarification pour la devise de facturation est déterminée. |
| EntitlementId | Représente l’ID d’abonnement Azure. |
| EntitlementDescription | Représente le nom de l’ID d’abonnement Azure. |
| PartnerEarnedCreditPercentage | Affiche le PartnerEarnedCredit de l’élément de ligne. Le crédit gagné aura une valeur de 0 ou de 15 pour cent |
