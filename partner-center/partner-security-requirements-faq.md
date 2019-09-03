---
title: Questions fréquentes (FAQ) sur les exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 08/23/2019
description: Questions fréquentes sur les exigences de sécurité du partenaire
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 54ac919aeadec85b941e0dce9b1556df843e5fcb
ms.sourcegitcommit: 435634c55c3d20a42083c0a58d96c7f6b8ec0a6d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/26/2019
ms.locfileid: "70020543"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Questions fréquentes sur les exigences de sécurité du partenaire

Cet article contient des questions fréquentes sur les [exigences de sécurité du partenaire](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Exigences de sécurité du partenaire

### <a name="what-are-the-new-partner-security-requirements"></a>Quelles sont les nouvelles exigences de sécurité du partenaire ?

Pour protéger nos partenaires et vos clients, nous demandons aux partenaires de prendre immédiatement les mesures suivantes :  

1. **Activer l’authentification MFA (Multi-Factor Authentication) pour tous les utilisateurs des locataires du partenaire**. Tous les utilisateurs des locataires du partenaire doivent utiliser l’authentification MFA (Multi-Factor Authentication) quand ils se connectent aux services cloud commerciaux Microsoft, ou quand ils effectuent des transactions dans le cadre du programme Fournisseur de solutions Cloud via l’Espace partenaires ou via des API. Grâce à l’activation des stratégies de protection de base de référence, l’authentification MFA est disponible gratuitement pour tous les utilisateurs des locataires du partenaire.

2. **Adopter le framework du modèle d’application sécurisé**. Tous les partenaires qui effectuent une intégration à l’aide d’une API Microsoft telle qu’Azure Resource Manager, Microsoft Graph et l’API de l’Espace partenaires doivent adopter le framework du modèle d’application sécurisé pour éviter toute interruption de leur intégration quand les stratégies de base de référence sont activées.

L’activation de l’authentification MFA et l’adoption du framework de modèle d’application sécurisé contribuent à préserver votre infrastructure et à protéger les données de vos clients contre les risques de sécurité potentiels tels que le vol d’identité ou tout autre incident frauduleux.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quels sont les partenaires qui doivent répondre aux exigences ?

Ces exigences concernent les groupes de partenaires suivants :

- Toutes les organisations partenaires qui participent au programme Fournisseur de solutions Cloud (CSP) et qui effectuent des transactions à l’aide des services cloud commerciaux Microsoft
  - Partenaires de facturation directe
  - Fournisseurs indirects
  - Revendeurs indirects
- Tous les fournisseurs de panneau de contrôle
- Tous les partenaires du programme Advisor  

Tous les partenaires qui effectuent des transactions via un cloud souverain (21Vianet, US Government et Germany) ne sont pas tenus de respecter les nouvelles exigences de sécurité dont la date d’entrée en vigueur est prévue pour le 1er août. Toutefois, nous recommandons vivement à tous les partenaires qui utilisent un cloud souverain de prendre les mesures nécessaires et d’adopter immédiatement ces nouvelles exigences de sécurité. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quelle est la chronologie clé et quelles en sont les étapes majeures ?

Les conditions associées à ces exigences de sécurité vont être immédiatement ajoutées au [Guide du programme Fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100). Vous devez implémenter ces exigences de sécurité pour garantir la conformité de votre participation au programme Fournisseur de solutions Cloud dont l’entrée en vigueur est prévue pour le 1er août 2019.

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Que se passe-t-il si je ne prends aucune mesure ?

Les partenaires qui ne se conforment pas à ces pratiques et obligations de sécurité ne pourront pas effectuer de transactions dans le cadre du programme Fournisseur de solutions Cloud, ni gérer les locataires des clients en tirant parti des droits d’administrateur délégué, une fois que les exigences de sécurité relatives aux partenaires auront été mises en œuvre. Nous sommes en train d’établir une date de mise en œuvre de ces exigences, que nous allons notifier aux partenaires avec des informations détaillées.

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>Que se passe-t-il si je n’implémente pas l’authentification MFA conformément aux nouvelles exigences de sécurité d’ici le 1er août 2019 ?

À compter du 1er août 2019, les conditions associées à ces exigences de sécurité dans le [Guide du programme Fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100) entrent en vigueur. Tous les partenaires qui participent au programme Fournisseur de solutions Cloud doivent satisfaire aux exigences pour être en conformité avec les conditions et protéger leur activité. Les partenaires qui ne respectent pas ces pratiques de sécurité risquent de ne plus pouvoir effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud ou de ne plus pouvoir gérer les locataires des clients en tirant parti des droits d’administrateur délégué, une fois que nous aurons commencé à mettre en œuvre les exigences de sécurité relatives aux partenaires. Nous sommes en train d’établir une date de mise en œuvre, que nous allons notifier prochainement aux partenaires.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Pourquoi la société Microsoft met-elle en œuvre ces nouvelles exigences ?

La sécurité et la confidentialité des clients et des partenaires sont la priorité absolue de Microsoft. Nous observons un nombre croissant d’attaques de sécurité toujours plus sophistiquées, principalement liées à des incidents de compromission d’identité. Dans la mesure où les contrôles préventifs jouent un rôle clé dans une stratégie de défense globale visant à contrer les attaques de sécurité, nous allons commencer à mettre en œuvre un ensemble d’exigences de sécurité obligatoires pour améliorer la protection des partenaires et de leurs clients.

### <a name="does-this-apply-to-all-geographies"></a>Cela s’applique-t-il à toutes les zones géographiques ?

Oui, cela s’applique à toutes les zones géographiques. Nous recommandons vivement que tous les partenaires qui effectuent des transactions par le biais d’un cloud souverain (21Vianet, gouvernement des États-Unis et Allemagne) agissent et adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Est-il possible d’obtenir l’exclusion d’un compte ?

Non, il n’est pas possible d’exclure un compte de l’exigence de mise en œuvre de l’authentification MFA. Compte tenu de la nature hautement privilégiée du statut de partenaire, le [Guide du programme Fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100) recommande impérativement la mise en œuvre de l’authentification MFA pour chaque compte de locataire du partenaire.

## <a name="required-actions"></a>Mesures à prendre

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quelles sont les principales mesures à prendre pour satisfaire aux exigences ?

Tous les partenaires du programme Fournisseur de solutions Cloud (facturation directe, fournisseur indirect et revendeur indirect), conseillers Advisor et fournisseurs de panneaux de contrôle doivent satisfaire aux exigences.

1. **Mettre en œuvre l’authentification MFA pour tous les utilisateurs**

    Tous les partenaires du programme Fournisseur de solutions Cloud, les conseillers et les fournisseurs de panneaux de contrôle sont tenus de mettre en œuvre l’authentification MFA pour tous les utilisateurs de leur locataire de partenaire. Pour ce faire, vous devez activer les stratégies de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) ainsi que toutes les stratégies de base de référence à venir. Les fonctionnalités fournies par les stratégies de base de référence vont continuer d’évoluer pour garantir la protection des partenaires et des clients contre les menaces de sécurité en perpétuelle évolution. Il est donc important de consulter la [documentation sur les stratégies de base de référence](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) pour en savoir plus.

    - Consultez [Stratégie de référence : Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) pour savoir comment activer la stratégie de base de référence correspondante.
    - Consultez [Stratégie de référence : Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) pour plus d’informations sur l’activation de la stratégie de base de référence correspondante.
    - Familiarisez-vous avec le concept des [stratégies de protection de base de référence](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considérations supplémentaires :

    - Les fournisseurs indirects doivent collaborer avec les revendeurs indirects pour intégrer l’Espace partenaires, s’ils ne l’ont pas déjà fait, et encourager leurs revendeurs à satisfaire aux exigences.
    - Azure MFA est mis gratuitement à la disposition de tous les utilisateurs du locataire de partenaire via les stratégies de base de référence avec pour seule méthode de vérification l’[application Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Des méthodes de vérification supplémentaires sont disponibles via les références SKU d’[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium), si d’autres méthodes telles que l’envoi de SMS ou d’e-mails sont nécessaires.
    - Les partenaires peuvent également tirer parti d’une solution d’authentification MFA tierce pour chaque utilisateur qui accède aux services cloud commerciaux Microsoft.

2. **Adopter le framework du modèle d’application sécurisé**

    Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft. Sinon, cela risque d’entraîner une interruption liée au déploiement de l’authentification MFA. Les ressources suivantes fournissent une vue d’ensemble et de l’aide sur l’adoption du modèle.

    - [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Espace partenaires : guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Si vous utilisez un panneau de contrôle, vous devez consulter le fournisseur concernant l’adoption du framework du modèle d’application sécurisé.

    Les fournisseurs de panneaux de contrôle doivent [intégrer](https://docs.microsoft.com/partner-center/enroll-as-cpv) l’Espace partenaires en tant que fournisseurs de panneaux de contrôle et commencer à mettre en œuvre cette exigence immédiatement. Consultez [Espace partenaires : framework du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Les fournisseurs de panneaux de contrôle doivent accepter et gérer le consentement des partenaires du programme Fournisseur de solutions Cloud au lieu d’informations d’identification. De plus, ils doivent vider toutes les informations d’identification existantes des partenaires du programme Fournisseur de solutions Cloud.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Qu’est-ce que l’authentification MFA (Multi-Factor Authentication) ?

L’authentification MFA est un mécanisme de sécurité qui permet aux personnes de s’authentifier via plusieurs procédures de sécurité et de validation. Ce mécanisme fonctionne en imposant deux ou plusieurs des méthodes d’authentification suivantes :

- Quelque chose que vous connaissez (généralement un mot de passe)
- Quelque chose que vous possédez (un périphérique de confiance qui n'est pas facilement dupliqué, comme un téléphone)
- Quelque chose que vous êtes (biométrie)

### <a name="what-are-baseline-protection-policies"></a>Que sont les stratégies de protection de base de référence ?

Les [stratégies de protection de base de référence Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (en préversion) constituent un ensemble de stratégies prédéfinies qui permettent de protéger les organisations contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure la pulvérisation de mot de passe, le rejeu et le hameçonnage. Les stratégies de base de référence sont disponibles dans toutes les éditions d’Azure Active Directory. Microsoft met ces stratégies de protection de base de référence à la disposition de tous, car les attaques basées sur l’identité ont augmenté ces dernières années. L’objectif de ces stratégies est de garantir à toutes les organisations l’activation d’un niveau de sécurité de base de référence, sans frais supplémentaires.

> [!NOTE]
> Les stratégies de base de référence Microsoft et les fonctionnalités associées vont continuer d’évoluer pour mieux protéger les partenaires et les clients contre les menaces de sécurité en perpétuelle évolution. Il est possible que des changements liés au nommage et à la taxonomie soient bientôt apportés aux stratégies de base de référence. Nous vous recommandons vivement de consulter directement les pages relatives aux stratégies de base de référence pour obtenir les dernières informations.

### <a name="what-baseline-policies-must-i-enable"></a>Quelles stratégies de base de référence dois-je activer ?

Si vous comptez utiliser les stratégies de protection de base de référence actuelles pour fournir une authentification MFA à chaque utilisateur du locataire du partenaire, vous devez activer les stratégies de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). Ces stratégies de protection de base de référence répondent à l’exigence d’authentification MFA de chaque utilisateur du locataire du partenaire. Elles sont gratuites et s’adressent uniquement aux partenaires qui utilisent les applications Microsoft Authenticator via un appareil mobile.

La stratégie de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) permet de protéger les utilisateurs administratifs de l’annuaire du partenaire, tandis que la stratégie de base de référence [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) sert à protéger les utilisateurs non administratifs du locataire du partenaire. L’activation de ces stratégies oblige les utilisateurs à s’inscrire dans le cadre de l’authentification MFA. Une fois l’utilisateur correctement inscrit, il est soumis à une authentification MFA durant ses tentatives de connexion, en fonction des critères de la stratégie appliquée. Les fonctionnalités fournies par les stratégies de base de référence vont continuer d’évoluer pour garantir la protection des partenaires et des clients contre les menaces de sécurité en perpétuelle évolution. Il est donc important de consulter la [documentation sur les stratégies de base de référence](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) pour en savoir plus.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Comment activer la stratégie Exiger l’authentification MFA pour les administrateurs ?

Vous pouvez activer la stratégie de base de référence Exiger l’authentification MFA pour les administrateurs via le portail de gestion Azure. Consultez [Stratégie de référence : Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) pour savoir comment activer cette stratégie de base de référence.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Comment activer la stratégie Protection de l’utilisateur final ?

Vous pouvez activer la stratégie de base de référence Protection de l’utilisateur final via le portail de gestion Azure. Consultez [Stratégie de référence : Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) pour savoir comment activer cette stratégie de base de référence.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>Les stratégies de base de référence sont-elles automatiquement activées ?

Non, pour activer ces stratégies, un utilisateur membre des rôles Administrateur général, Administrateur de la sécurité ou Administrateur de l’accès conditionnel doit les configurer afin qu’elles soient utilisées immédiatement.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Quel est le coût de l’activation de l’authentification MFA ?

Microsoft fournit gratuitement l’authentification MFA via l’implémentation des stratégies de protection de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). La seule option de vérification disponible dans cette version de l’authentification MFA est l’application [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si un appel téléphonique ou un SMS est nécessaire, vous devez acheter une licence [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Vous pouvez également utiliser une solution tierce pour fournir une authentification MFA à chaque utilisateur du locataire du partenaire. Dans ce cas, il vous incombe de vérifier que votre solution d’authentification MFA est mise en œuvre et que vous êtes en situation de conformité.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Si j’ai déjà une solution d’authentification MFA, quelles mesures dois-je prendre ?

Grâce à ces exigences de sécurité, les utilisateurs d’un locataire du partenaire doivent s’authentifier à l’aide de l’authentification MFA quand ils accèdent aux services cloud commerciaux Microsoft. Une solution tierce permet de répondre à ces exigences. Microsoft ne fournit plus de tests de validation aux fournisseurs d’identité indépendants en ce qui concerne la compatibilité avec Azure Active Directory. Si vous souhaitez tester l’interopérabilité de votre produit, consultez ces [recommandations](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Quelle méthode de vérification puis-je utiliser pour l’authentification MFA ?

Microsoft fournit gratuitement l’authentification MFA via l’implémentation des stratégies de protection de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). La seule option de vérification disponible dans cette version de l’authentification MFA est l’application [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si un appel téléphonique ou un SMS est nécessaire, vous devez acheter une licence [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Vous pouvez également utiliser une solution tierce pour fournir une authentification MFA à chaque utilisateur du locataire du partenaire. Dans ce cas, il vous incombe de vérifier que votre solution d’authentification MFA est mise en œuvre et que vous êtes en situation de conformité.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>J’utilise plusieurs locataires de partenaire pour effectuer des transactions. Dois-je mettre en œuvre l’authentification MFA sur chacun d’eux ?

Oui, vous devez appliquer l’authentification MFA pour chaque locataire Azure Active Directory associé au programme Fournisseur de solutions Cloud ou au programme Advisor. Si vous comptez acheter une licence Azure Active Directory Premium, vous devez l’acheter pour chaque utilisateur de chaque locataire Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Est-ce que l’authentification MFA doit être mise en œuvre pour chaque utilisateur du locataire du partenaire ?*

Les stratégies de protection de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) mettent en œuvre l’authentification MFA pour chaque utilisateur du locataire du partenaire. Si vous tirez parti de ces stratégies pour fournir l’authentification MFA et si vous utilisez l’application [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview), il n’est pas nécessaire d’acheter de licences supplémentaires. Sinon, vous devez acheter une solution appropriée pour fournir l’authentification MFA à chaque utilisateur du locataire du partenaire.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Je suis un partenaire de facturation directe Microsoft. Que dois-je faire ?

Les partenaires de facturation directe du programme Fournisseur de solutions Cloud doivent mettre en œuvre l’authentification MFA pour chaque utilisateur du locataire du partenaire.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Je suis un revendeur indirect et j’effectue des transactions uniquement via un distributeur. Suis-je quand même concerné ?

Tous les revendeurs indirects sont tenus d’appliquer l’authentification MFA pour chaque utilisateur du locataire du partenaire. Il s’agit d’une action que le revendeur indirect doit effectuer.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Je n’utilise pas l’API de l’Espace partenaires. Dois-je quand même mettre en œuvre l’authentification MFA ?

Oui, cette exigence de sécurité concerne tous les utilisateurs, notamment les utilisateurs administrateurs partenaires et les utilisateurs finaux d’un locataire du partenaire.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quels sont les fournisseurs tiers qui proposent des solutions d’authentification MFA compatibles avec Azure Active Directory ?

Il existe de nombreux avis indépendants sur les solutions d’authentification MFA en ligne, par exemple l’évaluation effectuée par [Gartner](https://www.gartner.com/en/webinars/3881781). Durant l’évaluation des fournisseurs et des solutions d’authentification MFA, les partenaires doivent vérifier que la solution choisie est compatible avec Azure Active Directory.

Microsoft ne fournit plus de tests de validation aux fournisseurs d’identité indépendants en ce qui concerne la compatibilité avec Azure Active Directory. Si vous souhaitez tester l’interopérabilité de votre produit, consultez ces [recommandations](https://www.microsoft.com/download/details.aspx?id=56843).

Pour plus d’informations, consultez la [liste de compatibilité de fédération Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Comment puis-je tester l’authentification MFA dans notre bac à sable d’intégration ?

Les stratégies de base de référence [Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) doivent être activées pour le locataire du bac à sable d’intégration. Cette stratégie impose à chaque utilisateur du locataire de s’authentifier via l’authentification MFA.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>L’activation de l’authentification MFA a-t-elle un impact sur mon interaction avec le locataire de mon client ?

Non. Le respect de ces exigences de sécurité n’impacte pas la façon dont vous gérez vos clients. Votre capacité à effectuer des opérations d’administration déléguées n’est pas interrompue.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Mes clients sont-ils soumis aux exigences de sécurité du partenaire ?

Non, il n’est pas nécessaire de mettre en œuvre l’authentification MFA pour chaque utilisateur sur les locataires Azure AD de votre client. Toutefois, il est recommandé de déterminer avec chaque client la meilleure façon de protéger ses utilisateurs.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>Les mots de passe d’application peuvent-ils être utilisés avec les stratégies de protection de base de référence ?

Oui, vous pouvez utiliser les [mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords). Vous devez passer en revue les considérations relatives à l’utilisation des mots de passe d’application documentées [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer si ces derniers sont pris en charge par rapport à vos besoins.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Un utilisateur peut-il être exclu de cette exigence ?

Non, chaque utilisateur, notamment les comptes de service, du locataire du partenaire doit s’authentifier via l’authentification MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Les exigences de sécurité du partenaire s’appliquent-elles au bac à sable d’intégration ?

Oui, les exigences de sécurité du partenaire s’appliquent au bac à sable d’intégration. Cela signifie que vous devez implémenter la solution d’authentification MFA appropriée pour les utilisateurs du locataire du bac à sable d’intégration. Il est recommandé de mettre en œuvre les stratégies de protection de base de référence pour fournir l’authentification MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Comment configurer un compte d’accès d’urgence (compte de secours) ?

Parmi les bonnes pratiques, il est recommandé de créer un ou deux comptes d’accès d’urgence pour éviter le verrouillage accidentel de l’accès à votre locataire Azure AD. En ce qui concerne les exigences de sécurité du partenaire, il est nécessaire que chaque utilisateur s’authentifie via l’authentification MFA. Cela signifie donc que vous devez modifier la définition d’un compte d’accès d’urgence. Il peut s’agir d’un compte qui tire parti d’une solution tierce pour l’authentification MFA.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>Comment les utilisateurs invités vont-ils être impactés par les exigences de sécurité du partenaire ?

Les utilisateurs invités doivent s’authentifier à l’aide de l’authentification MFA quand ils accèdent aux ressources du locataire du partenaire. Les exigences de sécurité du partenaire n’ont aucun impact sur l’utilisateur invité qui accède aux ressources de son propre locataire.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Si j’utilise une solution tierce, les services de fédération Active Directory (ADFS) sont-ils nécessaires ?

Non, les services de fédération Active Directory (ADFS) ne sont pas nécessaires si vous utilisez une solution tierce. Il est recommandé de travailler conjointement avec le fournisseur de la solution pour déterminer les exigences de cette dernière.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>Est-il nécessaire d’activer les stratégies de protection de base de référence ?

Non, il n’est pas nécessaire d’activer les stratégies de protection de base de référence. La seule exigence que vous devez respecter est la mise en œuvre de l’authentification MFA pour chaque utilisateur, notamment les comptes de service, sur le locataire du partenaire.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>L’accès conditionnel peut-il être utilisé pour répondre à l’exigence d’authentification MFA ?

Oui, vous pouvez utiliser l’accès conditionnel afin de mettre en œuvre l’authentification MFA pour chaque utilisateur, notamment les comptes de service, sur le locataire du partenaire. Toutefois, compte tenu de la nature hautement privilégiée du statut de partenaire, nous devons vérifier que chaque utilisateur est soumis à l’authentification MFA quand cela s’impose. Cela signifie que vous ne pouvez pas tirer parti des fonctionnalités d’accès conditionnel qui contournent l’exigence d’authentification MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quelles sont les options de vérification fournies par l’implémentation des stratégies de protection de base de référence ?

En ce qui concerne la version de l’authentification MFA disponible via l’implémentation des stratégies de protection de base de référence, la seule option de vérification disponible est une application d’authentification. L’appel téléphonique et l’envoi d’un sms sont considérés comme des options moins sécurisées. Ces options ne sont donc pas disponibles dans cette version de l’authentification MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Le compte de service utilisé par Azure AD Connect est-t-il impacté par les exigences de sécurité du partenaire ?

Non, le compte de service utilisé par Azure AD Connect n’est pas impacté par les exigences de sécurité du partenaire. Si vous rencontrez un problème avec Azure AD Connect en raison de la mise en œuvre de l’authentification MFA, ouvrez une demande de support technique auprès du Support Microsoft.

## <a name="secure-application-model"></a>Modèle d’application sécurisé

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Qui doit adopter le modèle d’application sécurisé pour répondre aux exigences ?

Microsoft propose un framework sécurisé et scalable pour l’authentification des partenaires du programme Fournisseur de solutions Cloud et des fournisseurs de panneaux de contrôle (CPV) qui tirent parti du service Multi-Factor Authentication. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Qu’est-ce que le modèle d’application sécurisé ?

Microsoft propose un framework sécurisé et scalable pour l’authentification des partenaires du programme Fournisseur de solutions Cloud et des fournisseurs de panneaux de contrôle (CPV) qui tirent parti du service Multi-Factor Authentication. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Comment implémenter le modèle d’application sécurisé ?

Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft. Sinon, cela risque d’entraîner une interruption liée au déploiement de l’authentification MFA. Les ressources suivantes fournissent une vue d’ensemble et de l’aide sur l’adoption du modèle.

- [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires : guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Si vous utilisez un panneau de contrôle, vous devez consulter le fournisseur concernant l’adoption du framework du modèle d’application sécurisé.

Les fournisseurs de panneaux de contrôle doivent [intégrer](https://docs.microsoft.com/partner-center/enroll-as-cpv) l’Espace partenaires en tant que fournisseurs de panneaux de contrôle et commencer à mettre en œuvre cette exigence immédiatement. Consultez [Espace partenaires : framework du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Les fournisseurs de panneaux de contrôle doivent accepter et gérer le consentement des partenaires du programme Fournisseur de solutions Cloud au lieu d’informations d’identification. De plus, ils doivent vider toutes les informations d’identification existantes des partenaires du programme Fournisseur de solutions Cloud.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Qu’est-ce qu’un fournisseur de panneau de contrôle (CPV) ?

Un fournisseur de panneau de contrôle est un éditeur de logiciels indépendant qui développe des applications que les partenaires du programme Fournisseur de solutions Cloud intègrent aux API de l’Espace partenaires. Un fournisseur de panneau de contrôle n’est pas un partenaire du programme Fournisseur de solutions Cloud ayant un accès direct au tableau de bord ou aux API de l’Espace partenaires. Une description détaillée est disponible dans [Espace partenaires : guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Le modèle d’application sécurisé doit-il uniquement être implémenté pour le kit SDK/l’API de l’Espace partenaires ?

Une fois que les stratégies de base de référence *Exiger l’authentification MFA pour les administrateurs* et *Protection de l’utilisateur final* sont activées, chaque utilisateur doit s’authentifier via le service Multi-Factor Authentication. Cela signifie que vous devez implémenter le modèle d’application sécurisé pour chaque API, CLI et module PowerShell (par exemple Azure, Azure AD, MS Online, Espace partenaires, etc.) destiné à s’exécuter de manière non interactive et qui repose sur l’utilisation des informations d’identification de l’utilisateur pour l’authentification.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>J’utilise des outils d’automation tels que PowerShell. Comment implémenter le modèle d’application sécurisé ?

Si votre automation doit être exécutée de manière non interactive et si elle repose sur les informations d’identification de l’utilisateur pour l’authentification, vous devez implémenter le modèle d’application sécurisé. Consultez [Modèle d’application sécurisé | Module PowerShell pour l’Espace partenaires](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) pour obtenir de l’aide sur l’implémentation de ce framework.  Notez que tous les outils d’automation ne permettent pas de s’authentifier à l’aide de jetons d’accès. Si vous avez besoin d’aide pour comprendre les changements à apporter, postez un message au groupe d’[aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quelles sont les informations d’identification de l’utilisateur que l’administrateur d’application doit fournir durant l’exécution du processus de consentement ?

Il est recommandé d’utiliser un compte de service disposant des autorisations les moins privilégiées. En ce qui concerne l’API de l’Espace partenaires, cela signifie que vous devez utiliser un compte auquel le rôle Commercial ou Agent d’administration a été attribué.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Pourquoi l’administrateur d’application ne doit-il pas fournir les informations d’identification de l’utilisateur relatives à l’Administrateur général durant l’exécution du processus de consentement ?

Parmi les bonnes pratiques, il est recommandé d’utiliser les identificateurs les moins privilégiés pour réduire les risques. Il n’est pas recommandé d’utiliser un compte disposant de privilèges d’administrateur général, car cela donne accès à plus d’autorisations que nécessaire

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Je suis un partenaire du programme Fournisseur de solutions Cloud. Comment savoir si mon fournisseur de panneau de contrôle travaille à l’implémentation de la solution ?

Pour les partenaires qui utilisent une solution basée sur un CPV (fournisseur de panneau de contrôle) afin d’effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud, il vous incombe de consulter votre CPV.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Je suis un CPV. Comment m’inscrire ?

Pour vous inscrire en tant que CPV (fournisseur de panneau de contrôle), suivez les recommandations fournies [ici](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Pour recevoir le lien d’inscription, les CPV doivent contacter [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) et indiquer le nom d’un employé Microsoft sponsor ayant une relation commerciale avec eux ou connaissant leur entreprise. Par exemple, un responsable de développement partenaire Microsoft.

Une fois que vous vous êtes inscrit à l’Espace partenaires et que vous avez inscrit vos applications, vous avez accès aux API de l’Espace partenaires. Si vous êtes un nouveau CPV, vous allez recevoir les informations relatives au bac à sable via une notification de l’Espace partenaires. Une fois que vous avez effectué votre inscription en tant que CPV Microsoft et que vous avez accepté le contrat CPV, vous pouvez :

1. Gérer les applications multilocataires (ajouter des applications au portail Azure, inscrire et désinscrire des applications dans l’Espace partenaires) Remarque: Les CPV doivent inscrire leurs applications dans l’Espace partenaires pour être autorisés à accéder aux API de l’Espace partenaires. L’ajout d’applications au seul portail Azure n’autorise pas les applications du CPV à accéder aux API de l’Espace partenaires.
2. Visualisez et gérez votre profil de CPV.
3. Visualisez et gérez les utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV. Le seul rôle qu’un CPV peut avoir est celui d’administrateur général.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>J’utilise le kit SDK de l’Espace partenaires. Le kit SDK adopte-t-il automatiquement le modèle d’application sécurisé ?

Non, vous devez suivre les instructions fournies dans le [guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>Puis-je générer un jeton d’actualisation pour le modèle d’application sécurisé avec des comptes pour lesquels l’authentification MFA n’est pas activée ?

Oui, vous pouvez générer un jeton d’actualisation à l’aide d’un compte pour lequel l’authentification MFA n’est pas mise en œuvre. Toutefois, cela est déconseillé, car un jeton généré à l’aide d’un compte pour lequel l’authentification MFA n’est pas activée n’a pas accès aux ressources en raison de l’exigence d’authentification MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Comment mon application doit-elle obtenir un jeton d’accès si nous activons l’authentification MFA ?

Vous devez suivre le [guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf), qui explique comment procéder, tout en respectant les nouvelles exigences de sécurité. Vous trouverez un exemple de code .NET [ici](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) et un exemple de code Java [ici](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>En tant que CPV, est-ce que je crée une application Azure AD sur notre locataire de CPV ou sur le locataire du partenaire du programme Fournisseur de solutions Cloud ?

Le CPV doit créer l’application Azure Active Directory sur le locataire associé à son inscription en tant que CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Je suis un fournisseur de solutions Cloud qui utilise l’authentification par application uniquement. Dois-je apporter des changements ?

L’authentification par application uniquement n’est pas impactée, car les informations d’identification de l’utilisateur ne sont pas utilisées pour demander un jeton d’accès. Si les informations d’identification de l’utilisateur sont partagées, les CPV (fournisseurs de panneaux de contrôle) doivent adopter le [framework du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) et vider les informations d’identification de partenaire existantes.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>En tant que CPV, puis-je utiliser l’authentification par application uniquement pour obtenir des jetons d’accès ?

Non, les partenaires fournisseurs de panneaux de contrôle ne peuvent pas utiliser l’authentification par application uniquement pour demander des jetons d’accès au nom du partenaire. Ils doivent implémenter le modèle d’application sécurisé, qui utilise l’authentification d’application + l’authentification utilisateur.

## <a name="key-resources"></a>Ressources clés

### <a name="how-to-get-started"></a>Mise en route

- [Exigences de sécurité du partenaire : guide pas à pas](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Adressez vos questions et commentaires au [Groupe d’aide sur la sécurité de l’Espace partenaires](https://aka.ms/MPCSecurityGuidance).
- Participez aux prochains webinaires pour partenaires qui ont lieu pendant les heures ouvrées. Consultez le [calendrier détaillé et les ressources ici](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Ressources pour l’activation de l’authentification MFA

- Familiarisez-vous avec le concept des [stratégies de protection de base de référence](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Consultez [Stratégie de référence : Exiger l’authentification MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) pour savoir comment activer la stratégie de base de référence correspondante.
- Consultez [Stratégie de référence : Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) pour plus d’informations sur l’activation de la stratégie de base de référence correspondante.

### <a name="resources-for-adopting-secure-application-model"></a>Ressources pour l’adoption du modèle d’application sécurisé

- [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires : guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Support

### <a name="where-can-i-get-support"></a>Où puis-je obtenir un support ?

Pour obtenir des ressources de support répondant aux exigences de sécurité, si vous bénéficiez d’un contrat ASfP (support avancé pour les partenaires), contactez votre responsable de compte de service. Si vous bénéficiez d’un contrat PSfP (support Premier pour les partenaires), contactez votre responsable de compte de service et votre responsable de compte technique.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Comment puis-je obtenir de l’aide sur l’activation des stratégies de base de référence ?

- Les partenaires peuvent tirer parti des avantages liés aux heures de conseil MPN pour obtenir une aide détaillée sur l’implémentation des exigences de sécurité.
- Les options de support technique pour Azure Active Directory sont disponibles via vos avantages MPN. Les partenaires ayant accès à un contrat ASfP ou PSfP actif peuvent travailler conjointement avec leur responsable de compte associé (gestionnaire des actifs logiciels/responsable technique de compte) pour mieux comprendre les options disponibles.
- Vous pouvez accéder à la prise en charge de l’implémentation des stratégies de base de référence avec l’Espace partenaires via une [demande de service de l’Espace partenaires](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Sélectionnez la rubrique *Authentification MFA et modèle d’application sécurisé*.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Comment puis-je obtenir des informations techniques et un support pour m’aider à adopter le framework de modèle d’application sécurisé ?

Les options de support technique pour Azure Active Directory sont disponibles via vos avantages MPN. Les partenaires ayant accès à un abonnement ASfP ou PSfP actif peuvent travailler conjointement avec leur responsable de compte associé (gestionnaire des actifs logiciels/responsable technique de compte) pour mieux comprendre les options disponibles.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Où puis-je trouver plus d’informations sur les problèmes techniques courants ?

Vous trouverez des informations sur les problèmes techniques courants [ici](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
