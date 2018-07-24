---
title: Les clients délèguent les privilèges d'administration à des partenaires | Espace partenaires
description: En tant que partenaire revendeur, votre client peut vous autoriser à être son administrateur délégué et il peut également supprimer des privilèges.
author: labrenne
keywords: privilèges d’administrateur délégués, administrateur pour le compte de, supprimer des privilèges
ms.openlocfilehash: 7f1bd81f40892f851e1582a7a842a64c55e4ff63
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/23/2018
ms.locfileid: "1913945"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Les clients délèguent les privilèges d'administration à des partenaires

**S'applique à:**

-  Espace partenaires

En tant que partenaire fournisseur de solutions Cloud et conseiller de confiance pour vos clients, ils peuvent vous autoriser à être leur administrateur délégué Office365 et de leur locataire AzureAD. Vous pouvez initialiser cette relation par le biais du Tableau de bord du partenaire en leur envoyant une invitation. 

1. Sélectionnez **Clients** à partir de votre menu **Tableau de bord**, puis sélectionnez **Demander une relation avec un client**.
2. Un e-mail avec formulaire contenant votre URL s'affiche. Vous pouvez copier et coller le formulaire dans un e-mail à envoyer à votre client. N’hésitez pas à ajouter des informations supplémentaires, mais veillez à bien inclure l’URL. Le client utilisera cette URL pour répondre à votre demande.  
3. Lorsque votre client accepte l’invitation, vous devenez l’administrateur de ses services.

En accédant au portail de service Office365, vos clients peuvent savoir qui de leurs partenaires disposent des privilèges d’administrateur pour leur locataire. Pour cela, procédez comme suit:

1. Connectez-vous au [Portail d'administration d'Office365Admin](https://portal.office.com/adminportal) en tant qu’administrateur général.
2. Sélectionnez **Paramètres** → **Relations de partenariat**.
3. Sur la page **Relations de partenariat**, ils verront une liste des partenaires avec lesquels ils travaillent et ceux qui disposent de privilèges d'administrateur délégués sur leur locataire.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Les clients peuvent gérer les privilèges d'administrateur délégués d'un partenaire 

Votre client peut décider de supprimer les privilèges d'administrateur dont vous disposez sur leur locataire, mais conserver la relation avec vous à des fins d'abonnement et de renouvellement des licences. Les clients gèrent les droits et autorisations pour leurs comptes Office365 sur la page **Relations de partenariat** du Centre d’administration Office365. Sur cette page, les clients peuvent:

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

## <a name="windows-autopilot"></a>WindowsAutoPilot 

À partir du Tableau de bord du partenaire, les partenaires fournisseurs de solutions Cloud peuvent gérer la configuration AutoPilot pour leurs clients même sans privilèges d'administrateur délégués. Découvrez comment [simplifier l’installation d'appareils avec WindowsAutoPilot](https://docs.microsoft.com/partner-center/autopilot).

Les possibilités offertes dépendent de votre statut de revendeur (direct ou indirect).

|**Opération**   |**Revendeur direct ou revendeur indirect**   |**Revendeur indirect**   |
|-----------------|-----------------------------------| -----------------------------|
|Ajouter des appareils (à l’aide d'un fichier CSV)  |Oui      |Non|
|Supprimer des appareils   |Oui   |Non|
|Ajouter un profil   |Oui   | Oui   |
|Mettre à jour le profil   |Oui    |Oui   |
|Supprimer le profil   |Oui   |Oui   |
|Appliquer le profil aux appareils   |Oui   |Oui   |
|Supprimer le profil des appareils   |Oui   |Oui   | 

- Les partenaires fournisseurs de solutions Cloud peuvent continuer à gérer la configuration AutoPilot pour les clients existants dans le cas d'une relation de revendeur, même si les clients ont supprimé les privilèges d'administrateur délégués de leurs partenaires.

- Vous pouvez gérer pour vos clients les appareils existants que vous ou un autre partenaire fournisseur de solutions Cloud avez ajoutés.

- Vous ne pouvez pas gérer les appareils que votre client a téléchargés (via MicrosoftStore pour Entreprises ou le portail MicrosoftIntune).

>**Important** L’expérience de gestion AutoPilot actuelle dans l'Espace partenaires Microsoft n’est pas définitive et peut être modifiée à tout moment. Au moment de la rédaction de cet article, les modifications suivantes sont à l'étude:

  - Avant de pouvoir ajouter/mettre à jour/supprimer des profils et appliquer/supprimer des profils pour l'ensemble des appareils dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d'administrateur délégués.

- Avant de pouvoir supprimer des appareils chargés par d'autres partenaires ou par le client dans le locataire du client, le partenaire doit se voir attribuer par le client des privilèges d'administrateur délégués. Dans le cas contraire, le partenaire ne pourra supprimer que les appareils qu'il a lui-même ajoutés.
