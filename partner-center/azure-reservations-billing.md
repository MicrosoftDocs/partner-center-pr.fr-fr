---
title: Facturation des réservations Azure | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
Description: Informations sur la facturation pour les réservations d’Azure.
author: LauraBrenner
ms.author: v-petand
keywords: Azure RI, azure, instances réservées, réservations, machines virtuelles, gérer, facturation, acheter
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b99cb2a72d69cd33f9267a956f921aa65dedd482
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135419"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Facturation de Microsoft Azure Reserved VM Instances

**S’applique à**

-  Espace partenaires
-  Portail Microsoft Azure
-  Partenaires fournisseurs de solutions Cloud

Les partenaires du programme Fournisseur de solutions Cloud peuvent proposer à leurs clients des instances réservées sur des machines virtuelles Microsoft Azure. Les clients peuvent réserver des machines virtuelles à l’avance : pour une période d'un ou de trois ans, et réaliser des économies conséquentes sur l’utilisation d’Azure.   

Vos clients paient à l’avance le service Azure Reserved VM Instances. Lorsque vous achetez des instances Azure Reserved VM Instances pour le compte d’un client, vous recevrez des factures et des fichiers de rapprochement pour ces frais ponctuels. 

>[!IMPORTANT]
>Si vous achetez Azure Reserved VM Instances pour un client dans un marché dont la devise est différente de la vôtre, la devise de facturation par défaut sera celle du marché du client, et non pas la vôtre. Si vous avez des clients dans plusieurs pays, vous recevrez des factures et fichiers de rapprochement distincts pour chaque devise de facturation des clients, ce qui vous permettra de facturer vos clients dans la devise appropriée. 

Pour accéder aux factures de facturer des frais uniques et les fichiers de réconciliation, sélectionnez **facturation** dans Partner Center, puis sélectionnez **une fois**. 

