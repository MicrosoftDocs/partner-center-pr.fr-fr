---
title: Exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Présentation de l’activation de l’authentification multifacteur (MFA) et de l’adoption du modèle d’application sécurisé, qui sont maintenant obligatoires pour les partenaires.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: high
ms.openlocfilehash: 146ed2d79c2b98dca6e08f9cf56dbb150e981535
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004978"
---
# <a name="partner-security-requirements"></a>Exigences de sécurité du partenaire

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
  - Facturation directe
  - Fournisseurs indirects
  - Revendeur indirect
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

**Rôles appropriés**
-   Administrateur global
-   Administrateur des utilisateurs
-   Agent d’administration
-   Administration de facturation
-   Administrateur partenaire MPN

L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place. Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.

## <a name="overview"></a>Vue d’ensemble

Les partenaires sont tenus d’appliquer l’authentification multifacteur à tous les comptes d’utilisateur de leur locataire de partenaire. Les termes associés aux exigences de sécurité du partenaire ont été ajoutés au Contrat Partenaire Microsoft. En ce qui concerne les conseillers, les mêmes exigences contractuelles sont en place.

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne pourront pas effectuer de transactions dans le cadre du programme Fournisseur de solutions Cloud, ni gérer les locataires de partenaires en tirant profit des droits d’administrateur délégué, une fois ces exigences appliquées. De plus, les partenaires qui n’implémentent pas les exigences de sécurité peuvent mettre en péril leur participation aux programmes.  

Pour votre protection et celle de vos clients, nous demandons aux partenaires de prendre immédiatement les mesures suivantes :  

1. **Activer l’authentification MFA (Multi-Factor Authentication) pour tous les comptes d’utilisateur de votre locataire de partenaire**. Tous les comptes d’utilisateur de vos locataires de partenaires doivent faire l’objet d’une authentification MFA durant les connexions aux services cloud commerciaux Microsoft, ou durant les transactions liées au programme Fournisseur de solutions Cloud via l’Espace partenaires ou via des API. 

2. **Adopter le framework du modèle d’application sécurisé**. Adoptez le framework du modèle d’application sécurisé. Tous les partenaires qui utilisent l’API de l’Espace partenaires doivent adopter le framework du modèle d’application sécurisé pour toutes les applications du modèle d’authentification d’application/utilisateur.

    > [!IMPORTANT]
    > Nous recommandons fortement aux partenaires d’implémenter le modèle d’application sécurisé pour permettre l’intégration à une API Microsoft telle qu’Azure Resource Manager, Microsoft Graph, ou pour tirer profit de l’automatisation, par exemple avec PowerShell via les informations d’identification de l’utilisateur, afin d’éviter toute interruption de service au moment de l’application de l’authentification MFA.

L’activation de l’authentification MFA et l’adoption du framework du modèle d’application sécurisé contribuent à préserver votre infrastructure et à protéger les données de vos clients contre les risques de sécurité potentiels tels que le vol d’identité ou tout autre incident frauduleux.  

## <a name="actions-that-you-need-to-take"></a>Actions que vous devez effectuer

Pour vous conformer aux exigences de sécurité des partenaires, vous devez appliquer l’authentification multifacteur à chaque compte d’utilisateur de votre locataire de partenaire. Pour ce faire, vous pouvez procéder de l’une des façons suivantes :

