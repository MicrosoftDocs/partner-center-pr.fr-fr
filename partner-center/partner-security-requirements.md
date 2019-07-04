---
title: Exigences de sécurité de partenaire | Partenaires
ms.topic: article
ms.date: 06/25/2019
description: En savoir plus sur les exigences de sécurité pour les conseillers et les partenaires participant au programme fournisseur de solutions Cloud.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, fournisseur de solutions Cloud programme CSP, le fournisseur de panneau de contrôle, CPV, multi-factor authentication, MFA, sécuriser le modèle d’application, le modèle d’application sécurisée, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 8f513b96619819cd6ba892625e47731170d22130
ms.sourcegitcommit: de88bb4cd994f1a106a5d02242261042958d4300
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/03/2019
ms.locfileid: "67549535"
---
# <a name="partner-security-requirements"></a>Exigences de sécurité de partenaire

**S’applique à**

- Tous les partenaires dans le programme fournisseur de solutions de Cloud
  - Bill direct
  - Fournisseur indirect
  - Revendeur indirect
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

Sécurité et confidentialité des clients et partenaires sont deux priorités de Microsoft. Nous continuons à voir un nombre croissant d’attaques de sécurité plus sophistiquées, principalement liées aux identités compromises. Comme les contrôles préventifs jouent un rôle clé dans une stratégie de défense globale pour contrer les attaques de sécurité, nous allons commencer en appliquant un ensemble d’exigences de sécurité obligatoire pour aider à protéger leurs clients et partenaires.

> [!NOTE]
> Nous recommandons que tous les partenaires définitif via un cloud souverain (21Vianet, US Government et Allemagne) agissent et adoptent ces nouvelles exigences de sécurité immédiatement. Toutefois, ces partenaires ne sont pas requis pour répondre aux nouvelles exigences de sécurité effectives le 1 août 2019. Microsoft fournira des détails supplémentaires concernant la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

## <a name="overview-of-the-requirements"></a>Vue d’ensemble de la configuration requise

Tous les partenaires qui participent dans le programme fournisseur de solutions de Cloud, les fournisseurs de panneau de contrôle et les partenaires d’Advisor sont nécessaire pour appliquer l’authentification multifacteur (MFA) pour chaque utilisateur, y compris les comptes de service, dans leur locataire partenaire. Cela est possible en activant deux [stratégies de base d’Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). Stratégies de base sont un ensemble de stratégies prédéfinies qui aident à protéger les organisations contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure anti-hameçonnage, relecture et pulvérisation de mot de passe. Stratégies de base sont disponibles dans toutes les éditions d’Azure Active Directory. Microsoft propose ces stratégies de protection de base à tous les utilisateurs à activer davantage de clients et partenaires d’implémenter les pratiques de sécurité de haute qualité.

Les stratégies de deux base qui doivent être activés sont décrits dans le tableau ci-dessous.

|**Règlement**| |
|-----|-----|
|**Exiger l’authentification Multifacteur pour les administrateurs**|L’activation de la MFA nécessitent de stratégie des administrateurs, oblige les utilisateurs dans les rôles d’administrateur à s’inscrire à MFA à l’aide de l’application d’authentification. Une fois l’inscription de l’authentification Multifacteur est terminée, les administrateurs doivent utiliser l’authentification Multifacteur chaque fois qu’ils connectez-vous.|
|**Protection de l’utilisateur final**|Protection de l’utilisateur final est une stratégie de base de l’authentification Multifacteur en fonction des risques qui protège tous les utilisateurs dans un répertoire. L’activation de cette stratégie nécessite tous les utilisateurs à s’inscrire à MFA à l’aide de l’application d’authentification. Les utilisateurs peuvent ignorer l’invite d’inscription MFA pendant 14 jours, après laquelle ils seront bloqués de se connecter jusqu'à ce qu’ils s’inscrivent pour l’authentification Multifacteur. Une fois inscrit pour l’authentification Multifacteur, les utilisateurs seront invités pour l’authentification Multifacteur uniquement pendant les tentatives de connexion à risque. Comptes d’utilisateur compromis sont bloquées jusqu'à ce que son mot de passe est réinitialisé et événements à risque ont été ignorées.|

Lorsque ces stratégies sont activées, chaque utilisateur sera en mesure d’utiliser l’authentification Multifacteur Azure sans coût supplémentaire. Si vous utilisez une solution tierce, vous devez appliquer l’authentification Multifacteur pour chaque utilisateur lors de l’accès aux services de cloud Commercial Microsoft.

