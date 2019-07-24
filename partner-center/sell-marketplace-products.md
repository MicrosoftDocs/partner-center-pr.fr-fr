---
title: Vendre des abonnements à des produits de la place de marché Azure | Espace partenaires
ms.topic: article
ms.date: 07/12/2019
description: Vous pouvez utiliser l’espace partenaires pour vendre les abonnements de vos clients aux produits SaaS (Software as a service) publiés sur la place de marché Azure par des éditeurs de logiciels indépendants (ISV).
author: JnHs
ms.author: jenhayes
keywords: abonnements, Marketplace, tiers, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 4dda776e7ebdece3a8a15c3576b64d93d3e4158c
ms.sourcegitcommit: dd961f85bc790e56c70479a5926177454dd8e855
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/12/2019
ms.locfileid: "67854506"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vendre des abonnements à des produits de la Place de marché Azure

**S’applique à**

- Espace partenaires

Vous pouvez utiliser l’espace partenaires pour vendre les abonnements de vos clients aux produits SaaS (Software as a service) publiés sur la place de [marché Azure](https://azuremarketplace.microsoft.com/marketplace) par des éditeurs de logiciels indépendants (ISV). Cela peut vous aider à faire la différence entre votre entreprise et fournir à vos clients des offres groupées de logiciels qui répondent à leurs besoins professionnels spécifiques. Vous gérez les licences et les abonnements pour ces produits SaaS de la place de marché Azure comme vous le feriez pour les produits Microsoft.

Pour plus d’informations sur la place de marché Azure, consultez le Forum aux questions sur la place de [marché Azure](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Afficher les offres de la place de marché et la tarification

Pour afficher toutes les offres disponibles, sélectionnez **Marketplace** dans le menu de navigation de gauche. Par défaut, vous verrez des produits de tous types et catégories. Vous pouvez filtrer par type et/ou catégorie, ou utiliser la zone de recherche pour rechercher des mots clés spécifiques. Sélectionnez un produit pour afficher des informations sur le serveur de publication et les références SKU disponibles, notamment si une période d’essai gratuite est proposée.

> [!NOTE]
> Certains produits disponibles dans la place de marché Azure peuvent ne pas être affichés ici. Les éditeurs de logiciels indépendants peuvent décider s’ils doivent proposer leurs produits aux partenaires du fournisseur de solutions Cloud (CSP) dans l’espace partenaires. Si vous voyez un produit dans la place de marché Microsoft Azure que vous souhaitez proposer à vos clients par le biais de l’espace partenaires, recherchez les coordonnées du serveur de publication dans la place de marché Azure et dites-leur que vous êtes intéressé.

Les prix des produits de la place de marché Azure peuvent changer fréquemment. Pour obtenir les informations de tarification actuelles pour tous les produits de la place de marché, sélectionnez **Exporter la liste des prix** dans le coin supérieur droit de la page **Marketplace** . Une feuille de calcul contenant toutes les données de tarification est alors générée. Les informations de tarification sont mises à jour quotidiennement, ce qui vous permet de vérifier le plus souvent que vous le souhaitez.

> [!TIP]
> Si un produit de cette liste offre une version d’évaluation gratuite, la feuille de calcul comprendra deux lignes pour ce produit. Une ligne affiche un prix de zéro, ce qui indique qu’une version d’évaluation gratuite est disponible. L’autre ligne inclura le prix et le terme qui s’appliqueront une fois la période d’évaluation terminée.

## <a name="purchase-marketplace-products-for-your-customers"></a>Acheter des produits de la place de marché pour vos clients

L’achat d’abonnements pour les produits SaaS de la place de marché Azure suit le même processus que l’achat d’abonnements pour les produits Microsoft. Lorsque vous ajoutez un abonnement pour un client, vous pouvez choisir d’afficher uniquement les offres Marketplace des ISV en sélectionnant **partenaire** dans le filtre **éditeur** . Pour plus d’informations, consultez [créer un nouvel abonnement](create-a-new-subscription.md).

> [!IMPORTANT]
> Vous pouvez acheter uniquement des abonnements de produits SaaS (Software as a service) dans l’espace partenaires. D’autres types d’offre (tels que les applications, les conteneurs ou les machines virtuelles Azure) sont gérés par le Portail Azure et facturés en fonction de leur consommation. Vous devez disposer d’un abonnement Azure pour activer les solutions de paiement à l’accès via le Portail Azure.

Notez que certaines offres que vous voyez dans la page **Marketplace** peuvent ne pas être disponibles pour un client spécifique. La disponibilité peut être affectée par un certain nombre de facteurs, notamment si l’ISV prend en charge le pays/la région de facturation du client.

> [!TIP]
> Vous pouvez également utiliser les API de l' [espace partenaires](https://docs.microsoft.com/partner-center/develop/) pour créer des abonnements de la place de marché Azure pour vos clients. Pour plus d’informations, consultez [créer un abonnement pour les produits de la place de marché Azure](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Avec les abonnements aux produits de la place de marché Azure, vous avez la possibilité d' [Annuler l’abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) au cours de la période d’annulation (24 heures pour les abonnements mensuels ou 14 jours pour les abonnements annuels). Vous pouvez également [choisir de renouveler ou non automatiquement l’abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-marketplace-products"></a>Activation de licence pour les produits de la place de marché

Pour les types d’offre SaaS (Software as a service), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit. Pour effectuer ce processus, vous devez visiter le site de l’éditeur, à l’aide d’un lien personnalisé avec un code d’autorisation qui permet à l’éditeur d’identifier votre achat spécifique. Vous pouvez trouver ce lien sur la page de confirmation qui s’affiche une fois que vous avez acheté une  offre SaaS et sur la page abonnements (dans la ligne de cette offre). Vous pouvez également [utiliser les API de l’espace partenaires pour récupérer ce lien](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Lorsque vous accédez au site de l’éditeur à l’aide de ce lien, vous verrez les informations ou actions supplémentaires nécessaires pour approvisionner et attribuer des licences, ou pour terminer le processus d’installation. Les étapes requises peuvent varier en fonction de l’éditeur et de l’offre. Vous êtes responsable de l’envoi des informations nécessaires (ou de l’envoi de l’URL à votre client pour fournir directement ces informations). Une fois les informations nécessaires fournies, le serveur de publication procède à l’approvisionnement et à l’attribution des licences appropriées. La facturation de l’abonnement commence uniquement une fois que les licences ont été attribuées avec succès.

## <a name="access-billing-info-for-marketplace-products"></a>Accéder aux informations de facturation des produits de la place de marché

Pour les produits de la place de marché, la période de facturation commence le premier jour du mois civil et se termine le dernier jour du mois civil. Nous rendons votre facture disponible le huitième jour du mois suivant. Vous pouvez accéder à ces factures dans l’espace partenaires ou à l’aide des API de l’espace partenaires.

Pour plus d’informations, consultez [comprendre les types de facturation dans l’espace partenaires](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fournir un support aux clients qui utilisent des produits de la place de marché

Tout comme pour les produits Microsoft, vous devez être le premier point de contact pour votre client pour des questions sur la facturation et la gestion des abonnements. Pour le support technique, vous devez contacter le serveur de publication. Microsoft n’assure pas la prise en charge des produits de la place de marché, mais vous fournit les informations de contact du support technique de l’éditeur.

Pour plus d’informations, consultez [prise en charge des produits de la place de marché Azure](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) et [prise en charge de vos clients](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gérer les abonnements à l’aide des API de l’espace partenaires

Vous pouvez créer un abonnement pour les produits de la place de marché Azure à l’aide des API de l’espace partenaires en obtenant une liste d’offres pour un marché, en créant et en soumettant une commande pour un abonnement à la place de marché Azure, puis en récupérant un lien d’activation. Vous pouvez également utiliser les API de l’espace partenaires pour effectuer la gestion du cycle de vie et gérer les factures pour ces abonnements.

Pour plus d’informations, consultez [créer un abonnement pour les produits de la place de marché Azure](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).