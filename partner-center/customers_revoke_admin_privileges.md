---
title: Les clients délèguent les privilèges d'administration à des partenaires | Espace partenaires
description: Comme un partenaire revendeur, votre client peut vous autoriser à être leur administrateur. Ils peuvent également supprimer des privilèges.
author: labrenne
keywords: privilèges d’administrateur délégués, administrateur pour le compte de, supprimer des privilèges, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8a6d14398bdd9a439bc001ecb3d03bc9d7774937
ms.sourcegitcommit: 3478fc6fe1a061e5973307fffd039b4bee5d8e1c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/08/2018
ms.locfileid: "3806677"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Les clients délèguent les privilèges d'administration à des partenaires

**S'applique à:**

-  Tableau de bord du partenaire

Pour gérer le service ou l'abonnement au nom d’un client, ce dernier doit accorder des autorisations d’administrateur pour ce service. Pour obtenir des autorisations d’administrateur de la part d’un client, envoyez-lui une demande de relation de revendeur par courrier électronique. Lorsque le client aura approuvé votre demande, vous serez en mesure d’ouvrir une session sur le portail d’administration du service et de gérer le service pour le compte du client. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Inviter un client à établir une relation de revendeur avec vous

1.  Sélectionnez **clients** , puis **demander une relation de revendeur**.

2.  Sur la page suivante, vérifiez le brouillon du message électronique. Vous pouvez ouvrir le brouillon du message dans votre application de messagerie électronique par défaut ou copier ce message dans votre Presse-papiers et le coller dans un message électronique. 

    >! IMPORTANT<br>
    >Vous pouvez modifier le texte du message électronique, mais veillez à inclure le lien car il s'agit d'un lien personnalisé qui permet d'associer le client directement à votre compte. 
    
3.  Sélectionnez **OK** lorsque vous avez terminé cette étape.

4.  Envoyez le message électronique au client.

5.  Une fois qu'il a accepté l’invitation, le client s’affiche sur votre page **Clients** et vous pouvez approvisionner et gérer son service à partir de cet emplacement.

6.  Pour gérer le compte du client, les services, les utilisateurs et les licences, développez la fiche du client en sélectionnant la flèche vers le bas côté de son nom, puis sélectionnez le portail d’administration pour le service que vous souhaitez gérer.


>**Important**<br>
Les clients peuvent réattribuer ou supprimer des autorisations d’administrateur sur le portail d’administration d’un service. Toutefois, tant que vous n'aurez pas renégocié votre accord avec le client, vous resterez tenu de lui fournir un support et de respecter les termes du contrat de revendeur Cloud, même si le client a déjà réattribué ou supprimé des autorisations d’administrateur. Dans ce cas, si le client a besoin d’aide, contactez le support Microsoft pour ouvrir une demande de service au nom du client.

Vos clients peuvent savoir qui de leurs partenaires disposent des privilèges d’administrateur pour leur locataire dans le portail d’administration Office 365. Pour cela, procédez comme suit:

1. Le client a besoin de se connecter au portail d’administration Office 365 en tant qu’un administrateur général.

2. Sélectionnez **Paramètres** → **Relations de partenariat**.

3. Sur la page **relations de partenariat** , le client verra une liste des partenaires avec lesquels ils travaillent et ceux qui ont été délégués sur leur locataire.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Les clients peuvent gérer les privilèges d'administrateur délégués d'un partenaire 

Votre client peut décider de supprimer vos privilèges d’administrateur délégués à partir de leur client, mais conserver la relation avec votre abonnement et à des fins de renouvellement de licence. Les clients gèrent les droits et autorisations pour leurs comptes Office365 sur la page **Relations de partenariat** du Centre d’administration Office365. Sur cette page, les clients peuvent:

- Voir avec quels partenaires ils ont établi une relation et quels partenaires ont des privilèges d'administrateur délégués

- Supprimer les privilèges d'administrateur délégués d'un partenaire sur le locataire

Pour supprimer les privilèges d'administrateur délégués d'un partenaire:

1. Sur la page **Relations de partenariat**, sélectionnez le partenaire qui vous intéresse.
2. Dans le volet d’informations, sélectionnez **Supprimer l'administrateur délégué**.
3. Dans le volet de confirmation, sélectionnez **Supprimer**.

>**Important**<br>
L'attribution des rôles AzureAD au partenaire est implicite. Si vous essayez de répertorier les membres des rôles AzureAD à l’aide du portail AzureAD/PowerShell/Graph, le partenaire n’est pas renvoyé. Pour savoir si des rôles AzureAD sont affectés aux partenaires, vous devez consulter la page Relations de partenariat sur le portail de Office 365 Admin pour savoir si des privilèges d'administrateur délégués ont été ou non accordés au partenaire.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilèges d’administrateur délégués dans AzureAD 

