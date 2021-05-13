---
title: Demander une relation avec un client
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Demandez une relation avec un client pour les scénarios multi-partenaires multicanaux ou si vos privilèges d’administrateur délégué pour un client doivent être restaurés.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: f8265973157540cff698790ddb2effa912abeeb7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856115"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Guide pratique pour demander une relation de revendeur à un client dans l’Espace partenaires

**Rôles appropriés**: agent admin | Administrateur général

Si vous souhaitez gérer le service ou l’abonnement d’un client en son nom, le client doit vous accorder des autorisations d’administrateur pour ce service ou cet abonnement et signer le contrat du client Microsoft.

Si vous souhaitez établir une relation de revendeur avec un client et gérer uniquement les abonnements Azure que vous approvisionnez, vous n’avez pas besoin d’obtenir des autorisations d’administrateur.

>[!NOTE] 
>L’option permettant de ne pas demander d’autorisations n’est pas disponible pour les partenaires qui fonctionnent dans Microsoft Cloud pour le gouvernement des États-Unis ou Microsoft Cloud Allemagne. Pour plus d’informations, consultez [clients déléguer des privilèges d’administration à des partenaires](customers-revoke-admin-privileges.md).

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Inviter un client à établir une relation de revendeur avec vous

Vous pouvez demander une relation de revendeur avec un client dans votre pays ou dans la même région.

1. Sélectionnez **Clients** à partir de votre menu **Espace partenaires**, puis sélectionnez **Demander une relation de revendeur**.

2. Pour demander des autorisations d’administrateur à ce client, sélectionnez **inclure des privilèges d’administration déléguée pour Azure Active Directory et Office 365**. Pour établir la relation sans demander d’autorisations d’administrateur, désactivez cette option.

3. Dans la page suivante, passez en revue le brouillon de message électronique. Vous pouvez ouvrir le brouillon de message dans votre application de messagerie par défaut, ou vous pouvez copier le message dans le Presse-papiers et le coller dans un e-mail.

   Vous pouvez modifier le texte de l’e-mail, mais veillez à inclure le lien car il s’agit d’un lien personnalisé qui permet d’associer le client directement à votre compte. Sélectionnez **Terminé** une fois que vous avez effectué cette étape.

4. Envoyez l’e-mail au client.

5. Une fois que le client a accepté votre invitation, il apparaît sur la page de vos **clients** et peut approvisionner et gérer le service pour le client à partir de là.

   > [!NOTE]
   > Si le client n’a pas encore accepté le contrat du client Microsoft, il est invité à le faire lorsqu’il accepte votre invitation. Le client doit être un administrateur général pour accepter l’invitation.

6. Pour gérer le compte, les services, les utilisateurs et les licences du client, développez la fiche du client en sélectionnant la flèche vers le bas située à côté de son nom.

> [!IMPORTANT]  
> Les clients peuvent réattribuer ou supprimer des autorisations d’administrateur sur le portail d’administration d’un service. Toutefois, sauf si et jusqu’à ce que vous renégociiez votre accord avec le client, vous êtes toujours responsable de la fourniture du support client et du respect des conditions de l’accord de partenariat Microsoft, même si un client réaffecte ou supprime des autorisations d’administrateur. Dans ce cas, si le client a besoin d’aide, vous pouvez contacter le support Microsoft pour ouvrir une demande de service pour le compte du client.

## <a name="changes-to-the-customer-invitation-experience"></a>Modifications apportées à l’expérience d’invitation du client

L’expérience client pour l’acceptation d’une invitation de revendeur revendeur d’un partenaire de fournisseur de solutions Cloud est hébergée par différents portails côté client. L’emplacement du portail varie selon qu’un client se trouve dans un cloud public Microsoft ou dans un Cloud national :

|Types de clients du Cloud  | Où un client accepte-t-il une invitation de relation de revendeur ? |
|---------|---------
| Clients dans le cloud public | Centre d’administration Microsoft 365 |
| Clients dans l’espace partenaires pour Microsoft Cloud Allemagne | Microsoft Office le portail d’administration |
| Clients dans l’espace partenaires pour Microsoft Cloud pour le gouvernement des États-Unis | Microsoft Office le portail d’administration |
|

## <a name="next-steps"></a>Étapes suivantes

- [Assigner des contacts de support](assign-support-contacts.md)

- [Supprimer une relation avec un client](remove-a-relationship.md)
