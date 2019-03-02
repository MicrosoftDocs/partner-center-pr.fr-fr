---
title: Présentation des types de la facturation dans l’espace partenaires | L’espace partenaires
ms.topic: article
ms.date: 03/01/2019
Description: Informations sur différents types de facturation, des périodes de facturation et les dates de facturation
author: labrenne
ms.author: labrenne
keywords: facturation, paiements, commandes, fichiers de rapprochement, fichier de rapprochement
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122291"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Présentation des types de la facturation dans l’espace partenaires

**S'applique à:**

-  Espace partenaires
-  Partenaires du programme fournisseur de solutions cloud

Selon les types de produit que vous achetez pour vos clients, vous pouvez avoir des périodes de facturation différentes et facturé à jours différents du même mois. Cet article explique quelle est la nouveauté à compter du 1er mars 2019, et comment les modifications auront un impact.

## <a name="billing-for-recurring-charges"></a>Facturation de frais récurrents

L’expérience de facturation de frais récurrents des abonnements basés sur les licences et basée sur l’utilisation ne change pas. Nous continuerons à vous facturer le jour du mois que vous avez sélectionné en tant que votre date de facturation et votre période de facturation continuent d’être le mois avant cette date. Si vous avez sélectionné le 15e jour du mois pour votre date de facturation, vous serez facturé pour toutes les activités du 15 d’un mois du calendrier sur le 14 du mois suivant. Factures et fichiers de rapprochement sont généralement disponibles 2 à 4 jours après la date de facturation.

Comme précédemment, nous allons vous facture pour ces produits dans la devise du pays/région que vous êtes situé dans, quel que soit l’emplacement du client, vous avez vendu le produit.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturation de frais récurrents à usage unique et sélections

À compter du 1er mars 2019, nous avons introduit une nouvelle expérience de facturation de frais d’abonnement et à usage unique pour les produits Microsoft et tiers éditeurs de logiciels indépendants.

Pour ces produits, la période de facturation commence le premier jour du mois du calendrier et se termine le dernier jour du mois du calendrier. Nous allons créer votre facture disponibles sur le jour 8 du mois suivant. 

En d’autres termes, les transactions que vous effectuez entre le 1er mai et le 31 mai 2019 seront affiche sur votre facture 8 juin. Les transactions que vous effectuez entre le 1er juin et le 30 juin 2019 seront affiche sur votre facture 8 juillet. Vous pourrez obtenir facturés pour les achats d’abonnement et à usage unique sur la même facture. 

Vous pouvez également vérifier votre solde de compte/facture chaque fois que vous souhaitez (par exemple, entre mai 1 et 7 juin), puis consultez la dernière activité de compte sans avoir à attendre que la facture. Notez que lorsque nous validez votre facture sur le 8, il inclut les taxes et d’autres frais applicables et les crédits, le montant final peut différer du contenu affiché pendant la période de facturation. 

Vous allez accéder à vos factures la même manière que vous le faites, dans l’espace partenaires ou par l’API. Ils s’affiche avant le jour du mois 8 à minuit UTC. 

|**Expérience de facturation**|**Types de produit**|**Date de facturation**|**Période de facturation**|**Devise de facturation**|**Activité en cours disponible?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Frais récurrents pour les licences et basée sur l’utilisation des abonnements |Tous les produits à partir du [catalogue de services en ligne](https://partner.microsoft.com/commerce/preferredoffers/list). Exemples: Office 365, Microsoft 365, Azure Active Directory, Azure (paiement), Dynamics 365, PowerBI Pro |La date que vous avez sélectionné lorsque vous avez créé votre compte espace partenaires |Le mois avant la date de facturation. |La devise du pays/région, vous êtes situé dans. Par exemple, si votre entreprise se trouve dans l’anglais (Royaume-Uni), nous allons vous facturer dans livres sterling (GBP). Si votre société se trouve en Inde, nous allons vous facturer en Inde Roupie (INR).  |Non |
|Frais d’abonnement et à usage unique pour les produits Microsoft et tiers éditeurs de logiciels indépendants |Tous les SaaS, réservations Azure, produits et abonnements logiciels (à durée indéterminée et sur l’abonnement) offertes par Microsoft et les éditeurs de logiciels tiers. Afficher les produits disponibles sur le [marché](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Exemples logiciel SUSE Linux (abonnement logiciel), Windows Server 2019 Essentials (logiciel à durée indéterminée), abonnement Azure éditeurs de logiciels indépendants SaaS. |Le jour 8 de chaque mois |À partir du premier jour au dernier jour de chaque mois du calendrier |Devise du pays/région dans que votre client se trouve. Cela signifie que vous recevrez des factures distincts et fichiers de rapprochement dans la devise du pays/région chaque client que vous a vendu dans la période de facturation. |Oui |
