---
title: Les clients délèguent les privilèges d'administration à des partenaires | Espace partenaires
ms.topic: article
ms.date: 12/18/2018
description: En tant que revendeur partenaire, vos clients peuvent déléguer à son administrateur. Ils peuvent également supprimer les privilèges.
author: LauraBrenner
ms.author: labrenne
keywords: des privilèges d’administrateur délégué, administrateur de la part de, supprimer les privilèges, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 9253bcca2d93d9f0d62d6d7241132f0c0c9bf5ec
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135449"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Les clients délèguent les privilèges d'administration à des partenaires

**S’applique à**

-  Espace partenaires

Pour gérer le service ou l'abonnement au nom d’un client, ce dernier doit accorder des autorisations d’administrateur pour ce service. Pour obtenir des autorisations d’administrateur de la part d’un client, envoyez-lui une demande de relation de revendeur par courrier électronique. Lorsque le client aura approuvé votre demande, vous serez en mesure d’ouvrir une session sur le portail d’administration du service et de gérer le service pour le compte du client. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Inviter un client à établir une relation de revendeur avec vous

1.  Sélectionnez **clients** , puis sélectionnez **demander une relation de revendeur**.

2.  Sur la page suivante, vérifiez le brouillon du message électronique. Vous pouvez ouvrir le brouillon du message dans votre application de messagerie électronique par défaut ou copier ce message dans votre Presse-papiers et le coller dans un message électronique. 

    >[!IMPORTANT]
    >Vous pouvez modifier le texte du message électronique, mais veillez à inclure le lien car il s'agit d'un lien personnalisé qui permet d'associer le client directement à votre compte. 
    
3.  Sélectionnez **OK** lorsque vous avez terminé cette étape.

4.  Envoyez le message électronique au client.

5.  Une fois qu'il a accepté l’invitation, le client s’affiche sur votre page **Clients** et vous pouvez approvisionner et gérer son service à partir de cet emplacement.

6.  Pour gérer le compte du client, les services, les utilisateurs et les licences, développez l’enregistrement du client en sélectionnant la flèche vers le côté de leur nom, puis sélectionnez le portail d’administration pour le service que vous souhaitez gérer.

>[!IMPORTANT]  
>Les clients peuvent réaffecter ou supprimer des autorisations d’administrateur dans le portail d’administration d’un service. Toutefois, tant que vous n'aurez pas renégocié votre accord avec le client, vous resterez tenu de lui fournir un support et de respecter les termes du contrat de revendeur Cloud, même si le client a déjà réattribué ou supprimé des autorisations d’administrateur. Dans ce cas, si le client nécessite l’aide, contactez le support Microsoft pour ouvrir une demande de service pour le compte du client.

Vos clients peuvent déterminer laquelle de leurs partenaires ont des privilèges d’administrateur à leur client à partir de dans le portail d’administration Office 365. Pour ce faire :

1. Le client doit se connecter au portail d’administration Office 365 en tant qu’administrateur général.

2. Sélectionnez **Paramètres** → **Relations de partenariat**.

3. Sur le **relations de partenaire** page, le client s’affiche une liste des partenaires avec lesquels ils fonctionnent et ceux qui ont été accordées délégué des privilèges d’administration à leur client.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Les clients peuvent gérer les privilèges d'administrateur délégués d'un partenaire 

Votre client pourrait décider de supprimer vos privilèges d’administrateur délégué à partir de son client tout en conservant la relation avec vous pour l’abonnement et à des fins de renouvellement de licence. Les clients gèrent les droits et autorisations pour leurs comptes Office 365 sur la page **Relations de partenariat** du Centre d’administration Office 365. Sur cette page, les clients peuvent :

- Voir avec quels partenaires ils ont établi une relation et quels partenaires ont des privilèges d'administrateur délégués

- Supprimer les privilèges d'administrateur délégués d'un partenaire sur le locataire

Pour supprimer les privilèges d'administrateur délégués d'un partenaire :

1. Sur la page **Relations de partenariat**, sélectionnez le partenaire qui vous intéresse.
2. Dans le volet d’informations, sélectionnez **Supprimer l'administrateur délégué**.
3. Dans le volet de confirmation, sélectionnez **Supprimer**.

