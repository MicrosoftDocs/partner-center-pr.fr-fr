---
title: Achat de logiciels et de solutions à partir de la place de marché Azure
description: En savoir plus sur les outils qui simplifient et rationalisent l’achat et la gestion de logiciels dans la place de marché Azure.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431543"
---
# <a name="azure-marketplace-purchasing"></a>Achat sur la place de marché Azure

La place de marché Azure offre de nombreux outils et fonctionnalités qui simplifient et rationalisent le processus d’achat, de facturation et de gestion de la stratégie d’achat.

## <a name="simplified-procurement"></a>Approvisionnement simplifié

La Place de marché Azure vous permet de simplifier le processus d’approvisionnement par le biais de différentes options d’achat. Si vous achetez des produits à l’aide d’une carte de crédit associée à votre compte Azure, tous les achats sont consolidés sur une facture unique et facturés sur la carte de crédit de votre choix. Si vous êtes un grand client, vous pouvez acheter à l’aide d’un Contrat Entreprise. Avec un contrat entreprise, les achats de logiciels sont automatiquement inclus dans votre facture Azure. Votre facture indique d’abord les frais d’utilisation d’Azure, suivis des frais de Place de marché Azure.

Lorsque vous achetez via la place de marché Azure, vous éliminez la complexité de la gestion des relations et des factures des fournisseurs individuels. Vous bénéficiez d’une facture mensuelle unique et consolidée de Microsoft qui comprend vos achats sur la place de marché Azure et vos frais Azure.

## <a name="permission-to-purchase"></a>Autorisation d’achat

Une fois que vous avez trouvé l’application logicielle appropriée, l’exécution de l’achat est simple. Toutefois, vous aurez besoin d’autorisations appropriées au sein de l’abonnement Azure. Étant donné qu’Azure fonctionne sur un modèle de [Access Control basé](/azure/role-based-access-control/overview) sur les rôles (RBAC), votre compte a besoin d’autorisations de propriétaire ou de **contributeur** d' **abonnement** pour effectuer un achat.

Avant d’effectuer un achat, assurez-vous que l’utilisateur dispose de la configuration appropriée dans le locataire Azure. Cela permet d’éviter les erreurs lors de l’achat.

Dans l’expérience de la place de marché Azure dans le Portail Azure, recherchez l’application que vous souhaitez acheter, puis sélectionnez **créer** ou **configurer + abonnement**. Vous serez invité à compléter certaines informations avant de pouvoir utiliser votre nouvelle solution.

> [!CAUTION]
> L’approbation sur la place de marché privée n’indique pas l’approvisionnement d’une solution.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Bouton de création de l’offre.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="Bouton configurer + s’abonner.":::

Si vous souhaitez déployer une solution à partir du magasin en ligne de la place de marché Azure, sélectionnez **obtenir maintenant** sur la page Description du produit, puis connectez-vous avec vos informations d’identification de compte Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="La boîte de dialogue Connexion à la place de marché Azure.":::

Une fois que vous êtes connecté, vous êtes redirigé vers le produit dans le Portail Azure pour finaliser votre achat.

## <a name="purchase-policy-management"></a>Gestion des stratégies d’achat

Microsoft vous permet de gérer les achats des utilisateurs via votre profil de facturation en tant qu’administrateur d’abonnements Azure. Choisissez parmi les trois options suivantes :

- **Gratuit + payant** : permet aux utilisateurs d’acquérir n’importe quelle application logicielle de la place de marché Azure.
- **Gratuit** : permet aux utilisateurs de déployer uniquement des logiciels gratuits à partir de la place de marché Azure.
- **Non** – empêche les utilisateurs de déployer des logiciels à partir de la place de marché Azure.

Ces paramètres s’appliquent à tous les utilisateurs ayant accès à votre abonnement Azure, ce qui vous donne la possibilité de contrôler l’approvisionnement informatique via l’Portail Azure.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Contrôle de l’approvisionnement informatique via l’Portail Azure.":::

## <a name="cost-management"></a>la gestion des coûts ;

Lorsque vous achetez des produits sur la place de marché Azure, vous souhaitez obtenir des informations qui vous aideront à gérer les coûts. Azure Cost Management est un outil gratuit permettant d’afficher des informations sur les produits que vous avez achetés. Vous pouvez utiliser Cost Management pour afficher des détails sur les services que vous consacrez au fil du temps et sur la façon dont ces coûts sont suivis par rapport aux budgets que vous avez définis. Outre la définition des budgets, vous pouvez planifier des rapports et analyser les coûts liés aux abonnements. En savoir plus sur les Azure Cost Management en complétant le module Microsoft Learn sur [analyser les coûts et créer des budgets avec Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Vous pouvez voir vos frais et factures de la Place de marché Azure dans l’outil d’analyse des coûts sous Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Utilisez Azure Cost Management pour obtenir des informations sur vos produits achetés.":::

## <a name="purchase-validation-checks"></a>Vérifications de validation des achats

L’achat d’une offre via la place de marché Azure peut échouer pour différentes raisons. L’utilisation de l’interface de ligne de commande (CLI) pour un achat est plus susceptible de provoquer des erreurs, car vous essayez peut-être d’acheter une offre qui n’est pas disponible ou visible dans la place de marché Azure. Voici les vérifications pouvant entraîner l’échec d’un achat :

1. L’abonnement appartient à un Contrat Entreprise (EA) et l’administrateur EA a désactivé la place de marché Azure.
1. L’administrateur EA a activé des achats uniquement pour les offres gratuites et l’offre est une offre payante.
1. L’offre est introuvable sur la place de marché.
1. L’éditeur de logiciels indépendant (ISV) a cessé de vendre l’offre au moins dans votre région.
1. L’abonnement que vous utilisez appartient à un compte de facturation dans une région où l’offre n’est pas disponible.
1. Le compte d’abonnement/de facturation n’est pas associé à un moyen de paiement valide (par exemple, une carte de crédit valide).
1. L’abonnement appartient à un fournisseur de solutions Cloud (CSP) et l’ISV a refusé de vendre via un CSP.
1. La place de marché privée est activée pour l’abonnement et l’offre ne figure pas dans la liste des offres autorisées.
1. L’offre est privée/préliminaire pour des clients spécifiques et l’abonnement ne figure pas dans la liste des clients autorisés.

## <a name="next-steps"></a>Étapes suivantes

- [Facturation](billing-invoicing.md)