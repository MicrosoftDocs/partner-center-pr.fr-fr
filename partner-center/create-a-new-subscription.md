---
title: Créer des abonnements clients dans l’espace partenaires
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment vendre des abonnements à vos clients pour des produits publiés par Microsoft ainsi que des produits SaaS publiés par des éditeurs de logiciels indépendants tiers.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201406"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Créer, suspendre ou annuler des abonnements client

**S’applique à**: espace partenaires | Espace partenaires pour Microsoft Cloud pour le gouvernement des États-Unis

**Rôles appropriés**: agent admin | Administrateur de facturation | Administrateur général | Agent du support technique | Agent des ventes

Une fois que vous avez créé un enregistrement de votre client dans l’Espace partenaires, vous pouvez lui vendre des abonnements aux produits figurant dans le catalogue. Cela comprend les produits publiés par Microsoft et les produits SaaS (Software as a service) publiés par des éditeurs de logiciels indépendants (ISV) tiers sur la place de [marché commerciale](https://azuremarketplace.microsoft.com/marketplace).

Certaines offres sont limitées à un seul abonnement par client. Pour voir la liste des offres limitées, consultez la page Tarification et offres de l'Espace partenaires.

>[!IMPORTANT]
> En tant que partenaire dans le programme CSP, vous pouvez acheter des abonnements Saas **basés sur une licence** ou **contrôlés** à partir d’éditeurs ISV dans l’espace partenaires. Cela signifie que vous pouvez acheter une **offre SaaS** **basée sur une licence** ou une offre à laquelle vous avez accès par l’éditeur ISV, y compris les [offres exclusives](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) auxquelles vous avez accès. Pour acheter ou gérer d’autres offres de la place de marché commercial auprès d’éditeurs de logiciels (ISV) (telles que des offres basées sur l’utilisation impliquant des applications Azure, des conteneurs ou des machines virtuelles), vous devez accéder au [portail Azure](https://portal.azure.com/).

>[!NOTE]
>Toutes les dates et heures de l’espace partenaires sont indiquées dans la norme heure UTC (Universal Time Coordinated). Cela peut être différent de 24 heures par rapport à votre heure locale.

## <a name="create-a-new-subscription"></a>Créer un abonnement

1. Connectez-vous au [tableau de bord de l’Espace partenaires](https://partner.microsoft.com/dashboard).

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Sélectionnez **Ajouter un abonnement**. L’onglet **services en ligne** affiche toutes les offres SaaS disponibles sur la place de marché.

4. Pour afficher uniquement certains types d’abonnements, effectuez les sélections dans les filtres disponibles :
   - **Éditeur**: choisissez **Microsoft** pour afficher uniquement les offres de Microsoft ou le **partenaire** pour consulter les produits de la place de marché commercialisés publiés par les éditeurs de logiciels indépendants.
   - **Type de facturation**: sélectionnez le type de facturation d’abonnement que vous souhaitez utiliser : **licence** ou **utilisation**. Consultez [facturation basée sur une licence](license-based-billing.md) pour obtenir des informations qui vous aideront à déterminer la fréquence de facturation mensuelle et annuelle.
   - **Catégorie**: choisissez **Enterprise**, **Small Business** ou **version d’évaluation**. Pour obtenir des informations sur les abonnements d’essai, consultez [Proposer à vos clients des abonnements d’essai aux produits Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Sélectionnez les abonnements de produits que vous souhaitez acheter pour votre client. Les produits que vous voyez dépendent du type de segment client (éducation, gouvernement, etc.) et des filtres que vous avez appliqués. Certaines offres affichées sur la place de marché ne sont pas toujours disponibles pour un client spécifique ou un partenaire CSP spécifique. Cela peut être dû aux raisons suivantes :

   - Le client a déjà un abonnement à ce produit et n’est autorisé qu’un seul

   - L’abonnement du client a peut-être été suspendu (dans ce cas, vous pouvez réactiver l’abonnement au lieu d’en acheter un nouveau.)

   - Pour les offres SaaS ISV, il peut y avoir plusieurs raisons pour lesquelles l’offre n’est pas disponible à l’achat : l’ISV peut ne pas prendre en charge le pays ou la région de facturation du client. l’éditeur de logiciels indépendant peut avoir choisi de ne pas rendre l’offre disponible par le biais du programme CSP. ou, l’ISV a peut-être rendu l’offre [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) uniquement à certains partenaires CSP. L’offre ISV n’est pas non plus utilisable via l’espace partenaires (par exemple, des conteneurs ou des offres basées sur l’utilisation).  

6. Pour chaque abonnement que vous souhaitez ajouter, entrez le nombre de licences (si nécessaire), puis sélectionnez **Ajouter au panier**.

7. Lorsque vous avez terminé d’ajouter des abonnements, sélectionnez **passer en revue** et passer en revue votre commande.

8. Une fois que vous avez consulté vos commandes et que vous êtes prêt à acheter ces abonnements, sélectionnez **acheter**.

9. Une fois que vous avez acheté un abonnement pour un client, voici ce qui se produit :

    - Vous pouvez consulter ou modifier l’abonnement en sélectionnant le nom de l’abonnement dans la page **abonnements** du client. À partir de là, vous pouvez sélectionner des licences de module complémentaire, le cas échéant, modifier le nombre de licences ou suspendre l’abonnement.

    **Pour les abonnements ISV SaaS (licence et compteurs) :**
    - Vous recevrez un lien vers le site de l’éditeur ISV. Ce lien doit vous aider à effectuer la configuration du déploiement ou du compte de l’abonnement du client.
      
    >[!NOTE]
    > Ni vous ni votre client ne recevrez un e-mail contenant des instructions pour terminer l’installation/la configuration de compte pour ce type d’abonnement ISV.)

    - Si votre abonnement est fourni avec une version d’évaluation gratuite de 30 jours, la période d’essai gratuite sera appliquée automatiquement. En tant que partenaire dans le programme CSP, vous ne pouvez pas renoncer à la période d’évaluation gratuite sur les offres que vous achetez pour les clients. Une fois la période d’essai gratuite terminée, la durée de l’abonnement commence et l’abonnement est converti en état payant. L’abonnement est ensuite renouvelé automatiquement en fonction de la même planification.
   
## <a name="update-subscriptions-with-add-ons"></a>Mettre à jour les abonnements avec des modules complémentaires 

Pour acheter un module complémentaire, le client doit d’abord disposer d’un abonnement de base actif.  Vous ne pouvez pas acheter de modules complémentaires par le biais du catalogue.

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Choisissez l’abonnement que vous souhaitez gérer.

4. Sous la section **État** , vous trouverez la liste des modules complémentaires disponibles pour l’abonnement.  

5. Mettez à jour le nombre de licences pour chaque module complémentaire requis. Ensuite, **envoyez** vos modifications.

La possibilité d’acheter des modules complémentaires via l’espace partenaires n’est disponible que pour les fournisseurs directs et indirects.
Seuls les modules complémentaires éligibles sont affichés en fonction des exigences de base et de la disponibilité régionale. Pour plus d’informations sur la tarification et les offres, reportez-vous à la matrice de l’offre du revendeur Cloud. La suspension de l’abonnement de base suspend également tous les modules complémentaires associés.

Les dates de début des modules complémentaires s’alignent sur l’abonnement de base, et les frais sont calculés à partir de la date de début de frais et de la date de fin de frais, avec des frais au prorata sur la première facture. Pour plus d’informations, consultez [facturation basée sur une licence](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Suspendre ou annuler un abonnement

Les partenaires peuvent suspendre ou annuler un abonnement à la demande du client ou dans les cas de fraude ou de défaut de paiement.

### <a name="suspend-a-subscription"></a>Suspendre un abonnement

Lorsque vous attribuez à un abonnement l’état **Suspendu**, les utilisateurs ne peuvent plus se connecter aux services ou y accéder.

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Choisissez l’abonnement que vous souhaitez gérer.

4. Dans la section **État**, choisissez **Suspendu**. Ensuite, **envoyez** vos modifications.

5. Toutes les données seront supprimées, sauf si l’abonnement est réactivé dans les 90 jours, ou 90 jours en plus du nombre de jours écoulés entre la date d'ouverture du compte et la première période de facturation (120 jours maximum).

Lorsque vous suspendez un abonnement, la date affichée sous le bouton **Suspendu** indique quand l’abonnement va automatiquement expirer si vous ne le réactivez pas. 

>[!NOTE]
>Les abonnements CSP n’ont pas de période d’expiration (la façon dont les abonnements directs Web le font) au cours desquels les services continuent de fonctionner, mais l’abonnement ne génère aucun frais de facturation. Les abonnements CSP sont actifs ou suspendus (ou entièrement supprimés).

### <a name="cancel-a-subscription"></a>Annuler un abonnement

Vous pouvez annuler les abonnements SaaS basés sur des licences à partir d’éditeurs ISV tiers au sein de la place de [marché commerciale](csp-commercial-marketplace-overview.md)de l’espace partenaires. Tant que vous annulez l’opération pendant la période d’annulation, vous recevrez un remboursement intégral.

Pour les éditeurs de logiciels, les offres sont facturées tous les mois :

- Si vous annulez moins de 24 heures après avoir passé la commande, vous recevrez un crédit complet sur la facture suivante.

- Si vous annulez plus de 24 heures après avoir passé la commande, l’annulation sera planifiée pour être renouvelée.

Pour les offres facturées annuellement :

- Si vous annulez moins de 14 jours après avoir placé la commande, vous recevrez un crédit complet sur la facture suivante.

- Si vous annulez plus de 14 jours après avoir placé la commande, l’annulation sera planifiée au renouvellement.

Une fois ces périodes supérieures, vous ne verrez plus l’option permettant d’annuler l’abonnement.

> [!NOTE]
> Les services ISV tiers basés sur l’utilisation et contrôlés (qui utilisent des machines virtuelles ou des conteneurs, par exemple) ne peuvent pas être retournés. Les services basés sur l’utilisation peuvent être désapprovisionnés en tant que méthode d’annulation. Étant donné que les frais sont facturés après utilisation, ces services ne peuvent pas être remboursés.

Pour annuler un abonnement SaaS basé sur une licence auprès d’un éditeur de logiciels indépendant, effectuez les étapes suivantes :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Recherchez l’abonnement que vous souhaitez annuler.

4. Dans la colonne **État** , sélectionnez **Annuler**. Ensuite, **envoyez** vos modifications.

5. Si une boîte de dialogue s’affiche, renseignez les détails pertinents, puis sélectionnez **Envoyer**.

6. Pour confirmer l’annulation, sélectionnez **Oui, annuler**.

> [!NOTE]
> Vous pouvez également choisir d’annuler un abonnement à la place de marché Azure à l’aide d’API. Pour ce faire, consultez [annuler un abonnement Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Choisir de renouveler automatiquement un abonnement à la place marché commerciale

Par défaut, les abonnements actifs sont définis pour se renouveler automatiquement à l’expiration de la période d’abonnement. Pour les [abonnements aux produits de la place de marché commercial](csp-commercial-marketplace-overview.md), vous pouvez éventuellement choisir de ne pas renouveler automatiquement l’abonnement.

Pour arrêter le renouvellement automatique d’un abonnement au marché commercial actif :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard) de l’Espace partenaires.

2. Dans le menu Espace partenaires, sélectionnez **Clients**, puis choisissez un client dans la liste.

3. Sélectionnez **Abonnements**. Cette liste répertorie tous les abonnements basés sur des licences que vous avez achetés pour le client.

4. Dans la colonne **abonnement** , sélectionnez l’abonnement que vous souhaitez modifier.

5. Dans la page Détails de l’abonnement, recherchez la section **État** et désactivez la case à cocher **renouvellement automatique** .

6. Sélectionnez **Envoyer**.

## <a name="next-steps"></a>Étapes suivantes

- [Acheter des produits de la place de marché commerciale pour vos clients](csp-commercial-marketplace-purchase.md)

- [Gérer les produits de la place de marché commerciale pour vos clients](csp-commercial-marketplace-manage.md)

- [Vue d’ensemble de la Place de marché commerciale](csp-commercial-marketplace-overview.md)