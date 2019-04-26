---
title: Présentation des types de facturation dans partenaires | Partenaires
ms.topic: article
ms.date: 03/01/2019
Description: Pour plus d’informations sur les différents types de facturation, périodes de facturation et de facturation dates
author: MaggiePucciEvans
ms.author: evansma
keywords: facturation, paiements, orders, fichiers de réconciliation, fichier de rapprochement
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 4b2b42c0d9bbb2654bbd486f987e3d5da9c562a2
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135379"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Présentation des types de facturation dans l’Espace partenaires

**S’applique à**

-  Espace partenaires
-  Partenaires du programme CSP

Selon les types de produits que vous achetez pour vos clients, vous pouvez avoir différentes périodes de facturation et facturés à des jours différents du même mois. Cet article explique ce qui a changé en commençant le 1 mars 2019, et comment les modifications auront un impact.

## <a name="billing-for-recurring-charges"></a>Facturation des frais récurrents

L’expérience de facturation des frais récurrents des abonnements basés sur licence et basée sur l’utilisation ne change pas. Nous continuerons à vous facturer le jour du mois que vous avez sélectionnée comme votre date de facturation et votre période de facturation continuera à être le mois avant cette date. Si vous avez sélectionné le 15 jours du mois pour la date de facturation, vous serez facturé pour toutes les activités du 15 d’un mois calendaire vers le 14 du mois calendaire suivant. Factures et les fichiers de réconciliation sont à la disposition générale 2 à 4 jours après la date de facturation.

Comme avant, nous débiterons vous pour ces produits dans la devise pour le pays/région que vous êtes situé dans, quel que soit l’emplacement du client, vous vendu le produit à.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturation des frais récurrents à usage unique et sélectionnez

En commençant le 1 mars 2019, nous avons introduit une nouvelle expérience de facturation pour les frais récurrents et à usage unique pour les produits Microsoft et tiers ISV.

Pour ces produits, la période de facturation commence le premier jour du mois du calendrier et se termine le dernier jour du mois du calendrier. Nous allons rendre votre facture disponible le 8ème jour du mois suivant. 

En d’autres termes, toutes les transactions effectuées entre le 1er mai et le 31 mai 2019 figurera sur votre facture le 8 juin. Toutes les transactions effectuées entre le 1er juin et le 30 juin 2019 apparaît sur votre facture le 8 juillet. Vous pouvez facturé Achats périodiques et à usage unique sur la même facture. 

Vous pouvez également vérifier votre solde de compte/facture chaque fois que vous souhaitez (par exemple, entre 1 mai et juin 7) et consultez la dernière activité de compte sans avoir à attendre la facture. Notez que lorsque nous publions votre facture sur les 8, il inclura taxes et d’autres frais applicables et crédits, donc la quantité finale peut-être différer de ce que vous voyez pendant la période de facturation. 

Vous accéderez à vos factures la même façon que vous faire maintenant, dans le centre de partenaires ou par l’API. Ceux-ci s’affichent avant minuit (UTC) la 8ème jour du mois. 

|**Expérience de facturation**|**Ou types de produits**|**Date de facturation**|**Période de facturation**|**Devise de facturation**|**Activité en cours disponible ?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Frais récurrents pour les abonnements basés sur licence et basée sur l’utilisation |Tous les produits à partir de la [catalogue de services en ligne](https://partner.microsoft.com/commerce/preferredoffers/list). Exemples : Office 365, Microsoft 365, Azure Active Directory, Azure (paiement à l’utilisation), Dynamics 365, Power BI Pro |La date que vous avez sélectionné lorsque vous avez créé votre compte espace partenaires |Le mois avant la date de facturation. |La devise du pays/région, vous êtes situé dans. Par exemple, si votre entreprise se trouve au Royaume-Uni, nous débiterons vous en livres sterling (GBP). Si votre société se trouve en Inde, nous débiterons vous en Inde Roupie (INR).  |Non |
|Frais récurrents et à usage unique pour les produits Microsoft et tiers les éditeurs de logiciels |Tous les SaaS abonnements, des réservations Azure et produits logiciels (perpétuels et basées sur abonnement) offertes par Microsoft et les éditeurs de logiciels tiers. Consultez les produits disponibles dans le [place de marché](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Exemples logiciel SUSE Linux (abonnement logiciel), Windows Server Essentials 2019 (logicielle perpétuelle), abonnement de produit Azure ISV SaaS. |La 8ème jour de chaque mois |À partir du premier jour au dernier jour de chaque mois du calendrier |La devise du pays/région, votre client se trouve dans. Cela signifie que vous recevez des factures distinctes et fichiers de réconciliation dans la devise du pays/région chaque client que vous avez vendu à dans la période de facturation. |Oui |
