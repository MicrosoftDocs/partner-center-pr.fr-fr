---
title: Résoudre les problèmes liés à la configuration de votre compte espace partenaires ou à des problèmes de renouvellement MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Résoudre les problèmes liés à l’inscription dans l’espace partenaires
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c1d850663224469f24d5d4442e33cc17c1bb6704
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220237"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Résoudre les problèmes de configuration de compte ou de renouvellement MPN

**S’applique à**

- Espace partenaires
 
**Rôles appropriés**

- Administrateur général
- Administrateur partenaire MPN 
 
Voici quelques suggestions pour résoudre les problèmes courants qui surviennent lors de la configuration de votre compte espace partenaires.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Que se passe-t-il si vous effectuez une migration à partir du centre d’appartenance au partenaire et que vous ne pouvez pas modifier les champs d’informations

Cela se produit dans les cas où votre société a déjà une présence dans l’espace partenaires (par exemple, le compte CSP). vous verrez alors un écran en lecture seule qui affiche toutes les informations relatives à votre société telles qu’elles existent dans l’espace partenaires.

Vous ne pouvez pas modifier les détails de cet écran. Cela est dû à la conception et non à une erreur.

Sélectionnez **accepter** et **Continuer** pour continuer.

## <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Vous essayez d’inscrire ou de migrer à partir du centre d’appartenance au partenaire. vous recevez un message d’erreur indiquant que le service informatique a désactivé l' **inscription à l’espace partenaires**.

Ce message s’affiche parce que les utilisateurs viraux sont désactivés ou que l’inscription virale est désactivée sur le locataire Azure AD. L’administrateur général de votre compte Azure AD peut activer les fonctionnalités requises en exécutant la commande PowerShell suivante :

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Pour plus d’informations, consultez [inscription en libre-service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Vous avez oublié votre mot de passe

Si vous avez oublié votre mot de passe, sélectionnez le lien vous **ne pouvez pas accéder à votre compte ?** sur la page de connexion pour réinitialiser votre mot de passe ou demandez à votre administrateur général de vous attribuer de nouvelles informations d’identification.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Sur l’écran « faites-nous part de votre société », vous recevez une erreur « un problème est survenu »

Cela se produit généralement si vous utilisez par inadvertance des caractères spéciaux, des espaces ou du code de pays dans le numéro de téléphone de votre entreprise. La valeur entrée dans le champ numéro de téléphone ne peut contenir que 10 caractères au maximum.

## <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Vous essayez de terminer l’achat par carte de crédit, mais vous recevez un message d’erreur indiquant que la commande a été refusée. Veuillez vérifier vos informations»

Vous devez toujours insérer l’adresse correspondant à votre carte de crédit et ne correspond pas à votre entité légale. En outre, assurez-vous que le code postal est correct et qu’il correspond à l’adresse que vous utilisez.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Vous souhaitez passer du paiement hors connexion au mode de paiement en ligne 

Vous devez annuler la commande d’origine et effectuer un achat à l’aide du mode de paiement par défaut.

Pour annuler une commande :

1. Sélectionnez l’onglet **offres d’appartenance** dans le tableau de bord.

2. Sélectionner **annuler la commande**

3. Une fenêtre de confirmation s’affiche et vous devez confirmer pour annuler la commande initiale.
