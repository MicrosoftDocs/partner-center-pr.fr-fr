---
title: Fichiers de réconciliation ponctuels et périodiques | Espace partenaires
ms.topic: article
ms.date: 11/21/2019
description: Comprendre les fichiers de réconciliation ponctuels et périodiques dans l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389677"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Fichiers de réconciliation ponctuels et périodiques

S’applique à :

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

Cette rubrique explique comment lire des fichiers de réconciliation ponctuels et périodiques dans l’espace partenaires.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Champs dans les fichiers de réconciliation ponctuels et périodiques

| colonne | Description |
| ------ | ----------- |
| PartnerId | Identificateur de locataire unique Azure Active Directory (Azure AD) pour une entité de facturation spécifique, au format GUID. Non requis pour le rapprochement. Identique dans toutes les lignes. |
| ID client | Identificateur unique du locataire Azure AD, au format GUID. Identifie le client. |
| Nom du client | Nom de l’organisation du client, tel qu’indiqué dans l’espace partenaires. |
| CustomerDomainName | Nom de domaine du client. Ce champ peut rester vide jusqu'au deuxième cycle de facturation. *N’utilisez pas ce champ comme identificateur unique pour le client. Le client/partenaire peut mettre à jour le personnel ou le domaine par défaut par le biais du portail Office 365.* |
| Pays du client | Le pays dans lequel se trouve le client. |
| Numéro de facture | Le numéro de la facture dans laquelle la transaction spécifiée apparaît. |
| MpnId | Identificateur MPN du partenaire CSP. |
| Revendeur MpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. |
| ID de commande | Identificateur unique d’une commande dans la plateforme Microsoft Commerce. Non utilisé pour le rapprochement. |
| Date de la commande | La date à laquelle la commande a été passée. |
| ProductId | Identificateur du produit. |
| SkuId | Identificateur d’une référence (SKU) particulière. |
| AvailabilityId | Identificateur pour la disponibilité d’une référence (SKU) particulière. Cela indique si la référence (SKU) est disponible à l’achat dans le pays, la devise, le secteur d’activité, etc. |
| Nom de la référence | Le titre d'une référence spécifique. |
| Nom du produit | Le nom du produit. |
| PublisherName | Nom de l’éditeur du produit.
| PublisherID | Identificateur unique d’un serveur de publication particulier. |
| Description de l’abonnement | Nom convivial d’un abonnement. |
| ID d’abonnement | Identificateur unique d’un abonnement dans la plateforme Microsoft Commerce. Non utilisé pour le rapprochement. *Cet identificateur n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* |
| ChargeStartDate | Date de début des frais. L’heure indique toujours le début de la journée, 0:00. |
| ChargeEndDate | Jour de fin des frais. L’heure indique toujours la fin de la journée, 23:59. |
| Term et Billingcycle | La durée et le cycle de facturation de l’achat (par exemple, *1 an, mensuel*). |
| Type de facturation | Le type de frais ou d’ajustement. |
| Prix unitaire | Prix unitaire publié dans la liste de prix au moment de l’achat. *Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement.* |
| Prix unitaire effectif | Le prix unitaire après ajustements a été effectué. |
| Quantité | Nombre d’unités. *Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement.* |
| Type d’unité | Type d’unité achetée. |
| DiscountDetails | Une explication de toute remise applicable. |
| Sous-total | Total avant impôt. Vérifie si votre sous-total correspond au total attendu, en cas de remise. |
| Total des taxes | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. |
| Total | Total après impôts. Vérifie si les impôts sont retenus sur la facture. |
| Currency | Type de devise. Chaque entité de facturation n’a qu’une devise. Assurez-vous que cela correspond à votre première facture, puis vérifiez à nouveau après toute mise à jour de la plateforme de facturation majeure. |
| AlternateID | Identificateur alternatif à un ID de **commande**. |
