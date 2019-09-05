---
title: Exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 08/30/2019
description: Découvrez les exigences de sécurité pour les conseillers et les partenaires participant au programme Fournisseur de solutions Microsoft Cloud.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: c95ec38f928ca4032ffecebaf25f23e87d10c079
ms.sourcegitcommit: de3cdc792b6b4bbc64d1288d371623d79d535205
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/03/2019
ms.locfileid: "70215649"
---
# <a name="partner-security-requirements"></a>Exigences de sécurité du partenaire

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
  - Facturation directe
  - Fournisseurs indirects
  - Revendeur indirect
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et s’assurer qu’ils disposent des protections de sécurité appropriées. Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.

À partir du 1er août 2019, tous les partenaires doivent mettre en œuvre l’authentification multifacteur pour tous les utilisateurs, y compris les comptes de service, dans leur locataire partenaire.

> [!NOTE]
> Nous recommandons vivement que tous les partenaires qui effectuent des transactions par le biais d’un cloud souverain (21Vianet, gouvernement des États-Unis et Allemagne) agissent et adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août 2019. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

Les conditions associées aux exigences de sécurité du partenaire ont été ajoutées au [guide du programme Fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100). À partir du 1er août 2019, tous les partenaires qui participent au programme Fournisseur de solutions Cloud doivent se conformer aux conditions. En ce qui concerne les conseillers, les mêmes exigences contractuelles sont en place.

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne seront pas en mesure d’effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud ou de gérer les locataires clients en tirant parti des droits d’administrateur délégué, une fois ces exigences appliquées. Nous sommes en train de mettre en place une date de mise en œuvre technique pour les exigences et notifieront les partenaires de la date avec des informations détaillées.

## <a name="what-actions-do-i-need-to-take"></a>Quelles actions dois-je effectuer ?

Étant donné la nature hautement privilégiée de la qualité de partenaire, nous devons nous assurer que chaque utilisateur a un test MFA pour chaque authentification unique. Pour ce faire, vous pouvez procéder de l’une des façons suivantes :