>[!IMPORTANT]  
>L'attribution des rôles Azure AD au partenaire est implicite. Si vous essayez de répertorier les membres des rôles Azure AD à l’aide du portail Azure AD/PowerShell/Graph, le partenaire n’est pas renvoyé. Pour savoir si des rôles Azure AD sont affectés aux partenaires, vous devez consulter la page Relations de partenariat sur le portail de Office 365 Admin pour savoir si des privilèges d'administrateur délégués ont été ou non accordés au partenaire.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilèges d’administrateur délégués dans Azure AD 

Le locataire Azure AD du partenaire dispose de deux groupes de sécurité utilisés pour l’administration déléguée : les agents d’administration et les agents du support technique. Lorsqu'un client accorde un privilège d'administrateur délégué à un partenaire :

- Le groupe agent administrateur est affecté au rôle d’administrateur général dans le locataire Azure AD du client.

- Le groupe agent du support technique est affecté au rôle d’administrateur du support technique dans le locataire Azure AD du client.

En fonction des rôles d'annuaire attribués, les membres des deux groupes peuvent se connecter au locataire Azure AD et aux services Office 365 du client à l’aide de leurs informations d’identification partenaires et de leur rôle d’administrateur pour le compte du client.

Si votre client supprime des privilèges d’administrateur délégués, les attributions de rôles Azure AD sont supprimées et vous ne serez plus en mesure de gérer le locataire Azure AD du client.

### <a name="azure-subscriptions-and-resource-management"></a>Abonnements et gestion des ressources Azure

Chaque abonnement Azure a son propre ensemble de rôles de gestion de ressources. Avant qu'un partenaire fournisseur de solutions Cloud puisse gérer l’abonnement Azure d’un client, un ou plusieurs rôles doivent lui être affectés dans le cadre de l’abonnement Azure. Plus précisément :

- Lorsqu’un client accepte une invitation revendeur et accorde un privilège d'administrateur délégué à un partenaire, ce dernier n’obtient pas automatiquement l’accès aux abonnements Azure existants sur le locataire du client.

- Lorsque le partenaire fournisseur de solutions Cloud fournit un nouvel abonnement Azure au client, le groupe agent administrateur sous le locataire dudit partenaire fournisseur se voit automatiquement attribuer le rôle de propriétaire dans le cadre de l'abonnement. Sur la base de cette attribution de rôles, les membres du groupe peuvent accéder aux ressources et les gérer dans le cadre de l'abonnement.

- Lorsqu’un client supprime des privilèges d'administrateur délégués d’un partenaire à l’aide du portail Office 365, le partenaire peut toujours gérer l'abonnement Azure du client tant que le partenaire dispose toujours d'un ou plusieurs rôles dans le cadre de l’abonnement. Pour empêcher le partenaire de gérer l'abonnement Azure, le client doit supprimer l'attribution de tous les rôles.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

À partir du centre de partenaires, les partenaires CSP peuvent gérer des profils Autopilot pour leurs clients sans privilèges d’administrateur délégué dans ces circonstances : 

- Si un client supprime les privilèges d’administration déléguée, mais conserve une relation de revendeur avec vous, vous pouvez continuer à gérer des profils Autopilot pour eux.

- Vous pouvez gérer des appareils clients que vous ou un autre partenaire ont ajoutés. 

- Vous ne pouvez pas gérer les appareils de que votre client a ajouté via le Microsoft Store pour entreprises, Microsoft Store pour l’éducation ou Microsoft Intune Portal.

Pour plus d’informations sur Autopilot, consultez [simplifier l’installation de périphérique avec Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L’expérience de gestion actuel Autopilot dans partenaires peut-être continuer à modifier. Au moment de que cet article a été publié, les modifications suivantes sont considérés comme des :

- Avant de pouvoir ajouter/mettre à jour/supprimer des profils et appliquer/supprimer des profils pour l'ensemble des appareils dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d'administrateur délégués.

- Partenaire doit disposer des privilèges de l’administration déléguée par le client avant le partenaire peut supprimer les appareils ajoutés par les autres partenaires ou par le client dans le locataire de client. Sinon, le partenaire peut supprimer uniquement les appareils ajoutés précédemment par le même partenaire.
