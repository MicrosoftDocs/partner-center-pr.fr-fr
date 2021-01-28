---
title: Gérer les sites dans votre compte partenaire
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925036"
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

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Prérequis pour l’ajout d’un nouveau compte pour une activité CSP

Pour ajouter un nouveau compte commercial CSP, commencez par veiller à remplir les prérequis.

1. Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité CSP. Pour créer une localisation MPN, consultez « Ajouter une localisation MPN » ci-dessous.
  
1. Pour créer un nouvel abonnement CSP Indirect Reseller, lisez [Travailler avec des fournisseurs indirects](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** compte CSP. N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.

2. Acceptez le Contrat Partenaire Microsoft et activez le compte.

## <a name="add-an-mpn-location"></a>Ajouter un site MPN

1. Connectez-vous avec le compte MPN dans l’Espace partenaires. (Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte. 

1. À partir de l’**icône Paramètres**, sélectionnez **Paramètres du compte**, puis **Profil de l’organisation**.

2. Sélectionnez **Légal**, puis sous l’onglet **Partenaire**, sélectionnez **Localisations d’entreprise** et cliquez sur **Ajouter une localisation**.

3. Fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact pour la localisation que vous souhaitez ajouter à votre société.
 
1. Cliquez sur **Ajouter une localisation**. Un nouvel ID MPN est créé pour la nouvelle localisation que vous pouvez utiliser pour les transactions et incentives CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Ajouter une nouvelle activité légale":::

> [!NOTE]
> Une fois qu’un site a été ajouté dans l’Espace partenaires, il ne peut plus être supprimé. Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.

## <a name="change-country-of-partner-global-account"></a>Changer le pays du compte global du partenaire 

1. Connectez-vous avec le compte MPN dans l’Espace partenaires. (Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte. 

2. Sous l’onglet **Partenaire**, accédez à **Localisations d’entreprise** et vérifiez que la localisation que vous voulez désigner comme entité légale figure bien dans la liste. 
 
1. Pour ajouter une localisation, cliquez sur **Ajouter une localisation**, puis dans le menu volant, fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact principal pour la localisation que vous souhaitez ajouter à votre entreprise. 
 
1. Sélectionnez **Changer votre pays** à côté de la liste déroulante **Pays/région** et suivez les étapes. 

:::image type="content" source="images/lbp.png" alt-text="Menu volant des données de profil de l’entreprise légale":::

5. Cliquez sur **Enregistrer**.

6. Le pays du compte global MPN sera remplacé par le nouveau pays légal.
  
## <a name="next-steps"></a>Étapes suivantes

- Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).
