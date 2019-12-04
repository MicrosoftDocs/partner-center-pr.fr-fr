---
title: Fichiers de rapprochement d’utilisation évalués quotidiennement | Espace partenaires
ms.topic: article
ms.date: 11/27/2019
description: Découvrez comment lire les fichiers de rapprochement d’utilisation évalués quotidiennement dans l’espace partenaires.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d7de5da8529aefb325961ac5c139a9375b66f7e0
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721862"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Fichiers de rapprochement d’utilisation évalués quotidiennement

**S’applique à**

- Espace partenaires
- Espace partenaires de Microsoft Cloud for US Government

**Rôles appropriés**

- Agent d’administration
- Administration de facturation
- Commercial
- Agent du support technique

Cette rubrique explique comment lire les fichiers de réconciliation d’utilisation évalués quotidiennement.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Champs dans les fichiers de rapprochement d’utilisation évalués quotidiennement

| Colonne | Description |
| ------ | ----------- |
| PartnerId | Identificateur de partenaire au format GUID. |
| PartnerName | Nom du partenaire. |
| CustomerId | Identificateur Microsoft unique du client au format GUID. |
| CustomerCompanyName | Nom de l’entreprise du client comme indiqué dans l’Espace partenaires. *Cette colonne est très importante pour rapprocher la facture de vos informations système.* |
| CustomerDomainName | Nom de domaine du client. Non disponible pour l’activité en cours. |
| Pays du client | Le pays dans lequel se trouve le client. |
| MPNID | Identificateur MPN du partenaire CSP. |
| Revendeur MPNID | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. Non disponible pour l’activité en cours. |
| InvoiceNumber | Le numéro de la facture dans laquelle la transaction spécifiée apparaît. Non disponible pour l’activité en cours. |
| ProductId | Identificateur du produit. |
| SkuId | Identificateur d’une référence (SKU) particulière. |
| AvailabilityId | Identificateur pour la disponibilité d’une référence (SKU) particulière. Cela indique si la référence (SKU) est disponible à l’achat dans le pays, la devise, le secteur d’activité, etc. |
| Nom de la référence | Le titre d'une référence spécifique. |
| PublisherName | Nom du serveur de publication. |
| PublisherID | Identificateur du serveur de publication au format GUID. Non disponible pour l’activité en cours. |
| Description de l’abonnement | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. (Il s’agit d’un champ identique à **OfferName**). |
| ID d’abonnement | Identificateur unique pour un abonnement dans la plateforme de facturation Microsoft. Non utilisé pour le rapprochement. *Cet identificateur n’est pas le même que l' **ID d’abonnement** dans la console d’administration partenaire.* |
| ChargeStartDate | Date de début du cycle de facturation (sauf lors de la présentation de dates de données d’utilisation latentes précédemment non facturées du cycle de facturation précédent). L’heure indique toujours le début de la journée, 0:00. |
| ChargeEndDate | Date de fin du cycle de facturation (sauf lors de la présentation de dates de données d’utilisation latentes précédemment non facturées du cycle bilingue précédent). L’heure indique toujours la fin de la journée, 23:59. |
| Date d’utilisation | Date d’utilisation du service. |
| Type de compteur | Type de compteur. |
| Catégorie du compteur | Service de niveau supérieur pour l’utilisation. |
| ID du compteur | Identificateur du compteur utilisé. |
| Sous-catégorie du compteur | Le type de service Azure, qui peut affecter la vitesse. |
| Nom du compteur | Unité de mesure du compteur consommé. |
| Région du compteur | Cette colonne identifie l’emplacement d’un centre de données dans la région (le cas échéant). |
| Unit | Unité du **nom**de la ressource. |
| Quantité consommée | Quantité de service utilisée (par exemple, *heures* ou *Go*) pendant la période de rapport. Comprend toute utilisation non facturée par rapport aux périodes précédentes. |
| Emplacement de la ressource | > le centre de données dans lequel le compteur est en cours d’exécution. |
| Service consommé | Service de plateforme Azure que vous avez utilisé. |
| URI de ressource | URI de la ressource en cours d’utilisation. |
| Type de frais | Le type de frais ou d’ajustement. Non disponible pour l’activité en cours. |
| Prix unitaire | Prix par licence, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que ce prix correspond aux informations stockées dans votre système de facturation au cours du rapprochement. |
| Quantité | Nombre de licences. Assurez-vous que ce prix correspond aux informations stockées dans votre système de facturation au cours du rapprochement. |
| Type d’unité | Type d’unité dans lequel le compteur est facturé. Non disponible pour l’activité en cours. |
| Facturation préalable | Montant total de la facturation avant taxes. |
| Devise de facturation | Devise dans la région géographique du client. |
| Total de la tarification Tarif | La tarification avant les taxes est ajoutée. |
| Devise de tarification | Devise dans la liste de prix. |
| Informations sur le service 1 | Nombre de connexions Service Bus qui ont été approvisionnées et utilisées pour un jour donné. |
| Informations sur le service 2 | Champ hérité qui capture les métadonnées facultatives propres au service. |
| Informations supplémentaires | Toutes les informations supplémentaires non couvertes dans d’autres colonnes. |
