---
title: Affecter des abonnements Azure à des clients
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment affecter des abonnements Azure à vos clients dans l’espace partenaires et comment permettre aux clients de gérer leurs propres abonnements.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aba4f97ad6a385c2a9e36c95354a9d53e38ba9e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149976"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a>Affectation d’abonnements Azure à des clients dans l’Espace partenaires

**Rôles appropriés**: administrateur général | Agent des ventes

## <a name="assign-azure-subscriptions-to-your-customers"></a>Affecter des abonnements Azure à vos clients

1. Sélectionnez **clients** dans le menu de l' **espace partenaires** et recherchez le client que vous souhaitez gérer.

2. Sélectionnez la flèche vers le bas à la fin de la ligne pour développer l’enregistrement du client, puis sélectionnez **portail de gestion Microsoft Azure**. Vous serez redirigé vers le [portail Azure](https://portal.azure.com/) dans lequel vous pouvez gérer les abonnements du client.

3. Dans le Portail Azure, sélectionnez **abonnements**.

4. Sélectionnez l’abonnement que vous souhaitez affecter, puis sélectionnez **Access Control**.

5. Sélectionnez **Ajouter** pour ajouter un utilisateur à l’abonnement. 

6. Après avoir ajouté l’utilisateur à l’abonnement, vous pouvez attribuer à l’utilisateur un rôle et le compte spécifique auquel l’utilisateur aura accès.

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a>Autoriser les clients à gérer leurs abonnements Windows Azure

Après avoir créé un abonnement Microsoft Azure pour un client, vous pouvez lui permettre de gérer son abonnement. Pour ce faire, vous devez vous connecter au portail de gestion Microsoft Azure du client. 

1. Pour ouvrir le Portail Azure du client, développez la liste des clients dans votre liste de clients ou sélectionnez le nom du client, puis sélectionnez **portail de gestion Microsoft Azure**.

   > [!NOTE]  
   > Si vous êtes invité à vous connecter au Portail Azure, vous ne disposez peut-être pas de privilèges d’administrateur délégués. Sélectionnez **Demander une relation** pour inviter le client à vous identifier comme son partenaire de référence. Une fois que le client a accepté votre invitation, vous vous voyez automatiquement attribuer des privilèges d'administration délégués.

2. Dans la Portail Azure, ouvrez la liste abonnements du client et sélectionnez l’abonnement Azure du client.

3. Attribuez un rôle à l’un des utilisateurs du client afin qu’il puisse créer et gérer des ressources dans le cadre de son abonnement.

## <a name="next-steps"></a>Étapes suivantes

- [Comment les partenaires CSP peuvent vendre des abonnements aux clients](customer-subscriptions.md)

- [Comment obtenir des autorisations pour gérer le service ou les abonnements d’un client](customers-revoke-admin-privileges.md)
