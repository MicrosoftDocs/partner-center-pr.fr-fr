---
title: Exigences de sécurité pour les partenaires
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Présente les exigences de sécurité des partenaires pour activer l’authentification multifacteur (MFA) et adopter le framework Modèle d’application sécurisé.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132975"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Exigences de sécurité concernant l’utilisation de l’Espace partenaires ou des API de l’Espace partenaires

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

**Utilisateurs appropriés**

- Tous les utilisateurs activés, y compris les utilisateurs invités

Cet article explique les exigences de sécurité obligatoires pour les conseillers Advisor, les fournisseurs de panneau de contrôle et les partenaires qui participent au programme Fournisseur de solutions Cloud, ainsi que les options d’authentification et d’autres considérations relatives à la sécurité. La sécurité et la protection de la confidentialité font partie de nos priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et vérifier que les protections de sécurité appropriées sont en place.

## <a name="mandatory-security-requirements"></a>Exigences de sécurité obligatoires

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne pourront pas effectuer de transactions dans le cadre du programme Fournisseur de solutions Cloud, ni gérer les locataires partenaires en tirant profit des droits d’administrateur délégué. De plus, les partenaires qui n’implémentent pas les exigences de sécurité peuvent mettre en péril leur participation aux programmes. Les termes associés aux exigences de sécurité du partenaire ont été ajoutés au Contrat Partenaire Microsoft. En ce qui concerne les conseillers, les mêmes exigences contractuelles s’appliquent.

Pour votre protection et celle de vos clients, nous demandons aux partenaires de prendre immédiatement les mesures suivantes :  

1. **Activer l’authentification multifacteur (MFA) pour tous les comptes d’utilisateur de votre locataire partenaire**. Vous devez appliquer MFA sur tous les comptes d’utilisateur de vos locataires partenaires. Les utilisateurs doivent faire l’objet d’un test MFA durant les connexions aux services cloud commerciaux Microsoft ou durant les transactions effectuées dans le cadre du programme Fournisseur de solutions Cloud par le biais de l’Espace partenaires ou d’API.

2. **Adopter le framework du modèle d’application sécurisé**. Tous les partenaires qui utilisent les API de l’Espace partenaires doivent adopter le [framework du modèle d’application sécurisé](/partner-center/develop/enable-secure-app-model) pour toutes les applications du modèle d’authentification d’application/utilisateur.

    > [!IMPORTANT]
    > Nous recommandons vivement aux partenaires d’implémenter le modèle d’application sécurisé pour permettre l’intégration à une API Microsoft telle qu’Azure Resource Manager ou Microsoft Graph, ou pour tirer profit de l’automatisation, par exemple avec PowerShell à l’aide des informations d’identification de l’utilisateur, afin d’éviter toute interruption de service au moment de l’application de MFA.

Ces exigences de sécurité vous aideront à protéger votre infrastructure et à protéger les données de vos clients contre les risques de sécurité potentiels, notamment l’usurpation d’identité ou d’autres incidents de fraude.  

## <a name="implementing-multi-factor-authentication"></a>Implémentation de l’authentification multifacteur

Pour vous conformer aux exigences de sécurité des partenaires, vous devez implémenter et appliquer MFA pour chaque compte d’utilisateur de votre locataire partenaire. Pour cela, plusieurs méthodes sont possibles :

