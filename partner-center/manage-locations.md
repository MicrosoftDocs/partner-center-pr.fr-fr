---
title: Gérer les localisations dans votre compte partenaire
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Découvrez comment ajouter une nouvelle localisation et comment l’ID MPN de localisation est utilisé dans les programmes d’incentives, l’activité CSP, les abonnements et autres transactions.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276822"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gérer les localisations dans votre compte MPN et ajouter (supprimer) une localisation


**Rôles appropriés** : Administrateur général | Administrateur de compte

L’ID MPN de localisation identifie chaque localisation spécifique de votre entreprise. Vous utilisez l’ID MPN de localisation pour vous inscrire aux programmes d’incentives, pour effectuer des transactions dans le cadre de l’activité CSP et pour d’autres transactions commerciales. L’ID MPN global est utilisé pour les activités hors transactions, comme les demandes de support.

## <a name="the-following-scenario-is-typical"></a>Le scénario suivant est très courant :

Contoso a son compte global de partenaire (PGA) au Royaume-Uni. Il s’agit de leur activité légalement enregistrée, et son ID MPN global est utilisé pour la gestion de toutes les activités hors transactions. Contoso a également des comptes de localisation partenaire (PLA) équivalents à des filiales ou des divisions ailleurs au Royaume-Uni, en France et aux États-Unis. Dans la structure des comptes MPN, ces comptes de localisation partenaire sont représentés sous forme d’ID MPN de localisation uniques. Les comptes de localisation partenaire sont utilisés pour les activités transactionnelles, comme les programmes CSP ou d’incentives. Les règlements sont associés à des sites spécifiques. 

>[!NOTE]
>Il existe une relation 1-1 entre un locataire CSP et un ID MPN de localisation.

:::image type="content" source="images/locations/locations1.png" alt-text="Structure des localisations MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Prérequis pour l’ajout d’un nouveau compte pour une activité CSP

Pour ajouter un nouveau compte commercial CSP, commencez par veiller à remplir les prérequis.

1. Vous devez avoir un ID MPN de localisation dans le pays où vous voulez exercer votre activité CSP. Pour créer une localisation MPN, consultez « Ajouter une localisation MPN » ci-dessous.
  
