---
title: FAQ sur les exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 07/18/2019
description: Forum aux questions sur les exigences de sécurité du partenaire
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme fournisseur de solutions Cloud, CSP, fournisseur du panneau de configuration, CPV, Multi-Factor Authentication, MFA, modèle d’application sécurisée, modèle d’application sécurisée, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820592"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Forum aux questions sur les exigences de sécurité du partenaire

Cet article contient des questions fréquemment posées sur les [exigences de sécurité du partenaire](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Conditions de sécurité pour les partenaires

### <a name="what-are-the-new-partner-security-requirements"></a>Quelles sont les nouvelles exigences en matière de sécurité des partenaires?

Pour protéger nos partenaires et vos clients, nous avons besoin de partenaires pour effectuer immédiatement les actions suivantes:  

1. **Activez Multi-Factor Authentication (MFA) pour tous les utilisateurs dans les locataires partenaires**. Tous les utilisateurs des locataires partenaires doivent utiliser l’authentification multifacteur (MFA) lors de la connexion aux services de Cloud Computing Microsoft ou pour effectuer des transactions dans CSP via l’espace partenaires ou via des API. Grâce à l’activation des stratégies de protection de base, l’authentification MFA est disponible gratuitement pour tous les utilisateurs de locataires partenaires.

2. **Adoptez l’infrastructure de modèle d’application sécurisée**. Tous les partenaires qui s’intègrent à une API Microsoft comme Azure Resource Manager, Microsoft Graph et l’API espace partenaires doivent adopter l’infrastructure de modèle d’application sécurisée pour éviter toute interruption de leur intégration lorsque les stratégies de base sont activées. 
 
L’activation de l’authentification multifacteur (MFA) et l’adoption de l’infrastructure de modèle d’application sécurisée vous aident à protéger votre infrastructure et à protéger les données de vos clients contre les risques de sécurité potentiels, tels que l’identification des vols ou autres incidents de fraude.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quels sont les partenaires qui doivent remplir les conditions requises?

Ces conditions sont requises pour les groupes de partenaires suivants:
- Toutes les organisations partenaires qui participent au programme fournisseur de solutions Cloud (CSP) qui sont en cours d’utilisation par les services Cloud commerciaux Microsoft
  - Partenaires de facturation directe
  - Fournisseurs indirects
  - Revendeurs indirects
- Tous les fournisseurs du panneau de configuration
- Tous les partenaires du programme Advisor  

Tous les partenaires qui passent par un nuage souverain (21Vianet, gouvernement des États-Unis et Allemagne) ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août. Toutefois, nous recommandons vivement à tous les partenaires qui utilisent un Cloud souverain d’agir et d’adopter immédiatement ces nouvelles exigences de sécurité. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quelles sont les chronologies et les jalons clés?

Les conditions associées à ces exigences de sécurité seront ajoutées immédiatement au Guide du programme fournisseur de solutions Cloud. Vous devrez implémenter ces exigences de sécurité pour être en conformité avec votre participation au programme CSP à compter du 1er août 2019. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Que se passe-t-il si je n’effectue aucune action?

Les partenaires qui ne respectent pas ces pratiques et obligations de sécurité ne seront pas en mesure d’effectuer des transactions dans le programme du fournisseur de solutions Cloud ou de gérer les locataires clients en tirant parti des droits d’administrateur délégué, une fois ces exigences de sécurité de partenaire appliquées. Nous sommes en train de mettre en place une date d’application pour les exigences et notifieront les partenaires de la date avec des informations détaillées.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Pourquoi Microsoft applique-t-il ces nouvelles exigences?
La sécurité et la confidentialité des clients et des partenaires sont les priorités principales de Microsoft. Nous continuons à voir les attaques de sécurité plus sophistiquées et plus complexes, principalement liées aux incidents de compromission d’identité. Comme les contrôles de prévention jouent un rôle clé dans une stratégie de défense globale visant à contrer les attaques de sécurité, nous allons commencer à appliquer un ensemble d’exigences de sécurité obligatoires pour aider les partenaires et leurs clients.

### <a name="does-this-apply-to-all-geographies"></a>Cela s’applique-t-il à toutes les zones géographiques?

Oui, cela s’applique à toutes les zones géographiques. Nous vous recommandons vivement de faire en sorte que tous les partenaires passent par un Cloud souverain (21Vianet, gouvernement des États-Unis et Allemagne) et adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

## <a name="required-actions"></a>Actions requises

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quelles sont les principales actions que je dois effectuer pour répondre aux exigences?  
Tous les partenaires du programme CSP (facture directe, fournisseur indirect et revendeur indirect), les conseillers et les fournisseurs du panneau de configuration doivent remplir les conditions requises.

1. **Appliquer MFA pour tous les utilisateurs**

    Tous les partenaires du programme CSP, les conseillers et les fournisseurs du panneau de configuration sont requis pour appliquer l’authentification multifacteur à tous les utilisateurs de leur locataire partenaire. Pour ce faire, vous pouvez activer l’option [exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), la ligne de base de protection de l' [utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)et toutes les futures stratégies de référence. La fonctionnalité fournie par les stratégies de base continuera à évoluer pour garantir la protection des partenaires et des clients contre les menaces de sécurité en perpétuelle évolution. Il est donc important de consulter la documentation des [stratégies de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) pour en savoir plus.

    - Consultez [stratégie de référence: Exiger MFA pour les](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) administrateurs pour plus d’informations sur la façon d’activer la stratégie de base de référence exiger l’authentification MFA pour l’administration.
    - Consultez [stratégie de référence: Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) de l’utilisateur final pour plus d’informations sur l’activation de la stratégie de base de protection de l’utilisateur final.
    - Comprendre le concept des [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considérations supplémentaires:

    - Les fournisseurs indirects doivent travailler avec des revendeurs indirects pour s’intégrer à l’espace partenaires s’ils ne l’ont pas déjà fait et encourager leurs revendeurs à répondre aux exigences.
    - Azure MFA est mis gratuitement à la disposition de tous les utilisateurs du locataire partenaire par le biais des stratégies de base avec la seule méthode de vérification de l’utilisation de l' [application Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Des méthodes de vérification supplémentaires sont disponibles par le biais des références (SKU) [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) , si d’autres méthodes telles que SMS ou e-mail sont requises.
    - Les partenaires peuvent également utiliser une solution MFA tierce pour chaque utilisateur lors de l’accès aux services Cloud commerciaux Microsoft.

2. **Adopter l’infrastructure de modèle d’application sécurisée**

    Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’API (comme Azure Resource Manager, Microsoft Graph, l’API espace partenaires, etc.) ou implémenter une automatisation personnalisée à l’aide d’outils tels que PowerShell devront adopter le [modèle d’application sécurisée. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services Cloud Microsoft. Si vous ne le faites pas, vous risquez d’interrompre le déploiement de MFA. Les ressources suivantes fournissent une vue d’ensemble et des conseils sur la façon d’adopter le modèle.

    - [Vue d’ensemble du modèle d’application sécurisée](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Espace partenaires: Guide de sécurisation du modèle d’application](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partenaires dans le programme CSP: exemple de code .NET pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Partenaires dans le programme CSP: Exemple de code Java pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Document d’authentification de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Document d’authentification multifacteur (MFA) PowerShell de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Si vous utilisez un panneau de configuration, vous devez consulter le fournisseur concernant l’adoption de l’infrastructure de modèle d’application sécurisée.

    Les fournisseurs du panneau de configuration doivent être [intégrés](https://docs.microsoft.com/partner-center/enroll-as-cpv) à l’espace partenaires en tant que fournisseur du panneau de configuration et commencer immédiatement à implémenter cette exigence. Reportez [-vous à l’espace partenaires: Infrastructure](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modèle d’application sécurisée. Les fournisseurs du panneau de configuration doivent accepter et gérer le consentement des partenaires CSP au lieu des informations d’identification et purger les informations d’identification des partenaires CSP existants.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-mfa"></a>Qu’est-ce que MFA?

L’authentification multifacteur (MFA) est un mécanisme de sécurité, mais les individus sont authentifiés par le biais de plusieurs procédures de validation et de sécurité requises. Il fonctionne en exigeant au moins deux des méthodes d’authentification suivantes:

- Quelque chose que vous connaissez (généralement un mot de passe)
- Quelque chose que vous possédez (un périphérique de confiance qui n'est pas facilement dupliqué, comme un téléphone)
- Quelque chose que vous êtes (biométrie)

### <a name="what-are-baseline-protection-policies"></a>Que sont les stratégies de protection de base? 

[Stratégies de Microsoft Baseline protection](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (actuellement en préversion) est un ensemble de stratégies prédéfinies qui permettent de protéger les organisations contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure la pulvérisation de mot de passe, la relecture et le hameçonnage. Les stratégies de base sont disponibles dans toutes les éditions de Azure Active Directory. Microsoft fait en sorte que ces stratégies de protection de base soient disponibles pour tout le monde, car les attaques basées sur les identités ont eu lieu au cours des dernières années. L’objectif de ces stratégies est de s’assurer que toutes les organisations ont un niveau de sécurité de ligne de base activé sans coût supplémentaire.

> [!NOTE]
> Les stratégies de base Microsoft et les fonctionnalités associées continueront d’évoluer pour mieux protéger les partenaires et les clients contre les menaces de sécurité en perpétuelle évolution. Il peut y avoir des modifications de nommage et de taxonomie avec les stratégies de base bientôt disponibles. Nous vous recommandons vivement de consulter les pages des stratégies de base directement pour consulter les dernières informations.

### <a name="what-baseline-policies-must-i-enable"></a>Quelles stratégies de référence dois-je activer?

Si vous envisagez d’utiliser les stratégies de protection de référence actuelles pour fournir une authentification MFA pour chaque utilisateur dans le locataire partenaire, vous devez activer les stratégies de ligne [de base exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et la protection des [utilisateurs finaux](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . Ces stratégies de protection de base répondent à l’exigence d’authentification MFA pour chaque utilisateur du locataire partenaire, gratuitement pour les partenaires qui utilisent des applications Microsoft Authenticator via un appareil mobile.

La [stratégie de ligne de base exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) est exploitée par les utilisateurs administratifs dans l’annuaire des partenaires, et la stratégie de ligne de base de protection de l' [utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) doit être exploitée pour protéger les utilisateurs non administratifs dans le locataire partenaire. L’activation de ces stratégies nécessite que les utilisateurs s’inscrivent pour l’authentification multifacteur. Une fois que l’utilisateur s’est inscrit correctement, il est invité à utiliser l’authentification multifacteur pendant les tentatives de connexion en fonction des critères de la stratégie. La fonctionnalité fournie par les stratégies de base continuera à évoluer pour garantir la protection des partenaires et des clients contre les menaces de sécurité en perpétuelle évolution. Il est donc important de consulter la documentation des [stratégies de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) pour en savoir plus.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Comment faire activer la stratégie exiger l’authentification MFA pour les administrateurs? 

La stratégie de base exiger l’authentification MFA pour les administrateurs peut être activée via le portail de gestion Azure. Consultez [stratégie de référence: Exiger MFA pour les](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) administrateurs pour plus d’informations sur l’activation de cette stratégie de référence.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Comment faire activer la stratégie de protection des utilisateurs finaux?

La stratégie de ligne de base de protection de l’utilisateur final peut être activée via le portail de gestion Azure. Consultez [stratégie de référence: Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) de l’utilisateur final pour plus d’informations sur l’activation de cette stratégie de référence.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>Les stratégies de base seront-elles automatiquement activées? 

Non, pour activer ces stratégies, un utilisateur membre du rôle administrateur général, administrateur de la sécurité ou administrateur de l’accès conditionnel devra configurer les stratégies pour utiliser immédiatement la stratégie.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Quel est le coût de l’activation de l’authentification multifacteur?

Microsoft fournit l’authentification MFA gratuitement par le biais de l’implémentation de l' [authentification MFA pour](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) les stratégies de protection de ligne de base d’administration et de [protection des utilisateurs finaux](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . La seule option de vérification disponible par le biais de cette version de MFA est l' [application Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si un appel téléphonique ou un message SMS est requis, vous devez acheter une licence [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Vous pouvez également utiliser une solution tierce pour fournir une authentification MFA pour chaque utilisateur de votre locataire partenaire. dans ce cas, il vous incombe de vous assurer que votre solution MFA est appliquée et que vous êtes conforme.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Si j’ai déjà une solution MFA, quelles actions dois-je effectuer?

Par le biais de ces exigences de sécurité, les utilisateurs d’un locataire partenaire devront s’authentifier à l’aide de l’authentification multifacteur lors de l’accès aux services Cloud commerciaux Microsoft. Une solution tierce peut être utilisée pour répondre à ces exigences. Microsoft ne fournit plus de test de validation aux fournisseurs d’identité indépendants pour la compatibilité avec Azure Active Directory. Si vous souhaitez tester votre produit à des fins d’interopérabilité, reportez-vous à ces [instructions](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Quelle méthode de vérification puis-je utiliser pour authentifier MFA?

Microsoft fournit l’authentification MFA gratuitement par le biais de l’implémentation de l' [authentification MFA pour](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) les stratégies de protection de ligne de base d’administration et de [protection des utilisateurs finaux](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . La seule option de vérification disponible par le biais de cette version de MFA est l' [application Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si un appel téléphonique ou un message SMS est requis, vous devez acheter une licence [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Vous pouvez également utiliser une solution tierce pour fournir une authentification MFA pour chaque utilisateur de votre locataire partenaire. dans ce cas, il vous incombe de vous assurer que votre solution MFA est appliquée et que vous êtes conforme.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>J’utilise plusieurs locataires partenaires pour la transaction. Dois-je implémenter l’authentification multifacteur?

Oui, vous devez appliquer l’authentification MFA pour chaque Azure Active Directory locataire associé au programme CSP ou au programme Advisor. Si vous envisagez d’acheter une licence Azure Active Directory Premium, une licence doit être achetée pour l’utilisateur dans chaque locataire Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Chaque utilisateur du locataire partenaire doit-il avoir une authentification MFA appliquée? 

L’authentification [MFA pour les stratégies de protection de ligne de base d’administration](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et de protection des [utilisateurs finaux](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) appliquera l’authentification MFA pour chaque utilisateur de votre locataire partenaire. Si vous tirez parti de ces stratégies pour fournir une authentification MFA et que vous utilisez l’application [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) , il n’est pas nécessaire d’acheter des licences supplémentaires. Dans le cas contraire, vous devrez acheter une solution appropriée pour fournir une authentification MFA à chaque utilisateur de votre locataire partenaire.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Je suis partenaire direct de Microsoft. Que dois-je faire?

Les partenaires du fournisseur de solutions direct Bill Cloud doivent appliquer l’authentification MFA pour chaque utilisateur dans son locataire partenaire.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Je suis un revendeur indirect et je suis un distributeur uniquement. Dois-je toujours effectuer cette opération?

Tous les revendeurs indirects sont requis pour appliquer l’authentification multifacteur à chaque utilisateur dans son locataire partenaire. Il s’agit d’une action que le revendeur indirect doit effectuer.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Je n’utilise pas l’API espace partenaires. Dois-je encore implémenter l’authentification multifacteur?

Oui, cette exigence de sécurité concerne tous les utilisateurs, y compris les utilisateurs d’administrateur partenaire et les utilisateurs finaux dans un locataire partenaire.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quels sont les fournisseurs tiers qui fournissent des solutions MFA compatibles avec Azure Active Directory?

Il existe de nombreuses révisions indépendantes des solutions MFA en ligne, comme [Gartner](https://www.gartner.com/en/webinars/3881781). Lors de la révision des fournisseurs et des solutions MFA, les partenaires doivent s’assurer que la solution qu’ils choisissent est compatible avec Azure Active Directory.

Microsoft ne fournit plus de test de validation aux fournisseurs d’identité indépendants pour la compatibilité avec Azure Active Directory. Si vous souhaitez tester votre produit à des fins d’interopérabilité, reportez-vous à ces [instructions](https://www.microsoft.com/download/details.aspx?id=56843).

Pour plus d’informations, consultez la [liste de compatibilité Azure ad](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)de la Fédération.

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Comment puis-je tester l’authentification MFA dans notre bac à sable (sandbox) d’intégration?

Les stratégies [de ligne de base exiger l’authentification MFA pour l’administrateur](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et la protection de l' [utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) doivent être activées pour votre locataire d’intégration sandbox. Par le biais de cette stratégie, chaque utilisateur du locataire devra s’authentifier à l’aide de l’authentification multifacteur.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>L’activation de l’effet MFA permet-elle d’interagir avec le locataire de mon client? 

Non. La réalisation de ces exigences de sécurité n’aura pas d’impact sur la façon dont vous gérez vos clients. Votre capacité à effectuer des opérations administratives déléguées ne sera pas interrompue.

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

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>L’accès conditionnel peut-il être utilisé pour répondre à l’exigence d’authentification multifacteur?

Oui, vous pouvez utiliser l’accès conditionnel pour appliquer l’authentification multifacteur pour chaque utilisateur, y compris les comptes de service, dans votre locataire partenaire. Toutefois, étant donné la nature hautement privilégiée d’un partenaire, nous devons nous assurer que chaque utilisateur a un défi MFA pour chaque authentification unique. Cela signifie que vous ne pourrez pas tirer parti de la fonctionnalité d’accès conditionnel qui contourne l’exigence de l’authentification MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quelles sont les options de vérification fournies par l’implémentation des stratégies de protection de base? 

En ce qui concerne la version de MFA qui est disponible par le biais de l’implémentation des stratégies de protection de base, la seule option de vérification disponible est une application authentificateur. L’utilisation d’un appel téléphonique et d’un message texte est considérée comme moins sécurisée. Par conséquent, ces options ne sont pas disponibles par le biais de cette version de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Le compte de service utilisé par Azure AD Connect sera-t-il affecté par les exigences de sécurité du partenaire?

Non, le compte de service utilisé par Azure AD Connect ne sera pas affecté par les exigences de sécurité du partenaire. Si vous rencontrez un problème avec Azure AD Connect comme résultat de l’application de l’authentification MFA, ouvrez une demande de support technique auprès du support Microsoft.

## <a name="secure-application-model"></a>Modèle d’application sécurisée

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Qui doit adopter le modèle d’application sécurisée pour répondre aux besoins?

Microsoft propose une infrastructure sécurisée et évolutive pour l’authentification des partenaires du fournisseur de solutions Cloud (CSP) et des fournisseurs du panneau de configuration (CPV) qui tirent parti de l’authentification multifacteur. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) . Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’API (comme Azure Resource Manager, Microsoft Graph, l’API espace partenaires, etc.) ou implémenter une automatisation personnalisée à l’aide d’outils tels que PowerShell devront adopter le [modèle d’application sécurisée. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services Cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Qu’est-ce que le modèle d’application sécurisée?

Microsoft propose une infrastructure sécurisée et évolutive pour l’authentification des partenaires du fournisseur de solutions Cloud (CSP) et des fournisseurs du panneau de configuration (CPV) qui tirent parti de l’authentification multifacteur. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Comment faire implémenter le modèle d’application sécurisée?

Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’API (comme Azure Resource Manager, Microsoft Graph, l’API espace partenaires, etc.) ou implémenter une automatisation personnalisée à l’aide d’outils tels que PowerShell devront adopter le [modèle d’application sécurisée. Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services Cloud Microsoft. Si vous ne le faites pas, vous risquez d’interrompre le déploiement de MFA. Les ressources suivantes fournissent une vue d’ensemble et des conseils sur la façon d’adopter le modèle.

- [Vue d’ensemble du modèle d’application sécurisée](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires: Guide de sécurisation du modèle d’application](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires dans le programme CSP: exemple de code .NET pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partenaires dans le programme CSP: Exemple de code Java pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Document d’authentification de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Document d’authentification multifacteur (MFA) PowerShell de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Si vous utilisez un panneau de configuration, vous devez consulter le fournisseur concernant l’adoption de l’infrastructure de modèle d’application sécurisée.

Les fournisseurs du panneau de configuration doivent être [intégrés](https://docs.microsoft.com/partner-center/enroll-as-cpv) à l’espace partenaires en tant que fournisseur du panneau de configuration et commencer immédiatement à implémenter cette exigence. Reportez [-vous à l’espace partenaires: Infrastructure](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modèle d’application sécurisée. Les fournisseurs du panneau de configuration doivent accepter et gérer le consentement des partenaires CSP au lieu des informations d’identification et purger les informations d’identification des partenaires CSP existants.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Qui est fournisseur du panneau de configuration (CPV)? 
Un fournisseur du panneau de configuration est un éditeur de logiciels indépendant qui développe des applications qui sont utilisées par les partenaires CSP pour s’intégrer aux API de l’espace partenaires. Un fournisseur du panneau de configuration n’est pas un partenaire CSP disposant d’un accès direct au tableau de bord ou aux API de l’espace partenaires. Une description détaillée est disponible dans l' [espace partenaires: Guide](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)du modèle d’applications sécurisées.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Le modèle d’application sécurisée doit-il être implémenté uniquement pour l’API/le kit de développement logiciel (SDK) de l’espace partenaires? 

Une fois que les stratégies exiger l’authentification *MFA pour les administrateurs* et la ligne de base de *protection des utilisateurs finaux* sont activées, chaque utilisateur doit s’authentifier à l’aide de Multi-Factor Authentication. Cela signifie que vous devez implémenter le modèle d’application sécurisée pour chaque API, CLI et module PowerShell (par exemple, Azure, Azure AD, MS Online, Partner Center, etc.) qui est destiné à s’exécuter de manière non interactive et qui s’appuie sur l’utilisation des informations d’identification de l’utilisateur pour l’authentification.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>J’utilise des outils d’automatisation tels que PowerShell. Comment faire implémenter le modèle d’application sécurisée?  

Si votre Automation est destinée à être exécutée de manière non interactive et s’appuie sur les informations d’identification de l’utilisateur pour l’authentification, vous devez implémenter le modèle d’application sécurisée. Voir le [modèle d’application sécurisée | Centre de partenaires PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) pour obtenir des conseils sur la façon d’implémenter ce Framework.  Notez que tous les outils d’automatisation n’offrent pas la possibilité de s’authentifier à l’aide de jetons d’accès. Si vous avez besoin d’aide pour comprendre les modifications qui doivent être apportées, publiez un message sur le groupe de conseils de sécurité de l' [espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quelles sont les informations d’identification de l’utilisateur que l’administrateur d’application doit fournir lors de l’exécution du processus de consentement? 

Il est recommandé d’utiliser un compte de service auquel ont été attribuées les autorisations les plus faibles. En ce qui concerne l’API espace partenaires, cela signifie que vous devez utiliser un compte auquel a été attribué le rôle agent de vente ou agents d’administration.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Pourquoi l’administrateur de l’application ne peut-il pas fournir d’informations d’identification d’administrateur général lors de l’exécution du processus de consentement?

Il est recommandé d’utiliser le moins de privilèges pour identifier la façon dont vous réduisez le risque. Il n’est pas recommandé d’utiliser un compte disposant de privilèges d’administrateur général, car cela fournirait plus d’autorisations que ce qui est requis

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Je suis un partenaire CSP. Comment faire savez-vous si mon fournisseur du panneau de configuration (CPV) travaille à l’implémentation de la solution? 

Pour les partenaires qui utilisent une solution de fournisseur du panneau de configuration (CPV) pour effectuer des transactions dans le programme fournisseur de solutions Cloud (CSP), il vous incombe de consulter votre CPV. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Je suis un CPV. Comment faire inscrire? 

Pour vous inscrire en tant que fournisseur du panneau de configuration (CPV), suivez les instructions fournies [ici](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Pour pouvoir recevoir le lien d’inscription, CPVs doit contacter [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) et fournir un sponsor d’employés Microsoft qui a une relation commerciale avec le CPV ou connaît son activité. Par exemple, un responsable du développement partenaire (PDM).

Une fois inscrit dans l’espace partenaires et inscrit vos applications, vous avez accès aux API de l’espace partenaires. Si vous êtes un nouveau CPV, vous recevrez vos informations de bac à sable (sandbox) via une notification de l’espace partenaires. Une fois que vous avez terminé l’inscription en tant que Microsoft CPV et accepté le contrat CPV, vous pouvez:

1. Gérer une application mutualisée (ajouter des applications à Portail Azure, inscrire et désinscrire des applications dans l’espace partenaires). Remarque : CPVs doit inscrire ses applications dans l’espace partenaires pour être autorisé à accéder aux API de l’espace partenaires. L’ajout d’applications au Portail Azure seul n’autorise pas les applications CPV pour les API de l’espace partenaires.
2. Affichez et gérez votre profil CPV.
3. Affichez et gérez les utilisateurs qui ont besoin d’accéder aux fonctionnalités du CPV. Le seul rôle qu’un CPV peut avoir est l’administrateur général.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>J’utilise le kit de développement logiciel (SDK) de l’espace partenaires. Le SDK adoptera-t-il automatiquement le modèle d’application sécurisé? 

Non, vous devrez suivre les instructions fournies dans le Guide du [modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Puis-je générer un jeton d’actualisation pour le modèle d’application sécurisée avec des comptes pour lesquels l’authentification MFA n’est pas activée?

Oui, un jeton d’actualisation peut être généré à l’aide d’un compte pour lequel l’authentification MFA n’est pas appliquée. Toutefois, cela ne doit pas être fait parce que tout jeton généré à l’aide d’un compte pour lequel l’authentification MFA n’est pas activée ne pourra pas accéder aux ressources en raison de l’exigence de l’authentification multifacteur.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Comment mon application doit-elle obtenir un jeton d’accès si nous activons l’authentification MFA?

Vous devez suivre le Guide du [modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) qui fournit des détails sur la façon de procéder, tout en respectant les nouvelles exigences en matière de sécurité. Vous trouverez [ici](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) un exemple de code .net et un exemple de code Java [ici](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>En guise de CPV, dois-je créer une application Azure AD dans notre locataire du CPV ou le locataire du partenaire CSP?

Le CPV devra créer l’application Azure Active Directory dans le locataire associé à son inscription en tant que CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Je suis un fournisseur de services de chiffrement qui utilise l’authentification d’application uniquement. Dois-je apporter des modifications?

L’authentification de l’application uniquement n’est pas affectée car les informations d’identification de l’utilisateur ne sont pas utilisées pour demander un jeton d’accès. Si les informations d’identification de l’utilisateur sont partagées, les fournisseurs du panneau de configuration (CPVs) doivent adopter l' [infrastructure de modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) et purger les informations d’identification de partenaire existantes.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>En guise de CPV, puis-je tirer parti du style d’authentification de l’application uniquement pour obtenir des jetons d’accès?

Non, le panneau de configuration les partenaires fournisseurs ne peuvent pas utiliser le style d’authentification application uniquement pour demander des jetons d’accès pour le compte du partenaire. Ils doivent implémenter le modèle d’application sécurisée, qui utilise le style d’authentification de l’application + utilisateur.

## <a name="key-resources"></a>Ressources clés

### <a name="how-to-get-started"></a>Mise en route

- [Conditions de sécurité pour les partenaires: Guide pas à pas](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Envoyez vos questions et vos commentaires à ce groupe de conseils de sécurité de l' [espace partenaires](https://aka.ms/MPCSecurityGuidance).
- Assistez aux prochains horaires et webinaires des partenaires. Veuillez consulter la [planification détaillée et les ressources ici](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Ressources pour l’activation de l’authentification multifacteur

- Comprendre le concept des [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Consultez [stratégie de référence: Exiger MFA pour les](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) administrateurs pour plus d’informations sur la façon d’activer la stratégie de base de référence exiger l’authentification MFA pour l’administration.
- Consultez [stratégie de référence: Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) de l’utilisateur final pour plus d’informations sur l’activation de la stratégie de base de protection de l’utilisateur final.

### <a name="resources-for-adopting-secure-application-model"></a>Ressources pour l’adoption d’un modèle d’application sécurisée

- [Vue d’ensemble du modèle d’application sécurisée](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires: Guide de sécurisation du modèle d’application](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires dans le programme CSP: exemple de code .NET pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partenaires dans le programme CSP: Exemple de code Java pour l’activation du modèle d’application sécurisée](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Document d’authentification de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Document d’authentification multifacteur (MFA) PowerShell de l’espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Assistance

### <a name="where-can-i-ask-get-support"></a>Où puis-je demander un support technique?

En outre, pour la prise en charge de l’utilisation des ressources pour répondre aux exigences de sécurité, si vous avez un support avancé pour les partenaires (ASfP), contactez votre responsable de compte de service. pour Support Premier accord des partenaires (PSfP), contactez votre responsable de compte de service et votre responsable technique de compte.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Comment puis-je obtenir de l’aide pour l’activation des stratégies de base?

- Les partenaires peuvent tirer parti des heures d’avis des avantages MPN pour obtenir des conseils plus détaillés sur la façon d’implémenter les exigences de sécurité.
- Les options de support technique pour Azure Active Directory sont disponibles par le biais de vos avantages MPN. Les partenaires ayant accès à un contrat ASfP ou PSfP actif peuvent travailler avec leur gestionnaire de compte associé (SAM/TAM) pour mieux comprendre les options disponibles.
- La prise en charge de l’implémentation des stratégies de référence avec l’espace partenaires est accessible via la demande de service de l' [espace partenaires](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Sélectionnez *MFA & modèle d’application sécurisée* comme rubrique.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>Comment faire obtenir des informations techniques pour adopter l’infrastructure de modèle d’application sécurisée? 

Les options de support technique pour Azure Active Directory sont disponibles par le biais de vos avantages MPN. Les partenaires ayant accès à un abonnement actif ASfP ou PSfP peuvent travailler avec leur gestionnaire de compte associé (SAM/TAM) pour mieux comprendre les options disponibles.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Où puis-je trouver plus d’informations sur les problèmes techniques courants? 

Vous trouverez des informations sur les problèmes techniques courants [ici](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