Le locataire AzureAD du partenaire dispose de deux groupes de sécurité utilisés pour l’administration déléguée: les agents d’administration et les agents du support technique. Lorsqu'un client accorde un privilège d'administrateur délégué à un partenaire:

- Le groupe agent administrateur est affecté au rôle d’administrateur général dans le locataire AzureAD du client.

- Le groupe agent du support technique est affecté au rôle d’administrateur du support technique dans le locataire AzureAD du client.

En fonction des rôles d'annuaire attribués, les membres des deux groupes peuvent se connecter au locataire AzureAD et aux services Office365 du client à l’aide de leurs informations d’identification partenaires et de leur rôle d’administrateur pour le compte du client.

Si votre client supprime des privilèges d’administrateur délégués, les attributions de rôles AzureAD sont supprimées et vous ne serez plus en mesure de gérer le locataire AzureAD du client.

### <a name="azure-subscriptions-and-resource-management"></a>Abonnements et gestion des ressources Azure

Chaque abonnement Azure a son propre ensemble de rôles de gestion de ressources. Avant qu'un partenaire fournisseur de solutions Cloud puisse gérer l’abonnement Azure d’un client, un ou plusieurs rôles doivent lui être affectés dans le cadre de l’abonnement Azure. Plus précisément:

- Lorsqu’un client accepte une invitation revendeur et accorde un privilège d'administrateur délégué à un partenaire, ce dernier n’obtient pas automatiquement l’accès aux abonnements Azure existants sur le locataire du client.

- Lorsque le partenaire fournisseur de solutions Cloud fournit un nouvel abonnement Azure au client, le groupe agent administrateur sous le locataire dudit partenaire fournisseur se voit automatiquement attribuer le rôle de propriétaire dans le cadre de l'abonnement. Sur la base de cette attribution de rôles, les membres du groupe peuvent accéder aux ressources et les gérer dans le cadre de l'abonnement.

- Lorsqu’un client supprime des privilèges d'administrateur délégués d’un partenaire à l’aide du portail Office365, le partenaire peut toujours gérer l'abonnement Azure du client tant que le partenaire dispose toujours d'un ou plusieurs rôles dans le cadre de l’abonnement. Pour empêcher le partenaire de gérer l'abonnement Azure, le client doit supprimer l'attribution de tous les rôles.

## <a name="windows-autopilot"></a>Windows Autopilot 

À partir du tableau de bord du partenaire, les partenaires de fournisseur de solutions cloud peuvent gérer des profils Autopilot pour leurs clients sans privilèges d’administrateur délégués. Découvrez comment [simplifier l’installation d'appareils avec WindowsAutoPilot](https://docs.microsoft.com/partner-center/autopilot).

Ce que vous pouvez faire varie sur quel modèle fournisseur de solutions cloud vous êtes inscrit.

|**Opération**   |**L’espace de facture direct et le fournisseur Indirect**   |**Revendeur indirect**   |
|-----------------|-----------------------------------| -----------------------------|
|Ajouter des appareils (à l’aide d'un fichier CSV)  |Oui      |Non|
|Supprimer des appareils   |Oui   |Non|
|Ajouter un profil   |Oui   | Oui   |
|Mettre à jour le profil   |Oui    |Oui   |
|Supprimer le profil   |Oui   |Oui   |
|Appliquer le profil aux appareils   |Oui   |Oui   |
|Supprimer le profil des appareils   |Oui   |Oui   | 

- Si un client supprime des privilèges d’administration délégués, mais conserve une relation de revendeur avec vous, vous pouvez continuer à gérer les profils Autopilot pour eux.

- Vous pouvez gérer les appareils clients que vous ou un autre partenaire avez ajoutés. 

- Vous ne pouvez pas gérer les appareils de que votre client a ajouté via le Microsoft Store pour entreprises, Microsoft Store pour éducation ou Microsoft Intune Portal.

>**Important** L’expérience de gestion Autopilot actuelle dans le tableau de bord peut continuer à modifier. Au moment de la que date de publication de cet article, les modifications suivantes sont envisagées:

  - Avant de pouvoir ajouter/mettre à jour/supprimer des profils et appliquer/supprimer des profils pour l'ensemble des appareils dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d'administrateur délégués.

- Partenaire doit se voir délégués par le client avant de pouvoir supprimer le périphériques ajoutés par d’autres partenaires ou par le client dans le locataire du client. Dans le cas contraire, le partenaire peut supprimer uniquement les périphériques ajoutés précédemment par le même partenaire.
