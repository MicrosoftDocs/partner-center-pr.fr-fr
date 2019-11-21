---
title: Les clients délèguent les privilèges d'administration à des partenaires | Espace partenaires
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Apprenez à demander aux clients de déléguer des autorisations d’administrateur à un revendeur ou de supprimer les mêmes autorisations et l’utilisation des autorisations.
author: LauraBrenner
ms.author: labrenne
keywords: privilèges d’administrateur délégué, administrateur pour le compte de, supprimer des privilèges, DAP, ADMINISTRATE
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253482"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Les clients délèguent les privilèges d'administration à des partenaires

**S’applique à**

-  Espace partenaires

Pour gérer le service ou l'abonnement au nom d’un client, ce dernier doit accorder des autorisations d’administrateur pour ce service. Pour obtenir des autorisations d’administrateur de la part d’un client, envoyez-lui une demande de relation de revendeur par courrier électronique. Lorsque le client aura approuvé votre demande, vous serez en mesure d’ouvrir une session sur le portail d’administration du service et de gérer le service pour le compte du client. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Inviter un client à établir une relation de revendeur avec vous

1.  Sélectionnez **clients** , puis sélectionnez **demander une relation de revendeur**.

2.  Sur la page suivante, vérifiez le brouillon de l’e-mail. Vous pouvez ouvrir le brouillon du message dans votre application de messagerie électronique par défaut ou copier ce message dans votre Presse-papiers et le coller dans un message électronique. 

    >[!IMPORTANT]
    >Vous pouvez modifier le texte du message électronique, mais veillez à inclure le lien car il s'agit d'un lien personnalisé qui permet d'associer le client directement à votre compte. 
    
3.  Sélectionnez **Terminé** une fois que vous avez effectué cette étape.

4.  Envoyez le message électronique au client.

5.  Une fois qu'il a accepté l’invitation, le client s’affiche sur votre page **Clients** et vous pouvez approvisionner et gérer son service à partir de cet emplacement.

6.  Pour gérer le compte, les services, les utilisateurs et les licences du client, développez l’enregistrement du client en sélectionnant la flèche vers le bas en regard de son nom, puis sélectionnez le portail d’administration pour le service que vous souhaitez gérer.

>[!IMPORTANT]  
>Les clients peuvent réaffecter ou supprimer des autorisations d’administrateur dans le portail d’administration d’un service. Toutefois, tant que vous n'aurez pas renégocié votre accord avec le client, vous resterez tenu de lui fournir un support et de respecter les termes du contrat de revendeur Cloud, même si le client a déjà réattribué ou supprimé des autorisations d’administrateur. Dans ce cas, si le client a besoin d’aide, contactez le support technique de Microsoft pour ouvrir une demande de service pour le compte du client.

Vos clients peuvent identifier les partenaires qui disposent de privilèges d’administrateur sur leur locataire à partir du portail d’administration Office 365. Pour ce faire :

1. Le client doit se connecter au portail d’administration Office 365 en tant qu’administrateur général.

2. Sélectionnez **paramètres** > les **relations de partenaire**.

3. Dans la page relations avec les **partenaires** , le client verra une liste des partenaires avec lesquels ils travaillent et ceux qui ont reçu des privilèges d’administration déléguées à leur locataire.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Les clients peuvent gérer les privilèges d’administrateur délégué d’un partenaire. 

Votre client peut décider de supprimer vos privilèges d’administrateur délégué de son locataire, tout en conservant la relation avec vous à des fins d’abonnement et de renouvellement de licence. Les clients gèrent les droits et autorisations pour leurs comptes Office 365 sur la page **Relations de partenariat** du Centre d’administration Office 365. Sur cette page, les clients peuvent :

- Voir avec quels partenaires ils ont établi une relation et quels partenaires ont des privilèges d'administrateur délégués

- Supprimer les privilèges d’administration déléguée d’un partenaire du locataire

Pour supprimer les privilèges d'administrateur délégués d'un partenaire :

1. Sur la page **Relations de partenariat**, sélectionnez le partenaire qui vous intéresse.
2. Dans le volet d’informations, sélectionnez **Supprimer l'administrateur délégué**.
3. Dans le volet de confirmation, sélectionnez **Supprimer**.

