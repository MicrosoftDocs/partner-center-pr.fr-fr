---
title: Créer, suspendre ou annuler des abonnements client | Espace partenaires
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment vendre vos abonnements clients à des produits dans le catalogue après avoir créé un enregistrement de client dans l’espace partenaires.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: abonnement, créer nouveau, ajouter un abonnement, suspendre, annuler, suspendre, suspendre, SaaS, licence, ISV, tiers
ms.localizationpriority: medium
ms.openlocfilehash: 05df57bc744263fd0bbd0eb52411a6e9368926f4
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721723"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Créer, suspendre ou annuler des abonnements client

**S’applique à**

-  Espace partenaires
-  Espace partenaires de Microsoft Cloud for US Government
-  Partenaires fournisseurs de solutions cloud

**Rôles appropriés**

- Agent d’administration
- Administration de facturation
- Administrateur global
- Agent du support technique
- Commercial

Une fois que vous avez créé un enregistrement de votre client dans l’Espace partenaires, vous pouvez lui vendre des abonnements aux produits figurant dans le catalogue. Cela comprend les produits publiés par Microsoft, ainsi que les produits SaaS (Software as a service) publiés par des éditeurs de logiciels indépendants tiers sur la place de [marché commerciale](https://azuremarketplace.microsoft.com/marketplace). 

Veuillez noter que certaines offres sont limitées à un abonnement par client. Pour voir la liste des offres limitées, consultez la page Tarification et offres de l'Espace partenaires.

>[!IMPORTANT]
En tant que partenaire dans le programme CSP, vous pouvez uniquement acheter des abonnements Saas **basés sur une licence** auprès d’éditeurs ISV au sein de l’espace partenaires. Cela signifie que vous pouvez acheter une offre SaaS basée sur une **licence** que l’éditeur ISV met à votre disposition, y compris les [offres exclusives](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) auxquelles vous avez accès. Pour acheter ou gérer d’autres offres de la place de marché commercial auprès d’éditeurs de logiciels (ISV) (telles que des offres basées sur **l’utilisation**, limitées ou basées sur l’utilisation impliquant des applications, des conteneurs ou des machines virtuelles Azure), vous devez accéder au [portail de gestion Azure](https://portal.azure.com/). Pour plus d’informations, consultez acheter des produits de la place de [marché commercial](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Créer un abonnement

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Sélectionnez **Ajouter un abonnement**. L’onglet **services en ligne** affiche toutes les offres SaaS disponibles sur la place de marché.

4. Pour afficher uniquement certains types d’abonnements, effectuez les sélections dans les filtres disponibles :
   - **Éditeur**: choisissez **Microsoft** pour afficher uniquement les offres de Microsoft ou le **partenaire** pour consulter les produits de la place de marché commercialisés publiés par les éditeurs de logiciels indépendants.
   - **Type de facturation**: sélectionnez le type de facturation d’abonnement que vous souhaitez utiliser : **licence** ou **utilisation**. Consultez [FAQ sur les nouvelles fonctionnalités de facturation](faq-about-new-billing-features.md) pour obtenir des informations qui vous aideront à décider entre la fréquence de facturation mensuelle et annuelle.
   - **Catégorie**: choisissez **Enterprise**, **Small Business**ou **version d’évaluation**. Pour obtenir des informations sur les abonnements d’essai, consultez [Proposer à vos clients des abonnements d’essai aux produits Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Sélectionnez les abonnements de produits que vous souhaitez acheter pour votre client. Les produits que vous voyez dépendent du type de segment client (éducation, gouvernement, etc.) et des filtres que vous avez appliqués. Certaines offres affichées sur la place de marché ne sont pas toujours disponibles pour un client spécifique ou un partenaire CSP spécifique. Cela peut être dû aux raisons suivantes :

    - Le client a déjà un abonnement à ce produit et n’est autorisé qu’un seul

    - L’abonnement du client a peut-être été suspendu (dans ce cas, vous pouvez réactiver l’abonnement au lieu d’en acheter un nouveau.)
    
    - Pour les offres SaaS ISV, il peut y avoir plusieurs raisons pour lesquelles l’offre n’est pas disponible à l’achat : l’ISV peut ne pas prendre en charge le pays ou la région de facturation du client. l’éditeur de logiciels indépendant peut avoir choisi de ne pas rendre l’offre disponible par le biais du programme CSP. ou, l’ISV a peut-être rendu l’offre [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) uniquement à certains partenaires CSP. L’offre ISV n’est pas non plus utilisable via l’espace partenaires (par exemple, des conteneurs ou des offres basées sur l’utilisation).  

6. Pour chaque abonnement que vous souhaitez ajouter, entrez le nombre de licences (si nécessaire), puis sélectionnez **Ajouter au panier**.

7. Lorsque vous avez terminé d’ajouter des abonnements, sélectionnez **passer en revue** et passer en revue votre commande.

8. Une fois que vous avez consulté vos commandes et que vous êtes prêt à acheter ces abonnements, sélectionnez **acheter**.

9. Une fois que vous avez acheté un abonnement pour un client, voici ce qui se produit :

    - Vous pouvez consulter ou modifier l’abonnement en sélectionnant le nom de l’abonnement dans la page **abonnements** du client. À partir de là, vous pouvez sélectionner des licences de module complémentaire, le cas échéant, modifier le nombre de licences ou suspendre l’abonnement.

    **Pour les abonnements ISV SaaS (basés sur une licence) :**
    - Vous recevrez un lien vers le site de l’éditeur ISV. Ce lien doit vous aider à effectuer la configuration du déploiement ou du compte de l’abonnement du client. (Notez que ni vous ni votre client ne recevrez un e-mail contenant des instructions pour terminer l’installation/la configuration des comptes pour ce type d’abonnement ISV.)
    
    - Si votre abonnement est fourni avec une version d’évaluation gratuite de 30 jours, la période d’essai gratuite sera appliquée automatiquement. En tant que partenaire dans le programme CSP, vous ne pouvez pas renoncer à la période d’évaluation gratuite sur les offres que vous achetez pour les clients. Une fois la période d’essai gratuite terminée, la durée de l’abonnement commence et l’abonnement est converti en paiement. L’abonnement est ensuite renouvelé automatiquement en fonction de la même planification.

## <a name="suspend-or-cancel-a-subscription"></a>Suspendre ou annuler un abonnement

Les partenaires peuvent suspendre ou annuler un abonnement à la demande du client ou dans les cas de fraude ou de défaut de paiement.

### <a name="suspend-a-subscription"></a>Suspendre un abonnement

Lorsque vous attribuez à un abonnement l’état **Suspendu**, les utilisateurs ne peuvent plus se connecter aux services ou y accéder.

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Choisissez l’abonnement que vous souhaitez gérer.

4. Dans la section **État**, choisissez **Suspendu**. Puis, sélectionnez **Envoyer** pour valider vos modifications.

5. Toutes les données seront supprimées, sauf si l’abonnement est réactivé dans les 90 jours, ou 90 jours en plus du nombre de jours écoulés entre la date d'ouverture du compte et la première période de facturation (120 jours maximum).

Lorsque vous suspendez un abonnement, la date affichée sous le bouton **Suspendu** indique quand l’abonnement va automatiquement expirer si vous ne le réactivez pas. Pour plus d’informations, consultez [FAQ sur les nouvelles fonctionnalités de facturation](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>Annuler un abonnement

Vous avez la possibilité d’annuler les abonnements SaaS basés sur des licences à partir d’éditeurs ISV tiers au sein de la place de [marché commerciale](csp-commercial-marketplace-overview.md)de l’espace partenaires. Tant que vous annulez l’opération pendant la période d’annulation, vous recevrez un remboursement intégral.

Pour les éditeurs de logiciels, les offres sont facturées tous les mois :

- Si vous annulez moins de 24 heures après avoir passé la commande, vous recevrez un crédit complet sur la facture suivante.

- Si vous annulez plus de 24 heures après avoir passé la commande, l’annulation sera planifiée pour être renouvelée.

Pour les offres facturées annuellement :

- Si vous annulez moins de 14 jours après avoir placé la commande, vous recevrez un crédit complet sur la facture suivante.

- Si vous annulez plus de 14 jours après avoir placé la commande, l’annulation sera planifiée au renouvellement.

Une fois ces périodes supérieures, vous ne verrez plus l’option permettant d’annuler l’abonnement.

> [!NOTE]
> Les services ISV tiers basés sur l’utilisation et contrôlés (qui utilisent des machines virtuelles ou des conteneurs, par exemple) ne peuvent pas être retournés. Les services basés sur l’utilisation peuvent être désapprovisionnés en tant que méthode d’annulation. Étant donné que les frais sont facturés après utilisation, ces services ne peuvent pas être remboursés.

Pour annuler un abonnement SaaS basé sur une licence d’un éditeur ISV, procédez comme suit :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Recherchez l’abonnement que vous souhaitez annuler.

4. Dans la colonne **État** , sélectionnez **Annuler**. Puis, sélectionnez **Envoyer** pour valider vos modifications.

5. Si une boîte de dialogue s’affiche, renseignez les détails pertinents, puis sélectionnez **Envoyer**.

6. Pour confirmer l’annulation, sélectionnez **Oui, annuler**.

> [!NOTE]
> Vous pouvez également choisir d’annuler un abonnement à la place de marché Azure à l’aide d’API. Pour ce faire, consultez [annuler un abonnement Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Choisir de renouveler automatiquement un abonnement à la place marché commerciale

Par défaut, les abonnements actifs sont configurés pour se renouveler automatiquement à l’expiration de la période d’abonnement. Pour les [abonnements aux produits de la place de marché commerciale](csp-commercial-marketplace-overview.md), vous pouvez éventuellement choisir de ne pas renouveler automatiquement l’abonnement.

Pour arrêter le renouvellement automatique d’un abonnement au marché commercial actif :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard)de l’espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3.  Sélectionnez **abonnements**. Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.

4.  Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez modifier.

5. Dans la page Détails de l’abonnement, recherchez la section **État** et désactivez la case à cocher **renouvellement automatique** . 

6. Sélectionnez **Envoyer**.

## <a name="see-also"></a>Articles associés

- [Acheter des produits de la place de marché commercial pour vos clients](csp-commercial-marketplace-purchase.md)
- [Gérer les produits de la place de marché commerciale pour vos clients](csp-commercial-marketplace-manage.md)
- [Vue d’ensemble de la Place de marché commerciale](csp-commercial-marketplace-overview.md)