1. Pour créer un nouvel abonnement CSP Indirect Reseller, lisez [Travailler avec des fournisseurs indirects](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >N’oubliez pas de vous connecter avec les **nouvelles** informations d’identification pour le **nouveau** compte CSP. N’utilisez pas vos informations d’identification existantes, car l’Espace partenaires vous reconnaîtra comme ayant déjà un compte.

2. Acceptez le Contrat Partenaire Microsoft et activez le compte.

1. Si vous souhaitez vous inscrire en tant que Direct Bill Partner, lisez les [Conditions requises qui s’y rattachent](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Afficher et mettre à jour vos localisations MPN

1. Connectez-vous au [tableau de bord](https://partner.microsoft.com/dashboard/home) de l’Espace partenaires avec vos informations d’identification de compte MPN. (Vos informations d’identification MPN peuvent être différentes de vos informations d’identification CSP.) 
 
1. À partir de l’icône **Paramètres**, sélectionnez **Paramètres du compte**, **Profil de l’organisation**, puis **Légal**. 

1. Sous l’onglet **Partenaire**, vérifiez qu’aucune bannière de message d’erreur ne vous invite à corriger les localisations migrées à partir de PMC.  Si vos localisations n’ont pas été correctement définies dans PMC et n’ont pas encore transité vers un PC, vous devez les mettre à jour.

:::image type="content" source="images/locations/location-two.png" alt-text="Capture d’écran montrant comment mettre à jour une localisation.":::
 
4.  Dans l’écran **Vérifier les localisations PMC**, sélectionnez **Mettre à jour**.
Mettez à jour les champs suivants :

- **Champ du nom** : Assurez-vous que le nom de la localisation de la société est correcte. Si une erreur de doublon s’affiche, essayez de remplacer Contoso par Contoso SARL, par exemple.

- **Champ de l’entité juridique** : Assurez-vous d’avoir choisi l’entité juridique à laquelle la localisation est liée.

- **Champs des lignes d’adresse 1 et 2** : Vérifiez que l’adresse est correcte.

- **Champs des ville et département/province** : Assurez-vous que la combinaison entre la ville et le département/la province est correcte. Certains pays ont un menu déroulant pour choisir le département/la province, alors que d’autres ont un champ qui doit être renseigné manuellement.

- **Champ du code postal** : Assurez-vous que le champ du code postal correspond au pays, à la région, à la ville ou à l’adresse indiqué(e).

- **Champs des informations du contact principal** : Assurez-vous que les champs du nom et du prénom sont remplis et que l’adresse e-mail indiquée est une adresse e-mail professionnelle et non personnelle (par exemple, @outlook.com @live.com, etc.)

- **Champ du numéro de téléphone** : Assurez-vous que le numéro de téléphone n’inclut PAS de caractères spéciaux, d’espaces ou d’indicatif. La valeur entrée dans le champ du numéro de téléphone contient toujours un maximum de 10 caractères.

5. Si aucun message d’erreur ne s’affiche, dans **Paramètres**, sélectionnez **Paramètres de compte**, **Profil de l’organisation** et **Identificateurs**.

6. Recherchez l’ID MPN avec le type « localisation » correspondant au pays de ce compte CSP et utilisez-le pour procéder à l’association.

7. Si vous ne trouvez pas l’ID MPN de localisation correspondant au compte CSP que vous souhaitez utiliser, vous pouvez ajouter une nouvelle localisation qui créera un nouvel ID MPN. Consultez **Ajouter une localisation MPN** ci-dessous.

## <a name="add-an-mpn-location"></a>Ajouter une localisation MPN

1. Connectez-vous avec le compte MPN dans l’Espace partenaires. (Vos informations d’identification MPN peuvent être différentes de celles de votre fournisseur de services de chiffrement) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte. 

1. À partir de l’**icône Paramètres**, sélectionnez **Paramètres du compte**, puis **Profil de l’organisation**.

2. Sélectionnez **Légal**. Sous l’onglet **Partenaire**, sélectionnez **Localisations d’entreprise** puis sélectionnez **Ajouter une localisation**.

3. Fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact pour la localisation que vous souhaitez ajouter à votre société.
 
1. Sélectionnez **Ajouter un emplacement**. Un nouvel ID MPN est créé pour la nouvelle localisation que vous pouvez utiliser pour les transactions et incentives CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Ajouter une nouvelle activité légale.":::

> [!NOTE]
> Une fois que vous ajoutez une localisation dans l’Espace partenaires, vous ne pouvez plus la supprimer. Vous verrez **MPN** dans le menu de gauche de l’Espace partenaires si vous avez utilisé le bon ID MPN pour vous connecter.

## <a name="add-the-registration-number-id"></a>Ajouter le numéro d’identification d’inscription

Si vous êtes fournisseur indirect, partenaire à facturation directe ou revendeur indirect et que vous travaillez avec des clients nouveaux ou existants dans les pays suivants, vous devez fournir les numéros d’identification d’inscription de votre entreprise. Si le pays avec lequel vous travaillez ne figure pas dans la liste ci-dessous, l’ID d’inscription est facultatif.

- Arménie 
- Azerbaïdjan 
- Bélarus 
- Brésil 
- Hongrie 
- Inde 
- Irak 
- Kazakhstan 
- Kirghizistan 
- Moldova 
- Myanmar 
- Pologne 
- Russie 
- Arabie Saoudite 
- Afrique du Sud 
- Soudan du Sud  
- Tadjikistan 
- Thaïlande
- Turquie 
- Ukraine 
- Émirats arabes unis 
- Ouzbékistan 
- Venezuela
- Vietnam 


Pour plus d’informations, consultez [Informations sur les numéros d’identification d’inscription](reg-number-id.md).

## <a name="delete-a-location"></a>Supprimer une localisation

Pour supprimer une localisation de votre compte, vous devez contacter [le support de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Veillez à bien comprendre l’impact de cette action. Les localisations supprimées ne peuvent pas être récupérées, et tout ce qui est lié à cet ID MPN n’est plus reconnu ni actif pour votre entreprise.

## <a name="change-country-of-partner-global-account"></a>Changer le pays du compte global du partenaire 

1. Connectez-vous avec le compte MPN dans l’Espace partenaires. (Vos informations d’identification MPN peuvent être différentes de celles de votre fournisseur de services de chiffrement) Le compte MPN doit disposer de privilèges d’administrateur général ou d’administrateur de compte. 

2. Sous l’onglet **Partenaire**, accédez à **Localisations d’entreprise** et vérifiez que la localisation que vous voulez désigner comme entité légale figure bien dans la liste. 
 
1. Pour ajouter une localisation, cliquez sur **Ajouter une localisation**, puis dans le menu volant, fournissez les informations requises, notamment le nom de l’entreprise, l’adresse et le contact principal pour la localisation que vous souhaitez ajouter à votre entreprise. 
 
1. Sélectionnez **Changer votre pays** à côté de la liste déroulante **Pays/région** et suivez les étapes. 

:::image type="content" source="images/lbp.png" alt-text="Menu volant des données de profil de l’entreprise légale.":::

5. Sélectionnez **Enregistrer**.

6. Le pays du compte global MPN sera remplacé par le nouveau pays légal.
  
## <a name="next-steps"></a>Étapes suivantes

- Découvrez plus d’informations sur le [processus de vérification](verification-responses.md).
