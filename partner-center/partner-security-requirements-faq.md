---
title: FAQ sur les exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 07/18/2019
description: Forum aux questions sur les exigences de sécurité du partenaire
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme fournisseur de solutions Cloud, CSP, fournisseur du panneau de configuration, CPV, Multi-Factor Authentication, MFA, modèle d’application sécurisée, modèle d’application sécurisée, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315548"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Forum aux questions sur les exigences de sécurité du partenaire

Cet article contient des questions fréquemment posées sur les [exigences de sécurité du partenaire](partner-security-requirements.md). Vous trouverez [ici](http://assetsprod.microsoft.com/security-requirements-faq.pdf)une liste complète des questions fréquemment posées.

## <a name="conditional-access"></a>Accès conditionnel

### <a name="can-conditional-access-be-used"></a>L’accès conditionnel peut-il être utilisé?

Oui, vous pouvez utiliser l’accès conditionnel pour appliquer l’authentification multifacteur pour chaque utilisateur, y compris les comptes de service, dans votre locataire partenaire. Toutefois, étant donné la nature hautement privilégiée d’un partenaire, nous devons nous assurer que chaque utilisateur a un défi MFA pour chaque authentification unique. Cela signifie que vous ne pourrez pas tirer parti de la fonctionnalité d’accès conditionnel qui contourne l’exigence de l’authentification MFA.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Mes clients sont-ils soumis aux exigences de sécurité des partenaires?

Non, il n’est pas nécessaire que vous appliquiez l’authentification MFA pour chaque utilisateur dans les locataires Azure AD de votre client. Toutefois, il est recommandé de travailler avec chaque client pour déterminer la meilleure façon de protéger leurs utilisateurs.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>Les mots de passe d’application peuvent-ils être utilisés avec les stratégies de protection de base?

Oui, [les mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) peuvent être utilisés. Vous devez examiner les considérations relatives à l’utilisation des mots de passe d’application documentés [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer s’ils sont pris en charge en cas de besoin.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>L’utilisateur peut-il être exclu de cette exigence? 

Non, chaque utilisateur, y compris les comptes de service, de votre locataire partenaire doit s’authentifier à l’aide de l’authentification multifacteur.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Les exigences de sécurité du partenaire s’appliquent-elles au bac à sable d’intégration?

Oui, les exigences de sécurité du partenaire s’appliquent au bac à sable d’intégration. Cela signifie que vous devez implémenter la solution MFA appropriée pour les utilisateurs dans le client du bac à sable (sandbox) d’intégration. Il est recommandé d’implémenter les stratégies de protection de base pour fournir une authentification MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Comment faire configurer un compte d’accès d’urgence (brise-verre)?

Il a été considéré comme meilleure pratique de créer un ou deux comptes d’accès d’urgence pour empêcher le verrouillage par inadvertance de votre locataire Azure AD. En ce qui concerne les exigences de sécurité du partenaire, il est nécessaire que chaque utilisateur s’authentifie à l’aide de l’authentification multifacteur. Cela signifie que vous devrez modifier la définition d’un compte d’accès d’urgence. Il peut s’agir d’un compte tirant parti d’une solution tierce pour l’authentification multifacteur.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Comment les utilisateurs invités seront-ils affectés par les exigences de sécurité du partenaire?

Les utilisateurs invités devront s’authentifier à l’aide de l’authentification multifacteur lors de l’accès aux ressources de votre locataire partenaire. Les exigences de sécurité du partenaire n’auront aucun impact sur l’utilisateur invité qui accédera aux ressources de son propre locataire.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Si j’utilise une solution tierce, Active Directory service FS (Federation Service) (ADFS) est-il nécessaire? 

Non, il n’est pas nécessaire d’avoir Active Directory service FS (Federation Service) (ADFS) si vous utilisez une solution tierce. Il est recommandé d’utiliser le fournisseur de la solution pour déterminer les exigences de la solution.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>Est-il nécessaire d’activer les stratégies de protection de base?

Non, il n’est pas nécessaire d’activer les stratégies de protection de base. La seule exigence est que vous appliquiez l’authentification MFA pour chaque utilisateur, y compris les comptes de service, dans votre locataire partenaire.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quelles sont les options de vérification fournies par l’implémentation des stratégies de protection de base? 

En ce qui concerne la version de MFA qui est disponible par le biais de l’implémentation des stratégies de protection de base, la seule option de vérification disponible est une application authentificateur. L’utilisation d’un appel téléphonique et d’un message texte est considérée comme moins sécurisée. Par conséquent, ces options ne sont pas disponibles par le biais de cette version de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Le compte de service utilisé par Azure AD Connect sera-t-il affecté par les exigences de sécurité du partenaire?

Non, le compte de service utilisé par Azure AD Connect ne sera pas affecté par les exigences de sécurité du partenaire. Si vous rencontrez un problème avec Azure AD Connect comme résultat de l’application de l’authentification MFA, ouvrez une demande de support technique auprès du support Microsoft.
