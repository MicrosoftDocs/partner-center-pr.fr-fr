---
title: Vendre des abonnements à des produits de la place de marché commerciale | Espace partenaires
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vous pouvez utiliser l’Espace partenaires pour vendre à vos clients des abonnements aux produits SaaS (Software as a Service) publiés sur la place de marché commerciale par des éditeurs de logiciels indépendants (ISV).
author: JnHs
ms.author: jenhayes
keywords: abonnements, Place de marché, tiers, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651637"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>Vendre des abonnements à des produits de la place de marché commerciale

**S’applique à**

- Espace partenaires

Vous pouvez utiliser l’Espace partenaires pour vendre à vos clients des abonnements aux produits SaaS (Software as a Service) publiés sur la place de marché commerciale ([Microsoft AppSource](https://appsource.microsoft.com/) et [Place de marché Azure](https://azuremarketplace.microsoft.com/)) par des éditeurs de logiciels indépendants (ISV). Cela peut vous aider à différencier votre entreprise et à fournir à vos clients des offres groupées de logiciels qui répondent à leurs besoins spécifiques. Vous gérez les licences et les abonnements pour ces produits SaaS de la Place de marché de la même façon que pour les produits Microsoft.

Pour plus d’informations sur la place de marché commerciale, consultez [FAQ sur la Place de marché](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

> [!IMPORTANT]
> Seuls des abonnements à la place de marché commerciale SaaS (Software as a Service) peuvent être achetés dans l’Espace partenaires. D’autres types d’offre de la place de marché commerciale (comme les machines virtuelles, les conteneurs ou les applications Azure) sont gérés par le biais du portail Azure et facturés en fonction de leur consommation. Vous devez disposer d’un abonnement Azure pour activer les solutions avec paiement à l’utilisation via le Portail Azure.

## <a name="view-marketplace-offers-and-pricing"></a>Afficher les offres et les prix de la Place de marché

Pour afficher toutes les offres disponibles de la place de marché commerciale, sélectionnez **Place de marché** dans le menu de navigation de gauche. Par défaut, vous verrez des produits de tous types et catégories. Vous pouvez filtrer par type et/ou catégorie, ou utiliser la zone de recherche pour rechercher des mots clés spécifiques. Sélectionnez un produit pour afficher des informations sur l’éditeur et les références SKU disponibles, notamment pour savoir si une période d’essai gratuite est proposée.

> [!NOTE]
> Certains produits disponibles dans la place de marché commerciale peuvent ne pas être affichés ici. Les éditeurs de logiciels indépendants peuvent décider de proposer ou non leurs produits aux partenaires CSP (Fournisseur de solutions Cloud) dans l’Espace partenaires. Si vous voyez un produit de la place de marché commercial que vous souhaitez proposer à vos clients via l’espace partenaires, recherchez les coordonnées du serveur de publication dans la liste des produits et indiquez-leur que vous êtes intéressé.

Les prix des produits de la place de marché commerciale peuvent changer fréquemment. Pour obtenir des informations à jour sur les tarifs de tous les produits de la place de marché commerciale, sélectionnez **Exporter la liste des prix** dans le coin supérieur droit de la page **Place de marché**. Une feuille de calcul contenant toutes les données sur les tarifs est alors générée. Ces informations sur les tarifs étant mises à jour quotidiennement, vous pouvez les consulter aussi souvent que vous le souhaitez pour obtenir des tarifs à jour.

> [!TIP]
> Si un produit de cette liste comporte un essai gratuit, la feuille de calcul comprend deux lignes pour ce produit. L’une des lignes affiche un prix égal à zéro, indiquant qu’un essai gratuit est disponible. L’autre ligne inclut le prix et la durée qui s’appliquent une fois la période d’essai terminée.
>
> Si un produit de cette liste utilise la [facturation limitée](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing), le champ de la durée est vide.

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>Acheter des produits de la place de marché commerciale pour vos clients

L’achat d’abonnements pour les produits SaaS de la place de marché commerciale suit le même processus que l’achat d’abonnements pour les produits Microsoft. Vous devez sélectionner un client ou ajouter un nouveau client avant d’acheter un abonnement.

Quand vous ajoutez un abonnement pour un client, vous pouvez choisir de voir uniquement les offres de la Place de marché proposées par les ISV en sélectionnant **Partenaire** dans le filtre **Éditeur**. Pour plus d’informations, consultez [Créer un abonnement](create-a-new-subscription.md).

Notez que certaines offres que vous voyez sur la page **Place de marché** peuvent ne pas être disponibles pour un client spécifique. La disponibilité peut être affectée par un certain nombre de facteurs, notamment si l’ISV prend en charge le pays/la région de facturation du client.

> [!TIP]
> Vous pouvez également utiliser les [API de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/) pour créer des abonnements de la place de marché commerciale pour vos clients. Pour plus d’informations, consultez [Créer un abonnement pour des produits de la place de marché commerciale](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Dans le cadre des abonnements à des produits de la place de marché commerciale, vous avez la possibilité [d’annuler un abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) au cours de la période d’annulation (24 heures pour les abonnements mensuels ou 14 jours pour les abonnements annuels). Vous pouvez également [choisir de renouveler ou non automatiquement l’abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-commercial-marketplace-products"></a>Activation des licences pour les produits de la place de marché commerciale

Pour les types d’offre SaaS (Software as a Service), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit. Pour effectuer ce processus, vous devez visiter le site de l’éditeur, à l’aide d’un lien personnalisé avec un code d’autorisation qui permet à l’éditeur d’identifier votre achat spécifique. Vous pouvez trouver ce lien dans la page de confirmation qui s’affiche une fois que vous avez acheté une offre SaaS et dans la page **Abonnements** (dans la ligne relative à cette offre). Vous pouvez également [utiliser les API de l’Espace partenaires pour récupérer ce lien](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Lorsque vous accédez au site de l’éditeur à l’aide de ce lien, vous verrez les informations ou actions supplémentaires nécessaires pour approvisionner et attribuer des licences, ou pour terminer le processus d’installation. Les étapes requises peuvent varier en fonction de l’éditeur et de l’offre. Vous êtes responsable de l’envoi des informations nécessaires (ou de l’envoi de l’URL à votre client pour qu’il fournisse ces informations directement). Une fois les informations nécessaires fournies, l’éditeur procède au provisionnement et à l’attribution des licences appropriées. La facturation de l’abonnement commence uniquement une fois que les licences ont été attribuées avec succès.

## <a name="access-billing-info-for-commercial-marketplace-products"></a>Accéder aux informations de facturation pour les produits de la place de marché commerciale

Pour les produits de la place de marché commerciale, la période de facturation commence le premier jour du mois civil et se termine le dernier jour du mois civil. Nous rendons votre facture disponible le huitième jour du mois suivant. Vous pouvez accéder à ces factures dans l’Espace partenaires ou à l’aide des API de l’Espace partenaires.

Pour plus d’informations, consultez [Présentation des types de facturation dans l’Espace partenaires](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>Fournir un support aux clients qui utilisent des produits de la place de marché commerciale

Tout comme pour les produits Microsoft, vous devez être le premier point de contact pour votre client en ce qui concerne la facturation et la gestion de l’abonnement. Pour un support technique, vous devez contacter l’éditeur. Microsoft n’assure pas la prise en charge des produits de la place de marché commerciaux, mais vous fournit les informations de contact du support technique de l’éditeur.

Pour plus d’informations, consultez [Support des produits de la place de marché commerciale](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products) et [Fournir un support à vos clients](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gérer les abonnements à l’aide des API de l’Espace partenaires

Vous pouvez créer un abonnement pour des produits de la place de marché commerciale à l’aide des API de l’Espace partenaires. Pour ce faire, vous devez d’abord obtenir une liste des offres pour un marché, puis créer et envoyer une commande pour un abonnement de la place de marché commerciale spécifique. Enfin, vous récupérez un lien d’activation pour l’abonnement.

Vous pouvez également utiliser les API de l’Espace partenaires afin d’effectuer la gestion du cycle de vie et de gérer les factures pour ces abonnements.

Pour plus d’informations, consultez [Créer un abonnement pour des produits de la place de marché commerciale](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).