- Implémentation d’Azure AD Premium et vérification de l’application de l’authentification multifacteur pour chaque utilisateur
- Implémentation des [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implémentation d’une solution tierce et vérification de l’application de l’authentification multifacteur pour chaque utilisateur

> [!IMPORTANT]
> Une fois que ces exigences sont techniquement appliquées, chaque authentification unique doit avoir un test MFA. Vous ne pouvez pas utiliser les fonctionnalités de l’accès conditionnel pour éviter l’authentification à l’aide de l’authentification multifacteur lors de l’accès aux services cloud commerciaux Microsoft.

### <a name="considerations"></a>Éléments à prendre en considération

Étant donné que ces exigences s’appliquent à tous les utilisateurs, y compris aux comptes de service, de votre locataire partenaire, plusieurs éléments doivent être pris en compte pour garantir un déploiement sans heurts. Ces considérations incluent l’identification des utilisateurs dans Azure AD qui ne peuvent pas effectuer l’authentification MFA, ainsi que les applications et appareils utilisés par votre organisation qui ne prennent pas en charge l’authentification moderne.

Avant d’effectuer une action, il est recommandé d’identifier les éléments suivants :

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Disposez-vous d’une application ou d’un appareil qui ne prend pas en charge l’utilisation de l’authentification multifacteur lors de l’authentification ?

Quand vous appliquez l’utilisation de l’authentification MFA héritée, les protocoles tels qu’IMAP, POP3 et SMTP sont bloqués, car ils ne prennent pas en charge l’authentification MFA. Pour passer outre cette limitation, vous pouvez utiliser une fonctionnalité appelée [Mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pour vous assurer que l’application ou l’appareil peut toujours s’authentifier. Vous devez consulter les considérations relatives à l’utilisation des mots de passe d’application documentées [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer si vous pouvez utiliser ces derniers dans votre environnement.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Avez-vous des utilisateurs qui recourent à Office 365 dans le cadre de licences associées à votre locataire partenaire ?

Avant d’implémenter une solution, il est recommandé de déterminer la version de Microsoft Office qui est utilisée par les utilisateurs de votre locataire partenaire. Consultez [Planifier l’authentification multifacteur pour les déploiements d’Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) avant d’entreprendre une action. Il y a un risque que vos utilisateurs rencontrent des problèmes de connectivité avec des applications comme Outlook. Avant d’appliquer l’authentification multifacteur, il est important de s’assurer qu’Outlook 2013 SP1, ou version ultérieure, est utilisé et que l’authentification moderne est activée pour votre organisation. Pour plus d’informations, consultez [Activer l’authentification moderne dans Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Pour activer l’authentification moderne pour tous les appareils exécutant Windows et sur lesquels Microsoft Office 2013 est installé, vous devez créer deux clés de registre. Consultez [Activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Si vous avez activé vos utilisateurs pour l’authentification multifacteur Azure AD et qu’ils ont des appareils exécutant Office 2013 qui ne sont pas activés pour l’authentification moderne, ils doivent utiliser des mots de passe d’application sur ces appareils. Vous trouverez plus d’informations sur les mots de passe d’application et sur quand, où et comment les utiliser ici : [Mots de passe d’application avec Azure Multi-Factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe-t-il une stratégie qui empêche les utilisateurs de recourir à leurs appareils mobiles quand ils travaillent ?

Il est important d’identifier toute stratégie d’entreprise qui empêche les employés d’utiliser des appareils mobiles quand ils travaillent, car elle influe sur la solution MFA que vous implémentez. Il existe des solutions MFA, telles que celles fournies par l’implémentation des [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), qui autorisent uniquement l’utilisation d’une application d’authentification pour la vérification. Si votre organisation a une stratégie qui empêche l’utilisation d’appareils mobiles, vous devez envisager l’une des options suivantes :

- Déployer une application TOTP (mot de passe à usage unique et durée définie) qui peut s’exécuter sur un système sécurisé
- Implémenter une solution tierce qui applique l’authentification MFA pour chaque utilisateur du locataire partenaire et qui fournit l’option de vérification la plus appropriée
- Acheter des licences [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) pour les utilisateurs concernés

La prise en charge de l’utilisation de clés de sécurité FIDO est inscrite sur la feuille de route des stratégies de protection de base. Une fois la prise en charge ajoutée, vous pourrez tirer parti des clés de sécurité FIDO pour le second facteur d’authentification. En attendant, vous êtes limité à l’utilisation de l’application d’authentification.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quelles sont les fonctionnalités d’automatisation ou d’intégration qui tirent parti des informations d’identification de l’utilisateur pour l’authentification ?

Dans la mesure où il est nécessaire d’appliquer l’authentification MFA pour chaque utilisateur, y compris pour les comptes de service, dans l’annuaire des partenaires, toute automatisation ou intégration qui tire parti des informations d’identification de l’utilisateur pour l’authentification est impactée. C’est pourquoi il est important d’identifier les comptes qui sont utilisés dans ces situations. Voici une liste d’exemples d’applications ou de services qui doivent être pris en compte :

- Panneau de contrôle utilisé pour provisionner les ressources pour le compte de vos clients
- Intégration à toute plateforme utilisée pour la facturation (par rapport au programme CSP) et prise en charge de vos clients
- Scripts PowerShell qui utilisent les modules Az, AzureRM, Azure AD, MS Online, etc.

La liste ci-dessus n’est pas exhaustive. Il est donc important d’effectuer une évaluation complète de toutes les applications ou services dans votre environnement qui tirent parti des informations d’identification de l’utilisateur pour l’authentification. Pour composer avec l’exigence de l’authentification multifacteur, vous devez, dans la mesure du possible, implémenter les conseils indiqués dans le [framework Modèle d’application sécurisé](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model). Voici des ressources supplémentaires qui vous aideront à comprendre comment implémenter le framework Modèle d’application sécurisé :

- [Exemples .NET pour l’Espace partenaires](https://github.com/microsoft/partner-center-dotnet-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de .NET, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Exemples Java pour l’Espace partenaires](https://github.com/microsoft/partner-center-java-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de Java, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Module PowerShell pour l’Espace partenaires - Modèle d’application sécurisé](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) : cet article fournit des détails sur la façon d’implémenter le framework Modèle d’application sécurisé à l’aide de PowerShell.
- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : cette communauté en ligne vous permet de découvrir les événements à venir et de poser des questions.

### <a name="enforcing-mfa-for-all-users"></a>Application de l’authentification MFA pour tous les utilisateurs

Cette section explique comment vous pouvez utiliser les [stratégies de protection de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) afin d’appliquer l’authentification multifacteur pour chaque utilisateur, y compris pour les comptes de service, dans votre locataire partenaire. Si vous envisagez d’utiliser Azure AD Premium, suivez les étapes décrites [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Une solution tierce, compatible avec Azure AD, peut être utilisée afin d’appliquer l’authentification MFA pour tous les utilisateurs, y compris pour les comptes de service. Pour plus d’informations sur la façon dont la solution doit être implémentée, reportez-vous à la documentation du fournisseur.

Les stratégies de protection de base sont un ensemble de stratégies prédéfinies qui contribuent à protéger les entreprises contre de nombreuses attaques courantes. Ces attaques courantes peuvent inclure la pulvérisation de mot de passe, le rejeu et le hameçonnage. Les stratégies de protection de base sont disponibles dans toutes les éditions d’Azure Active Directory. Microsoft met ces stratégies de protection de base à la disposition de tous afin de permettre aux clients et partenaires de mettre en œuvre les meilleures pratiques de sécurité.

Les deux stratégies de protection de base qui doivent être activées sont décrites dans le tableau ci-dessous.

|**Règlement**| |
|-----|-----|
|**Exiger l’authentification multifacteur pour les administrateurs**|L’activation de la stratégie Exiger l’authentification multifacteur pour les administrateurs requiert que les utilisateurs des rôles d’administrateur s’inscrivent à l’authentification MFA à l’aide de l’application d’authentification. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.|
|**Protection de l’utilisateur final**|La protection de l’utilisateur final est une stratégie de protection de référence MFA basée sur les risques qui protège tous les utilisateurs dans un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent à l’authentification MFA à l’aide de l’application d’authentification. Les utilisateurs peuvent ignorer l’invite d’inscription à l’authentification MFA pendant 14 jours, après quoi il leur est impossible de se connecter tant qu’ils ne s’inscrivent pas à l’authentification MFA. Une fois inscrits à l’authentification multifacteur, les utilisateurs sont invités à utiliser l’authentification multifacteur uniquement pendant les tentatives de connexion risquées. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que leur mot de passe soit réinitialisé et que les événements à risque soient ignorés.|

Quand ces stratégies sont activées, chaque utilisateur peut utiliser l’authentification multifacteur Azure à l’aide de l’application d’authentification à des fins de vérification sans coût supplémentaire.

#### <a name="configure-self-service-password-reset"></a>Configurer la réinitialisation du mot de passe en libre-service

La réinitialisation de mot de passe en libre-service (SSPR) est une fonctionnalité Azure Active Directory qui permet aux utilisateurs de réinitialiser leur mot de passe sans avoir à contacter leur équipe de support. Les utilisateurs doivent s’inscrire à la réinitialisation de mot de passe en libre-service ou être inscrits à celle-ci avant d’utiliser le service. Pendant l’inscription, l’utilisateur choisit une ou plusieurs méthodes d’authentification activées par son organisation.

Quand la stratégie de protection de référence [Protection de l’utilisateur final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) est activée, tous les comptes d’utilisateur compromis sont bloqués jusqu’à ce que leur mot de passe soit réinitialisé et que les événements à risque soient ignorés. Ainsi, il est recommandé que tous les utilisateurs qui sont administrateurs généraux effectuent les opérations suivantes pour s’inscrire à SSPR afin qu’ils ne soient pas bloqués.

1. Accédez à la [page de configuration de SSPR](https://aka.ms/ssprsetup).
2. Entrez vos nom d’utilisateur et mot de passe.
3. Configurez au moins l’une des options de vérification à utiliser pour vérifier qui vous êtes lors de la réinitialisation de votre mot de passe.  

Quand un compte a été compromis, un administrateur doit prendre des mesures afin de restaurer l’accès pour l’utilisateur impacté. Pour plus d’informations sur le processus de déblocage de l’utilisateur, consultez les [étapes de déblocage d’un utilisateur](#recovering-compromised-accounts).

#### <a name="require-mfa-for-admins"></a>Exiger l’authentification multifacteur pour les administrateurs

La stratégie de référence *Exiger l’authentification multifacteur pour les administrateurs* requiert l’authentification MFA pour les rôles d’annuaire suivants, considérés comme les rôles Azure Active Directory les plus privilégiés :

- Administrateur général
- Administrateur SharePoint
- Administrateur Exchange
- Administrateur de l’accès conditionnel
- Administrateur de sécurité
- Administrateur du support technique/administrateur de mots de passe
- Administrateur de facturation
- Administrateur utilisateur

Lors de l’activation de la stratégie Exiger l’authentification multifacteur pour les administrateurs, les neuf rôles d’administrateur ci-dessus doivent s’inscrire à l’authentification MFA à l’aide de l’application d’authentification. Une fois l’inscription MFA terminée, les administrateurs doivent effectuer une authentification MFA chaque fois qu’ils se connectent.

Si votre organisation utilise ces comptes dans des scripts ou du code, envisagez de les remplacer par des  [identités managées](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Pour activer cette stratégie et protéger vos administrateurs :

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **Accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **Stratégie de référence : exiger l’authentification multifacteur pour les administrateurs**.
4. Définissez **Activer la stratégie** sur **Utiliser la stratégie immédiatement**.
5. Cliquez sur  **Enregistrer**.

> [!WARNING]
> Avant d’activer cette stratégie, vérifiez que vos utilisateurs n’utilisent pas de protocoles d’authentification héritée. Par le biais de l’implémentation de cette stratégie, l’authentification héritée est bloquée.

> [!IMPORTANT]
> Il existe un problème connu qui impacte votre capacité à vous connecter à Exchange Online PowerShell à l’aide de privilèges d’administrateur délégués. Consultez le problème connu [Exchange Online PowerShell](#exchange-online-powershell) avant d’activer cette stratégie si vous utilisez ce module PowerShell.

#### <a name="end-user-protection"></a>Protection de l’utilisateur final

La stratégie de référence de protection de l’utilisateur final protège tous les utilisateurs dans un annuaire. L’activation de cette stratégie nécessite que tous les utilisateurs s’inscrivent à l’authentification Azure MFA dans un délai de 14 jours. Une fois inscrits, les utilisateurs sont invités à utiliser l’authentification multifacteur uniquement pendant les tentatives de connexion risquées. Les comptes d’utilisateurs compromis sont bloqués jusqu’à ce que le mot de passe soit réinitialisé et les risques ignorés.

La Stratégie **Stratégie de référence : protection de l’utilisateur final** est préconfigurée et s’affiche en haut de l’affichage quand vous accédez au panneau Accès conditionnel dans portail Azure.

Pour activer cette stratégie et protéger vos utilisateurs :

1. Connectez-vous au **portail Azure** en tant qu’administrateur général, administrateur de sécurité ou administrateur de l’accès conditionnel.
2. Accédez à **Azure Active Directory** > **Accès conditionnel**.
3. Dans la liste des stratégies, sélectionnez **Stratégie de référence : Protection de l’utilisateur final (préversion)** .
4. Définissez **Activer la stratégie** sur **Utiliser la stratégie immédiatement**.
5. Cliquez sur  **Enregistrer**.

> [!WARNING]
> Avant d’activer cette stratégie, vérifiez que vos utilisateurs n’utilisent pas de protocoles d’authentification héritée. Par le biais de l’implémentation de cette stratégie, l’authentification héritée est bloquée.

> [!IMPORTANT]
> Il existe un problème connu qui impacte votre capacité à vous connecter à Exchange Online PowerShell à l’aide de privilèges d’administrateur délégués. Consultez le problème connu [Exchange Online PowerShell](#exchange-online-powershell) avant d’activer cette stratégie si vous utilisez ce module PowerShell.

## <a name="assessing-your-environment"></a>Évaluation de votre environnement

L’une des exigences de sécurité actuelles des partenaires vous oblige à appliquer l’authentification multifacteur à chaque utilisateur de votre locataire partenaire. Cette exigence pouvant être remplie à l’aide de différentes méthodes, il peut s’avérer difficile d’évaluer si des actions supplémentaires sont requises. Vous pouvez tirer parti d’outils comme les journaux d’audit Azure Active Directory et [Degré de sécurisation Microsoft ](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score) afin d’évaluer si des actions supplémentaires sont requises pour sécuriser votre locataire avec l’authentification MFA. Microsoft travaille sur une expérience de l’Espace partenaires pour assurer une vérification de conformité rapide aux exigences de l’authentification MFA et du modèle d’application sécurisé.

L’outil Degré de sécurisation Microsoft vous offre des visualisations robustes, une intégration à d’autres produits Microsoft, une comparaison de votre score avec d’autres sociétés, le filtrage par catégorie et bien plus encore. Avec cet outil, vous pouvez effectuer des actions d’amélioration de la sécurité au sein de votre organisation et suivre l’historique de votre score. Le score peut également refléter le moment où des solutions tierces ont pris en charge des actions d’amélioration recommandées.

![Degré de sécurisation Microsoft](images/security/secure-score.png)

> [!NOTE]
> Il peut s’écouler jusqu’à 24 heures avant que ne soient reflétées les actions que vous êtes susceptibles d’entreprendre pour améliorer votre degré de sécurisation Microsoft.

L’outil Degré de sécurisation Microsoft fournit uniquement une représentation numérique de votre méthode de sécurité. Pour mieux comprendre ce qui, ou qui, fait l’objet d’une authentification sans test MFA, il est recommandé d’interroger les journaux d’audit Azure Active Directory. Pour ce faire, vous pouvez utiliser le module [Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) et le script ci-dessous. Il génère un rapport qui fournit un insight sur les tentatives d’authentification qui se sont produites au cours du dernier jour sans faire l’objet d’un test MFA.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Une fois le script ci-dessus exécuté, les détails sont disponibles dans le fichier report.csv. Il contient une liste des tentatives d’authentification qui se sont produites au cours du dernier jour sans que l’utilisateur ait fait l’objet d’un test MFA. Vous devez examiner chaque entrée pour déterminer s’il s’agit du comportement attendu et agir si nécessaire.

![Rapport d’évaluation](images/security/assessment-report.png)

## <a name="common-issues"></a>Problèmes courants

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Après avoir activé les stratégies de référence, vous pouvez être amené à constater que l’automatisation ou l’intégration rencontre une exception semblable à la suivante :

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Cette exception est due au fait que vous vous authentifiez à l’aide des informations d’identification de l’utilisateur et que l’authentification multifacteur est maintenant requise. Pour résoudre cette exception, vous devez utiliser un jeton d’accès pour l’authentification. Pour plus d’informations, consultez le [Guide du modèle d’application sécurisé](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

>[!IMPORTANT]
>La plupart des modules PowerShell et des API modernes prennent en charge la possibilité d’utiliser un jeton d’accès pour l’authentification. Toutefois, certains ne prennent pas en charge cette fonctionnalité. Si vous avez besoin d’aide pour déterminer si l’API ou le module PowerShell que vous essayez d’utiliser prend en charge l’utilisation d’un jeton d’accès pour l’authentification, publiez un message sur la communauté du [groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

#### <a name="aadsts700082"></a>AADSTS700082

Une fois que vous avez implémenté le framework Modèle d’application sécurisé, il y a un risque que vous receviez l’exception suivante 90 jours après la génération du jeton d’actualisation initial.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

En ce qui concerne Azure Active Directory, la durée de vie maximale d’un jeton d’actualisation est de 90 jours. Pour résoudre cette erreur, vous devez générer et stocker de manière sécurisée un nouveau jeton d’actualisation. Notez qu’il est possible de mettre à jour le jeton d’actualisation par programmation, car à chaque demande de jeton d’accès adressée à Azure Active Directory un nouveau jeton d’actualisation est retourné. Vous pouvez implémenter la logique appropriée pour mettre à jour le jeton d’actualisation stocké de manière sécurisée avant qu’il n’expire.

Pour plus d’informations, consultez [Durées de vie des jetons configurables dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

### <a name="recovering-compromised-accounts"></a>Récupération de comptes compromis

Pour contribuer à protéger nos clients, le service de Microsoft dédié aux fuites des informations d’identification recherche les paires nom d’utilisateur/mot de passe disponibles publiquement. Si elles correspondent à l’un de nos utilisateurs, nous aidons à sécuriser immédiatement ce compte. Les utilisateurs identifiés comme ayant fait l’objet d’une fuite d’informations d’identification sont considérés comme compromis. Ces utilisateurs ne pourront pas se connecter tant que leur mot de passe ne sera pas réinitialisé.

Les utilisateurs disposant d’une licence Azure AD Premium peuvent restaurer l’accès via la réinitialisation de mot de passe en libre-service (SSPR) si la fonctionnalité est activée dans leur annuaire. Les utilisateurs sans licence Premium qui font l’objet d’un blocage doivent contacter un administrateur pour que soit effectuée une réinitialisation manuelle du mot de passe et que soit ignoré l’événement à risque pour l’utilisateur marqué d’un indicateur.

#### <a name="steps-to-unblock-a-user"></a>Étapes pour débloquer un utilisateur

Vérifiez que l’utilisateur a été bloqué par la stratégie en examinant ses journaux de connexion.

1. Un administrateur doit se connecter au **portail Azure** et accéder à **Azure Active Directory** > **Utilisateurs**, puis cliquer sur le nom de l’utilisateur et accéder à Connexions.
2. Pour lancer la réinitialisation du mot de passe sur un utilisateur bloqué, un administrateur doit accéder à **Azure Active Directory** > **Utilisateurs avec indicateur de risque**.
3. Cliquez sur l’utilisateur dont le compte est bloqué pour afficher des informations sur l’activité de connexion récente de l’utilisateur.
4. Cliquez sur Réinitialiser le mot de passe pour affecter un mot de passe temporaire qui doit être changé lors de la prochaine connexion.
5. Cliquez sur Ignorer tous les événements pour réinitialiser le score de risque de l’utilisateur.

L’utilisateur peut désormais se connecter, réinitialiser son mot de passe et accéder à l’application.

## <a name="known-issues"></a>Problèmes connus

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Quand l’authentification MFA est appliquée, les partenaires ne peuvent pas utiliser leurs privilèges d’administrateur délégués avec Exchange Online PowerShell pour effectuer des actions sur leurs clients. Pour plus d’informations sur cette limitation, consultez [Se connecter à Exchange Online PowerShell avec l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).

Vous pouvez contourner cette limitation en créant un compte et en ne l’utilisant jamais pour effectuer une authentification interactive. Nous vous recommandons d’utiliser [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) pour créer le compte et effectuer la configuration initiale. La commande PowerShell suivante permet de créer et de configurer le compte.

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

La prochaine fois que vous vous connecterez à Exchange Online par le biais de PowerShell, utilisez ce compte ; il fonctionnera comme prévu.

> [!IMPORTANT]
> Il sera possible à l’avenir pour les partenaires d’utiliser leurs privilèges d’administrateur délégués avec Exchange Online PowerShell pour effectuer des actions sur leurs clients quand l’authentification MFA est appliquée. En attendant, vous devez tirer parti de cette solution de contournement.

## <a name="resources-and-support"></a>Ressources et support

Par le biais de la [communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance), vous pouvez trouver des ressources supplémentaires et des informations sur les événements à venir, tels que des permanences techniques. Consultez le document [Forum aux questions](partner-security-requirements-faq.md) pour en savoir plus sur les exigences.
