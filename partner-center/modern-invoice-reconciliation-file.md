---
title: Rapprocher les champs de fichier des achats à usage unique du CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: En savoir plus sur tous les éléments de votre fichier de rapprochement d’achats unique CSP dans l’espace partenaires, y compris les exemples de valeurs.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 74974c68c607ddcee4aff6abd53284a60653fb0b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712254"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Champs du fichier de rapprochement des achats à usage unique CSP

## <a name="using-the-recon-file"></a>Utilisation du fichier de rapprochement
Le tableau ci-dessous fournit des descriptions et des exemples de valeurs pour les champs du fichier de rapprochement pour les achats à usage unique du CSP.

Pour plus d’informations sur les fichiers de rapprochement, consultez [utiliser les fichiers de rapprochement](use-the-reconciliation-files.md).

| Colonne | Description | Exemple de valeur |
| ------ | ----------- | ------------ |
| PartnerId | Identificateur unique au format GUID pour une entité de facturation spécifique. Non requis pour le rapprochement. Identique dans toutes les lignes. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificateur Microsoft unique du client au format GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’Espace partenaires. Cette colonne est importante pour rapprocher la facture de vos informations système. | *Jeanne moderne client DE2* |
| CustomerDomainName | Nom de domaine du client. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Pays dans lequel se trouve votre client. Consultez la [liste complète des pays](./regional-authorization-overview.md) de votre région.  | *DE* |
| InvoiceNumber | Numéro de facture associé au fichier de rapprochement.  | *G002297372* |
| MpnId | Identificateur MPN du partenaire CSP. Pour plus d’informations, consultez [Comment dénombrer par partenaire](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. | *6048879* |
| OrderId | Identificateur unique d’une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la commande lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Date à laquelle la commande a été passée. | *10/3/2020* |
| ProductId | Identificateur unique du produit. | *DZH318Z0BNZ5* |
| SkuId | Identificateur unique de la référence (SKU). | *006G* |
| AvailabilityId | Identificateur unique de disponibilité. | *DZH318Z08B80* |
| skuName | Nom de la référence (SKU). | *Tables-LRS* |
| ProductName | Nom du produit. | *Tables* |
| ChargeType | [Type de frais ou d'](./recon-file-charge-types.md) ajustement. | *Nouveau* |
| UnitPrice | Prix par licence, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *0,045* |
| quantité ; | Nombre de licences. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *1* |
| Sous-total | Total avant impôt. Le sous-total doit être égal à la quantité facturable multipliée par le prix unitaire effectif. | *0* |
| TaxTotal | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *0* |
| Total | Le montant total est égal au sous-total et au montant des taxes. | *0* |
| Devise | Votre facture est générée dans le contexte de la devise du client. Cela signifie que si vous êtes un partenaire qui collabore avec des clients utilisant différentes devises facturables, vous recevrez une facture pour chaque type de devise client.  | *EUR* |
| PriceAdjustmentDescription | Les raisons des ajustements du prix unitaire. Il s’agit des principales raisons, mais elles ne sont pas limitées à la détermination du prix unitaire effectif. | *[« 15,0% crédit gagné pour les services gérés »]* |
| PublisherName | Éditeur du produit.  | *Microsoft* |
| PublisherId | Identificateur unique utilisé par l’espace partenaires pour identifier le serveur de publication. | *NA* |
| SubscriptionDescription | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. Cette colonne est un champ identique à OfferName. | *Plan Azure* |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme de facturation Microsoft. Non utilisé pour le rapprochement. Notez que cet identificateur n’est pas le même que l’ID d’abonnement dans la console d’administration partenaire. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Date à laquelle le centre partenaires facture les frais d’abonnement. Si l’abonnement est acheté avec un terme de facturation annuelle et un plan de facturation mensuel, puis dans le premier fichier de réconciliation, il s’agit du jour de l’achat de l’abonnement. À partir du prochain fichier de rapprochement, il sera incrémenté de 30 jours. | *9/1/2020* |
| ChargeEndDate | Jour de fin des frais pour le cycle de facturation de l’abonnement. Si l’abonnement est acheté avec un terme de facturation annuelle et un plan de facturation mensuel, puis dans le premier fichier de rapprochement, il s’agit du 30 jours suivant l’achat de l’abonnement. À partir du prochain fichier de rapprochement, il sera incrémenté de 30 jours. | *30/09/2020* |
| TermAndBillingCycle | Durée d’engagement pour poursuivre l’abonnement au moment de l’achat. | *Données stockées (Go/mois)* |
| EffectiveUnitPrice | Prix unitaire au prorata pour calculer le coût du cycle de facturation. Les remises, les ajustements en jours de facturation et d’autres facteurs déterminent le prix unitaire effectif. Pour plus d’informations, consultez [calcul du prix unitaire effectif](./effective-unit-price-calculation.md).  | *0,03825* |
| Unité | Type d’unité dans laquelle le compteur est facturé. | *1 Go/mois* |
| AlternateId | Autre ID de l’élément de ligne de commande référencé. | *6dc5c039750a* |
| BillableQuantity | Quantité totale facturée.  | *0,005001* |
| BillingFrequency | Plan de facturation sélectionné au moment de l’achat. | *NA*  |
| PricingCurrency | Devise utilisée dans la liste de prix. | *USD* |
| PCToBCExchangeRate | Taux de change appliqué pour la devise de tarification à la devise de facturation. | *0,846202666* |
| PCToBCExchangeRateDate | Date à laquelle la devise de tarification pour la devise de facturation est déterminée. | *30/09/2020* |
| MeterDescription | Description du compteur.  | *Tables-données stockées LRS (Go/mois)* |
| ReservationOrderId | ID de la commande de réservation. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Description du crédit. | *Crédit de consommation Azure* |

>[!NOTE]
>Vous pouvez rapprocher votre consommation Azure dans votre fichier de rapprochement d’achat à usage unique. Pour ce faire, accédez à votre fichier de rapprochement d’utilisation évalué quotidiennement et recherchez votre SubscriptionID. Cela permet d’afficher tous les coûts associés à votre ID de plan Azure. Votre SubscriptionID Azure est affiché en tant que EntitlementID.

## <a name="next-steps"></a>Étapes suivantes

- [Facturation et taxes](billing.md)
