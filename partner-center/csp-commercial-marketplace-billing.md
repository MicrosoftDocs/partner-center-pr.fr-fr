---
title: Facturation pour les produits de la place de marché commercial | Espace partenaires
ms.topic: article
ms.date: 02/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment la facturation fonctionne pour les produits ou abonnements SaaS ISV achetés pour les clients à partir de la place de marché commerciale dans l’espace partenaires.
author: MicheleHope
ms.author: v-mihope
keywords: abonnements, produits, achats, Marketplace, tiers, ISV, facturation, factures, rapprochement, fichier de rapprochement
ms.localizationpriority: medium
ms.openlocfilehash: 35db6e9e1fbdfe5e455e5b4e73e39b76cad496aa
ms.sourcegitcommit: 717ef04f5c0040611af3ba9e5a324ab67e99ba14
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2020
ms.locfileid: "78240196"
---
# <a name="billing-for-commercial-marketplace-products"></a>Facturation pour les produits de la place de marché commercial

**S’applique à**

- Centre pour partenaires
- Partenaires du programme Fournisseur de solutions Microsoft Cloud

**Rôles appropriés**

- Administrateur global
- Administration de facturation

En tant que partenaire dans le programme CSP, vous pouvez utiliser l’espace partenaires pour acheter des produits SaaS basés sur une licence auprès d’éditeurs ISV dans le Marketplace commercial. Après cela, vous pouvez accéder à une facture pour ces types d’achats. La période de facturation commence le premier jour du mois civil et se termine le dernier jour du mois civil. Les factures sont rendues disponibles le huitième jour du mois suivant.