- Implémentation des [paramètres de sécurité par défaut d’Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Acheter Azure Active Directory Premium pour chaque compte d’utilisateur. Pour plus d’informations, consultez [Planification d’un déploiement Azure Multi-Factor Authentication basé sur le cloud](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

- Utiliser une solution de tiers pour appliquer l’authentification multifacteur pour chaque compte d’utilisateur de votre locataire partenaire. Pour plus d’informations, consultez [Mode d’application des exigences de sécurité](#how-the-requirements-will-be-enforced) afin de garantir que la solution fournira les informations attendues.

> [!NOTE]
> Bien que l’authentification multifacteur ne soit pas obligatoire pour un cloud souverain (21Vianet, US Government et Germany), il est fortement recommandé d’adopter ces exigences de sécurité.

## <a name="security-defaults"></a>Paramètres de sécurité par défaut

- Les paramètres de sécurité par défaut remplacent les stratégies de base de référence. 

- Les stratégies de base de référence vont rester en vigueur pendant les prochains mois, et le ciblage sera déprécié à la fin de février 2020.

- Les partenaires qui ont déjà adopté des stratégies de base de référence doivent prendre des mesures pour assurer la transition vers les paramètres de sécurité par défaut.

- Avec les paramètres de sécurité par défaut, toutes les stratégies vont être activées en même temps. 

- Pour obtenir des informations détaillées, consultez [Activer l’authentification MFA (Multi-Factor Authentication) pour votre organisation](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-get-started) et [Paramètres de sécurité par défaut d’Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Les paramètres de sécurité par défaut d’Azure AD représentent l’évolution des stratégies de protection de base de référence simplifiées. Si vous avez déjà activé les stratégies de protection de base de référence, il est vivement recommandé d’activer les paramètres de sécurité par défaut.

Pour passer des stratégies de base de référence aux paramètres de sécurité par défaut, consultez [Que sont les paramètres de sécurité par défaut ?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Facteur

Dans la mesure où ces exigences s’appliquent à tous les comptes d’utilisateur de votre locataire de partenaire, vous devez prendre en considération plusieurs éléments pour garantir un déploiement fluide, notamment l’identification des comptes d’utilisateur Azure Active Directory qui ne permettent pas l’authentification multifacteur ainsi que les applications et appareils utilisés par votre organisation, qui ne prennent pas en charge l’authentification moderne.

Avant d’effectuer toute action, nous vous recommandons d’identifier les éléments suivants : 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Avez-vous une application ou un appareil qui ne prend pas en charge l’utilisation de l’authentification moderne ?

Quand vous appliquez l’authentification multifacteur, les protocoles tels qu’IMAP, POP3, SMTP, etc., sont bloqués, car ils ne prennent pas en charge l’authentification multifacteur. Pour dépasser cette limitation, vous pouvez utiliser une fonctionnalité appelée [Mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) afin de vérifier si l’application ou l’appareil peut toujours s’authentifier. Vous devez consulter les considérations relatives à l’utilisation des mots de passe d’application documentées [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer si vous pouvez utiliser ces derniers dans votre environnement.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Avez-vous des utilisateurs qui recourent à Office 365 dans le cadre de licences associées à votre locataire partenaire ?

Avant d’implémenter une solution, nous vous recommandons de déterminer la version de Microsoft Office employée par les utilisateurs de votre locataire de partenaire. Consultez [Planifier l’authentification multifacteur pour les déploiements d’Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) avant d’entreprendre une action. Il y a un risque que vos utilisateurs rencontrent des problèmes de connectivité avec des applications comme Outlook. Avant d’appliquer l’authentification multifacteur, il est important de vérifier qu’Outlook 2013 SP1 ou ultérieur est utilisé et que l’authentification moderne est activée pour votre organisation. Pour plus d’informations, consultez [Activer l’authentification moderne dans Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Pour activer l’authentification moderne pour tous les appareils exécutant Windows et sur lesquels Microsoft Office 2013 est installé, vous devez créer deux clés de registre. Consultez [Activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe-t-il une stratégie qui empêche les utilisateurs de recourir à leurs appareils mobiles quand ils travaillent ?

Il est important d’identifier toute stratégie d’entreprise qui empêche les employés d’utiliser des appareils mobiles quand ils travaillent, car elle influe sur la solution d’authentification multifacteur que vous implémentez. Il existe des solutions, par exemple celle fournie via l’implémentation des [paramètres de sécurité par défaut d’Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), qui autorisent uniquement l’utilisation d’une application d’authentification pour la vérification. Si votre organisation a une stratégie qui empêche l’utilisation d’appareils mobiles, vous devez envisager l’une des options suivantes :

- Déployer une application TOTP (mot de passe à usage unique et durée définie) qui peut s’exécuter sur un système sécurisé

- Implémenter une solution de tiers qui applique l’authentification multifacteur pour chaque compte d’utilisateur du locataire partenaire et qui fournit l’option de vérification la plus appropriée

- Acheter des licences [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) pour les utilisateurs impactés

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quelles sont les fonctionnalités d’automatisation ou d’intégration qui tirent parti des informations d’identification de l’utilisateur pour l’authentification ?

Dans la mesure où il est nécessaire d’appliquer l’authentification MFA pour chaque utilisateur, y compris pour les comptes de service, dans l’annuaire des partenaires, toute automatisation ou intégration qui tire parti des informations d’identification de l’utilisateur pour l’authentification est impactée. C’est pourquoi il est important d’identifier les comptes qui sont utilisés dans ces situations. Voici une liste d’exemples d’applications ou de services qui doivent être pris en compte :

- Panneau de contrôle utilisé pour provisionner les ressources pour le compte de vos clients 

- Intégration à toute plateforme utilisée pour la facturation (par rapport au programme CSP) et prise en charge de vos clients

- Scripts PowerShell qui utilisent les modules Az, AzureRM, Azure AD, MS Online, etc.

La liste ci-dessus n’est pas exhaustive. Il est donc important d’effectuer une évaluation complète de toutes les applications ou services dans votre environnement qui tirent parti des informations d’identification de l’utilisateur pour l’authentification. Pour composer avec l’exigence de l’authentification multifacteur, vous devez, dans la mesure du possible, implémenter les conseils figurant dans le [framework Modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="accessing-your-environment"></a>Accéder à votre environnement

Pour mieux comprendre ce qui est authentifié sans faire l’objet d’une authentification multifacteur, nous vous recommandons de consulter l’activité de connexion. Avec Azure Active Directory Premium, vous pouvez tirer profit du rapport de connexions. Pour plus d’informations, consultez les [rapports d’activité de connexion dans le portail Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins). Si vous n’avez pas Azure Active Directory Premium ou si vous cherchez un moyen de l’obtenir via PowerShell, vous devez tirer profit de l’applet de commande [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) à partir du module [PowerShell de l’Espace partenaires](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Comment les spécifications seront appliquées

Les exigences de sécurité des partenaires seront appliquées par Azure Active Directory et ensuite par l’Espace partenaires, en vérifiant la présence de la revendication MFA pour déterminer si la vérification de l’authentification multifacteur a eu lieu. À partir du 18 novembre 2019, Microsoft va mettre en place des dispositif de protection de la sécurité supplémentaires (anciennement « contraintes techniques ») auprès des locataires de partenaires. 

Au moment de l’activation, les utilisateurs du locataire de partenaire sont invités à effectuer une authentification MFA dans le cadre des opérations AOBO (administration pour le compte de). Nous allons continuer à étendre les dispositifs de protection de la sécurité à d’autres scénarios et rôles d’utilisateur, tout en informant nos partenaires à l’avance. Pour plus d’informations, consultez ce document qui sera mis à jour fréquemment. Les partenaires qui n’ont pas respecté les exigences doivent implémenter ces mesures dès que possible pour éviter toute interruption des activités. 

Si vous utilisez les paramètres de sécurité par défaut de l’authentification MFA (Multi-Factor Authentication) Azure ou d’Azure AD, vous n’avez pas à effectuer d’actions supplémentaires.

Lors de l’utilisation d’une solution d’authentification multifacteur de tiers, il est possible que la revendication MFA ne soit pas émise. Si cette revendication est manquante, Azure Active Directory ne pourra pas déterminer si la demande d’authentification a fait l’objet d’une authentification multifacteur. Pour plus d’informations sur la manière de vérifier si votre solution émet la revendication attendue, consultez [Test des exigences de sécurité du partenaire](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Si votre solution de tiers n’émet pas la revendication attendue, vous devez collaborer avec le fournisseur qui a développé la solution pour déterminer les actions à entreprendre.

## <a name="resources-and-support"></a>Ressources et support

Vous trouverez ci-dessous des ressources de support et des exemples de code :

- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : cette communauté en ligne vous permet de découvrir les événements à venir et de poser des questions.
- [Exemples .NET pour l’Espace partenaires](https://github.com/microsoft/partner-center-dotnet-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de .NET, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Exemples Java pour l’Espace partenaires](https://github.com/microsoft/partner-center-java-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de Java, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Module PowerShell pour l’Espace partenaires - Authentification multifacteur](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) : cet article fournit des détails sur la façon d’implémenter le framework Modèle d’application sécurisé avec PowerShell.
