---
title: Vendre des abonnements à des produits de la Place de marché Azure | Espace partenaires
ms.topic: article
ms.date: 08/07/2019
description: Vous pouvez utiliser l’Espace partenaires pour vendre à vos clients des abonnements aux produits SaaS (Software as a Service) publiés sur la Place de marché Azure par des éditeurs de logiciels indépendants (ISV).
author: JnHs
ms.author: jenhayes
keywords: abonnements, Place de marché, tiers, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 204a0638399034c753474bb0ce92434ca318f5bb
ms.sourcegitcommit: ea68a16c2ed386cca983dd3fa85032450eacf871
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/09/2019
ms.locfileid: "68860946"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vendre des abonnements à des produits de la Place de marché Azure

**S’applique à**

- Espace partenaires

Vous pouvez utiliser l’Espace partenaires pour vendre à vos clients des abonnements aux produits SaaS (Software as a Service) publiés sur la [Place de marché Azure](https://azuremarketplace.microsoft.com/marketplace) par des éditeurs de logiciels indépendants (ISV). Cela peut vous aider à différencier votre entreprise et à fournir à vos clients des offres groupées de logiciels qui répondent à leurs besoins spécifiques. Vous gérez les licences et les abonnements pour ces produits SaaS de la Place de marché Azure de la même façon que pour les produits Microsoft.

Pour plus d’informations sur la Place de marché Azure, consultez le [Forum aux questions sur la Place de marché Azure](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Afficher les offres et les prix de la Place de marché

Pour afficher toutes les offres disponibles, sélectionnez **Place de marché** dans le menu de navigation de gauche. Par défaut, vous voyez des produits de tous types et catégories. Vous pouvez filtrer par type et/ou catégorie, ou utiliser la zone de recherche pour rechercher des mots clés spécifiques. Sélectionnez un produit pour afficher des informations sur l’éditeur et les références SKU disponibles, notamment pour savoir si une période d’essai gratuite est proposée.

> [!NOTE]
> Certains produits disponibles dans la Place de marché Azure peuvent ne pas être affichés ici. Les éditeurs de logiciels indépendants peuvent décider de proposer ou non leurs produits aux partenaires CSP (Fournisseur de solutions Cloud) dans l’Espace partenaires. Si vous voyez dans la Place de marché Azure un produit que vous souhaitez proposer à vos clients par le biais de l’Espace partenaires, recherchez les coordonnées de l’éditeur dans la Place de marché Azure et informez-le que vous êtes intéressé.

Les prix des produits de la Place de marché Azure peuvent changer fréquemment. Pour obtenir des informations à jour sur les tarifs de tous les produits de la Place de marché, sélectionnez **Exporter la liste des prix** dans le coin supérieur droit de la page **Place de marché**. Une feuille de calcul contenant toutes les données sur les tarifs est alors générée. Les informations sur les tarifs étant mises à jour quotidiennement, vous pouvez les consulter aussi souvent que vous le souhaitez pour obtenir des tarifs à jour.

> [!TIP]
> Si un produit de cette liste comporte un essai gratuit, la feuille de calcul comprend deux lignes pour ce produit. L’une des lignes affiche un prix égal à zéro, indiquant qu’un essai gratuit est disponible. L’autre ligne inclut le prix et la durée qui s’appliquent une fois la période d’essai terminée.
>
> Si un produit de cette liste utilise la [facturation limitée](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing), le champ de la durée est vide.

## <a name="purchase-marketplace-products-for-your-customers"></a>Acheter des produits de la Place de marché pour vos clients

L’achat d’abonnements pour les produits SaaS de la Place de marché Azure suit le même processus que l’achat d’abonnements pour les produits Microsoft. Quand vous ajoutez un abonnement pour un client, vous pouvez choisir de voir uniquement les offres de la Place de marché proposées par les ISV en sélectionnant **Partenaire** dans le filtre **Éditeur**. Pour plus d’informations, consultez [Créer un abonnement](create-a-new-subscription.md).

> [!IMPORTANT]
> Vous pouvez uniquement acheter des abonnements de produits SaaS (Software as a Service) dans l’Espace partenaires. D’autres types d’offre (tels que les machines virtuelles, les conteneurs ou les applications Azure) sont gérés par le biais du portail Azure et facturés en fonction de leur consommation. Vous devez disposer d’un abonnement Azure pour activer les solutions avec paiement à l’utilisation via le Portail Azure.

Notez que certaines offres que vous voyez sur la page **Place de marché** peuvent ne pas être disponibles pour un client spécifique. La disponibilité peut être impactée par un certain nombre de facteurs, notamment la prise en charge ou non par l’ISV du pays ou de la région de facturation du client.

> [!TIP]
> Vous pouvez également utiliser [les API de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/) pour créer des abonnements de la Place de marché Azure pour vos clients. Pour plus d’informations, consultez [Créer un abonnement pour des produits de la place de marché Azure](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Dans le cadre des abonnements à des produits de la Place de marché Azure, vous avez la possibilité d’[annuler un abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) au cours de la période d’annulation (24 heures pour les abonnements mensuels ou 14 jours pour les abonnements annuels). Vous pouvez également [choisir de renouveler ou non automatiquement l’abonnement](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-marketplace-products"></a>Activation des licences pour les produits de la Place de marché

Pour les types d’offre SaaS (Software as a Service), l’attribution et l’activation de licences sont gérées par l’éditeur de logiciels indépendant (ISV) qui a publié le produit. Pour effectuer ce processus, vous devez visiter le site de l’éditeur, à l’aide d’un lien personnalisé contenant un code d’autorisation qui permet à l’éditeur d’identifier votre achat spécifique. Vous pouvez trouver ce lien dans la page de confirmation qui s’affiche une fois que vous avez acheté une offre SaaS et dans la page **Abonnements** (dans la ligne relative à cette offre). Vous pouvez également [utiliser les API de l’Espace partenaires pour récupérer ce lien](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Quand vous accédez au site de l’éditeur à l’aide de ce lien, vous voyez les informations ou action supplémentaires nécessaires pour provisionner et attribuer les licences, ou pour terminer le processus d’installation. Les étapes requises peuvent varier en fonction de l’éditeur et de l’offre. Vous êtes responsable de l’envoi des informations nécessaires (ou de l’envoi de l’URL à votre client pour qu’il fournisse ces informations directement). Une fois les informations nécessaires fournies, l’éditeur procède au provisionnement et à l’attribution des licences appropriées. La facturation de l’abonnement commence uniquement une fois que les licences ont été attribuées avec succès.

## <a name="access-billing-info-for-marketplace-products"></a>Accéder aux informations de facturation des produits de la Place de marché

Pour les produits de la Place de marché, la période de facturation commence le premier jour du mois civil et se termine le dernier jour du mois civil. Votre facture est disponible le huitième jour du mois suivant. Vous pouvez accéder à ces factures dans l’Espace partenaires ou à l’aide des API de l’Espace partenaires.

Pour plus d’informations, consultez [Présentation des types de facturation dans l’Espace partenaires](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fournir un support aux clients qui utilisent des produits de la Place de marché

Tout comme pour les produits Microsoft, vous devez être le premier point de contact pour votre client en ce qui concerne la facturation et la gestion de l’abonnement. Pour un support technique, vous devez contacter l’éditeur. Microsoft n’assure pas de support pour les produits de la Place de marché, mais vous fournit les informations de contact du support technique de l’éditeur.

Pour plus d’informations, consultez [Support des produits de la place de marché Azure](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) et [Fourniture d’un support à vos clients](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gérer les abonnements à l’aide des API de l’Espace partenaires

Vous pouvez créer un abonnement pour des produits de la place de marché Azure à l’aide des API de l’Espace partenaires en obtenant une liste d’offres pour un marché, en créant et en soumettant une commande pour un abonnement à la Place de marché Azure, puis en récupérant un lien d’activation. Vous pouvez également utiliser les API de l’Espace partenaires afin d’effectuer la gestion du cycle de vie et de gérer les factures pour ces abonnements.

Pour plus d’informations, consultez [Créer un abonnement pour des produits de la place de marché Azure](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).