Vous pouvez accéder aux factures depuis le [tableau de bord](https://partner.microsoft.com/dashboard/) de l’espace partenaires ou à l’aide des API de l' [espace partenaires](https://docs.microsoft.com/partner-center/develop/).

Les partenaires du programme CSP sont facturés pour les solutions de la place de marché commercial ISV achetées pour un client lors de l’achat de ces produits à partir de l’espace partenaires ou du Portail Azure (à l’aide du locataire Azure du client précédent acheté).

>[!NOTE]
>Si les clients utilisent leur propre Azure AD locataire (non acheté par un partenaire dans le programme CSP), les clients peuvent également choisir d’acheter leur propre solution SaaS ISV directement à partir de ([Microsoft AppSource](https://appsource.microsoft.com/) ou place de [marché Azure](https://azuremarketplace.microsoft.com/)). S’ils le font, ils recevront leur propre facture directement de la part de Microsoft. De même, si un partenaire du programme CSP vend un abonnement Azure ou le nouveau plan Azure au client et accorde à ce locataire l' [accès en fonction du rôle](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) de client (ou de revendeur indirect) (en attribuant un rôle au client en plus du **lecteur**), ce client (ou revendeur indirect) peut également acheter des offres de la place de marché commercial sans l’approbation préalable ou la notification au partenaire Dans ce cas, Microsoft ne notifie pas directement les partenaires du programme CSP aux achats effectués par leurs clients. Toutefois, Microsoft propose un mécanisme de [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) facultatif que vous pouvez utiliser pour définir des alertes ou des notifications sur l’activité d’un abonnement Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Accéder aux informations de facturation pour les produits de la place de marché commercial

L’administrateur général ou l’administrateur de facturation de votre entreprise reçoit un e-mail dès qu’une facture est consultable. Pour accéder aux derniers fichiers de facture et de rapprochement pour les achats de produits de la place de marché commercial :

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/) de l’Espace partenaires.

2. Dans le menu de l’Espace partenaires, sélectionnez **Facturation**. 

    Vous verrez deux onglets en haut de la page facturation : les achats **périodiques** et **périodiques et les achats ponctuels**. Chaque onglet vous permet d’accéder aux fichiers de facture et de rapprochement (rapprochement) des différents produits de la place de marché :

    - Onglet **périodique** : affiche les fichiers de facturation et de rapprochement des abonnements associés à Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro et Microsoft Azure.

    - Onglet **achats récurrents et ponctuels** : affiche les fichiers de facturation et de rapprochement pour le plan Azure, les réservations Azure, les logiciels et les produits de la place de marché commercial.
  
3. Sélectionnez l’onglet **achats récurrents et ponctuels** . Si vous avez acheté des abonnements pour un client dans une devise différente, vous verrez un onglet pour chaque devise. Vous pouvez effectuer quelques opérations fr : OM de cette page :

    - Pour afficher le dernier fichier de facture et de rapprochement, sélectionnez **facture** ou **fichier de réconciliation**. (Si vous le souhaitez, vous pouvez également accéder à la dernière facture et rapprocher les données du fichier à l’aide des API de l' [espace partenaires](https://docs.microsoft.com/partner-center/develop/).

    - Pour afficher les factures et les fichiers de rapprochement antérieurs, développez la ligne de l' **historique de facturation** ci-dessous.

    - Pour vérifier le solde de votre compte ou votre facture à tout moment en fonction de l’activité de compte la plus récente, sélectionnez un lien sous le titre **estimations** .  

    >[!NOTE]
    > Lorsque nous publions votre facture le 8 du mois, les taxes et les crédits applicables seront inclus. Cela signifie que le montant final dû peut différer de ce que vous voyez au cours de la période de facturation.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>En savoir plus sur les factures et les fichiers de rapprochement pour les produits de la place de marché commercial

Cette section fournit plus d’informations sur les fichiers de facture et de rapprochement pour les abonnements SaaS de la place de marché commercial achetés pour les clients auprès d’éditeurs ISV tiers.

Lorsque vous sélectionnez des **achats récurrents et ponctuels** à partir de l’option **facturation** dans le menu de l’espace partenaires, vous accédez aux factures et aux fichiers de rapprochement pour les frais liés aux achats Microsoft (premier tiers) et ISV (tiers). Ces achats peuvent être associés à :

- Abonnements SaaS (à partir des éditeurs Microsoft ou ISV)

- plan Azure

- Réservations Azure

- Autres logiciels basés sur un abonnement (de Microsoft ou des éditeurs ISV)

Des exemples de ces achats peuvent inclure le logiciel SUSE Linux (abonnement logiciel) ou un abonnement à un produit Azure ISV SaaS.

>[!NOTE]
> Pour plus d’informations sur la lecture des factures et des fichiers de rapprochement, voir aussi [vue d’ensemble](billing.md)de la facturation.

### <a name="tips-on-reading-your-invoice"></a>Conseils sur la lecture de votre facture

Lorsque vous achetez un produit SaaS basé sur une licence auprès d’un éditeur ISV tiers, vous verrez uniquement les frais liés aux frais de licence sur votre facture. Cela est vrai même lorsque le produit SaaS de l’ISV utilise (ou consomme) des ressources d’infrastructure Azure sous-jacentes. Cela est dû au fait que les frais d’utilisation de l’infrastructure Azure de votre client pour le produit SaaS d’un ISV sont facturés directement à l’ISV. (Les fournisseurs de logiciels indépendants verront les frais de consommation Azure associés dans leur propre fichier de rapprochement des factures de l’utilisation d’Azure.)

Votre facture contiendra plusieurs pages :

- **Page 1 de la facture :** Contient une vue d’ensemble du résumé des détails de facturation du partenaire du programme CSP. Cela comprend un résumé des frais pour la période de facturation, un numéro de facture, des conditions de paiement (net 60 jours) et des modes de paiement de facturation pour payer par câble ou par chèque.

- **Page 2 (et toutes les pages suivantes) de la facture :** Détails des frais liés aux achats Microsoft internes et aux achats tiers (basés sur des licences) à partir de la place de marché commerciale. Vous pouvez identifier les achats basés sur des licences ISV par la ligne **éditeur** sous chaque nom de produit. Le fichier de rapprochement associé offre plus de détails sur la facturation des frais de facture spécifiques.

- **Dernière page de la facture :** Si vous avez été facturé pour des produits Marketplace basés sur des licences à partir d’un éditeur de logiciels, cette dernière page affiche plus de détails sur le nom et l’adresse de l’éditeur ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Conseils sur la lecture de votre fichier de réconciliation

Le fichier de réconciliation **des achats périodique et ponctuel** contient plusieurs colonnes avec des détails supplémentaires qui correspondent aux frais de votre facture. La colonne **PublisherName** indique si l’achat provient de Microsoft ou d’un éditeur ISV tiers.

Certains frais dans votre fichier de rapprochement peuvent s’afficher avec un coût de $0. Cela peut être dû à une offre « essai gratuit » ISV (en général 30 ou 60 jours) ou à une offre de licence.

Dans le cas d’une version d’évaluation gratuite, les éditeurs de logiciels indépendants :

- La période d’évaluation gratuite couvre le coût du produit SaaS basé sur une licence de l’ISV pendant ce laps de temps. Vous ne serez pas non plus facturé pour l’utilisation de l’infrastructure Azure associée à ce produit SaaS.  Toutefois, si vous utilisez une offre ISV basée sur l’utilisation, la version d’évaluation gratuite n’inclut pas le coût de l’utilisation de l’infrastructure Azure sous-jacente. Dans ce cas, les frais d’utilisation de l’infrastructure Azure s’affichent dans un fichier de rapprochement Azure distinct.

- Lorsque vous achetez et déployez le produit gratuit d’évaluation d’un ISV pour votre client, le client est automatiquement inscrit dans la version d’évaluation gratuite de l’éditeur ISV. La période d’évaluation gratuite se termine automatiquement après la période définie par l’éditeur ISV. Une fois la période terminée, le client est facturé. Cela signifie que le fichier de rapprochement peut afficher deux lignes pour un produit éligible à l’évaluation : un qui effectue le suivi de la période d’évaluation et un pour le suivi de l’offre payante (qui affiche un coût de $0 jusqu’à la fin de la période d’évaluation). Une fois l’évaluation terminée, la ligne affichant l’offre payante commence à afficher les frais. 

Pour plus d’informations sur ce que représente chaque colonne, consultez [utiliser vos fichiers de réconciliation](use-the-reconciliation-files.md). Voir aussi [types de facturation dans l’espace partenaires](billing-different-types.md)

## <a name="next-steps"></a>Étapes suivantes

- [Gérer les produits de la place de marché commercial pour les clients](csp-commercial-marketplace-manage.md)
- [En savoir plus sur la prise en charge des produits de la place de marché commerciale](csp-commercial-marketplace-support.md)
