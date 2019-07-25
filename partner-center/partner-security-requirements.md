---
title: Conditions de sécurité pour les partenaires | Espace partenaires
ms.topic: article
ms.date: 07/18/2019
description: En savoir plus sur les exigences de sécurité pour les conseillers et les partenaires participant au programme du fournisseur de solutions Cloud.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme fournisseur de solutions Cloud, CSP, fournisseur du panneau de configuration, CPV, Multi-Factor Authentication, MFA, modèle d’application sécurisée, modèle d’application sécurisée, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 0ce8a8dd5a58d1647c8d9e53dec0d0bbf7fe6592
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/18/2019
ms.locfileid: "68313934"
---
# <a name="partner-security-requirements"></a>Conditions de sécurité pour les partenaires

**S’applique à**

- Tous les partenaires du programme fournisseur de solutions Cloud
  - Facture directe
  - Fournisseur indirect
  - Revendeur indirect
- Tous les fournisseurs du panneau de configuration
- Tous les conseillers

Les meilleures priorités et la sécurité sont de plus en plus sécurisées. Nous savons que la meilleure défense est la prévention et que nous sommes uniquement aussi forts que notre lien le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et s’assurer qu’ils disposent des protections de sécurité appropriées. Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs du panneau de configuration et les partenaires participant au programme du fournisseur de solutions Cloud.

À partir du 1er août 2019, tous les partenaires sont requis pour mettre en œuvre l’authentification multifacteur pour tous les utilisateurs, y compris les comptes de service, dans leur locataire partenaire.

> [!NOTE]
> Nous vous recommandons vivement de faire en sorte que tous les partenaires passent par un Cloud souverain (21Vianet, gouvernement des États-Unis et Allemagne) et adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août 2019. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

Les termes associés aux conditions de sécurité du partenaire ont été ajoutés au [Guide du programme fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100). À partir du 1er août 2019, tous les partenaires qui participent au programme fournisseur de solutions Cloud doivent être conformes aux termes du présent contrat. En ce qui concerne les conseillers, les mêmes exigences contractuelles sont en place.

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne seront pas en mesure d’effectuer des transactions dans le programme du fournisseur de solutions Cloud ou de gérer les locataires clients en tirant parti des droits d’administrateur délégué, une fois ces exigences appliquées. Nous sommes en train de mettre en place une date de mise en œuvre technique pour les exigences et notifieront les partenaires de la date avec des informations détaillées.

## <a name="what-actions-do-i-need-to-take"></a>Quelles actions dois-je effectuer?

Étant donné la nature hautement privilégiée d’un partenaire, nous devons nous assurer que chaque utilisateur a un défi MFA pour chaque authentification unique. Pour ce faire, vous pouvez procéder de l’une des façons suivantes:

