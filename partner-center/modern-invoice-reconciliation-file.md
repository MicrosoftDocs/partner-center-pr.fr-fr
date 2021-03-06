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
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073796"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Champs du fichier de rapprochement des achats à usage unique CSP

**Rôles appropriés**: administrateur de compte | Agent de facturation

## <a name="using-the-recon-file"></a>Utilisation du fichier de rapprochement
Le tableau ci-dessous fournit des descriptions et des exemples de valeurs pour les champs du fichier de rapprochement pour les achats à usage unique du CSP.

Pour plus d’informations sur les fichiers de rapprochement, consultez [utiliser les fichiers de rapprochement](use-the-reconciliation-files.md).

| Colonne | Description | Exemple de valeur |
| ------ | ----------- | ------------ |
| PartnerId | Identificateur unique au format GUID pour une entité de facturation spécifique. Non requis pour le rapprochement. Identique dans toutes les lignes. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificateur Microsoft unique du client au format GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nom de l’organisation du client comme indiqué dans l’Espace partenaires. Cette colonne est importante pour rapprocher la facture de vos informations système. | *Jeanne moderne client DE2* |
| CustomerDomainName | Nom de domaine du client. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Pays dans lequel se trouve votre client. Consultez la [liste complète des pays](./regional-authorization-overview.md) de votre région.  | *ANNULATION* |
| InvoiceNumber | Numéro de facture associé au fichier de rapprochement.  | *G002297372* |
| MpnId | Identificateur MPN du partenaire CSP. Pour plus d’informations, consultez [Comment dénombrer par partenaire](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identificateur MPN du revendeur de l’enregistrement pour l’abonnement. | *6048879* |
| OrderId | Identificateur unique d’une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la commande lorsque vous contactez le support technique. Non utilisé pour le rapprochement. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Date en heure UTC à laquelle la commande a été placée. | *10/3/2020* |
| ProductId | Identificateur unique du produit. | *DZH318Z0BNZ5* |
| SkuId | Identificateur unique de la référence (SKU). | *006G* |
| AvailabilityId | Identificateur unique de disponibilité. | *DZH318Z08B80* |
| skuName | Nom de la référence (SKU). | *Tables-LRS* |
| ProductName | Nom du produit. | *Tables* |
| ChargeType | [Type de frais ou d'](./recon-file-charge-types.md) ajustement. | *Nouveau* |
| UnitPrice | Prix par licence, tel que publié dans la liste de prix au moment de l’achat. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *0,045* |
| Quantité | Nombre de licences. Assurez-vous que cela correspond aux informations stockées dans votre système de facturation au cours du rapprochement. | *1* |
| Sous-total | Total avant impôt. Le sous-total doit être égal à la quantité facturable multipliée par le prix unitaire effectif. | *0* |
| TaxTotal | Frais liés au montant des taxes. Selon les règles fiscales et les circonstances spécifiques de votre marché. | *0* |
| Total | Le montant total est égal au sous-total et au montant des taxes. | *0* |
| Devise | Votre facture est générée dans le contexte de la devise du client. Cela signifie que si vous êtes un partenaire qui collabore avec des clients utilisant différentes devises facturables, vous recevrez une facture pour chaque type de devise client.  | *0,35* |
| PriceAdjustmentDescription | Les raisons des ajustements du prix unitaire. Il s’agit des principales raisons, mais elles ne sont pas limitées à la détermination du prix unitaire effectif. | *[« 15,0% crédit gagné pour les services gérés »]* |
| PublisherName | Éditeur du produit.  | *Microsoft* |
| PublisherId | Identificateur unique utilisé par l’espace partenaires pour identifier le serveur de publication. | *NA* |
| SubscriptionDescription | Le nom de l’offre de service achetée par le client, comme défini dans la liste des prix. Cette colonne est un champ identique à OfferName. | *Plan Azure* |
| SubscriptionId | Identificateur unique d’un abonnement dans la plateforme de facturation Microsoft. Non utilisé pour le rapprochement. Notez que cet identificateur n’est pas le même que l’ID d’abonnement dans la console d’administration partenaire. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Date de début de la période de facturation d’un abonnement. | *9/1/2020* |
| ChargeEndDate | Date de fin de la période de facturation d’un abonnement. | *30/09/2020* |
| TermAndBillingCycle | Durée d’engagement pour poursuivre l’abonnement au moment de l’achat. | *Données stockées (Go/mois)* |
| EffectiveUnitPrice | Prix unitaire au prorata pour calculer le coût du cycle de facturation. Les remises, les ajustements en jours de facturation et d’autres facteurs déterminent le prix unitaire effectif. Pour plus d’informations, consultez [calcul du prix unitaire effectif](./effective-unit-price-calculation.md).  | *0,03825* |
| Unité | Type de l’unité dans laquelle le compteur est facturé. | *1 Go/mois* |
| AlternateId | Autre ID de l’élément de ligne de commande référencé. | *6dc5c039750a* |
| BillableQuantity | Quantité totale facturée.  | *0,005001* |
| BillingFrequency | Plan de facturation sélectionné au moment de l’achat. | *NA*  |
| PricingCurrency | Devise utilisée dans la liste de prix. | *USD* |
| PCToBCExchangeRate | Taux de change appliqué pour la devise de tarification à la devise de facturation. | *0,846202666* |
| PCToBCExchangeRateDate | Date à laquelle la devise de tarification pour la devise de facturation est déterminée. | *30/09/2020* |
| MeterDescription | Description du compteur.  | *Tables-données stockées LRS (Go/mois)* |
| ReservationOrderId | ID de la commande de réservation. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Description du crédit. | *Crédit de consommation Azure* |
| SubscriptionStartDate | Date à laquelle un abonnement est acheté. | *5/1/2021* |
| SubscriptionEndDate | Date d’expiration d’un abonnement. | *4/30/2022* |
| ReferenceID | Liaison à toutes les transactions qui se produisent pendant les mises à niveau. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | Identificateur pour connaître les achats de complément ou d’essai. | *[« Module complémentaire »]* |
| PromotionID | Identificateur à utiliser pour extraire les informations de la promotion. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Vous pouvez rapprocher votre consommation Azure dans votre fichier de rapprochement d’achat à usage unique. Pour ce faire, accédez à votre fichier de rapprochement d’utilisation évalué quotidiennement et recherchez votre SubscriptionID. Cela permet d’afficher tous les coûts associés à votre ID de plan Azure. Votre SubscriptionID Azure est affiché en tant que EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Comment connecter l’abonnement de base à l’abonnement mis à niveau ?

Vous devez utiliser l’ID d’abonnement du produit de base pour rechercher les ID de référence correspondants et les utiliser pour extraire toutes les transactions associées. Associé à l’ID d’abonnement et à l’ID de référence, vous pouvez connecter toutes les mises à niveau qui se sont produites en un seul événement.

## <a name="next-steps"></a>Étapes suivantes

- [Facturation et taxes](billing.md)
