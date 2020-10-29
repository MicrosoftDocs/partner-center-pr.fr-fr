---
title: Fonctionnalités de facturation directe limitées
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En savoir plus sur les conditions requises pour les partenaires de facturation directe et la procédure à suivre pour éviter que des fonctionnalités soient limitées. Déterminez si vos fonctionnalités ont été limitées.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ee6f4fdb537752cccbceb68716ed22bb8c5fb3a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795765"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Fonctionnalités de facture directe restreintes et exigences requises pour les partenaires de facturation directe de fournisseurs de solutions Cloud  

## <a name="overview"></a>Vue d’ensemble

Les partenaires de facturation directe doivent répondre aux nouvelles [exigences](direct-partner-new-requirements.md) pour rester dans le programme de partenaire de facture directe du fournisseur de solutions Cloud. Dans le cas contraire, leur accès aux fonctionnalités de facturation directe finira par être limité et ils ne pourront plus effectuer des tâches spécifiques comme procéder à de nouveaux achats pour leurs clients.

> [!Note]
> Les partenaires directs qui ne remplissent pas les nouvelles conditions requises pour le programme de partenaire de facturation directe sont informés par Microsoft lorsque leurs fonctionnalités de facture directe sont limitées. Cela s’applique à tous les partenaires de facturation directe, qu’ils aient opté pour [la transition entre le partenaire direct Bill et les revendeurs indirects](transition-direct-to-indirect.md) .  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Comment savoir si vos fonctionnalités de facture directe ont été limitées

Pour vérifier si l’accès du locataire du partenaire de facturation directe aux fonctionnalités de facture directe a été restreint, procédez comme suit.

1. Connectez-vous au [tableau de bord de l’espace partenaires](https://partner.microsoft.com/dashboard).

2. Accédez à **paramètres du partenaire**  ->  **profil de partenaire** .

3. Sous **informations sur le programme** , recherchez **Microsoft Cloud État du fournisseur de solutions** .

4. Si l’état du programme a une valeur **restreinte** , cela signifie que l’accès de votre locataire de partenaires directs aux fonctionnalités de facturation directe a été restreint.

## <a name="affected-direct-bill-capabilities"></a>Fonctionnalités de facture directe affectées

Si vos capacités de facturation directe ont été restreintes, vous ne pouvez plus effectuer de nouveaux achats pour vos clients dans l’espace partenaires. Cette restriction comprend les éléments suivants :

- Abonnements Azure

- Abonnements basés sur une licence

- Ajoutez de nouveaux modules complémentaires aux abonnements existants basés sur une licence.

- Achetez des logiciels et des produits de réservation à l’heure (par exemple, les abonnements logiciels, les logiciels perpétuelles et les instances de machines virtuelles réservées Azure).

Vous ne pouvez pas non plus utiliser l' [offre de services partagés de partenaires Azure](shared-services.md) dans le cadre du programme CSP pour acheter de nouveaux abonnements Azure pour votre usage personnel.

Les abonnements à facture directe existants ne sont pas affectés. Ils restent valides et sont renouvelés automatiquement. Vous continuerez à être facturé directement par Microsoft jusqu’à ce qu’il soit annulé. Vous pouvez toujours gérer les abonnements existants des manières suivantes :

- Suspendre les abonnements existants

- Ajuster le nombre de licences des abonnements basés sur une licence existants

- Ajustez le nombre de licences des modules complémentaires existants à un abonnement. 
 
    >[!Note] 
    >Vous ne pouvez pas ajouter de nouveaux modules complémentaires aux abonnements existants, car ils sont traités comme un nouvel achat.

- Déployez de nouvelles ressources Azure et gérez les ressources Azure existantes dans les abonnements Azure existants. Cela comprend les ressources qui sont disponibles via la place de marché Azure et les abonnements Visual Studio.

En plus des nouveaux achats, vous ne pouvez pas accéder aux fonctionnalités de facture directe suivantes dans l’espace partenaires :

- Vous ne pouvez pas créer de nouveaux locataires client. L’option **créer un client** sous la page **clients** dans l’espace partenaires n’est pas disponible.

- Vous ne pouvez pas générer d’invitation à un client demandant une relation directe des revendeurs. L’option **demander une relation de revendeur** sous la page **clients** de l’espace partenaires n’est pas disponible.

    >[!NOTE]
    >Dans le cadre de la transition entre un partenaire de facturation directe et un revendeur indirect, si vous avez déjà inscrit votre locataire de partenaire direct Bill en tant que revendeur indirect, vous pouvez générer une invitation au client demandant une relation de revendeur indirect à la place.

- Vous ne pouvez pas créer un locataire sandbox. Chaque locataire de partenaire direct Bill peut créer un locataire sandbox dans le cadre de l’intégration de l’API de facturation directe. Si vous n’en avez pas encore créé une, vous n’êtes pas autorisé à le faire une fois que vous avez restreint la fonctionnalité de partenaire de facturation.  

## <a name="next-steps"></a>Étapes suivantes

- [Informations supplémentaires sur la façon de devenir un revendeur indirect](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nouvelles conditions requises pour les partenaires directs CSP](direct-partner-new-requirements.md)