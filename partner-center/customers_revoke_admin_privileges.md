---
title: Les clients délèguent les privilèges d’administrateur à des partenaires | Espace partenaires
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment demander aux clients de déléguer des autorisations d’administrateur à un revendeur ou de supprimer ces mêmes autorisations, et comment utiliser les autorisations.
author: LauraBrenner
ms.author: labrenne
keywords: privilèges d’administrateur délégués, administrateur pour le compte de, supprimer des privilèges, DAP, AOBO
ms.localizationpriority: high
ms.openlocfilehash: 9b82ed4828a112f28f3e2ef1da1a64745c9ffdc0
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340057"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Les clients délèguent les privilèges d’administrateur à des partenaires

**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Agent d’administration
- Agent commercial

Pour gérer le service ou l’abonnement d’un client pour son compte, le client doit vous accorder des autorisations d’administrateur pour ce service. Pour obtenir des autorisations d’administrateur de la part d’un client, envoyez-lui une demande de relation de revendeur par e-mail. Une fois que le client a approuvé votre demande, vous êtes en mesure de vous connecter au portail d’administration du service et de gérer le service pour le compte du client. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Inviter un client à établir une relation de revendeur avec vous

1.  Sélectionnez **Clients**, puis **Demander une relation de revendeur**.

2.  Sur la page suivante, vérifiez le brouillon de l’e-mail. Vous pouvez ouvrir le brouillon du message dans votre application de messagerie par défaut, ou bien copier le message dans votre Presse-papiers et le coller dans un e-mail. 

    >[!IMPORTANT]
    >Vous pouvez modifier le texte de l’e-mail, mais veillez à inclure le lien car il s’agit d’un lien personnalisé qui permet d’associer le client directement à votre compte. 
    
3.  Sélectionnez **Terminé** une fois que vous avez effectué cette étape.

4.  Envoyez l’e-mail au client.

5.  Une fois qu’il a accepté votre invitation, le client s’affiche dans votre page **Clients**. Vous pouvez alors provisionner et gérer son service à partir de là.

6.  Pour gérer le compte, les services, les utilisateurs et les licences du client, développez la fiche du client en sélectionnant la flèche vers le bas située à côté de son nom, puis sélectionnez le portail d’administration pour le service que vous voulez gérer.

>[!IMPORTANT]  
>Les clients peuvent réattribuer ou supprimer des autorisations d’administrateur sur le portail d’administration d’un service. Toutefois, tant que vous n’avez pas renégocié votre contrat avec le client, vous restez tenu de lui fournir un support client et de respecter les termes du Contrat de revendeur Cloud, même si le client a déjà réattribué ou supprimé des autorisations d’administrateur. Dans ce cas, si le client a besoin d’aide, contactez le support Microsoft pour ouvrir une demande de service pour le compte du client.

En accédant au portail d’administration Office 365, vos clients peuvent savoir lesquels de leurs partenaires disposent de privilèges d’administrateur pour leur locataire. Pour ce faire :

1. Le client doit se connecter au portail d’administration d’Office 365 en tant qu’Administrateur général.

2. Sélectionnez **Paramètres** > **Relations de partenariat**.

3. Dans la page **Relations de partenariat**, le client voit la liste des partenaires avec lesquels il travaille et ceux qui disposent de privilèges d’administrateur délégué sur son locataire.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Les clients peuvent gérer les privilèges d’administrateur délégués d’un partenaire 

Votre client peut décider de supprimer les privilèges d’administrateur délégués dont vous disposez sur leur locataire, mais de conserver la relation avec vous à des fins d’abonnement et de renouvellement des licences. Les clients gèrent les droits et autorisations pour leurs comptes Office 365 dans la page **Relations de partenariat** du Centre d’administration Office 365. Dans cette page, les clients peuvent :

- Voir avec quels partenaires ils ont établi une relation et quels partenaires ont des privilèges d’administrateur délégués

- Supprimer les privilèges d’administrateur délégué d’un partenaire sur le locataire

Pour supprimer les privilèges d’administrateur délégué d’un partenaire :

1. Dans la page **Relations de partenariat**, sélectionnez le partenaire qui vous intéresse.
2. Dans le volet d’informations, sélectionnez **Supprimer l’administrateur délégué**.
3. Dans le volet de confirmation, sélectionnez **Supprimer**.

