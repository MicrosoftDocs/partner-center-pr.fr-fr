---
title: Gérer les sites dans votre compte partenaire
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663893"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gérer les localisations de votre compte MPN et ajouter une nouvelle localisation

**S’applique à**

- Espace partenaires

**Rôles appropriés**

- Administrateur général
- Administrateur des comptes

L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise. Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales. L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.

## <a name="the-following-is-a-typical-scenario"></a>Voici un scénario courant :

Contoso a comme localisation de son compte global de partenaire (PGA) le Royaume-Uni. Il s’agit de leur activité légalement enregistrée et elle a un ID MPN utilisé pour la gestion de toutes les activités hors transactions. Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis. Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques. Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives. Les règlements sont associés à des sites spécifiques. 

>[!NOTE]
>Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Structure des localisations MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Prérequis pour pouvoir ajouter une nouvelle localisation pour une activité CSP

Pour ajouter une nouvelle localisation d’activité CSP, il y a plusieurs prérequis :

1. Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité.

1. Vous avez besoin d’un nouveau locataire Azure AD dans la région de l’activité, qui ne soit pas déjà inscrit dans le programme CSP. Créez cela quand vous vous inscrivez dans le programme CSP.
 
3. Utilisez le nouveau locataire AAD pour vous inscrire au programme CSP dans la région.
Spécifiez les informations détaillées officielles de votre entreprise, comme le nom de la société, l’adresse et les coordonnées du contact principal. Ce compte sera soumis à une vérification : veillez donc à ajouter des informations valides.

>[!NOTE] 
 >N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** locataire Azure AD. N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.

4. Acceptez le Contrat Partenaire Microsoft et activez le compte.

## <a name="add-a-location"></a>Ajouter une localisation

1. À partir de l’**icône de paramètres**, sélectionnez **Partner settings** (Paramètres partenaire).

2. Sélectionnez **Locations** (Sites).

3. Sélectionnez **Add a location** (Ajouter un site).  

4. Dans la page **Add a location** (Ajouter un site), insérez les coordonnées du site que vous souhaitez ajouter à votre entreprise ainsi que son contact principal.

> [!NOTE]
> Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé.

## <a name="change-global-partner-account-location"></a>Changer la localisation du compte de partenaire global

1. Dans la page **Locations** (Sites), vérifiez que le site que vous voulez désigner comme entité légale figure bien dans la liste des sites. Si ce n’est pas le cas, ajoutez-le.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Structure des localisations MPN":::

2. Sélectionnez **Partner profile** (Profil partenaire), puis **Update legal business profile** (Mettre à jour le profil d’entreprise légale).

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Structure des localisations MPN":::

3. Sélectionnez la région et l’entité légale et choisissez **Submit** (Soumettre).

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Structure des localisations MPN":::

## <a name="next-steps"></a>Étapes suivantes

- Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).