>[!IMPORTANT]  
>L'attribution des rôles Azure AD au partenaire est implicite. Si vous essayez de répertorier les membres des rôles Azure AD à l’aide du portail Azure AD/PowerShell/Graph, le partenaire n’est pas renvoyé. Pour savoir si des rôles Azure AD sont affectés aux partenaires, vous devez consulter la page Relations de partenariat sur le portail de Office 365 Admin pour savoir si des privilèges d'administrateur délégués ont été ou non accordés au partenaire.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilèges d’administrateur délégués dans Azure AD 

Il existe deux groupes de sécurité : les agents d’administration et les agents du support technique dans le locataire Azure AD du partenaire qui sont utilisés pour l’administration déléguée. Lorsqu'un client accorde un privilège d'administrateur délégué à un partenaire :

- Le groupe d’agents d’administration est attribué au rôle d’administrateur général dans le locataire Azure AD du client.

- Le groupe d’agents du support technique est attribué au rôle administrateur du support technique dans le locataire Azure AD du client.

En fonction des rôles d’annuaire affectés, les membres des deux groupes peuvent se connecter aux services Azure AD locataire et O365 du client à l’aide de leurs informations d’identification de partenaire et de leur administrateur pour le compte du client.

Si votre client supprime les privilèges d’administrateur délégué, les attributions de rôle Azure AD sont supprimées et vous ne pourrez plus gérer le locataire Azure AD du client.

### <a name="azure-subscriptions-and-resource-management"></a>Abonnements et gestion des ressources Azure

Chaque abonnement Azure a son propre ensemble de rôles de gestion de ressources. Pour qu’un partenaire CSP puisse gérer l’abonnement Azure d’un client, celui-ci doit être affecté à un ou plusieurs rôles dans le cadre de l’abonnement Azure. Plus précisément :

- Lorsqu’un client accepte une invitation revendeur et accorde un privilège d'administrateur délégué à un partenaire, ce dernier n’obtient pas automatiquement l’accès aux abonnements Azure existants sur le locataire du client.

- Lorsque le partenaire fournisseur de solutions Cloud fournit un nouvel abonnement Azure au client, le groupe agent administrateur sous le locataire dudit partenaire fournisseur se voit automatiquement attribuer le rôle de propriétaire dans le cadre de l'abonnement. Sur la base de cette attribution de rôles, les membres du groupe peuvent accéder aux ressources et les gérer dans le cadre de l'abonnement.

- Lorsqu’un client supprime des privilèges d’administration délégués d’un partenaire à l’aide du portail Office 365, le partenaire peut toujours gérer l’abonnement Azure du client tant que le partenaire est toujours affecté à un ou plusieurs rôles dans le cadre de l’abonnement. Pour empêcher le partenaire de gérer l'abonnement Azure, le client doit supprimer l'attribution de tous les rôles.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Dans l’espace partenaires, les partenaires CSP peuvent gérer les profils AutoPilot pour leurs clients sans privilèges d’administrateur délégués dans les circonstances suivantes : 

- Si un client supprime des privilèges d’administration délégués mais conserve une relation de revendeur avec vous, vous pouvez continuer à gérer les profils AutoPilot pour eux.

- Vous pouvez gérer les appareils clients que vous ou un autre partenaire avez ajoutés. 

- Vous ne pouvez pas gérer les appareils que votre client a ajoutés par le biais du Microsoft Store pour entreprises, Microsoft Store pour l’éducation ou Microsoft Intune portail.

Pour plus d’informations sur AutoPilot, consultez [simplifier la configuration des appareils avec Windows AutoPilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L’expérience de gestion AutoPilot actuelle dans l’espace partenaires peut continuer à changer. Au moment de la publication de cet article, les modifications suivantes sont prises en compte :

- Avant de pouvoir ajouter/mettre à jour/supprimer des profils et appliquer/supprimer des profils pour l'ensemble des appareils dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d'administrateur délégués.

- Le client doit disposer d’un privilège d’administration déléguée par le client avant que le partenaire puisse supprimer des appareils ajoutés par d’autres partenaires ou par le client du locataire client. Dans le cas contraire, le partenaire peut supprimer uniquement les appareils ajoutés précédemment par le même partenaire.
