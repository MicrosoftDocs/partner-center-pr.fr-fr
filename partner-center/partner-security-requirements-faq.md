---
title: Questions fréquentes (FAQ) sur les exigences de sécurité Partenaires
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Questions fréquentes sur les exigences de sécurité Partenaires : ce qu’elles sont, comment les partenaires doivent les implémenter et comment savoir si vous y répondez.'
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 89c53daff52877c9d1facffe8c03e75a1f5b3dae
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998365"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Questions fréquentes sur les exigences de sécurité du partenaire

**Utilisateurs appropriés**

- Tous les utilisateurs activés, y compris les utilisateurs invités

Cet article contient des questions fréquentes sur les [exigences de sécurité du partenaire](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Exigences de sécurité du partenaire

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>Que sont les exigences de sécurité Partenaires, et pourquoi les partenaires doivent-ils les implémenter ?

La qualité et la continuité des mesures de sécurité et de confidentialité font partie de nos principales priorités, et nous continuons à aider les partenaires à protéger leurs clients et leurs locataires. Nous observons un nombre croissant d’attaques de sécurité toujours plus sophistiquées, principalement liées à des incidents de compromission d’identité. Dans la mesure où les contrôles préventifs jouent un rôle clé dans une stratégie de défense globale visant à contrer les attaques de sécurité, nous avons introduit des [exigences de sécurité obligatoires](partner-security-requirements.md) en 2019. Tous les partenaires qui participent au programme Fournisseur de solutions Microsoft Cloud (CSP), les fournisseurs de panneau de contrôle et les conseillers Advisor doivent implémenter les exigences pour rester conformes.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quelle est la chronologie clé et quelles en sont les étapes majeures ?

Les termes associés à ces exigences de sécurité sont inclus dans le Contrat Partenaire Microsoft en 2019. Vous devez implémenter ces exigences de sécurité le plus tôt possible pour garantir la conformité de votre participation au programme Fournisseur de solutions Cloud.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Que se passe-t-il si je n’implémente pas ces exigences de sécurité Partenaires ?

Selon le Contrat Partenaire Microsoft, vous devez appliquer une authentification multifacteur aux comptes d’utilisateur, et vous devez adopter le modèle d’application sécurisé pour interagir avec l’API de l’Espace partenaires. 

Les partenaires qui ne respectent pas ces pratiques de sécurité risquent de ne plus pouvoir effectuer de transactions dans le cadre du programme Fournisseur de solutions Cloud, ou de ne plus pouvoir gérer des locataires de clients à l’aide des droits d’administrateur délégué.

### <a name="does-this-apply-to-all-geographies"></a>Cela s’applique-t-il à toutes les zones géographiques ?

Oui, cela s’applique à toutes les zones géographiques. Nous recommandons vivement que tous les partenaires qui effectuent des transactions par le biais d’un cloud souverain (21Vianet, gouvernement des États-Unis et Allemagne) agissent et adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Est-il possible d’obtenir l’exclusion d’un compte ?

Non, il n’est pas possible d’exclure un compte d’utilisateur de l’obligation d’implémentation de l’authentification MFA. Compte tenu de la nature hautement privilégiée du statut de partenaire, le Contrat Partenaire Microsoft impose l’application de l’authentification multifacteur à chaque compte d’utilisateur de votre locataire de partenaire.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Comment savoir si j’ai répondu aux exigences de sécurité du partenaire ?

Vous devez effectuer les étapes ci-dessous

- Vous devez répondre à toutes les exigences décrites dans [Exigences de sécurité du partenaire](https://docs.microsoft.com/partner-center/partner-security-requirements)
- Vous devez vous assurer que l’authentification multifacteur est appliquée à tous les comptes d’utilisateur de votre locataire partenaire.

Pour vous aider à identifier les domaines clés dans lesquels vous pouvez prendre des mesures, nous fournissons le rapport sur le [statut des exigences de sécurité](https://partner.microsoft.com/pcv/security/compliance) qui est disponible via l’Espace partenaires.

Pour plus d’informations sur le rapport sur le statut, consultez le [statut des exigences de sécurité des partenaires](https://docs.microsoft.com/partner-center/partner-security-compliance).

## <a name="required-actions"></a>Mesures à prendre

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quelles sont les principales mesures à prendre pour satisfaire aux exigences ?

Tous les partenaires du programme Fournisseur de solutions Cloud (facturation directe, fournisseur indirect et revendeur indirect), conseillers Advisor et fournisseurs de panneaux de contrôle doivent satisfaire aux exigences.

1. **Mettre en œuvre l’authentification MFA pour tous les utilisateurs**

    Tous les partenaires du programme Fournisseur de solutions Cloud, les conseillers et les fournisseurs de panneaux de contrôle sont tenus de mettre en œuvre l’authentification MFA pour tous les utilisateurs de leur locataire de partenaire.

    Considérations supplémentaires :

    - Les fournisseurs indirects doivent collaborer avec les revendeurs indirects pour intégrer l’Espace partenaires, s’ils ne l’ont pas déjà fait, et encourager leurs revendeurs à satisfaire aux exigences.
    - Azure MFA est mis gratuitement à la disposition de tous les utilisateurs du locataire de partenaire via les paramètres de sécurité par défaut d’Azure AD avec pour seule méthode de vérification une application d’authentification qui prend en charge les TOTP (mots de passe à usage unique et durée définie).
    - Des méthodes de vérification supplémentaires sont disponibles via les références SKU d’[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium), si d’autres méthodes telles qu'un appel téléphonique ou SMS sont nécessaires.
    - Les partenaires peuvent également tirer parti d’une solution d’authentification MFA tierce pour chaque compte qui accède aux services cloud commerciaux Microsoft.

2. **Adopter le framework du modèle d’application sécurisé**

    Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft. Sinon, cela risque d’entraîner une interruption liée au déploiement de l’authentification MFA. Les ressources suivantes fournissent une vue d’ensemble et de l’aide sur l’adoption du modèle.

    - [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Espace partenaires : guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Si vous utilisez un panneau de contrôle, contactez le fournisseur concernant l’adoption du framework du modèle d’application sécurisé.

    Les fournisseurs de panneaux de contrôle doivent [intégrer](https://docs.microsoft.com/partner-center/enroll-as-cpv) l’Espace partenaires en tant que fournisseurs de panneaux de contrôle et commencer à mettre en œuvre cette exigence immédiatement. Consultez [Espace partenaires : framework du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Les fournisseurs de panneaux de contrôle doivent accepter et gérer le consentement des partenaires du programme Fournisseur de solutions Cloud au lieu d’informations d’identification. De plus, ils doivent vider toutes les informations d’identification existantes des partenaires du programme Fournisseur de solutions Cloud.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Qu’est-ce que l’authentification MFA (Multi-Factor Authentication) ?

L’authentification MFA est un mécanisme de sécurité qui permet aux personnes de s’authentifier via plusieurs procédures de sécurité et de validation. Ce mécanisme fonctionne en imposant deux ou plusieurs des méthodes d’authentification suivantes :

- Quelque chose que vous connaissez (généralement un mot de passe)
- Quelque chose que vous possédez (un périphérique de confiance qui n'est pas facilement dupliqué, comme un téléphone)
- Quelque chose que vous êtes (biométrie)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Quel est le coût de l’activation de l’authentification MFA ?

Microsoft fournit gratuitement une authentification MFA via l’implémentation des paramètres de sécurité par défaut d’Azure AD. La seule option de vérification disponible dans cette version de l’authentification MFA est une application d’authentification. Si un appel téléphonique ou un SMS est nécessaire, vous devez acheter une licence [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Vous pouvez également utiliser une solution tierce pour fournir une authentification MFA à chaque utilisateur du locataire de partenaire. Dans ce cas, il vous incombe de vérifier que votre solution d’authentification MFA est appliquée et que vous êtes en situation de conformité.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Quelles mesures dois-je prendre si j’ai déjà une solution d’authentification MFA ?

Grâce à ces exigences de sécurité, les utilisateurs d’un locataire du partenaire doivent s’authentifier à l’aide de l’authentification MFA quand ils accèdent aux services cloud commerciaux Microsoft. Les solutions tierces permettent de répondre à ces exigences. Microsoft ne fournit plus de tests de validation aux fournisseurs d’identité indépendants en ce qui concerne la compatibilité avec Azure Active Directory. Pour tester l’interopérabilité de votre produit, consultez [ces recommandations](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Quand vous utilisez une solution tierce, il est important de vérifier que cette solution émet la revendication de référence de méthode d’authentification (AMR) qui inclut la valeur MFA. Consultez [Test des exigences de sécurité du partenaire](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) pour plus d’informations sur la façon dont la validation de votre solution tierce émet la revendication attendue.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>J’utilise plusieurs locataires de partenaire pour effectuer des transactions. Dois-je mettre en œuvre l’authentification MFA sur chacun d’eux ?

Oui, vous devez appliquer l’authentification MFA pour chaque locataire Azure Active Directory associé au programme Fournisseur de solutions Cloud ou au programme Advisor. Pour acheter une licence Azure Active Directory Premium, vous devez l’acheter pour chaque utilisateur de chaque locataire Azure Active Directory.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Est-ce que l’authentification MFA doit être appliquée à chaque compte d’utilisateur de mon locataire de partenaire ?

Oui, l’authentification MFA doit être appliquée à chaque utilisateur. Toutefois, si vous utilisez les paramètres de sécurité par défaut d’Azure AD, aucune action supplémentaire n’est nécessaire, car cette fonctionnalité permet d’appliquer l’authentification MFA à tous les comptes d’utilisateur. L’activation des paramètres de sécurité par défaut est un moyen simple et gratuit de garantir la conformité de vos comptes d’utilisateur à l’authentification MFA, et de vérifier qu’ils ne sont pas impactés quand elle est appliquée.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Je suis un partenaire de facturation directe Microsoft. Que dois-je faire ?

Les partenaires de facturation directe du programme Fournisseur de solutions Cloud doivent mettre en œuvre l’authentification MFA pour chaque utilisateur du locataire du partenaire.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Je suis un revendeur indirect et j’effectue des transactions uniquement via un distributeur. Suis-je quand même concerné ?

Tous les revendeurs indirects sont tenus d’appliquer l’authentification MFA pour chaque utilisateur du locataire du partenaire. Il s’agit d’une action que le revendeur indirect doit effectuer.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Je n’utilise pas l’API de l’Espace partenaires. Dois-je quand même mettre en œuvre l’authentification MFA ?

Oui, cette exigence de sécurité concerne tous les utilisateurs, notamment les utilisateurs administrateurs partenaires et les utilisateurs finaux d’un locataire du partenaire.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quels sont les fournisseurs tiers qui proposent des solutions d’authentification MFA compatibles avec Azure Active Directory ?

Durant l’évaluation des fournisseurs et des solutions d’authentification MFA, les partenaires doivent vérifier que la solution choisie est compatible avec Azure Active Directory.

Microsoft ne fournit plus de tests de validation aux fournisseurs d’identité indépendants en ce qui concerne la compatibilité avec Azure Active Directory. Si vous souhaitez tester l’interopérabilité de votre produit, consultez ces [recommandations](https://www.microsoft.com/download/details.aspx?id=56843).

Pour plus d’informations, consultez la [liste de compatibilité de fédération Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Comment puis-je tester l’authentification MFA dans notre bac à sable d’intégration ?

La fonctionnalité des paramètres de sécurité par défaut d’Azure AD doit être activée. Sinon, vous pouvez tirer profit d’une solution tierce basée sur la fédération.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>L’activation de l’authentification MFA a-t-elle un impact sur mon interaction avec le locataire de mon client ?

Non. Le respect de ces exigences de sécurité n’impacte pas la façon dont vous gérez vos clients. Votre capacité à effectuer des opérations d’administration déléguées n’est pas interrompue.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Mes clients sont-ils soumis aux exigences de sécurité du partenaire ?

Non, il n’est pas nécessaire de mettre en œuvre l’authentification MFA pour chaque utilisateur sur les locataires Azure AD de votre client. Toutefois, il est recommandé de déterminer avec chaque client la meilleure façon de protéger ses utilisateurs.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>Un utilisateur peut-il être exclu de cette exigence ?

Non, chaque utilisateur, notamment les comptes de service, du locataire du partenaire doit s’authentifier via l’authentification MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Les exigences de sécurité du partenaire s’appliquent-elles au bac à sable d’intégration ?

Oui, les exigences de sécurité du partenaire s’appliquent au bac à sable d’intégration. Cela signifie que vous devez implémenter la solution d’authentification MFA appropriée pour les utilisateurs du locataire du bac à sable d’intégration. Il est recommandé d’implémenter les paramètres de sécurité par défaut d’Azure AD pour fournir une authentification MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Comment configurer un compte d’accès d’urgence (compte de secours) ?

Parmi les bonnes pratiques, il est recommandé de créer un ou deux comptes d’accès d’urgence pour éviter le verrouillage accidentel de l’accès à votre locataire Azure AD. En ce qui concerne les exigences de sécurité du partenaire, il est nécessaire que chaque utilisateur s’authentifie via l’authentification MFA. Cela signifie que vous devez modifier la définition d’un compte d’accès d’urgence. Il peut s’agir d’un compte qui tire parti d’une solution tierce pour l’authentification MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Les services de fédération Active Directory (ADFS) sont-ils nécessaires si j’utilise une solution tierce ?

Non, les services de fédération Active Directory (ADFS) ne sont pas nécessaires si vous utilisez une solution tierce. Il est recommandé de travailler conjointement avec le fournisseur de la solution pour déterminer les exigences de cette dernière.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Est-il obligatoire d’activer les paramètres de sécurité par défaut d’Azure AD ?

Non, il n’est pas obligatoire d’activer les paramètres de sécurité par défaut d’Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>L’accès conditionnel peut-il être utilisé pour répondre à l’exigence d’authentification MFA ?

Oui, vous pouvez utiliser l’accès conditionnel afin de mettre en œuvre l’authentification MFA pour chaque utilisateur, notamment les comptes de service, sur le locataire du partenaire. Toutefois, compte tenu de la nature hautement privilégiée du statut de partenaire, nous devons vérifier que chaque utilisateur est soumis à l’authentification MFA quand cela s’impose. Cela signifie que vous ne pouvez pas tirer parti de la fonctionnalité d’accès conditionnel qui contourne l’exigence d’authentification MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Le compte de service utilisé par Azure AD Connect est-t-il impacté par les exigences de sécurité du partenaire ?

Non, le compte de service utilisé par Azure AD Connect n’est pas impacté par les exigences de sécurité du partenaire. Si vous rencontrez un problème avec Azure AD Connect en raison de la mise en œuvre de l’authentification MFA, ouvrez une demande de support technique auprès du Support Microsoft.

## <a name="secure-application-model"></a>Modèle d’application sécurisé

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Qui doit adopter le modèle d’application sécurisé pour répondre aux exigences ?

Microsoft propose un framework sécurisé et scalable pour l’authentification des partenaires du programme Fournisseur de solutions Cloud et des fournisseurs de panneaux de contrôle (CPV) qui tirent parti du service Multi-Factor Authentication. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Qu’est-ce que le modèle d’application sécurisé ?

Microsoft propose un framework sécurisé et scalable pour l’authentification des partenaires du programme Fournisseur de solutions Cloud et des fournisseurs de panneaux de contrôle (CPV) qui tirent parti du service Multi-Factor Authentication. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Comment implémenter le modèle d’application sécurisé ?

Tous les partenaires qui ont développé une intégration personnalisée à l’aide d’une API (par exemple Azure Resource Manager, Microsoft Graph, l’API de l’Espace partenaires, etc.) ou qui ont implémenté une automation personnalisée à l’aide d’outils tels que PowerShell doivent adopter le [framework du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) à intégrer aux services cloud Microsoft. Sinon, cela risque d’entraîner une interruption liée au déploiement de l’authentification MFA. Les ressources suivantes fournissent une vue d’ensemble et de l’aide sur l’adoption du modèle.

- [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires : guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Si vous utilisez un panneau de contrôle, vous devez consulter le fournisseur au sujet de l’adoption du framework du modèle d’application sécurisé.

Les fournisseurs de panneaux de contrôle doivent [intégrer](https://docs.microsoft.com/partner-center/enroll-as-cpv) l’Espace partenaires en tant que fournisseurs de panneaux de contrôle et commencer à mettre en œuvre cette exigence immédiatement. Consultez [Espace partenaires : framework du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Les fournisseurs de panneaux de contrôle doivent accepter et gérer le consentement des partenaires du programme Fournisseur de solutions Cloud au lieu d’informations d’identification. De plus, ils doivent vider toutes les informations d’identification existantes des partenaires du programme Fournisseur de solutions Cloud.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Le modèle d’application sécurisé doit-il uniquement être implémenté pour le kit SDK/l’API de l’Espace partenaires ?

En cas d’application de l’authentification multifacteur à tous les comptes d’utilisateur, toute automatisation ou intégration destinée à s’exécuter de manière non interactive est impactée. Bien que les exigences de sécurité du partenaire nécessitent de votre part l’activation du modèle d’application sécurisé pour l’API de l’Espace partenaires, vous pouvez en tirer profit pour répondre au besoin d’un second facteur d’authentification avec l’automatisation et l’intégration. Notez que la ressource faisant l’objet d’un accès doit prendre en charge l’authentification par jeton d’accès.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>J’utilise des outils d’automation tels que PowerShell. Comment implémenter le modèle d’application sécurisé ?

Vous devez implémenter le modèle d’application sécurisé si votre automation doit être exécutée de manière non interactive et si elle repose sur les informations d’identification de l’utilisateur pour l’authentification. Consultez [Modèle d’application sécurisé | Module PowerShell pour l’Espace partenaires](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) pour obtenir de l’aide sur l’implémentation de ce framework.  Notez que tous les outils d’automation ne permettent pas de s’authentifier à l’aide de jetons d’accès. Si vous avez besoin d’aide pour comprendre les changements à apporter, postez un message au groupe d’[aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance). 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quelles sont les informations d’identification de l’utilisateur que l’administrateur d’application doit fournir durant l’exécution du processus de consentement ?

Il est recommandé d’utiliser un compte de service disposant des autorisations les moins privilégiées. En ce qui concerne l’API de l’Espace partenaires, cela signifie que vous devez utiliser un compte auquel le rôle Commercial ou Agent d’administration a été attribué.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Pourquoi l’administrateur d’application ne doit-il pas fournir les informations d’identification de l’utilisateur relatives à l’Administrateur général durant l’exécution du processus de consentement ?

Parmi les bonnes pratiques, il est recommandé d’utiliser les identificateurs les moins privilégiés pour réduire les risques. Il n’est pas recommandé d’utiliser un compte disposant de privilèges d’administrateur général, car cela donne accès à plus d’autorisations que nécessaire.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Je suis un partenaire du programme Fournisseur de solutions Cloud. Comment savoir si mon fournisseur de panneau de contrôle travaille à l’implémentation de la solution ?

Pour les partenaires qui utilisent une solution basée sur un CPV (fournisseur de panneau de contrôle) afin d’effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud, il vous incombe de consulter votre CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Qu’est-ce qu’un fournisseur de panneau de contrôle (CPV) ?

Un fournisseur de panneau de contrôle est un éditeur de logiciels indépendant qui développe des applications que les partenaires du programme Fournisseur de solutions Cloud intègrent aux API de l’Espace partenaires. Un fournisseur de panneau de contrôle n’est pas un partenaire du programme Fournisseur de solutions Cloud ayant un accès direct au tableau de bord ou aux API de l’Espace partenaires. Une description détaillée est disponible dans [Espace partenaires : guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Je suis un CPV. Comment m’inscrire ?

Pour vous inscrire en tant que CPV (fournisseur de panneau de contrôle), suivez les recommandations fournies [ici](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Les CPV doivent contacter [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) pour recevoir le lien d’inscription, et indiquer le nom d’un employé Microsoft sponsor ayant une relation commerciale avec eux ou connaissant leur entreprise. Par exemple, un responsable de développement partenaire Microsoft.

Une fois que vous vous êtes inscrit à l’Espace partenaires et que vous avez inscrit vos applications, vous avez accès aux API de l’Espace partenaires. Si vous êtes un nouveau CPV, vous recevrez les informations relatives au bac à sable via une notification de l’Espace partenaires. Une fois que vous avez effectué votre inscription en tant que CPV Microsoft et que vous avez accepté le contrat CPV, vous pouvez :

1. Gérer les applications multilocataires (ajouter des applications au portail Azure, inscrire et désinscrire des applications dans l’Espace partenaires) Remarque : Les CPV doivent inscrire leurs applications dans l’Espace partenaires pour être autorisés à accéder aux API de l’Espace partenaires. L’ajout d’applications au seul portail Azure n’autorise pas les applications du CPV à accéder aux API de l’Espace partenaires.
2. Visualisez et gérez votre profil de CPV.
3. Visualisez et gérez les utilisateurs ayant besoin d’accéder aux fonctionnalités de CPV. Le seul rôle qu’un CPV peut avoir est celui d’administrateur général.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>J’utilise le kit SDK de l’Espace partenaires. Le kit SDK adopte-t-il automatiquement le modèle d’application sécurisé ?

Non, vous devez suivre les instructions fournies dans le [guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Puis-je générer un jeton d’actualisation pour le modèle d’application sécurisé avec des comptes pour lesquels l’authentification MFA n’est pas activée ?

Oui, vous pouvez générer un jeton d’actualisation à l’aide d’un compte pour lequel l’authentification MFA n’est pas mise en œuvre. Toutefois, cela est déconseillé, car un jeton généré à l’aide d’un compte pour lequel l’authentification MFA n’est pas activée n’a pas accès aux ressources en raison de l’exigence d’authentification MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Comment mon application doit-elle obtenir un jeton d’accès si nous activons l’authentification MFA ?

Vous devez suivre le [guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf), qui explique comment procéder, tout en respectant les nouvelles exigences de sécurité. Vous trouverez un exemple de code .NET [ici](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) et un exemple de code Java [ici](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>En tant que CPV, est-ce que je crée une application Azure AD sur notre locataire de CPV ou sur le locataire du partenaire du programme Fournisseur de solutions Cloud ?

Le CPV doit créer l’application Azure Active Directory sur le locataire associé à son inscription en tant que CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Je suis un fournisseur de solutions Cloud qui utilise l’authentification par application uniquement. Dois-je apporter des changements ?

L’authentification par application uniquement n’est pas impactée, car les informations d’identification de l’utilisateur ne sont pas utilisées pour demander un jeton d’accès. Si les informations d’identification de l’utilisateur sont partagées, les CPV (fournisseurs de panneaux de contrôle) doivent adopter le [framework du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) et vider les informations d’identification de partenaire existantes.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>En tant que CPV, puis-je utiliser l’authentification par application uniquement pour obtenir des jetons d’accès ?

Non, les partenaires fournisseurs de panneaux de contrôle ne peuvent pas utiliser l’authentification par application uniquement pour demander des jetons d’accès au nom du partenaire. Ils doivent implémenter le modèle d’application sécurisé, qui utilise l’authentification d’application + l’authentification utilisateur.

## <a name="technical-enforcement"></a>Mise en œuvre technique

### <a name="what-is-the-activation-of-security-safeguards"></a>Qu’est-ce que l’activation des mesures de sécurité ?

Tous les partenaires qui participent au programme Fournisseur de solutions Microsoft Cloud (CSP), les fournisseurs de panneau de contrôle et les conseillers Advisor doivent implémenter les exigences de sécurité obligatoires pour rester conformes.

Pour renforcer la protection, Microsoft a commencé l’activation de mesures de sécurité qui aident les partenaires à sécuriser leurs locataires et leurs clients en exigeant une vérification MFA afin d’empêcher tout accès non autorisé.  

Nous avons terminé l’activation pour les fonctionnalités « Administrateur pour le compte de » (AOBO) pour tous les locataires partenaires. Afin de renforcer la protection des partenaires et des clients, avec comme objectif le deuxième trimestre 2020, nous allons commencer l’activation pour les transactions de l’Espace partenaires dans CSP, aidant ainsi les partenaires à protéger leurs activités et leurs clients contre les incidents liés au vol d’identité.

Pour plus d’informations, consultez la page [Imposer l’authentification multifacteur (MFA) à votre locataire partenaire](partner-security-requirements-mandating-mfa.md).

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>J’utilise une solution MFA tierce et je suis bloqué. Que dois-je faire ?

Pour valider le fait que le compte accédant aux ressources a fait l’objet d’un test d’authentification multifacteur, nous allons vérifier la revendication de [référence de méthode d’authentification](https://tools.ietf.org/html/rfc8176) pour déterminer si l’authentification multifacteur est listée. Certaines solutions tierces n’émettent pas cette revendication ou n’incluent pas la valeur MFA. Si la revendication est manquante, ou si la valeur MFA n’est pas listée, il n’existe aucun moyen de déterminer si le compte authentifié a fait l’objet d’un test d’authentification multifacteur. Vous devez collaborer avec le fournisseur de votre solution tierce pour déterminer les actions à entreprendre afin que la solution émette la revendication de référence de méthode d’authentification.

Consultez [Test des exigences de sécurité du partenaire](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0) si vous avez des doutes sur le fait que votre solution tierce émette la revendication attendue.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>L’authentification multifacteur m’empêche de prendre en charge mon client utilisant AOBO. Que dois-je faire ?

Les contraintes techniques relatives aux exigences de sécurité du partenaire impliquent de vérifier si le compte authentifié a fait l’objet d’un test d’authentification multifacteur. Dans la négative, vous êtes redirigé vers la page de connexion et vous êtes invité à vous authentifier à nouveau. Découvrez une expérience et des conseils plus détaillés dans cette documentation [Imposer l’authentification multifacteur (MFA) à votre locataire partenaire](partner-security-requirements-mandating-mfa.md#partner-delegated-administration). Dans le scénario dans lequel votre domaine n’est pas fédéré, une fois l’authentification réussie, vous êtes invité à configurer l’authentification multifacteur. Une fois cette opération terminée, vous serez en mesure de gérer vos clients à l’aide d’AOBO. Dans le scénario dans lequel votre domaine est fédéré, vous devez vous assurer que le compte fait l’objet d’un test d’authentification multifacteur.

## <a name="security-defaults-transition"></a>Transition vers les paramètres de sécurité par défaut

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Comment puis-je passer des stratégies de ligne de référence aux paramètres de sécurité par défaut ou d’autres solutions MFA ?

Les [stratégies « ligne de base » Azure Active Directory (Azure AD) sont supprimées et remplacées](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) par les « paramètres de sécurité par défaut », un ensemble plus complet de stratégies de protection pour vous et vos clients. Les [paramètres de sécurité par défaut](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) peuvent aider à protéger votre organisation contre les attaques de sécurité liées au vol d’identité.

Votre implémentation MFA sera supprimée en raison du retrait des stratégies de ligne de base si vous n’avez pas effectué la transition des stratégies de ligne de base vers la stratégie de paramètres de sécurité par défaut ou [d’autres options d’implémentation MFA](partner-security-requirements.md#actions-that-you-need-to-take). Tous les utilisateurs de vos locataires partenaires qui effectuent des opérations d’authentification MFA devront effectuer une vérification MFA. Pour obtenir des recommandations plus détaillées, consultez [cette page](partner-security-requirements-mandating-mfa.md).
Pour rester conforme et réduire les interruptions, effectuez l’une des actions suivantes :

- Transition vers les paramètres de sécurité par défaut
    - La stratégie de paramètres de sécurité par défaut est l’une des options que les partenaires peuvent choisir pour implémenter MFA. Elle offre un niveau de sécurité de base sans coût supplémentaire.
    - Découvrez comment activer MFA pour votre organisation avec Azure AD et passez en revue les [considérations essentielles relatives aux paramètres de sécurité par défaut](partner-security-requirements.md#security-defaults).
    - Activez la stratégie de paramètres de sécurité par défaut si elle répond aux besoins de votre entreprise.
- Transition vers l’accès conditionnel
    - Si la stratégie de paramètres de sécurité par défaut ne répond pas à vos besoins, activez l’accès conditionnel. Pour plus d’informations, consultez la documentation sur l’accès conditionnel Azure AD.

## <a name="key-resources"></a>Ressources clés

### <a name="how-to-get-started"></a>Mise en route

- [Exigences de sécurité du partenaire : guide pas à pas](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Adressez vos questions et commentaires au [Groupe d’aide sur la sécurité de l’Espace partenaires](https://aka.ms/MPCSecurityGuidance).
- Participez aux prochains webinaires pour partenaires qui ont lieu pendant les heures ouvrées. Consultez le [calendrier détaillé et les ressources ici](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Ressources pour l’adoption du modèle d’application sécurisé

- [Vue d’ensemble du modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Espace partenaires : guide du modèle d’application sécurisé](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code .NET pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partenaires du programme Fournisseur de solutions Cloud : exemple de code Java pour l’activation du modèle d’application sécurisé](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Authentification auprès de l’Espace partenaires](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Authentification MFA (Multi-Factor Authentication) via le module PowerShell de l’Espace partenaires](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Assistance

### <a name="where-can-i-get-support"></a>Où puis-je obtenir un support ?

Pour obtenir des ressources de support répondant aux exigences de sécurité, si vous bénéficiez d’un contrat ASfP (support avancé pour les partenaires), contactez votre responsable de compte de service. Si vous bénéficiez d’un contrat PSfP (support Premier pour les partenaires), contactez votre responsable de compte de service et votre responsable de compte technique.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Comment puis-je obtenir des informations techniques et un support pour m’aider à adopter le framework de modèle d’application sécurisé ?

Les options de support technique pour Azure Active Directory sont disponibles via vos avantages MPN. Les partenaires ayant accès à un abonnement ASfP ou PSfP actif peuvent travailler conjointement avec leur responsable de compte associé (gestionnaire des actifs logiciels/responsable technique de compte) pour mieux comprendre les options disponibles.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Comment contacter le support en cas de perte d'accès à l'Espace partenaires ?

Accédez au [Support des partenaires Microsoft](https://partner.microsoft.com/support), puis sélectionnez **Afficher toutes les options de support**. Les options permettant de contacter le Support des partenaires Microsoft s'affichent. Celles-ci incluent un numéro de téléphone pour appeler le support et une option pour converser avec le support. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Où puis-je trouver plus d’informations sur les problèmes techniques courants ?

Vous trouverez des informations sur les problèmes techniques courants [ici](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).

