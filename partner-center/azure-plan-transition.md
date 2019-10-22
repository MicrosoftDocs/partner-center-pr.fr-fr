---
title: Transition des clients vers le plan Azure | Espace partenaires
ms.topic: article
ms.date: 10/15/2019
description: ''
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 34895de69eaa1aed16a485ddec032769f8dfc7a3
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171292"
---
# <a name="transition-your-customers-to-azure-plan"></a>Faire passer vos clients au plan Azure

Les partenaires pourront faire passer leurs clients d’offres de mise sur le marché (Go-to-Markets) ou Fournisseur de solutions Cloud (CSP) Azure existantes à la nouvelle expérience de commerce disponible dans le programme CSP pour Azure. Les clients pourront acheter des services cloud de façon simplifiée, que ce soit auprès de partenaires, de vendeurs Microsoft ou directement sur le Web. La possibilité de transition s’adresse uniquement aux clients qui passent à la nouvelle expérience de commerce et qui ont signé le Contrat client Microsoft, et non à d’autres offres du programme CDP, comme Office 365 ou Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Passer d’offres CSP existantes à un plan Azure

Vous pouvez faire basculer les offres CSP Azure existantes d’un client vers les services Azure relevant du plan Azure de la nouvelle expérience de commerce du programme CSP, et ce à partir de l’Espace partenaires. Cette transition est soumise à une seule condition :

- Le partenaire et le client final doivent avoir établi une relation de revendeur via l’Espace partenaires, et le client doit avoir signé le Contrat client Microsoft.

### <a name="select-transition-to-azure-plan"></a>Sélectionner la transition vers le plan Azure

1. Sélectionnez le plan Azure pour votre client.

2. Sélectionnez **Transition de la facturation vers un plan Azure**.

![transition](images/azure/transition1.png)

3. Sélectionnez **Continuer**.

![transition](images/azure/transition2.png)

Vous accédez alors au portail Azure où la transition se déroule. La transition de votre client vers le plan Azure s’opère sans avoir rien d’autre à faire. 

**Le workflow de transition automatise les étapes prérequises** : 

- Achat d’un ou plusieurs plans Azure 
- Un plan par client dans les scénarios CSP Direct  
- Un plan par revendeur  

Par exemple, un partenaire a acheté deux offres Microsoft Azure et a inclus deux partenaires de référence distincts dans l’achat. Dans ce cas, le workflow de transition achète deux plans Azure (un par revendeur) et mappe automatiquement les abonnements Azure respectifs dans le cadre des plans Azure.  

**Mappage d’un abonnement Azure à un plan Azure**

Après l’achat d’un ou plusieurs plans Azure, notre système mappe les abonnements Azure existants aux plans Azure. La progression peut être examinée sur le portail Azure et dans l’Espace partenaires. 

4. Revenez à la page de **Abonnements** de l’Espace partenaires de votre client pour mettre à jour sa limite budgétaire dans sa devise locale. 

![Transition](images/azure/transition3.png)

>[!Note]
>Le budget que vous définissez dans l’Espace partenaires n’est pas reporté sur le portail Azure. Vous devez aussi définir le budget et l’alerte sur le portail Azure.

Quand vous passez au plan Azure, vous ne pouvez plus acheter d’abonnements Azure pour ce client. Vous devez créer les abonnements relevant du plan Azure sur le portail Azure.

### <a name="track-your-transition-details"></a>Suivre les détails de votre transition

Vous pouvez suivre la progression de la transition sur le portail Azure et dans l’Espace partenaires.

![Afficher les détails](images/azure/details1.png)

**Impact sur la facturation des partenaires**

Si vous opérez la transition d’un client à partir d’une offre Azure CSP existante, les impacts sur la facturation seront les suivants :

- Votre facture CSP existante portera sur l’ensemble de votre consommation jusqu’à la date de fin de l’abonnement Azure CSP d’origine.

- Si vous disposiez de droits d’accès d’administrateur à l’abonnement CSP existant, vous continuerez d’y avoir accès une fois la migration de l’abonnement effectuée.

Pour opérer la transition de contrats Entreprise directs vers des inscriptions CSP et Serveur et des inscriptions Cloud vers des services Azure, consultez [Obtenir la propriété de facturation d’abonnements Azure pour un Contrat Partenaire Microsoft]()

**Journal d’audit** :

Pour rapprocher la facturation, affichez l’historique de vos abonnements « Microsoft Azure » (0145P) dans la page **Abonnements**. 

L’abonnement « Microsoft Azure » (0145P) comporte deux parties :
1. Abonnement Commerce 
2. Abonnement Azure (droit d’utilisation)

Une fois la transition terminée, l’abonnement Azure est rattaché à un nouveau plan Azure et l’abonnement Commerce est suspendu de façon à éviter toute communication de consommation supplémentaire.  

>[Remarque] : Quand l’abonnement Microsoft Azure (0145P) est acheté dans le cadre du programme CSP, l’abonnement Commerce et l’abonnement Azure (droit d’utilisation) ont la même valeur. Ce n’est qu’en cas de changements ou de transferts de propriété de facturation que les valeurs diffèrent. 

**Échec**

Pendant les transitions, aucun échec n’est censé se produire. Si cela devait se produire, nous vous en informerons dans le workflow de transition proprement dit. Il n’y aura aucune perturbation dans l’utilisation d’Azure.  

**Étapes suivantes**

- [Gérer les abonnements et les ressources dans le cadre du plan Azure](azure-plan-manage.md)

- [Crédit Partenaires – Vue d’ensemble](partner-earned-credit.md)



