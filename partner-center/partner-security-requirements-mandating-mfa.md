---
title: Obligation de l’authentification MFA pour votre locataire partenaire | Espace partenaires
ms.topic: article
ms.date: 09/25/2019
description: Détails sur l’authentification MFA pour les exigences de sécurité de votre locataire partenaire
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: medium
ms.openlocfilehash: 8f68d4628bd6212b800ea926c6c3b9f412e3d5cc
ms.sourcegitcommit: dcc2a2077ef17255ecf7a2fa5fae6bbeefaa9eb0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/07/2019
ms.locfileid: "71997793"
---
# <a name="mandating-mfa-for-your-partner-tenant"></a>Obligation de l’authentification MFA pour votre locataire partenaire

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
  - Facturation directe
  - Fournisseurs indirects
  - Revendeur indirect
- Tous les conseillers

Ces partenaires doivent effectuer la vérification de l’authentification MFA pour les domaines suivants :

- [Tableau de bord espace partenaires](#partner-center-dashboard)
- [API espace partenaires](#partner-center-api)
- [Administration déléguée du partenaire](#partner-delegated-administration)

L’objectif de cette fonctionnalité est d’aider les partenaires à sécuriser leur accès aux ressources client contre la compromission des informations d’identification.

## <a name="partner-center-dashboard"></a>Tableau de bord espace partenaires
Certaines pages du tableau de bord espace partenaires sont protégées par MFA, notamment :

* Toutes les pages sous l’onglet **clients** .
* Toutes les pages sous l’onglet **support → demandes client** .

Si vous essayez d’accéder à l’une de ces pages et que vous n’avez pas effectué la vérification de l’authentification MFA plus tôt, vous devez le faire.

Les types d’utilisateurs suivants sont autorisés à accéder à ces pages protégées par MFA et sont donc affectés par cette fonctionnalité, notamment :

* Agents d’administration
* Agents commerciaux
* Agents du support technique

Pour illustrer ce fonctionnement, prenez en compte les deux exemples suivants.

**Exemple 1 : le partenaire a implémenté Azure AD MFA**
1.  Jane fonctionne pour CSP contoso. Contoso a implémenté l’authentification MFA pour tous ses utilisateurs sous le locataire partenaire contoso à l’aide de l’authentification multifacteur Azure AD.
2.  À partir de son poste de travail, Jane démarre une nouvelle session de navigateur et accède à la page de présentation du tableau de bord de l’espace partenaires (qui n’est pas protégée par MFA). L’espace partenaires redirige Jane vers Azure AD pour se connecter.
3.  En raison de la configuration Azure AD MFA existante par Contoso, Jane est nécessaire pour effectuer la vérification de l’authentification MFA. À la fin de la connexion et de la vérification de l’authentification MFA, Jane est redirigé vers la page vue d’ensemble du tableau de bord de l’espace partenaires.
4.  Jane tente d’accéder à l’une des pages protégées par MFA dans l’espace partenaires. Dans la mesure où Jane a déjà effectué la vérification de l’authentification multifacteur lors de la connexion, Jane peut accéder à la page protégée par MFA sans être obligé de repasser par la vérification MFA.

**Exemple 2 : un partenaire a implémenté l’authentification MFA tierce à l’aide de la Fédération des identités**
1. Trent fonctionne pour les fournisseurs de solutions Cloud Wingtip. Wingtip a implémenté l’authentification MFA pour tous ses utilisateurs sous le locataire partenaire Wingtip à l’aide de l’authentification multifacteur tierce, qui est intégrée à Azure AD via la Fédération des identités.
2. À partir de son poste de travail, Trent démarre une nouvelle session de navigateur et accède à la page vue d’ensemble du tableau de bord de l’espace partenaires (qui n’est pas protégée par MFA). L’espace partenaires redirige Justin vers Azure AD pour se connecter.
3. Dans la mesure où Wingtip a configuré la Fédération d’identité, Azure AD redirige Trent vers le fournisseur d’identité fédérée pour effectuer la vérification de la connexion et de l’authentification MFA. Lors de la connexion et de la vérification de l’authentification MFA, Trent est redirigé vers Azure AD puis vers la page de présentation du tableau de bord de l’espace partenaires.
4. Justin tente d’accéder à l’une des pages protégées par MFA dans l’espace partenaires. Étant donné que Trent a déjà effectué la vérification de l’authentification multifacteur lors de la connexion précédente, Trent peut accéder à la page protégée par MFA sans être obligé de repasser par la vérification MFA.

**Exemple 3 : le partenaire n’a pas implémenté l’authentification MFA**
1. John travaille pour CSP fabrikam. Fabrikam n’a implémenté l’authentification MFA pour aucun utilisateur sous le locataire partenaire fabrikam.
2. À partir de son poste de travail, John démarre une nouvelle session de navigateur et accède à la page vue d’ensemble du tableau de bord de l’espace partenaires (qui n’est pas protégée par MFA). L’espace partenaires redirige John vers Azure AD pour se connecter.
3. Comme Fabrikam n’a pas implémenté l’authentification MFA, John n’est pas obligé d’effectuer la vérification de l’authentification MFA. Une fois la connexion établie, John est redirigé vers la page vue d’ensemble du tableau de bord de l’espace partenaires.
4. John tente d’accéder à l’une des pages protégées par MFA dans l’espace partenaires. Comme John n’a pas effectué la vérification de l’authentification MFA, l’espace partenaires redirige John vers Azure AD pour effectuer la vérification de l’authentification MFA. Étant donné qu’il s’agit de la première fois que John est requis pour effectuer l’authentification multifacteur, John est également invité à s’inscrire à MFA à l’aide de Microsoft Authenticator application. En cas de réussite de l’inscription MFA et de la vérification de l’authentification multifacteur, John peut désormais accéder à la page protégée par MFA.

## <a name="partner-center-api"></a>API espace partenaires

L’API espace partenaires prend en charge l’authentification d’application uniquement et l’authentification d’application + utilisateur. Lorsque l’authentification d’application + utilisateur est utilisée, l’espace partenaires exige une vérification MFA. Plus précisément, lorsqu’une application partenaire souhaite envoyer une demande d’API à l’espace partenaires, elle doit inclure un jeton d’accès dans l’en-tête d’autorisation de la demande. Lorsque l’espace partenaires reçoit une demande d’API avec un jeton d’accès obtenu à l’aide de l’authentification d’application + utilisateur, l’API espace partenaires vérifie la présence de la valeur *MFA* dans la revendication de la *référence de méthode d’authentification (AMR)* . Vous pouvez utiliser un décodeur JWT pour vérifier si un jeton d’accès contient la valeur de référence de méthode d’authentification attendue (AMR) ou non :

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Si la valeur est présente, Partner Center conclut que la vérification de l’authentification multifacteur a été effectuée et traite la demande de l’API. Si la valeur n’est pas présente, l’API de l’espace partenaires rejettera la demande avec la réponse suivante :

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>Administration déléguée du partenaire

### <a name="using-service-portals"></a>Utilisation des portails de service

Les comptes de partenaires, y compris les agents d’administration et les agents du support technique, peuvent utiliser leurs privilèges d’administrateur délégué partenaire pour gérer les ressources client via les portails Microsoft Online Services, l’interface de ligne de commande (CLI) et les API (à l’aide de l’authentification d’application + utilisateur).

Lors de l’accès aux portails Microsoft Online Services à l’aide des privilèges d’administrateur délégué du partenaire pour gérer les ressources client, un grand nombre de ces portails requièrent que le compte partenaire s’authentifie de manière interactive, avec le client Azure Active Directory client défini comme le contexte d’authentification : le compte de partenaire est nécessaire pour se connecter au locataire client.

Lorsque Azure Active Directory reçoit de telles demandes d’authentification, il exige que le compte de partenaire termine la vérification MFA. Il existe deux expériences utilisateur possibles, selon que le compte de partenaire est une identité gérée ou fédérée :

- Si le compte partenaire est une identité **gérée** , Azure Active Directory invite directement l’utilisateur à effectuer une vérification mfa. Si le compte partenaire n’est pas inscrit pour l’authentification MFA avec Azure Active Directory avant, l’utilisateur est invité à effectuer d’abord l' [inscription MFA](#mfa-registration-experience) .

- Si le compte partenaire est une identité **fédérée** , l’expérience dépend de la manière dont l’administrateur partenaire a configuré la fédération dans Azure Active Directory. Lors de la configuration de la Fédération dans Azure Active Directory, l’administrateur partenaire peut indiquer à Azure Active Directory si le fournisseur d’identité fédérée prend en charge MFA ou non. Si c’est le cas, Azure Active Directory redirigera l’utilisateur vers le fournisseur d’identité fédérée pour effectuer la vérification de l’authentification MFA. Dans le cas contraire, Azure Active Directory invite directement l’utilisateur à effectuer une vérification MFA. Si le compte partenaire n’est pas inscrit pour l’authentification MFA avec Azure Active Directory avant, l’utilisateur est invité à effectuer d’abord l' [inscription MFA](#mfa-registration-experience) .

L’expérience globale est très similaire au scénario dans lequel un locataire client final a implémenté l’authentification MFA pour ses administrateurs. Par exemple, le locataire client a activé [Azure ad stratégie de référence – MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), ce qui nécessite que tous les comptes avec des droits d’administration se connectent au locataire client avec la vérification MFA, y compris les agents d’administration et les agents du support technique. À des fins de test, les partenaires peuvent activer la [stratégie MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) dans le locataire client, puis essayer d’utiliser des privilèges d’administration déléguée de partenaire pour accéder au locataire client.

> [!NOTE]
> Tous les portails Microsoft Online Service ne nécessitent pas que les comptes de partenaires se connectent au locataire client lorsqu’ils accèdent aux ressources client à l’aide de privilèges d’administrateur délégué partenaire. Au lieu de cela, ils ont uniquement besoin que les comptes de partenaires se connectent au locataire partenaire. Le centre d’administration Exchange en est un exemple. Au fil du temps, nous nous attendons à ce que ces portails requièrent que les comptes des partenaires se connectent au locataire du client lorsqu’ils utilisent des privilèges d’administrateur délégué partenaire.

### <a name="using-service-apis"></a>Utilisation des API de service
Certaines API Microsoft Online Services (par exemple, Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) prennent en charge les partenaires qui utilisent des privilèges d’administrateur délégué partenaire pour gérer par programmation les ressources client. Pour tirer parti des privilèges d’administrateur délégué par le partenaire avec ces API, l’application partenaire doit inclure un jeton d’accès dans l’en-tête d’autorisation de demande d’API, où le jeton d’accès est obtenu en demandant à un compte d’utilisateur partenaire de s’authentifier auprès de Azure AD, avec la le client Azure AD défini comme contexte d’authentification. L’application partenaire doit avoir un compte d’utilisateur partenaire qui se connecte au locataire client.

Lorsque Azure AD reçoit comme demande d’authentification, Azure AD exige que le compte d’utilisateur partenaire termine la vérification MFA. Si le compte d’utilisateur partenaire n’est pas inscrit pour l’authentification MFA avant, le compte d’utilisateur est invité à effectuer d’abord l’inscription MFA.

Toutes les applications partenaires intégrées à ces API à l’aide de privilèges d’administrateur délégué partenaire sont affectées par cette fonctionnalité. Pour s’assurer que les applications partenaires peuvent continuer à travailler avec ces API sans interruption :

- Le partenaire doit éviter d’utiliser une méthode d’authentification utilisateur non interactive avec Azure AD pour obtenir le jeton d’accès. En cas d’utilisation d’une méthode d’authentification utilisateur non interactive telle que le [Workflow de mot de passe](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure ad ne peut pas inviter l’utilisateur à effectuer une vérification mfa. Le partenaire doit passer à l’utilisation de la méthode d’authentification utilisateur interactive, comme [OpenID Connect Flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) à la place.
- Pendant la méthode d’authentification des utilisateurs interactifs, le partenaire doit utiliser un compte d’utilisateur partenaire déjà activé pour MFA. Si vous y êtes invité par Azure AD, le partenaire peut également effectuer une vérification de l’authentification MFA et de l’authentification MFA lors de la connexion.
- Cela est très similaire au scénario dans lequel un locataire client final a implémenté l’authentification MFA pour ses administrateurs. Par exemple, le locataire client a activé [Azure ad stratégie de référence – MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), ce qui nécessite que tous les comptes d’utilisateur disposent de droits d’administration pour se connecter au locataire client avec la vérification MFA, y compris les agents d’administration et les agents du support technique. À des fins de test, les partenaires peuvent activer la [stratégie MFA pour les administrateurs](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) dans le locataire client, puis essayer d’utiliser des privilèges d’administration déléguée de partenaire pour accéder par programme au locataire client.

### <a name="mfa-registration-experience"></a>Expérience d’inscription MFA
Pendant la vérification de l’authentification multifacteur, si le compte partenaire n’est pas inscrit pour l’authentification MFA avant, Azure AD invite l’utilisateur à effectuer d’abord l’inscription MFA :

![Étape d’inscription MFA 1](images/MfaRegistration1.png)

Après avoir cliqué sur **suivant**, l’utilisateur est invité à choisir parmi une liste de méthodes de vérification (notamment téléphone, SMS et application d’authentificateur).

![Étape d’inscription MFA 2](images/MfaRegistration2.png)

Une fois l’inscription terminée, l’utilisateur est tenu d’effectuer la vérification de l’authentification multifacteur en fonction de la vérification choisie par l’utilisateur.



## <a name="request-for-technical-exception"></a>Demande d’exception technique

Les partenaires peuvent demander une exception technique pour supprimer la vérification de l’authentification MFA s’ils rencontrent des problèmes techniques avec Microsoft Online Services et qu’il n’existe pas de solution ou de solution de contournement faisable. Avant cela, consultez les sections suivantes :

 - [Liste des problèmes courants signalés par les partenaires](#list-of-common-issues-reported-by-partners)
 - [Envoi d’une demande d’exception technique](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Liste des problèmes courants signalés par les partenaires
Avant d’appliquer une exception technique, consultez la liste des problèmes courants signalés par d’autres partenaires pour déterminer s’il s’agit de raisons valables pour une exception technique ou non.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problème 1 : le partenaire a besoin de plus de temps pour mettre en œuvre l’authentification multifacteur pour ses agents partenaires
Un partenaire n’a pas démarré ou est toujours en train de mettre en œuvre l’authentification multifacteur pour ses agents partenaires qui nécessitent l’accès aux portails Microsoft Online Services à l’aide de privilèges d’administration délégués partenaires pour gérer les ressources client. Le partenaire a besoin de plus de temps pour effectuer l’implémentation de l’authentification MFA. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: non. Le partenaire doit faire en sorte de mettre en œuvre l’authentification MFA pour ses utilisateurs afin d’éviter toute interruption.

> [!NOTE]
> Même si le partenaire n’a pas implémenté l’authentification multifacteur pour ses agents partenaires, les agents partenaires peuvent toujours accéder aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée des partenaires, à condition qu’ils puissent effectuer l’inscription MFA et la vérification de l’authentification multifacteur. Lorsque vous y êtes invité pendant la connexion au locataire client. La finalisation de l’inscription MFA n’active pas automatiquement l’utilisateur pour MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problème 2 : le partenaire n’a pas implémenté l’authentification MFA pour les comptes d’utilisateur n’utilisant pas de privilèges d’administrateur délégué
Un partenaire a des utilisateurs dans leurs locataires partenaires qui n’ont pas besoin d’accéder aux portails Microsoft Online Services pour gérer les ressources client à l’aide des privilèges d’administration délégués de partenaire. Le partenaire est en train de mettre en œuvre l’authentification multifacteur pour ces utilisateurs et d’avoir besoin de plus de temps. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: non. Étant donné que ces comptes d’utilisateur n’utilisent pas de privilèges d’administration déléguée de partenaire pour gérer les ressources client, ils n’ont pas besoin de se connecter au locataire client. Ils ne seront pas affectés par les Azure AD nécessitant une vérification MFA lors de la connexion au locataire client.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problème 3 : le partenaire n’a pas implémenté l’authentification MFA pour les comptes de service utilisateur
Un partenaire possède des comptes d’utilisateur dans leurs locataires partenaires qui sont utilisés par les appareils comme comptes de service. Il s’agit généralement de comptes à faibles privilèges qui n’ont pas besoin d’accéder à l’espace partenaires ou aux portails Microsoft Online Services pour gérer les ressources client à l’aide des privilèges d’administration délégués du partenaire. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: non. Étant donné que ces comptes d’utilisateur n’utilisent pas de privilèges d’administration déléguée de partenaire pour gérer les ressources client, ils n’ont pas besoin de se connecter au locataire client. Ils ne seront pas affectés par les Azure AD nécessitant une vérification MFA lors de la connexion au locataire client.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problème 4 : le partenaire ne peut pas implémenter MFA à l’aide de l’application MS Authenticator
Un partenaire dispose d’une stratégie de « nettoyage » qui ne permet pas aux employés de placer leurs appareils mobiles personnels dans leur zone de travail. Sans accès à leurs appareils mobiles personnels, les employés ne peuvent pas installer l’application MS Authenticator, qui est la seule vérification MFA prise en charge par Azure AD stratégies de base de référence. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: non, il ne s’agit pas d’une raison valable pour une exception technique. Le partenaire doit prendre en compte les alternatives suivantes, afin que ses employés puissent toujours effectuer la vérification de l’authentification multifacteur lors de l’accès à l’espace partenaires :
- Outre l’application MS Authenticator, Azure AD stratégies de base de référence peuvent également être utilisées avec une application d’authentificateur compatible tierce, qui peut être des ordinateurs Windows pris en charge exécutant Microsoft Windows.
- Le partenaire peut également s’inscrire à Azure AD Premium ou à des solutions MFA tierces (compatibles avec Azure AD) qui peuvent fournir des méthodes de vérification supplémentaires.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problème 5 : le partenaire ne peut pas implémenter MFA en raison de l’utilisation de protocoles d’authentification hérités
Un partenaire a des agents partenaires qui utilisent encore des protocoles d’authentification hérités, qui ne sont pas compatibles MFA. Par exemple, les utilisateurs utilisent toujours Outlook 2010 qui est basé sur les protocoles d’authentification hérités. L’activation de l’authentification multifacteur pour ces agents partenaires perturbera l’utilisation des protocoles d’authentification hérités.

**Réponse**: non, il ne s’agit pas d’une raison valable pour une exception technique. Les partenaires sont vivement encouragés à quitter l’utilisation des protocoles d’authentification hérités en raison des implications potentielles de la sécurité, car ces protocoles ne peuvent pas être protégés par la vérification MFA et sont bien plus vulnérables à la compromission des informations d’identification. Si le déplacement à partir de l’utilisation de protocoles d’authentification hérités n’est pas une option, les partenaires doivent s’inscrire à Azure AD Premium, qui prend en charge l’utilisation de mots de passe d’application. Les mots de passe d’application sont des mots de passe à usage unique générés par le système qui sont généralement plus forts que les mots de passe générés par les humains. En utilisant des mots de passe d’application, les partenaires peuvent implémenter l’authentification multifacteur pour leurs utilisateurs, tout en revenant aux mots de passe d’application pour les protocoles d’authentification hérités uniquement.

> [!NOTE]
> Même si le partenaire n’a pas implémenté l’authentification multifacteur pour ses agents partenaires, les agents partenaires peuvent toujours accéder aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée des partenaires, à condition qu’ils puissent effectuer l’inscription MFA et la vérification de l’authentification multifacteur. Lorsque vous y êtes invité pendant la connexion au locataire client. La finalisation de l’inscription MFA n’active pas automatiquement l’utilisateur pour MFA.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>Problème 6 : un partenaire utilise Exchange Online PowerShell qui ne prend pas en charge MFA
Un partenaire utilise Exchange Online PowerShell avec des privilèges d’administration déléguée de partenaire pour gérer le service Exchange Online pour le compte de ses clients. Exchange Online PowerShell ne prend pas en charge MFA. Si le partenaire implémente l’authentification multifacteur pour ses utilisateurs, ces utilisateurs ne seront plus en mesure d’accéder à Exchange Online PowerShell. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: Oui, cela peut être considéré comme une raison valable pour une exception technique. Le [module Exchange Online PowerShell existant qui prend en charge l’administration déléguée partenaire](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ne requiert pas que l’utilisateur partenaire se connecte au locataire client et n’est donc pas affecté par Azure ad nécessitant une vérification mfa. Toutefois, il n’est pas compatible avec MFA. L’équipe Microsoft Exchange Online développe un nouveau module PowerShell qui prend en charge les privilèges d’administration délégués partenaires et l’authentification multifacteur. Tant que le nouveau module PowerShell n’est pas disponible, les partenaires ne peuvent pas implémenter l’authentification multifacteur pour les utilisateurs qui doivent utiliser le module PowerShell existant. Si ces utilisateurs rencontrent des difficultés à accéder à d’autres services Microsoft Online Services en raison de Azure AD nécessitant une vérification de l’authentification multifacteur lors de la connexion entre locataires, les partenaires peuvent demander une exception technique pour supprimer la vérification MFA.

> [!NOTE]
> Même si le partenaire ne peut pas implémenter l’authentification multifacteur pour les utilisateurs qui ont besoin d’accéder au module Exchange Online PowerShell, ces utilisateurs peuvent toujours accéder aux services en ligne de Microsoft pour gérer les ressources client à l’aide des privilèges d’administration délégués partenaires fournis. ils peuvent effectuer une inscription MFA et une vérification MFA lorsque vous y êtes invité pendant la connexion au locataire client. L’inscription de l’authentification MFA n’active pas automatiquement l’utilisateur pour l’authentification MFA et n’a donc pas d’incidence sur l’accès au module Exchange Online PowerShell.

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>Problème 7 : le partenaire a implémenté l’authentification MFA tierce qui n’est pas reconnue par Azure AD
Un partenaire a implémenté l’authentification MFA pour ses utilisateurs à l’aide d’une solution MFA tierce. Toutefois, le partenaire ne parvient pas à configurer correctement la solution MFA tierce pour qu’elle relaie à Azure AD que la vérification de l’authentification multifacteur a été effectuée pendant l’authentification de l’utilisateur. S’agit-il d’une raison valable pour une exception technique ?

**Réponse**: Oui, cela peut être considéré comme une raison valable pour une exception technique. Avant de soumettre une demande d’exception technique, veuillez confirmer auprès du fournisseur de solutions MFA tiers que la solution MFA ne peut pas être configurée pour transmettre la revendication *authenticationmethodsreferences* (avec la valeur *multipleauthn*) à Azure ad pour indiquer que la vérification de l’authentification multifacteur a été effectuée pendant l’authentification de l’utilisateur. Lorsque vous soumettez une demande d’exception technique, fournissez les détails de la solution MFA tierce utilisée et indiquez la méthode d’intégration (par exemple, la Fédération d’identité ou l’utilisation d’Azure AD contrôle personnalisé).

### <a name="how-to-submit-a-request-for-technical-exception"></a>Envoi d’une demande d’exception technique

Pour soumettre une demande d’exception technique :

1. Connectez-vous à l’espace partenaires en tant qu’administrateur général ou agent d’administration.
2. Pour créer une demande de service partenaire, accédez à **prise en charge** → **demandes de support partenaires** , puis cliquez sur **nouvelle requête**.
4. Sous **MFA et Secure Application Model** , rubrique **soumettre une demande d’exception technique** comme type de problème.
6. Fournissez les détails nécessaires pour soumettre une demande de service pour une exception technique, puis cliquez sur **Envoyer**.

Microsoft peut prendre jusqu’à 3 jours ouvrables pour fournir une réponse à une demande d’exception technique.