Pour plus d’informations sur la facturation dans le cadre du programme Fournisseur de solutions Cloud, voir [Notions de base de facturation](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Définitions des fichiers de facture Azure Reserved VM Instances

**Informations de facturation générales**

|**Champ** |**Définition**|
|:----------------|:-----------------------------|
|Numéro d’identification américain FEIN |Votre numéro fiscal fédéral. |
|Adresse de facturation |L’adresse professionnelle légale utilisé à des fins de fiscalité. Pour modifier cette adresse, accédez à Paramètres du compte > Profil de facturation du partenaire. |
|Frais |Tous les frais en cours. |
|Crédits |Les crédits pour tout remboursement effectué depuis l'achat initial. |
|Remises |Les remises pouvant s’appliquer à des réservations Azure ou à d’autres éléments de la commande du client. |
|Taxes |Total des taxes des frais en cours correspond au total de la section des détails commençant à la page&nbsp;2 de la facture. |
|Total des frais en cours |Montant dû dans votre devise de facturation pour la période de facturation, à payer à la date d’échéance. |
|Instructions pour le paiement |Décrit quand et comment payer votre facture en fonction de votre région. Indiquez toujours votre numéro de facture lors du paiement. |
|N⁰ de facture |Numéro de votre facture. |
|Date de facturation |Date à laquelle votre facture a été créée. |
|Modalités de paiement |Pour les achats ponctuels, le délai sera toujours de 60 jours. |
|Date d’échéance du paiement |Votre paiement doit être reçu au plus tard à cette date. |


**Liste détaillée des frais à usage unique**

|**Champ** |**Définition**|
|:----------------|:-----------------------------|
|Date |Date d’achat. |
|Description |Nom du produit. |
|Quantité |Le nombre de produits (réservations, par exemple) achetés. |
|Prix unitaire |Prix par produit (par exemple, réservation). |
|Remises |Toutes les remises applicables. |
|Montant hors taxe |Sous-total des achats avant impôts. |
|Taxe de vente |Montant des taxes. |
|Total |Total à payer. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Descriptions des fichiers de réconciliation Azure Reserved VM Instances

|**Champ** |**Définition**|
|:----------------|:-----------------------------|
|PartnerId |ID partenaire au format GUID. |
|CustomerId |ID unique de Microsoft, au format GUID, utilisé pour identifier le client. |
|CustomerName |Nom de l’entreprise du client comme indiqué dans l’Espace partenaires. Cela est très important pour rapprocher la facture des informations de votre système. |
|CustomerDomainName |Le nom de domaine du client. |
|CustomerCountry |Le pays dans lequel se trouve le client. |
|InvoiceNumber |Le numéro de la facture dans laquelle la transaction spécifiée apparaît. |
|MpnId |L'identifiant MPN du partenaire fournisseur de solutions Cloud (direct ou indirect). |
|ID&nbsp;MPN revendeur |Apparaît uniquement dans les fichiers de rapprochement pour les partenaires dans le modèle indirect. ID MPN du revendeur de référence pour la réservation. Cet ID correspond à l’ID de revendeur indiqué pour la réservation dans l’Espace partenaires. Si un partenaire Fournisseur de solutions Cloud a vendu la réservation directement au client, son ID MPN est indiqué deux fois, en tant qu’ID MPN et ID MPN revendeur. Si un partenaire&nbsp;CSP a un revendeur dépourvu d’ID&nbsp;MPN, cette valeur est définie à la place sur l’ID&nbsp;MPN du partenaire. Si le partenaire&nbsp;CSP supprime un&nbsp;ID revendeur, cette valeur est définie sur&nbsp;-1. |
|OrderId |Identificateur unique pour une commande dans la plateforme de facturation Microsoft. Peut être utile pour identifier la réservation Azure lors du contact avec le support technique, mais pas pour le rapprochement. |
|OrderDate |La date à laquelle la commande a été passée. |
|ProductId |ID du produit. |
|SkuId  |L’ID d'une référence SKU spécifique. |
|AvailabilityId |L’ID d'une disponibilité spécifique. La « Disponibilité » indique si une référence spécifique est disponible ou non à l'achat pour un pays, une devise, un secteur etc. |
|SkuName  |Le titre d'une référence spécifique. |
|ProductName |Le nom du produit. |
|ChargeType |Le type de frais ou d’ajustement. |
|UnitPrice |Prix par produit commandé. |
|Quantité |Nombre de produits commandés. |
|Sous-total |Total avant impôt. Vérifiez que le sous-total correspond au total prévu, en cas de remise. |
|TaxTotal |La somme totale de toutes les taxes applicables. |
|Total |Le montant total de cet achat. |
|Symbole monétaire |Type de devise. Chaque entité de facturation n’a qu’une devise. Vérifiez qu’elle correspond à votre première facture, et revérifiez après toute mise à jour importante de la plateforme de facturation. |
|DiscountDetails |Liste détaillée des remises éventuelles pertinentes. |


## <a name="manage-your-billing"></a>Gérer vos facturations

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Consultez le statut actuel de la facturation, des factures et des fichiers de rapprochement

1.  Dans le centre de partenaires, sélectionnez **facturation** , puis **une fois** pour afficher l’état de votre facturation. 
2.  Sélectionnez une facture ou un fichier de rapprochement pour afficher des informations plus détaillées. 

### <a name="view-a-customers-order-history"></a>Afficher l’historique des commandes d’un client

1.  Sélectionnez **clients** dans le menu espace partenaires.
2.  Sur votre page **Clients**, recherchez le client dont vous souhaitez afficher l’historique de commandes, puis sélectionnez la flèche allant vers le bas pour développer son dossier. 
3.  Sélectionnez **Afficher les commandes** pour afficher l’historique des commandes.

### <a name="create-a-credit-or-void-note"></a>Créer un crédit ou annuler une facture

Vous pouvez avoir besoin d'annuler une facture et d'en créer une nouvelle. Par exemple, un client peut modifier le nom de son entreprise, puis recevoir une facture sur laquelle figure l'ancien nom. 

Pour annuler une facture et en créer une nouvelle, téléchargez le formulaire disponible sur la page Facturation, sous la section Ajustements.

## <a name="azure-reservations-resources"></a>Ressources des réservations Azure
|**Pour plus d’informations sur**   |**Lisez ce**    |
|:-----------------------------|:-----------------|
|Réservations Azure dans la vue d’ensemble des fournisseurs de solutions Cloud  | [Vendez des Instances de machine virtuelle réservée Azure de Microsoft](azure-reservations.md)
|Achat de réservations Azure pour vos clients dans l’espace partenaires   |[Acheter des réservations Azure](azure-reservations-buying.md)
| Gestion des réservations d’Azure dans l’espace partenaires | [Gestion des réservations d’Azure dans l’espace partenaires](azure-reservations-manage.md)
|Achat de réservations Azure dans le portail Azure | [Prépaiement des machines virtuelles avec Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) dans l’aide d’Azure |
|Gestion des réservations Azure dans le portail Azure   |[Gérer les instances de machines virtuelles réservées](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) dans l’aide d’Azure  |
|Achat de réservations Azure à l’aide de l'API de l'Espace partenaires | [Acheter Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) dans la documentation pour développeurs Espace partenaires

 