> [!IMPORTANT]
> Étant donné que l’authentification Multifacteur sera appliquée pour chaque utilisateur dans l’annuaire des partenaires, il y aura un impact sur n’importe quel automation ou l’intégration qui utilise les informations d’identification de l’utilisateur. Pour résoudre cet impact, vous devrez modifier la façon dont votre automatisation ou l’intégration se connecte aux services de cloud commercial de Microsoft. Si le service que vous vous connectez à prend en charge l’authentification par jeton, il est recommandé d’implémenter le [framework du modèle d’Application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="what-actions-do-i-need-to-take"></a>Quelles actions dois-je prendre ? 

Pour garantir la protection des utilisateurs dans le client partenaire, vous devez appliquer l’authentification Multifacteur pour chaque utilisateur (y compris les comptes de service). Cela est possible en activant le [requièrent une authentification Multifacteur pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) stratégies de base. Avant d’activer ces stratégies, il est important de comprendre ce qu’ils font et comment elles affectent toute automation ou l’intégration et vos utilisateurs.

> [!NOTE]
> [Stratégies de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) continuera à évoluer au fil du temps. Il est recommandé de revoir périodiquement la documentation pour en savoir plus sur l’évolution des stratégies.

### <a name="considerations"></a>Observations

Étant donné que les exigences de sécurité s’appliquent à tous les utilisateurs dans un annuaire des partenaires, plusieurs considérations doivent être apportées pour garantir un déploiement sans heurts. Ces considérations incluent l’identification des utilisateurs dans Azure Active Directory qui ne peuvent pas ou ne devez pas effectuer d’authentification Multifacteur, ainsi que les applications et les clients utilisés par votre organisation qui ne prennent pas en charge l’authentification moderne.

#### <a name="self-service-password-reset"></a>Réinitialisation du mot de passe libre-service

Réinitialisation de mot de passe libre-service (SSPR) est une fonctionnalité d’Azure Active Directory qui permet aux employés de réinitialiser leurs mots de passe sans devoir contacter le personnel informatique. Employés doivent s’inscrire aux ou être inscrits pour le mot de passe libre-service, réinitialisation avant d’utiliser le service. Pendant l’inscription, l’employé choisit une ou plusieurs méthodes d’authentification activées par leur organisation.

SSPR permet aux employés de rapidement débloqué et continuer à travailler, quel que soit leur ou l’heure du jour. En permettant aux utilisateurs de se débloquer, votre organisation peut réduire le temps non productif et les coûts de prise en charge élevée pour des problèmes les plus courants liés au mot de passe.

Lorsque le [protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) activé de stratégie de base des comptes d’utilisateur compromis seront bloqués jusqu'à ce que son mot de passe est réinitialisé et événements à risque ont été ignorées. Compte tenu de cela, il est recommandé que chaque utilisateur, ce qui est un administrateur global, procédez comme suit pour s’inscrire au SSPR

1. Accédez à la [page de configuration SSPR](https://aka.ms/ssprsetup)
2. Entrez votre nom d’utilisateur et le mot de passe
3. Configurer au moins une des options de vérifications qui seront utilisées pour vérifier qui vous êtes lors de la réinitialisation de votre mot de passe.  

Lorsqu’un compte a été compromis, un administrateur devra prendre des mesures pour rétablir l’accès pour l’utilisateur concerné. Consultez le [étapes pour débloquer un utilisateur](#recovering-compromised-accounts) pour plus d’informations sur le processus pour débloquer l’utilisateur.

#### <a name="legacy-protocols"></a>Protocoles hérités

Protocoles d’authentification hérités (IMAP, SMTP, POP3, etc.) sont utilisés par les clients de messagerie pour effectuer des demandes d’authentification. Ces protocoles ne prennent pas en charge MFA. La plupart de la compromission de compte est dues à des mauvais acteurs, effectuer des attaques contre des protocoles hérités de contourner MFA. Pour garantir l’authentification Multifacteur est requise lors de la connexion à un compte dans un annuaire des partenaires et mauvais acteurs ne sont pas capables de contourner MFA, ces exigences de sécurité bloque toutes les demandes d’authentification à partir de protocoles hérités.

### <a name="enabling-the-baseline-policies"></a>Activer les stratégies de base

Consultez le [implémentant le didacticiel d’exigences de sécurité partenaire](tutorials/partner-security-requirements.yml) pour une expérience interactive concernant l’implémentation des stratégies de base.  

#### <a name="require-mfa-for-admins"></a>Exiger l’authentification Multifacteur pour les administrateurs

Le *requièrent une authentification Multifacteur pour l’administration* stratégie de base exige l’authentification Multifacteur pour les rôles d’annuaire suivantes, considérées comme les rôles d’Azure Active Directory plus privilégiés :

- Administrateur général
- Administrateur SharePoint
- Administrateur Exchange
- Administrateur de l’accès conditionnel
- Administrateur de sécurité
- Administrateur du support technique / mots de passe administrateur
- Administrateur de facturation
- Administrateur de l’utilisateur

Lors de l’activation de la MFA nécessitent de stratégie des administrateurs, les rôles de neuf administrateur ci-dessus devront s’inscrire à MFA à l’aide de l’application d’authentification. Une fois l’inscription de l’authentification Multifacteur est terminée, les administrateurs doivent utiliser l’authentification Multifacteur chaque fois qu’ils connectez-vous.

Si votre organisation dispose de ces comptes en cours d’utilisation dans des scripts ou du code, envisagez d’en les remplaçant par [gérés identités](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Pour activer cette stratégie et protéger vos administrateurs :

1. Se connecter à la **Azure portal** comme administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **stratégie de référence : Exiger l’authentification Multifacteur pour les administrateurs**.
4. Définissez **activer la stratégie** à **utiliser immédiatement la stratégie**.
5. Cliquez sur **enregistrer**.

    ![Exiger l’authentification Multifacteur pour les administrateurs](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> Avant d’activer cette stratégie, assurez-vous que vos utilisateurs n’utilisent pas de protocoles d’authentification hérités. Consultez l’article [Comment : L’authentification héritée de bloc à Azure Active Directory avec l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) pour plus d’informations.

> [!IMPORTANT]
> Il existe un problème connu, ce qui a un impact sur votre capacité à se connecter à Exchange Online PowerShell à l’aide des privilèges d’administrateur délégués. Consultez le [Exchange Online PowerShell](#exchange-online-powershell) problème avant d’activer cette stratégie si vous utilisez ce module PowerShell.

#### <a name="end-user-protection"></a>Protection de l’utilisateur final

La stratégie de base utilisateur final protection protège tous les utilisateurs dans un répertoire. L’activation de cette stratégie nécessite tous les utilisateurs à s’inscrire pour Azure MFA dans les 14 jours. Une fois inscrit, les utilisateurs seront invités pour l’authentification Multifacteur uniquement pendant les tentatives de connexion à risque. Comptes d’utilisateur compromis sont bloquées jusqu'à ce que la réinitialisation de mot de passe et risque de licenciement.

La stratégie **stratégie de référence : Protection de l’utilisateur final** est préconfigurée et s’affichera en haut lorsque vous accédez au panneau d’accès conditionnel dans le portail Azure.

Pour activer cette stratégie et protéger vos utilisateurs :

1. Se connecter à la **Azure portal** comme administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **stratégie de référence : Protection de l’utilisateur final (version préliminaire)** .
4. Définissez **activer la stratégie** à **utiliser immédiatement la stratégie**.
5. Cliquez sur **enregistrer**.

    ![Protection de l’utilisateur final](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> Avant d’activer cette stratégie, assurez-vous que vos utilisateurs n’utilisent pas de protocoles d’authentification hérités. Consultez l’article [Comment : L’authentification héritée de bloc à Azure Active Directory avec l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) pour plus d’informations.

> [!IMPORTANT]
> Il existe un problèmes connus, ce qui a un impact sur votre capacité à se connecter à Exchange Online PowerShell à l’aide des privilèges d’administrateur délégués. Consultez le [Exchange Online PowerShell](#exchange-online-powershell) problème avant d’activer cette stratégie si vous utilisez ce module PowerShell.

## <a name="common-issues"></a>Problèmes courants

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Après avoir activé les stratégies de base, vous constaterez peut-être que votre automatisation ou une intégration rencontre une exception semblable à ce qui suit

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

La raison de cette exception est que vous vous authentifiez à l’aide des informations d’identification utilisateur et MFA est désormais obligatoire. Pour résoudre cette exception, vous devez utiliser un jeton d’accès pour l’authentification. Consultez le [guide du modèle d’Application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) pour plus d’informations.

>[!IMPORTANT]
>La plupart des modules PowerShell et API prend en charge la possibilité d’utiliser un jeton d’accès pour l’authentification. Toutefois, il existe certaines qui ne prennent actuellement pas en charge cette fonctionnalité. Si vous avez besoin d’aide pour déterminer si le module PowerShell ou d’API que vous voulez tirer parti de prend en charge l’utilisation d’un jeton d’accès pour l’authentification, puis poster un message sur le [Partner Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) Communauté.

#### <a name="aadsts700082"></a>AADSTS700082

Une fois que vous avez implémenté l’infrastructure de modèle d’Application sécurisée, il est probable que vous recevrez l’exception suivante 90 jours après la génération du jeton d’actualisation initiale

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

En ce qui concerne Azure Active Directory la durée de vie maximale pour une actualisation de jeton est de 90 jours. Pour résoudre cette erreur, vous devrez générer et stocker en toute sécurité un nouveau jeton d’actualisation. Notez qu’il est possible de mettre à jour par programme le jeton d’actualisation, car avec chaque demande à Azure Active Directory pour un jeton d’accès, un nouveau jeton d’actualisation est retourné. Vous pouvez implémenter la logique appropriée pour mettre à jour le jeton d’actualisation stocké de façon sécurisée avant son expiration.

Consultez [des durées de vie de jeton configurables dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pour plus d’informations.

### <a name="recovering-compromised-accounts"></a>La récupération de compte compromis

Pour protéger nos clients, le service informations d’identification de Microsoft recherche des paires nom d’utilisateur/mot de passe disponible publiquement. Si elles correspondent à une de nos utilisateurs, nous aider à sécuriser ce compte immédiatement. Utilisateurs identifiés comme ayant des informations d’identification volées sont confirmées compromis. Ces utilisateurs ne pourra se connecter jusqu'à ce que son mot de passe est réinitialisé.

Les utilisateurs reçoivent une licence Azure AD Premium peuvent restaurer l’accès via la réinitialisation de mot de passe libre-service (SSPR) si la fonctionnalité est activée dans son annuaire. Les utilisateurs sans licence premium qui sont bloquent doivent contacter un administrateur pour effectuer une réinitialisation de mot de passe manuelle et d’ignorer l’événement à risque utilisateur avec indicateur.

#### <a name="steps-to-unblock-a-user"></a>Étapes pour débloquer un utilisateur

Vérifiez que l’utilisateur a été bloqué par la stratégie en examinant les journaux de connexion de l’utilisateur.

1. Un administrateur doit se connecter à la **Azure portal** et accédez à **Azure Active Directory** > **utilisateurs** > cliquez sur le nom de l’utilisateur et accédez à des connexions.
2. Pour lancer le mot de passe réinitialisé sur un utilisateur bloqué, un administrateur doit accéder à **Azure Active Directory** > **utilisateurs avec indicateur de risque**
3. Cliquez sur l’utilisateur dont le compte est bloqué pour afficher des informations sur l’activité de connexion récente de l’utilisateur.
4. Cliquez sur Réinitialiser le mot de passe pour affecter un mot de passe temporaire qui doit être modifié lors de la prochaine connexion.
5. Cliquez sur Ignorer tous les événements pour réinitialiser le score de risque de l’utilisateur.

L’utilisateur peut désormais se connecter, de réinitialiser leur mot de passe et d’accéder à l’application.

## <a name="known-issues"></a>Problèmes connus

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Lors de l’authentification Multifacteur est activée partenaires ne sera pas en mesure d’utiliser leurs privilèges d’administration déléguées avec Exchange Online PowerShell pour effectuer des actions par rapport à leurs clients. Consultez [se connecter à Exchange Online PowerShell à l’aide de l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) pour plus d’informations concernant cette limitation.

## <a name="resources-and-support"></a>Prise en charge et ressources

Via le [Communauté de partenaires Center Security Guidance Group](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) vous pouvez trouver des ressources supplémentaires et en savoir plus sur les événements à venir telles que des heures de bureau technique. Consultez le [Forum aux questions](http://assetsprod.microsoft.com/security-requirements-faq.pdf) document pour en savoir plus sur la configuration requise.

### <a name="developers"></a>Développeurs

- [L’activation du modèle d’Application sécurisée](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Exemples .NET de partenaires](https://github.com/microsoft/partner-center-dotnet-samples)
- [Exemples Java de partenaires](https://github.com/microsoft/partner-center-java-samples)
- [PowerShell partenaires implémentant le modèle d’Application sécurisée](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