- Implémenter [les paramètres de sécurité par défaut d’Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Pour en savoir plus, consultez la [section suivante](#security-defaults).

- Acheter Azure Active Directory Premium pour chaque compte d’utilisateur. Pour plus d’informations, consultez [Planifier un déploiement Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Utiliser une solution tierce pour appliquer MFA pour chaque compte d’utilisateur de votre locataire partenaire. Pour garantir que la solution fournira la solution attendue, consultez [Mode d’application des exigences de sécurité](#how-the-requirements-are-enforced).

> [!NOTE]
> Bien que l’authentification multifacteur ne soit pas obligatoire pour un cloud souverain (US Government et Allemagne), il est vivement recommandé d’adopter ces exigences de sécurité.

### <a name="security-defaults"></a>Paramètres de sécurité par défaut

L’une des options que les partenaires peuvent choisir pour implémenter MFA est d’activer les paramètres de sécurité par défaut dans Azure AD. Les paramètres de sécurité par défaut offrent un niveau de sécurité de base sans coût supplémentaire. Avant d’activer les paramètres de sécurité par défaut, examinez ci-dessous les principaux éléments à prendre en considération et découvrez comment activer MFA pour votre organisation avec Azure AD.

- Les partenaires qui ont déjà adopté des stratégies de base de référence doivent prendre des mesures pour assurer la transition vers les paramètres de sécurité par défaut.

- Les paramètres de sécurité par défaut, désormais en disponibilité générale, remplacent les stratégies de référence en préversion. Une fois qu’un partenaire active les paramètres de sécurité par défaut, il ne peut plus activer les stratégies de référence.

- Avec les paramètres de sécurité par défaut, toutes les stratégies vont être activées en même temps.

- Pour les partenaires qui utilisent l’[accès conditionnel](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), les [paramètres de sécurité par défaut ne sont pas disponibles](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Nous ne bloquons pas l’authentification héritée pour l’instant. Cependant, dans la mesure où la plupart des événements liés aux identités compromises viennent de tentatives de connexion utilisant l’authentification héritée, les partenaires sont encouragés à abandonner ces anciens protocoles.

- Le compte de synchronisation Azure AD Connect est exclu des paramètres de sécurité par défaut.

Pour obtenir des informations détaillées, consultez la [vue d’ensemble d’Azure Multi-Factor Authentication pour votre organisation](/azure/active-directory/authentication/concept-mfa-get-started) et la [présentation des paramètres de sécurité par défaut](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Les paramètres de sécurité par défaut d’Azure AD représentent l’évolution des stratégies de protection de base de référence simplifiées. Si vous avez déjà activé les stratégies de protection de base de référence, il est vivement recommandé d’activer les [paramètres de sécurité par défaut](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Considérations relatives à l’implémentation

Comme ces exigences s’appliquent à tous les comptes d’utilisateur de votre locataire partenaire, vous devez prendre en compte plusieurs éléments pour garantir un déploiement sans problèmes. Pae exemple, identifiez les comptes d’utilisateur dans Azure AD qui ne peuvent pas effectuer MFA, ainsi que les applications et les appareils utilisés dans votre organisation qui ne prennent pas en charge l’authentification moderne.

Avant d’effectuer toute action, nous vous recommandons de procéder aux validations suivantes. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Avez-vous une application ou un appareil qui ne prend pas en charge l’utilisation de l’authentification moderne ?

Quand vous appliquez MFA, les protocoles d’authentification hérités tels qu’IMAP, POP3, SMTP, etc. sont bloqués, car ils ne prennent pas en charge MFA. Pour passer outre cette limitation, utilisez la fonctionnalité [Mots de passe d’application](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pour que l’application ou l’appareil puisse toujours s’authentifier. Passez en revue les [considérations relatives à l’utilisation des mots de passe d’application](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer si vous pouvez utiliser ces derniers dans votre environnement.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Avez-vous des utilisateurs Office 365 avec des licences associées à votre locataire partenaire ?

Avant d’implémenter une solution, nous vous recommandons de déterminer la version de Microsoft Office employée par les utilisateurs de votre locataire de partenaire. Il y a un risque que vos utilisateurs rencontrent des problèmes de connectivité avec des applications comme Outlook. Avant d’appliquer MFA, il est important de vérifier que vous utilisez Outlook 2013 SP1 ou ultérieur et que l’authentification moderne est activée pour votre organisation. Pour plus d’informations, consultez [Activer l’authentification moderne dans Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Pour activer l’authentification moderne pour les appareils exécutant Windows et sur lesquels Microsoft Office 2013 est installé, vous devez créer deux clés de registre. Consultez [Activer l’authentification moderne pour Office 2013 sur les appareils Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe-t-il une stratégie qui empêche les utilisateurs de recourir à leurs appareils mobiles quand ils travaillent ?

Il est important d’identifier toute stratégie d’entreprise qui empêche les employés d’utiliser des appareils mobiles quand ils travaillent, car elle influe sur la solution MFA que vous implémentez. Il existe des solutions, par exemple celle fournie via l’implémentation des [paramètres de sécurité par défaut d’Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), qui autorisent uniquement l’utilisation d’une application d’authentification pour la vérification. Si votre organisation applique une stratégie qui empêche l’utilisation d’appareils mobiles, vous devez envisager l’une des options suivantes :

- Déployer une application TOTP (mot de passe à usage unique et durée définie) qui peut s’exécuter sur un système sécurisé.

- Implémenter une solution tierce qui applique MFA pour chaque compte d’utilisateur du locataire partenaire et qui fournit l’option de vérification la plus appropriée.

- Acheter des licences [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) pour les utilisateurs impactés.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Quelles sont les fonctionnalités d’automatisation ou d’intégration qui tirent parti des informations d’identification de l’utilisateur pour l’authentification ?

Dans la mesure où nous appliquons MFA pour chaque utilisateur, y compris pour les comptes de service, dans l’annuaire des partenaires, toute automatisation ou intégration qui tire parti des informations d’identification de l’utilisateur pour l’authentification est impactée. C’est pourquoi il est important d’identifier les comptes qui sont utilisés dans ces situations. Consultez la liste ci-dessous qui comprend des exemples d’applications ou de services à prendre en compte :

- Panneau de contrôle utilisé pour provisionner les ressources pour le compte de vos clients

- Intégration à toute plateforme utilisée pour la facturation (par rapport au programme CSP) et prise en charge de vos clients

- Scripts PowerShell qui utilisent les modules Az, AzureRM, Azure AD, MS Online, etc.

La liste ci-dessus n’est pas exhaustive. Il est donc important d’effectuer une évaluation complète de toutes les applications ou services dans votre environnement qui tirent parti des informations d’identification de l’utilisateur pour l’authentification. Pour composer avec l’exigence de l’authentification multifacteur, vous devez, dans la mesure du possible, implémenter les conseils indiqués dans le [framework Modèle d’application sécurisé](/partner-center/develop/enable-secure-app-model).

## <a name="accessing-your-environment"></a>Accéder à votre environnement

Pour mieux comprendre ce qui, ou qui, fait l’objet d’une authentification sans test MFA, nous vous recommandons de passer en revue l’activité de connexion. Avec Azure Active Directory Premium, vous pouvez tirer profit du rapport de connexions. Pour plus d’informations à ce sujet, consultez les [rapports d’activité de connexion dans le portail Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Si vous n’avez pas Azure Active Directory Premium ou si vous cherchez un moyen d’obtenir cette activité de connexion par le biais de PowerShell, vous devez utiliser l’applet de commande [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) à partir du module [PowerShell de l’Espace partenaires](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-are-enforced"></a>Mode d’application des exigences

Les exigences de sécurité des partenaires sont appliquées par Azure AD et ensuite par l’Espace partenaires, en vérifiant la présence de la revendication MFA pour déterminer si la vérification MFA a eu lieu. À partir du 18 novembre 2019, Microsoft a mis en place des dispositifs de protection de la sécurité supplémentaires (anciennement « contraintes techniques ») auprès des locataires partenaires.

Au moment de l’activation, les utilisateurs du locataire partenaire sont invités à effectuer une vérification MFA dans le cadre des opérations AOBO (administration pour le compte de), en accédant au portail de l’Espace partenaires ou en appelant les API de l’Espace partenaires. Pour plus d’informations, consultez [Imposer l’authentification multifacteur (MFA) à votre locataire partenaire](partner-security-requirements-mandating-mfa.md). 

Les partenaires qui n’ont pas respecté les exigences doivent implémenter ces mesures dès que possible pour éviter toute interruption des activités. Si vous utilisez les paramètres de sécurité par défaut de l’authentification MFA (Multi-Factor Authentication) Azure ou d’Azure AD, vous n’avez pas à effectuer d’actions supplémentaires.

Si vous utilisez une solution MFA tierce, il est possible que la revendication MFA ne soit pas émise. Si cette revendication est manquante, Azure AD ne pourra pas déterminer si la demande d’authentification a fait l’objet d’un test MFA. Pour plus d’informations sur la manière de vérifier si votre solution émet la revendication attendue, consultez [Test des exigences de sécurité du partenaire](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Si votre solution de tiers n’émet pas la revendication attendue, vous devez collaborer avec le fournisseur qui a développé la solution pour déterminer les actions à entreprendre.

## <a name="resources-and-samples"></a>Ressources et exemples

Consultez les ressources suivantes pour obtenir de l’aide et des exemples de code :

- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : La communauté du groupe d’aide sur la sécurité de l’Espace partenaires est une communauté en ligne qui vous permet de découvrir les événements à venir et de poser des questions.
- [Exemples .NET de l’Espace partenaires](https://github.com/microsoft/partner-center-dotnet-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de .NET, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Exemples Java de l’Espace partenaires](https://github.com/microsoft/partner-center-java-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de Java, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Espace partenaires PowerShell - Authentification MFA](/powershell/partnercenter/multi-factor-auth) : cet article fournit des détails sur la façon d’implémenter le framework Modèle d’application sécurisé avec PowerShell.

## <a name="next-steps"></a>Étapes suivantes

- [Imposer l’authentification multifacteur (MFA) à votre locataire partenaire](partner-security-requirements-mandating-mfa.md)