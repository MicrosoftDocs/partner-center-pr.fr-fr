---
title: Résoudre les problèmes liés à la configuration de votre compte espace partenaires ou à des problèmes de renouvellement MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Résolvez les problèmes lors de la tentative d’inscription dans l’espace partenaires. Répond aux défis avec les modes de paiement, les oublis de mots de passe et bien plus encore.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431746"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Résoudre les problèmes de configuration de compte ou de renouvellement MPN

**Rôles appropriés**: administrateur général | Administrateur du partenaire MPN
 
Voici quelques suggestions pour résoudre les problèmes courants qui surviennent lors de la configuration de votre compte espace partenaires.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Que se passe-t-il si vous effectuez une migration à partir du centre d’appartenance au partenaire et que vous ne pouvez pas modifier les champs d’informations

Dans les cas où votre société a déjà une présence dans l’espace partenaires (par exemple, un compte fournisseur de solutions Cloud (CSP)), un écran en lecture seule s’affiche. Cet écran affiche toutes les informations sur votre société telles qu’elles existent dans l’espace partenaires.

Vous ne pouvez pas modifier les détails de cet écran. Cela est dû à la conception et non à une erreur.

Pour continuer, sélectionnez **accepter**, puis cliquez sur **Continuer**.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Si le service informatique a désactivé l' **inscription à l’espace partenaires**

Ce message s’affiche parce que les utilisateurs viraux sont désactivés ou parce que l’inscription virale est désactivée sur le locataire Azure Active Directory (AD). L’administrateur général de votre compte Azure AD peut activer les fonctionnalités requises en exécutant la commande PowerShell suivante :

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Pour plus d’informations, consultez [inscription en libre-service](/azure/active-directory/users-groups-roles/directory-self-service-signup).

## <a name="you-forgot-your-password"></a>Vous avez oublié votre mot de passe

Si vous avez oublié votre mot de passe, dans la page de connexion, sélectionnez **ne peut pas accéder à votre compte ?**. Cette option vous permet de réinitialiser votre mot de passe ou de demander à votre administrateur général de vous attribuer de nouvelles informations d’identification.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Sur l’écran « faites-nous part de votre entreprise », vous recevez une erreur « un problème est survenu »

Ce message d’erreur s’affiche généralement si vous utilisez par inadvertance des caractères spéciaux, des espaces ou un code de pays dans le numéro de téléphone de votre entreprise. La valeur entrée dans le champ numéro de téléphone ne peut contenir que 10 caractères au maximum.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Votre achat par carte de crédit reçoit un message d’erreur indiquant que la commande a été refusée. Veuillez vérifier vos informations»


Utilisez toujours l’adresse correspondant à votre carte de crédit plutôt qu’à votre entité légale. En outre, assurez-vous que le code postal est correct et qu’il correspond à l’adresse que vous utilisez.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Vous souhaitez passer du paiement hors connexion au mode de paiement en ligne 

Vous devez annuler la commande d’origine et effectuer un achat à l’aide du mode de paiement par défaut.

Pour annuler une commande :

1. Dans le tableau de bord espace partenaires, sélectionnez l’onglet **offres d’abonnement** .

2. Sélectionner **annuler la commande**

3. Une fenêtre de confirmation s’affiche et vous devez confirmer pour annuler la commande initiale.

## <a name="next-steps"></a>Étapes suivantes

- [Gérer votre compte dans l’Espace partenaires](partner-center-account-setup.md)
- [Comment lire votre facture et votre fichier de rapprochement](read-your-bill.md)
