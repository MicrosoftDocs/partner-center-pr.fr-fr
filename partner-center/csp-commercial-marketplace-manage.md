---
title: Gérer les produits de la place de marché & offres
ms.topic: article
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: À l’aide de l’espace partenaires, Découvrez comment les fournisseurs de solutions Cloud peuvent gérer des offres ISV tierces achetées pour les clients à partir de la place de marché commerciale.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 076cd97dcecc706b9cd47ffc4a4227c93d20d632
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435088"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Gérer les produits et offres de la place de marché commercial pour vos clients

**S’applique à**

- Espace partenaires
- Partenaires du programme Fournisseur de solutions Microsoft Cloud

**Rôles appropriés**

- Administrateur général
- Agent d’administration

Les partenaires du programme fournisseur de solutions Cloud (CSP) peuvent utiliser le portail espace partenaires pour acheter de nombreuses offres ou abonnements SaaS ISV pour leurs clients à partir du Marketplace commercial. Une fois que vous avez acheté une offre, vous disposez de différentes méthodes pour la gérer.

## <a name="view-or-edit-a-subscription"></a>Afficher ou modifier un abonnement

Après avoir acheté un abonnement auprès d’un éditeur ISV tiers, vous pouvez le consulter ou le modifier comme suit :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires, puis sélectionnez **clients** dans le menu de navigation de gauche.

2. Sélectionnez un client approprié, puis sélectionnez **abonnements**. Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.

3. Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez afficher ou modifier. Cela vous donne plus d’informations sur la configuration ou la configuration de l’offre. (Si une action supplémentaire est nécessaire sur l’offre, vous pouvez également voir l’état « action nécessaire » affiché dans la colonne État. Cela peut également être accompagné d’un lien vers le site de l’éditeur ISV.)

4. Une fois que vous avez sélectionné l’abonnement que vous souhaitez afficher ou modifier, la page de détails de l’abonnement vous permet de modifier l’abonnement et d’effectuer des opérations telles que :

    - Modifier le surnom de l’abonnement

    - Ajouter/réduire le nombre de sièges (licences) dans l’abonnement

    - Annuler l’abonnement

    - Désactiver le renouvellement automatique

    - Ajouter un ID MPN du revendeur indirect, le cas échéant

> [!NOTE]
> Vous devrez peut-être effectuer certaines étapes définies par l’éditeur ISV avant de pouvoir effectuer certaines modifications dans un abonnement, telles que l’annulation d’un abonnement.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Attribuer des licences et activer un abonnement pour le compte d’un client

Lorsque vous achetez une offre SaaS (Software as a service) fournie par un éditeur de logiciels indépendant (ISV) dans la place de marché commercial, l’éditeur ISV vous aide à gérer le processus d’attribution des licences et d’activation de l’abonnement pour le compte de votre client.

Le serveur de publication doit vous fournir un lien personnalisé et un code d’autorisation qui identifie votre achat spécifique.

1. Vous pouvez trouver ce lien personnalisé à partir de l’éditeur ISV de plusieurs façons :

   - Vous pouvez voir le lien à partir de la page de confirmation qui s’affiche une fois que vous avez acheté une offre SaaS ISV. Pour trouver ce lien sur la page, recherchez et sélectionnez **accéder au site de l’éditeur**.

   - Vous pouvez voir le lien à partir de la page abonnements d’un client spécifique. Ce lien vers l’éditeur apparaît sur la ligne associée à l’offre ISV ou à l’abonnement acheté pour le client.

   - Vous pouvez [récupérer le lien à l’aide des API de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Pour ce faire, pour le compte de votre client, vous devrez peut-être copier le lien personnalisé, le coller dans un navigateur privé et entrer les informations d’identification du client.

2. Une fois que vous êtes dans le site ou le système de l’éditeur ISV, le serveur de publication vous informe des étapes supplémentaires que vous devez suivre pour terminer le processus de configuration du client et approvisionner ou attribuer des licences.

3. En tant que partenaire dans le programme CSP qui travaille pour le compte de votre client, vous êtes chargé d’effectuer les tâches suivantes :

    - Envoyez toutes les informations requises au serveur de publication.

    - Envoyer toute l’URL requise directement à votre client (ou communiquer directement les détails de cet abonnement à votre client)

4. Une fois que vous avez fourni les informations requises au serveur de publication, le serveur de publication provisionne et attribue les licences appropriées. La facturation de l’abonnement démarre uniquement lorsque les événements suivants se produisent :

    - L’éditeur ISV a correctement attribué les licences appropriées

    - L’éditeur ISV a confirmé à Microsoft (via une API de réalisation SaaS distincte) que la configuration du compte a été effectuée avec succès.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Annuler un abonnement SaaS basé sur une licence à partir d’un éditeur ISV

Lorsque vous vous abonnez à un produit SaaS basé sur une licence proposé par un éditeur ISV sur la place de marché commercial, vous avez la possibilité d’annuler l’abonnement au cours de sa période d’annulation désignée. Cette période d’annulation varie selon que vous disposez d’un abonnement mensuel ou annuel. Vous pouvez également choisir de renouveler ou non automatiquement l’abonnement.

Pour plus d’informations sur les périodes d’annulation qui s’appliquent, sur l’annulation ou le renouvellement automatique d’un abonnement, voir :

- [Annuler un abonnement](create-a-new-subscription.md#cancel-a-subscription)

- [Renouvellement automatique d’un abonnement au marché commercial](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Ajouter ou supprimer des licences pour un abonnement SaaS

Pour les offres de la place de marché commercial SaaS, vous pouvez ajouter ou supprimer des licences utilisateur pour un abonnement client.

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires, puis sélectionnez **clients** dans le menu de navigation de gauche.

2. Sélectionnez un client approprié, puis sélectionnez **abonnements**. Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.

3. Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez modifier.

4. Dans la page Détails de l’abonnement, recherchez le champ **quantité** . C’est là que vous pouvez augmenter ou diminuer le nombre de licences.

5. Modifiez la quantité, puis sélectionnez **Envoyer**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gérer les abonnements à l’aide des API de l’Espace partenaires

Vous pouvez également utiliser les API de l’espace partenaires pour effectuer la gestion du cycle de vie et gérer les factures pour vos abonnements. Pour plus d’informations, consultez [créer un abonnement pour les produits de la place de marché commercial](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Étapes suivantes

- [Acheter des offres de la place de marché commercial](csp-commercial-marketplace-purchase.md)
- [En savoir plus sur la facturation dans la place de marché commerciale](csp-commercial-marketplace-billing.md)