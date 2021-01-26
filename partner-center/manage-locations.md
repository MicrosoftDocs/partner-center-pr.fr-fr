---
title: Gérer les sites dans votre compte partenaire
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773426"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation


**Rôles appropriés**

- Administrateur général
- Administrateur des comptes

L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise. Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales. L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.

## <a name="the-following-is-a-typical-scenario"></a>Voici un scénario courant :

Contoso a son compte global de partenaire (PGA) au Royaume-Uni. Il s’agit de leur activité légalement enregistrée et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions. Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis. Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques. Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives. Les règlements sont associés à des sites spécifiques. 

>[!NOTE]
>Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a>Prérequis pour l’ajout d’une nouvelle localisation de compte pour une activité CSP

Pour ajouter une nouvelle localisation d’activité CSP, il y a plusieurs prérequis :

1. Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité.

1. Vous avez besoin d’un nouveau locataire Azure AD dans la [région de l’activité](regional-authorization-overview.md), qui ne soit pas déjà inscrit dans le programme CSP. Créez cela quand vous vous inscrivez dans le programme CSP.
 
3. Utilisez le nouveau locataire AAD pour vous inscrire au programme CSP dans la région.
Spécifiez les informations détaillées officielles de votre entreprise, comme le nom de la société, l’adresse et les coordonnées du contact principal. Ce compte sera soumis à une vérification : veillez donc à ajouter des informations valides.

>[!NOTE] 
 >N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** locataire Azure AD. N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.

4. Acceptez le Contrat Partenaire Microsoft et activez le compte.

## <a name="add-an-mpn-location"></a>Ajouter un site MPN

1. Connectez-vous avec le compte MPN dans l’Espace partenaires. Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte. 

1. À partir de l’**icône de paramètres**, sélectionnez **Organization settings** (Paramètres de l’organisation).

2. Sélectionnez **Legal**, puis **Locations** (Sites).

3. Sélectionnez **Add a location** (Ajouter un site) et insérez les coordonnées du site que vous souhaitez ajouter à votre entreprise ainsi que son contact principal.

> [!NOTE]
> Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé. Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.

## <a name="change-global-partner-account-location"></a>Changer la localisation du compte de partenaire global

1. Dans **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** (Sites commerciaux), vérifiez que le site que vous voulez désigner comme entité légale figure bien dans la liste. Si ce n’est pas le cas, ajoutez-le.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Capture d’écran de la page Emplacements des comptes de l’Espace partenaires, avec la liste de tous les emplacements actuels.":::

2. Sélectionnez **Legal**, puis **Update legal business profile** (Mettre à jour le profil d’entreprise légale).
  
3. Sélectionnez la région et l’entité légale et choisissez **Submit** (Soumettre).

  
## <a name="next-steps"></a>Étapes suivantes

- Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).