- Implémentation de Azure AD Premium et vérification de l’application de l’authentification multifacteur pour chaque utilisateur
- Implémentation des [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implémentation d’une solution tierce et vérification de l’application de l’authentification MFA pour chaque utilisateur

> [!IMPORTANT]
> Une fois ces exigences techniquement appliquées, chaque authentification unique doit avoir une stimulation MFA. Vous ne pouvez pas utiliser les fonctionnalités de l’accès conditionnel pour éviter l’authentification à l’aide de l’authentification multifacteur lors de l’accès aux services Cloud commerciaux Microsoft.

### <a name="considerations"></a>Observations

Étant donné que ces exigences s’appliquent à tous les utilisateurs, y compris les comptes de service, de votre locataire partenaire, plusieurs éléments doivent être pris en compte pour garantir un déploiement sans heurts. Ces considérations incluent l’identification des utilisateurs dans Azure AD qui ne peuvent pas effectuer l’authentification MFA, ainsi que les applications et appareils utilisés par votre organisation qui ne prennent pas en charge l’authentification moderne.

Avant d’effectuer une action, il est recommandé d’identifier les éléments suivants:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Disposez-vous d’une application ou d’un appareil qui ne prend pas en charge l’utilisation de l’authentification multifacteur lors de l’authentification?

Lorsque vous appliquez l’authentification MFA héritée, les protocoles tels que IMAP, POP3, SMTP, etc. sont bloqués, car ces protocoles ne prennent pas en charge MFA. Pour résoudre ce problème, une fonctionnalité appelée [mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) peut être utilisée pour s’assurer que l’application ou l’appareil peut toujours s’authentifier. Vous devez examiner les considérations relatives à l’utilisation des mots de passe d’application documentés [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer s’ils peuvent être utilisés dans votre environnement.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe-t-il une stratégie qui empêche les utilisateurs d’utiliser leurs appareils mobiles quand ils travaillent?

Il est important d’identifier toute stratégie d’entreprise qui empêche les employés d’utiliser des appareils mobiles en cours de travail, car elle influencera la solution MFA que vous implémentez. Il existe des solutions MFA, telles que celles fournies par l’implémentation des [stratégies de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), qui autorisent uniquement l’utilisation d’une application authentificateur pour la vérification. Si votre organisation a une stratégie qui empêche l’utilisation d’appareils mobiles, vous devez vous intéresser à l’achat de [Azure ad Premium](https://azure.microsoft.com/pricing/details/active-directory/) pour les utilisateurs concernés ou vous pouvez implémenter une solution tierce qui offre la vérification la plus appropriée. option.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quelles sont les fonctionnalités d’automatisation ou d’intégration qui tirent parti des informations d’identification de l’utilisateur pour l’authentification?

Dans la mesure où il est nécessaire d’appliquer l’authentification MFA pour chaque utilisateur, y compris les comptes de service, dans le répertoire de votre partenaire, toute automatisation ou intégration qui tire parti des informations d’identification de l’utilisateur pour l’authentification sera affectée. C’est pourquoi il est important d’identifier les comptes qui sont utilisés dans ces situations. Voici une liste d’exemples d’applications ou de services qui doivent être pris en compte

- Panneau de configuration utilisé pour approvisionner les ressources pour le compte de vos clients
- Intégration à toute plateforme utilisée pour la facturation (par rapport au programme CSP) et prise en charge de vos clients
- Scripts PowerShell qui utilisent les modules AZ, AzureRM, Azure AD, MS Online, etc.

La liste ci-dessus n’est pas exhaustive. Il est donc important d’effectuer une évaluation complète des applications ou services de votre environnement qui tire parti des informations d’identification de l’utilisateur pour l’authentification. Pour être en concurrence avec l’exigence de l’authentification multifacteur, vous devez implémenter les conseils dans l' [infrastructure de modèle d’application sécurisée](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) , dans la mesure du possible. Vous trouverez ci-dessous des ressources supplémentaires qui vous aideront à comprendre comment l’infrastructure de modèle d’application sécurisée peut être implémentée

- [Exemples .net de l’espace partenaires](https://github.com/microsoft/partner-center-dotnet-samples) : ce dépôt github contient des exemples, développés à l’aide de .net, qui illustrent la façon dont vous pouvez implémenter l’infrastructure de modèle d’application sécurisée.
- [Exemples Java de l’espace partenaires](https://github.com/microsoft/partner-center-java-samples) : ce dépôt github contient des exemples, développés à l’aide de Java, qui illustrent la façon dont vous pouvez implémenter l’infrastructure de modèle d’application sécurisée.
- [Partner Center PowerShell-modèle d’application sécurisée](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) : cet article fournit des détails sur la façon d’implémenter l’infrastructure de modèle d’application sécurisée à l’aide de PowerShell.
- [Groupe de conseils de sécurité de l’espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : communauté en ligne qui vous permet de découvrir les événements à venir et de poser des questions.

### <a name="enforcing-mfa-for-all-users"></a>Application de l’authentification MFA pour tous les utilisateurs

Cette section explique comment vous pouvez utiliser les [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) pour appliquer l’authentification multifacteur pour chaque utilisateur, y compris les comptes de service, dans votre locataire partenaire. Si vous envisagez d’utiliser Azure AD Premium, suivez les étapes décrites [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Une solution tierce, compatible avec Azure AD, peut être utilisée pour appliquer l’authentification MFA pour tous les utilisateurs, y compris les comptes de service. Pour plus d’informations sur la façon dont la solution doit être implémentée, reportez-vous à la documentation du fournisseur.

Les stratégies de protection de base sont un ensemble de stratégies prédéfinies qui contribuent à protéger les entreprises contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure la pulvérisation de mot de passe, la relecture et le hameçonnage. Les stratégies de protection de base sont disponibles dans toutes les éditions de Azure Active Directory. Microsoft met ces stratégies de protection de base à la disposition de tous afin de permettre aux clients et partenaires de mettre en œuvre les meilleures pratiques de sécurité.

Les deux stratégies de protection de base qui doivent être activées sont décrites dans le tableau ci-dessous.

|**Règlement**| |
|-----|-----|
|**Exiger l’authentification MFA pour les administrateurs**|L’activation de la stratégie exiger l’authentification MFA pour les administrateurs requiert que les utilisateurs des rôles d’administrateur s’inscrivent à l’authentification MFA à l’aide de l’application Authenticator. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.|
|**Protection de l’utilisateur final**|La protection de l’utilisateur final est une stratégie de protection MFA basée sur les risques qui protège tous les utilisateurs dans un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent pour MFA à l’aide de l’application Authenticator. Les utilisateurs peuvent ignorer l’invite d’inscription MFA pendant 14 jours, après quoi ils seront bloqués de se connecter jusqu’à ce qu’ils s’inscrivent pour l’authentification MFA. Une fois inscrit pour l’authentification multifacteur, les utilisateurs sont invités à utiliser l’authentification multifacteur uniquement pendant les tentatives de connexion risquée. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que leur mot de passe soit réinitialisé et que les événements à risque soient ignorés.|

Lorsque ces stratégies sont activées, chaque utilisateur peut utiliser l’authentification multifacteur Azure à l’aide de l’application de l’authentificateur à des fins de vérification sans coût supplémentaire.

#### <a name="configure-self-service-password-reset"></a>Configurer la réinitialisation du mot de passe libre-service

La réinitialisation de mot de passe libre-service (SSPR) est une fonctionnalité Azure Active Directory qui permet aux utilisateurs de réinitialiser leur mot de passe sans avoir à contacter leur équipe de support. Les utilisateurs doivent s’inscrire à la réinitialisation de mot de passe en libre-service ou être inscrits avant d’utiliser le service. Pendant l’inscription, l’utilisateur choisit une ou plusieurs méthodes d’authentification activées par son organisation.

Lorsque la stratégie de protection de base protection de l' [utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) est activée, tous les comptes d’utilisateur compromis sont bloqués jusqu’à ce que leur mot de passe soit réinitialisé et que les événements à risque soient ignorés. En tenant compte de cela, il est recommandé que chaque utilisateur, qui est un administrateur général, effectue les opérations suivantes pour s’inscrire à SSPR afin qu’il ne soit pas verrouillé.

1. Accédez à la [page de configuration de SSPR](https://aka.ms/ssprsetup)
2. Entrez votre nom d’utilisateur et votre mot de passe
3. Configurez au moins l’une des options de vérification qui seront utilisées pour vérifier qui vous êtes lors de la réinitialisation de votre mot de passe.  

Lorsqu’un compte a été compromis, un administrateur doit prendre des mesures pour restaurer l’accès pour l’utilisateur concerné. Pour plus d’informations sur le processus de déblocage de l’utilisateur, consultez les [étapes pour débloquer un utilisateur](#recovering-compromised-accounts) .

#### <a name="require-mfa-for-admins"></a>Exiger l’authentification MFA pour les administrateurs

La stratégie *de ligne de base exiger l’authentification MFA pour l’administration* requiert l’authentification MFA pour les rôles d’annuaire suivants, considérée comme les rôles Azure Active Directory les plus privilégiés:

- Administrateur général
- Administrateur SharePoint
- Administrateur Exchange
- Administrateur de l’accès conditionnel
- Administrateur de sécurité
- Administrateur du support technique/administrateur de mots de passe
- Administrateur de facturation
- Administrateur d’utilisateurs

Lors de l’activation de la stratégie exiger l’authentification MFA pour les administrateurs, les neuf rôles d’administrateur ci-dessus doivent être inscrits pour l’authentification MFA à l’aide de l’application de l’authentificateur. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.

Si votre organisation dispose de ces comptes en cours d’utilisation dans des scripts ou du code [](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview), envisagez de les remplacer par des identités gérées.

Pour activer cette stratégie et protéger vos administrateurs:

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de la sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **stratégie de référence: Exiger l’authentification MFA**pour les administrateurs.
4. Définissez **activer la stratégie** pour **utiliser la stratégie immédiatement**.
5. Cliquez sur **Enregistrer**.

> [!WARNING]
> Avant d’activer cette stratégie, assurez-vous que vos utilisateurs n’utilisent pas les protocoles d’authentification hérités. Par le biais de l’implémentation de cette stratégie, l’authentification héritée est bloquée.

> [!IMPORTANT]
> Il existe un problème connu qui a un impact sur votre capacité à se connecter à Exchange Online PowerShell à l’aide de privilèges d’administrateur délégués. Consultez le problème connu [Exchange Online PowerShell](#exchange-online-powershell) avant d’activer cette stratégie si vous utilisez ce module PowerShell.

#### <a name="end-user-protection"></a>Protection de l’utilisateur final

La stratégie de ligne de base de protection de l’utilisateur final protège tous les utilisateurs dans un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent à Azure MFA dans un délai de 14 jours. Une fois inscrite, les utilisateurs sont invités à utiliser l’authentification multifacteur uniquement pendant les tentatives de connexion risquée. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que la réinitialisation du mot de passe et le risque d’échec.

Stratégie de **ligne de base de stratégie: La protection** des utilisateurs finaux est préconfigurée et s’affiche en haut de l’affichage lorsque vous accédez au panneau accès conditionnel dans portail Azure.

Pour activer cette stratégie et protéger vos utilisateurs:

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de la sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **stratégie de référence: Protection de l’utilisateur final (** version préliminaire).
4. Définissez **activer la stratégie** pour **utiliser la stratégie immédiatement**.
5. Cliquez sur **Enregistrer**.

> [!WARNING]
> Avant d’activer cette stratégie, assurez-vous que vos utilisateurs n’utilisent pas les protocoles d’authentification hérités. Par le biais de l’implémentation de cette stratégie, l’authentification héritée est bloquée.

> [!IMPORTANT]
> Il existe un problème connu qui a un impact sur votre capacité à se connecter à Exchange Online PowerShell à l’aide de privilèges d’administrateur délégués. Consultez le problème connu [Exchange Online PowerShell](#exchange-online-powershell) avant d’activer cette stratégie si vous utilisez ce module PowerShell.

## <a name="common-issues"></a>Problèmes courants

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Après avoir activé les stratégies de base, vous constaterez peut-être que votre Automation ou votre intégration rencontre une exception semblable à la suivante:

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Cette exception est due au fait que vous vous authentifiez à l’aide des informations d’identification de l’utilisateur et que l’authentification multifacteur est maintenant requise. Pour résoudre cette exception, vous devrez utiliser un jeton d’accès pour l’authentification. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisée](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .

>[!IMPORTANT]
>La plupart des API modernes et des modules PowerShell prennent en charge la possibilité d’utiliser un jeton d’accès pour l’authentification. Toutefois, certaines d’entre elles ne prennent pas en charge cette fonctionnalité actuellement. Si vous avez besoin d’aide pour déterminer si l’API ou le module PowerShell que vous essayez d’utiliser prend en charge l’utilisation d’un jeton d’accès pour l’authentification, publiez un message sur la communauté du groupe de conseils de sécurité de l' [espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

#### <a name="aadsts700082"></a>AADSTS700082

Une fois que vous avez implémenté l’infrastructure de modèle d’application sécurisée, il y a un risque que vous receviez l’exception suivante 90 jours après la génération du jeton d’actualisation initial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

En ce qui concerne Azure Active Directory la durée de vie maximale d’un jeton d’actualisation est de 90 jours. Pour résoudre cette erreur, vous devez générer et stocker en toute sécurité un nouveau jeton d’actualisation. Notez qu’il est possible de mettre à jour le jeton d’actualisation par programme, car chaque requête adressée à Azure Active Directory pour un jeton d’accès un nouveau jeton d’actualisation est retourné. Vous pouvez implémenter la logique appropriée pour mettre à jour le jeton d’actualisation stocké en toute sécurité avant qu’il n’expire.

Pour plus d’informations [, consultez durées de vie des jetons configurables dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .

### <a name="recovering-compromised-accounts"></a>Récupération de comptes compromis

Pour protéger nos clients, le service d’informations d’identification divulgué de Microsoft recherche les paires nom d’utilisateur/mot de passe disponibles publiquement. S’ils correspondent à l’un de nos utilisateurs, nous vous aidons à sécuriser immédiatement ce compte. Les utilisateurs identifiés comme ayant une fuite d’informations d’identification sont considérés comme compromis. La connexion de ces utilisateurs est bloquée jusqu’à ce que leur mot de passe soit réinitialisé.

Les utilisateurs disposant d’une licence Azure AD Premium peuvent restaurer l’accès via la réinitialisation de mot de passe en libre-service (SSPR) si la fonctionnalité est activée dans leur annuaire. Les utilisateurs sans licence Premium qui sont bloqués doivent contacter un administrateur pour effectuer une réinitialisation manuelle du mot de passe et ignorer l’événement à risque pour l’utilisateur.

#### <a name="steps-to-unblock-a-user"></a>Étapes pour débloquer un utilisateur

Confirmez que l’utilisateur a été bloqué par la stratégie en examinant les journaux de connexion de l’utilisateur.

1. Un administrateur doit se connecter au **portail Azure** et accéder à **Azure Active Directory** > **utilisateurs** > cliquez sur le nom de l’utilisateur et accédez à connexions.
2. Pour initier la réinitialisation du mot de passe sur un utilisateur bloqué, un administrateur doit accéder à **Azure Active Directory** > **utilisateurs avec indicateur de risque**
3. Cliquez sur l’utilisateur dont le compte est bloqué pour afficher des informations sur l’activité de connexion récente de l’utilisateur.
4. Cliquez sur Réinitialiser le mot de passe pour affecter un mot de passe temporaire qui doit être modifié lors de la prochaine connexion.
5. Cliquez sur faire disparaître tous les événements pour réinitialiser le score de risque de l’utilisateur.

L’utilisateur peut désormais se connecter, réinitialiser son mot de passe et accéder à l’application.

## <a name="known-issues"></a>Problèmes connus

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Lorsque l’authentification MFA est activée, les partenaires ne peuvent pas utiliser leurs privilèges d’administrateur délégués avec Exchange Online PowerShell pour effectuer des actions sur leurs clients. Pour plus d’informations sur cette limitation, consultez [se connecter à Exchange Online PowerShell à l’aide de Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) .

## <a name="resources-and-support"></a>Ressources et support

Par le biais de la communauté du groupe de conseils de sécurité de l' [espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) , vous trouverez des ressources supplémentaires et des informations sur les événements à venir, tels que les horaires des bureaux techniques. Consultez le document Forum [aux questions](http://assetsprod.microsoft.com/security-requirements-faq.pdf) pour en savoir plus sur la configuration requise.
