---
title: Intégrations des partenaires à la Place de marché Azure
description: Découvrez les solutions de la place de marché Azure qui s’intègrent à votre environnement Azure et obtenez un lien vers les guides de déploiement auprès des partenaires Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006903"
---
# <a name="azure-marketplace-partner-integrations"></a>Intégrations des partenaires à la Place de marché Azure

Découvrez comment intégrer des solutions de partenaires dans votre environnement Azure. Cet article donne une vue d’ensemble de chaque solution et des liens vers des guides de déploiement détaillés. Les solutions sont répertoriées par ordre alphabétique. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka sur le Cloud confluent

![Confluent Cloud](./media/partners/confluent-cloud.png)

Azure vous permet d’intégrer le Cloud confluent en plus de vos applications Cloud. Les clients confluents naviguent souvent entre le Portail Azure et le Cloud confluent. Par exemple, une fois qu’un utilisateur achète une offre Cloud confluente dans la place de marché Azure, il est censé configurer un compte avec le Cloud confluent. Ce processus ajoute de la complexité et du temps, et exige que les utilisateurs gèrent la configuration et les ressources entre les deux portails. Pour réduire la charge de gestion sur les plateformes, Microsoft, en partenariat avec le Cloud confluent, a créé une couche d’approvisionnement intégrée d’Azure vers le Cloud confluent. La solution est disponible dans la place de marché Azure et offre une expérience transparente pour l’utilisation de l’offre Cloud confluent sur Azure

La solution utilise un fournisseur de ressources activé dans Azure pour approvisionner des ressources cloud confluentes. Cela permet aux utilisateurs d’accéder à la diffusion d’événements en temps réel via les kits de développement logiciel (SDK) Portail Azure, Azure CLI et Azure. Le Cloud confluent possède et exécute l’application SaaS, qui comprend des environnements, des clusters, des rubriques, des clés API et des connecteurs gérés.

L’intégration profonde avec le Cloud confluent offre les fonctionnalités suivantes :

- Approvisionnez une nouvelle ressource d’organisation Cloud confluente à partir de l’Portail Azure avec une infrastructure entièrement gérée.
- Rationalisation de l’authentification unique à partir d’Azure pour confluent le Cloud avec Azure Active Directory ; aucune authentification distincte n’est nécessaire à partir du portail Cloud confluent.
- Bénéficiez d’une facturation unifiée des frais de consommation du Cloud à l’aide de la facturation d’abonnement Azure.
- Gérez les ressources cloud confluentes à partir de la Portail Azure et suivez-les dans la page **toutes les ressources** , à côté de vos ressources Azure.

[Guides de déploiement de Cloud confluent](https://docs.confluent.io/current/cloud/marketplace/index.html)

Pour les problèmes liés à la confluent sur Azure, accédez à [https://support.confluent.io](https://support.confluent.io) . Si vous êtes un utilisateur pour la première fois, réinitialisez votre mot de passe avant de vous connecter au portail de support technique confluent. Si vous n’avez pas de compte avec confluent, veuillez envoyer un e-mail à [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logo DataDog](./media/partners/datadog.png)

Datadog fournit des outils d’observation et de sécurité permettant aux utilisateurs Azure de comprendre l’intégrité et les performances de leurs applications dans des environnements hybrides et multiclouds. Mais pour configurer les intégrations nécessaires, il faut souvent naviguer entre le portail Azure et Datadog. Pour simplifier la configuration et la gestion des ressources sur les portails, Microsoft a travaillé avec Datadog pour créer une solution Datadog intégrée sur Azure. Disponible via la place de marché Azure, cette solution offre une expérience transparente aux clients Azure pour utiliser la solution de surveillance Cloud de Datadog.

Consultez la [documentation Azure Monitor](/azure/azure-monitor/platform/partners#datadog) pour en savoir plus sur cette solution et vous inscrire à la version préliminaire publique.

## <a name="next-steps"></a>Étapes suivantes

- [Boutique en ligne Azure Marketplace](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn : créer un compte Azure](/learn/modules/create-an-azure-account/)