>[!IMPORTANT]  
>Les attributions de rôles Azure AD au partenaire sont implicites. Si vous essayez de lister les membres des rôles Azure AD à l’aide du portail Azure AD/PowerShell/Graph, le partenaire n’est pas retourné. Pour savoir si des rôles Azure AD sont attribués aux partenaires, vous devez consulter la page Relations de partenariat sur le portail Office 365 Admin afin de savoir si des privilèges d’administrateur délégué ont été, ou non, accordés au partenaire.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilèges d’administrateur délégué dans Azure AD 

Le locataire Azure AD du partenaire dispose de deux groupes de sécurité utilisés pour l’administration déléguée : Agents d’administration et Agents du support technique. Quand un client accorde un privilège d’administrateur délégué à un partenaire :

- Le groupe Agent d’administration est attribué au rôle Administrateur général dans le locataire Azure AD du client.

- Le groupe Agent du support technique est attribué au rôle Administrateur du support technique dans le locataire Azure AD du client.

En fonction des rôles d’annuaire attribués, les membres des deux groupes peuvent se connecter au locataire Azure AD et aux services Office 365 du client à l’aide des informations d’identification de leurs partenaires et de leur administrateur pour le compte du client.

Si votre client supprime des privilèges d’administrateur délégué, les attributions de rôles Azure AD sont supprimées et vous ne serez plus en mesure de gérer le locataire Azure AD du client.

### <a name="azure-subscriptions-and-resource-management"></a>Abonnements Azure et gestion des ressources

Chaque abonnement Azure a son propre ensemble de rôles de gestion de ressources. Avant qu’un partenaire CSP (fournisseur de solutions Cloud) puisse gérer l’abonnement Azure d’un client, un ou plusieurs rôles doivent lui être attribués dans le cadre de l’abonnement Azure. Plus précisément :

- Quand un client accepte une invitation de revendeur et accorde un privilège d’administrateur délégué à un partenaire, ce dernier n’obtient pas automatiquement l’accès aux abonnements Azure existants sous le locataire du client.

- Quand le partenaire CSP (fournisseur de solutions Cloud) provisionne un nouvel abonnement Azure pour le client, le groupe Agent d’administration sous le locataire dudit partenaire CSP se voit automatiquement attribuer le rôle de propriétaire sous l’abonnement. Sur la base de cette attribution de rôles, les membres du groupe peuvent accéder aux ressources et les gérer sous l’abonnement.

- Quand un client supprime des privilèges d’administrateur délégué d’un partenaire à l’aide du portail Office 365, le partenaire peut toujours gérer l’abonnement Azure du client tant que le partenaire dispose d’un ou de plusieurs rôles sous l’abonnement. Pour que le partenaire cesse de gérer l’abonnement Azure, le client doit supprimer l’attribution des rôles.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Dans l’Espace partenaires, les partenaires CSP peuvent gérer les profils Autopilot pour leurs clients sans privilèges d’administrateur délégué dans les cas suivants : 

- Si un client supprime des privilèges d’administrateur délégué mais conserve une relation de revendeur avec vous, vous pouvez continuer à gérer les profils Autopilot pour lui.

- Vous pouvez gérer les appareils clients que vous ou un autre partenaire avez ajoutés. 

- Vous ne pouvez pas gérer des appareils que votre client a ajoutés par le biais de Microsoft Store pour Entreprises, de Microsoft Store pour Éducation ou du portail Microsoft Intune.

Pour plus d’informations sur Autopilot, consultez [Simplifier l’installation des appareils avec Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L’expérience de gestion Autopilot actuelle dans l’Espace partenaires peut continuer à changer. Au moment de la publication de cet article, les changements suivants sont à l’étude :

- Avant de pouvoir ajouter/mettre à jour/supprimer des profils et appliquer/supprimer des profils pour l’ensemble des appareils dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d’administrateur délégué.

- Avant de pouvoir supprimer des appareils ajoutés par d’autres partenaires ou par le client dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d’administrateur délégué. Sinon, le partenaire ne peut supprimer que les appareils qu’il a lui-même ajoutés.
