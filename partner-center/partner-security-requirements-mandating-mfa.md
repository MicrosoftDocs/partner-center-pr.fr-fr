---
title: Imposer l’authentification multifacteur (MFA) à votre locataire partenaire
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment le fait d’imposer l’authentification multifacteur à vos locataires partenaires contribuera à sécuriser votre accès aux ressources client. Inclut des exemples de scénarios.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b6985054e927dd777d61ae30bd435ab4c6c4ea8c
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133103"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Imposer l’authentification multifacteur (MFA) à votre locataire partenaire

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

**Rôles affectés**

- Agent d’administration
- Agent commercial
- Agent du support technique
- Administrateur de facturation
- Administrateur général

Cet article donne des exemples et des conseils détaillés pour imposer l’authentification multifacteur (MFA) dans l’Espace partenaires. L’objectif de cette fonctionnalité est d’aider les partenaires à sécuriser leur accès aux ressources client contre toute compromission des informations d’identification. Les partenaires sont tenus d’appliquer MFA à tous les comptes d’utilisateur de leur locataire partenaire, y compris les utilisateurs invités. Les utilisateurs seront chargés d’effectuer la vérification MFA pour les domaines suivants :

- [Tableau de bord de l’Espace partenaires](#partner-center-dashboard)
- [API d’Espace partenaires](#partner-center-api)
- [Administration déléguée de partenaire](#partner-delegated-administration)

La qualité et la continuité des mesures de sécurité et de confidentialité font partie de nos principales priorités, et nous continuons à aider les partenaires à protéger leurs clients et leurs locataires. Tous les partenaires qui participent au programme Fournisseur de solutions Microsoft Cloud (CSP), les fournisseurs de panneau de contrôle (CPV) et les conseillers Advisor doivent implémenter les [exigences de sécurité du partenaire](partner-security-requirements.md) pour rester conformes.

Pour aider les partenaires à protéger leurs entreprises et leurs clients contre l’usurpation d’identité et l’accès non autorisé, nous avons activé des protections de sécurité supplémentaires pour les locataires partenaires qui imposent et vérifient MFA. 

## <a name="partner-center-dashboard"></a>Tableau de bord de l’Espace partenaires

Certaines pages du tableau de bord de l’Espace partenaires seront protégées par l’authentification multifacteur, notamment :

- Toutes les pages sous l’onglet **Clients** , par exemple toutes les pages accessibles par le biais de l’URL suivante : https://partner.microsoft.com/commerce/*
- Toutes les pages sous l’onglet **Support > Demandes client** , par exemple la page accessible sous https://partner.microsoft.com/dashboard/support/csp/customers/*
- Page de facturation

Le tableau suivant montre les types d’utilisateurs qui sont autorisés à accéder à ces pages protégées par MFA (et qui sont donc affectés par cette fonctionnalité).


| Page protégée par MFA       | Agents d’administration      |  Agents commerciaux     |   Agents du support technique     | Administrateur général      |  Administrateur de facturation     | 
|---    |---    |---    |---    |---    |---    |
| Toutes les pages sous l’onglet Clients      |   x    |    x   |  x     |       |       |
| Toutes les pages sous l’onglet Support > Demandes client     | x      |       |    x   |       |       |
| Page de facturation     |   x    |       |       |    x   |   x    |

Si vous essayez d’accéder à l’une de ces pages alors que vous n’avez pas encore effectué la vérification MFA, vous êtes tenu de l’effectuer. Les autres pages de l’Espace partenaires, telles que la page de vue d’ensemble et la page de vérification de l’état d’intégrité des services, ne nécessitent pas MFA.

## <a name="verification-examples"></a>Exemples de vérification

Pour illustrer le fonctionnement de la vérification dans le tableau de bord de l’Espace partenaires, examinez les exemples suivants.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Exemple 1 : Le partenaire a implémenté l’authentification multifacteur Azure AD

1. Jane travaille pour le fournisseur de solutions Cloud Contoso. Contoso a implémenté l’authentification multifacteur pour tous ses utilisateurs sous le locataire partenaire Contoso à l’aide de l’authentification multifacteur Azure Active Directory (Azure AD).

2. Jane démarre une nouvelle session de navigateur et accède à la page de présentation du tableau de bord de l’Espace partenaires (qui n’est pas protégée par authentification multifacteur). L’Espace partenaires redirige Jane vers Azure AD pour lui permettre de se connecter.

3. En raison de la configuration existante de l’authentification multifacteur Azure AD par Contoso, Jane est tenue d’effectuer la vérification MFA. Une fois la connexion et la vérification MFA réussies, Jane est redirigée vers la page de vue d’ensemble du tableau de bord de l’Espace partenaires.

4. Jane tente d’accéder à l’une des pages protégées par authentification multifacteur dans l’Espace partenaires. Comme Jane a déjà effectué la vérification MFA pour se connecter précédemment, elle peut accéder à la page protégée par authentification multifacteur sans avoir à répéter la vérification MFA.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Exemple 2 : Le partenaire a implémenté une authentification multifacteur tierce utilisant la fédération d’identité

1. Trent travaille pour le fournisseur de solutions Cloud Wingtip. Wingtip a implémenté l’authentification multifacteur pour tous ses utilisateurs sous le locataire partenaire Wingtip à l’aide d’une authentification multifacteur tierce, qui est intégrée à Azure AD via la fédération d’identité.

2. Trent démarre une nouvelle session de navigateur et accède à la page de présentation du tableau de bord de l’Espace partenaires (qui n’est pas protégée par authentification multifacteur). L’Espace partenaires redirige Trent vers Azure AD pour lui permettre de se connecter.

3. Comme Wingtip a configuré la fédération d’identité, Azure AD redirige Trent vers le fournisseur d’identité fédérée pour effectuer la connexion et la vérification MFA. Une fois la connexion et la vérification MFA réussies, Trent est redirigé vers Azure AD, puis vers la page de vue d’ensemble du tableau de bord de l’Espace partenaires.

4. Trent tente d’accéder à l’une des pages protégées par authentification multifacteur dans l’Espace partenaires. Comme Trent a déjà effectué la vérification MFA pour se connecter précédemment, il peut accéder à la page protégée par authentification multifacteur sans avoir à répéter la vérification MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Exemple 3 : Le partenaire n’a pas implémenté l’authentification multifacteur

1. John travaille pour le fournisseur de solutions Cloud Fabrikam. Fabrikam n’a implémenté l’authentification multifacteur pour aucun utilisateur sous le locataire partenaire Fabrikam.

2. John démarre une nouvelle session de navigateur et accède à la page de présentation du tableau de bord de l’Espace partenaires (qui n’est pas protégée par authentification multifacteur). L’Espace partenaires redirige John vers Azure AD pour lui permettre de se connecter.

3. Comme Fabrikam n’a pas mis en œuvre l’authentification multifacteur, John n’est pas tenu d’effectuer la vérification MFA. Une fois la connexion réussie, John est redirigé vers la page de vue d’ensemble du tableau de bord de l’Espace partenaires.

4. John tente d’accéder à l’une des pages protégées par authentification multifacteur dans l’Espace partenaires. Comme John n’a pas effectué la vérification MFA, l’Espace partenaires redirige John vers Azure AD pour lui permettre d’effectuer la vérification MFA. Comme il s’agit de la première fois que John est tenu d’effectuer la vérification MFA, il est également invité à [effectuer l’inscription MFA](#mfa-registration-experience). Une fois l’inscription MFA et la vérification MFA réussies, John peut désormais accéder à la page protégée par authentification multifacteur.

5. Un autre jour avant que Fabrikam implémente l’authentification multifacteur, John démarre une nouvelle session de navigateur et accède à la page de vue d’ensemble du tableau de bord de l’Espace partenaires (qui n’est pas protégée par MFA). L’Espace partenaires redirige John vers Azure AD pour lui permettre de se connecter sans invite MFA. 

6. John tente d’accéder à l’une des pages protégées par authentification multifacteur dans l’Espace partenaires. Comme John n’a pas effectué la vérification MFA, l’Espace partenaires redirige John vers Azure AD pour lui permettre d’effectuer la vérification MFA. John s’étant inscrit pour l’authentification MFA, cette fois-ci il lui suffit de procéder à la vérification MFA.

> [!NOTE]
>Action : Les administrateurs d’entreprise ont [trois options](partner-security-requirements.md#implementing-multi-factor-authentication) pour implémenter MFA.

## <a name="partner-center-api"></a>API d’Espace partenaires

L’API d’Espace partenaires prend en charge l’authentification d’application uniquement et l’authentification Application+Utilisateur. 

Lorsque l’authentification Application+Utilisateur est utilisée, l’Espace partenaires exige la vérification MFA. Plus précisément, lorsqu’une application partenaire souhaite envoyer une demande d’API à l’Espace partenaires, elle doit inclure un jeton d’accès dans l’en-tête d’autorisation de la demande. 

> [!NOTE]
>Le [modèle d’application sécurisé](/partner-center/develop/enable-secure-app-model) est un framework scalable pour l’authentification des partenaires CSP et des CPV par le biais de l’architecture Microsoft Azure MFA lors de l’appel des API de l’Espace partenaires. Vous devez implémenter ce framework avant d’activer MFA sur votre locataire. 

Quand l’Espace partenaires reçoit une demande d’API avec un jeton d’accès obtenu à l’aide de l’authentification Application+Utilisateur, l’API de l’Espace partenaires vérifie la présence de la valeur *MFA* dans la revendication de *référence de méthode d’authentification (AMR)* . Vous pouvez utiliser un décodeur JWT pour vérifier si un jeton d’accès contient la valeur de référence de méthode d’authentification (AMR) attendue ou non :

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
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Si cette valeur est présente, l’Espace partenaires conclut que la vérification MFA a été effectuée et traite la demande d’API. Si cette valeur n’est pas présente, l’API d’Espace partenaires rejette la demande avec la réponse suivante :

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Quand l’authentification d’application uniquement est utilisée, les API qui la prennent en charge fonctionnent en continu sans nécessiter l’authentification MFA.

## <a name="partner-delegated-administration"></a>Administration déléguée de partenaire

Les comptes de partenaire, y compris les agents d’administration et les agents du support technique, peuvent utiliser leurs privilèges d’administration déléguée de partenaire pour gérer les ressources client par le biais des portails Microsoft Online Services, de l’interface de ligne de commande (CLI) et des API (à l’aide de l’authentification Application+Utilisateur).

### <a name="using-service-portals"></a>Utilisation des portails de service

Lors de l’accès aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée de partenaire (Administration pour le compte de) pour gérer les ressources client, un grand nombre de ces portails requièrent l’authentification interactive du compte de partenaire, avec le locataire Azure AD client défini comme contexte d’authentification : le compte de partenaire est nécessaire pour se connecter au locataire client.

Quand Azure AD reçoit de telles demandes d’authentification, il exige que le compte de partenaire effectue la vérification MFA. Il existe deux expériences utilisateur possibles, selon que le compte de partenaire est une identité managée ou fédérée :

- Si le compte de partenaire est une **identité managée** , Azure AD invite directement l’utilisateur à effectuer la vérification MFA. Si le compte de partenaire n’a pas effectué l’inscription MFA avec Azure AD, l’utilisateur est d’abord invité à [effectuer l’inscription MFA](#mfa-registration-experience).

- Si le compte de partenaire est une identité **fédérée** , l’expérience dépend de la manière dont l’administrateur partenaire a configuré la fédération dans Azure AD. Lors de la configuration de la fédération dans Azure AD, l’administrateur partenaire peut indiquer à Azure AD si le fournisseur d’identité fédérée prend en charge ou non MFA. Si c’est le cas, Azure AD redirige l’utilisateur vers le fournisseur d’identité fédérée pour effectuer la vérification MFA. Dans le cas contraire, Azure AD invite directement l’utilisateur à effectuer la vérification MFA. Si le compte de partenaire n’a pas effectué l’inscription MFA avec Azure AD, l’utilisateur est d’abord invité à [effectuer l’inscription MFA](#mfa-registration-experience).

L’expérience globale est similaire au scénario dans lequel un locataire client final a mis en œuvre l’authentification multifacteur pour ses administrateurs. Par exemple, le locataire client a activé les [paramètres Azure AD de sécurité par défaut](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), ce qui nécessite que tous les comptes avec des droits d’administration se connectent au locataire client avec la vérification MFA, y compris les agents d’administration et les agents du support technique. À des fins de test, les partenaires peuvent activer les [paramètres Azure AD de sécurité par défaut](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) dans le locataire client, puis essayer d’utiliser les privilèges d’administration déléguée de partenaire pour accéder au locataire client.

> [!NOTE]
> Tous les portails Microsoft Online Services ne nécessitent pas que les comptes de partenaire se connectent au locataire client lorsqu’ils accèdent aux ressources client à l’aide des privilèges d’administration déléguée de partenaire. Au lieu de cela, ils ont uniquement besoin que les comptes de partenaire se connectent au locataire partenaire. Le Centre d’administration Exchange en est un exemple. À l’avenir, nous pensons que ces portails exigeront que les comptes de partenaire se connectent au locataire client lorsqu’ils utiliseront les privilèges d’administration déléguée de partenaire.

### <a name="using-service-apis"></a>Utilisation des API de service

Certaines API Microsoft Online Services (telles qu’Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) prennent en charge les partenaires qui utilisent les privilèges d’administration déléguée de partenaire pour gérer par programmation les ressources client. Pour tirer parti des privilèges d’administration déléguée de partenaire avec ces API, l’application de partenaire doit inclure un jeton d’accès dans l’en-tête d’autorisation de demande d’API, où le jeton d’accès est obtenu en amenant un compte d’utilisateur de partenaire à s’authentifier auprès d’Azure AD, avec le client Azure AD défini comme contexte d’authentification. L’application de partenaire doit amener un compte d’utilisateur de partenaire à se connecter au locataire client.

Quand Azure AD reçoit une telle demande d’authentification, il exige que le compte d’utilisateur de partenaire effectue la vérification MFA. Si le compte d’utilisateur de partenaire n’a pas encore effectué l’inscription MFA, le compte d’utilisateur est invité à effectuer d’abord l’inscription MFA.

Toutes les applications de partenaire intégrées à ces API à l’aide de privilèges d’administration déléguée de partenaire sont affectées par cette fonctionnalité. Pour s’assurer que les applications de partenaire pourront continuer à travailler avec ces API sans interruption :

- Le partenaire doit éviter d’utiliser une méthode d’authentification utilisateur non interactive avec Azure AD pour obtenir le jeton d’accès. Lorsqu’il utilise une méthode d’authentification utilisateur non interactive telle que le [flux de mot de passe](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure AD ne pourra pas inviter l’utilisateur à effectuer la vérification MFA. Le partenaire doit utiliser à la place une méthode d’authentification utilisateur interactive comme le [flux OpenID Connect](/azure/active-directory/develop/v1-protocols-openid-connect-code).

- Dans le cadre de la méthode d’authentification utilisateur interactive, le partenaire doit utiliser un compte d’utilisateur de partenaire déjà configuré pour utiliser l’authentification multifacteur. Autrement, quand Azure AD l’y invite, le partenaire peut effectuer l’inscription MFA et la vérification MFA lors de la connexion.

- Cela est similaire au scénario dans lequel un locataire client final a mis en œuvre l’authentification multifacteur pour ses administrateurs. Par exemple, le locataire client a activé les [paramètres Azure AD de sécurité par défaut](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), ce qui nécessite que tous les comptes d’utilisateur avec des droits d’administration se connectent au locataire client avec la vérification MFA, y compris les agents d’administration et les agents du support technique. À des fins de test, les partenaires peuvent activer les [paramètres Azure AD de sécurité par défaut](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) dans le locataire client, puis essayer d’utiliser les privilèges d’administration déléguée de partenaire pour accéder par programmation au locataire client.

### <a name="mfa-registration-experience"></a>Expérience d’inscription MFA

Pendant la vérification MFA, si le compte de partenaire n’a pas encore effectué l’inscription MFA, Azure AD invite l’utilisateur à effectuer d’abord l’inscription MFA :

:::image type="content" source="images/MfaRegistration1.png" alt-text="Inscription MFA – Étape 1":::

Après avoir cliqué sur **Suivant** , l’utilisateur est invité à choisir parmi une liste de méthodes de vérification.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Inscription MFA – Étape 2":::

Une fois l’inscription réussie, l’utilisateur est tenu d’effectuer la vérification MFA en fonction de la méthode choisie par l’utilisateur.
 
## <a name="list-of-common-issues"></a>Liste des problèmes courants

Avant de demander une [exception technique](#how-to-submit-a-request-for-technical-exception) en vue de vous soustraire à l’obligation d’implémenter MFA, passez en revue la liste des problèmes courants signalés par les autres partenaires pour déterminer si votre demande est valide.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problème 1 : Le partenaire a besoin de plus de temps pour mettre en œuvre l’authentification multifacteur pour ses agents partenaires
Un partenaire n’a pas démarré ou est toujours en phase de mise en œuvre de l’authentification multifacteur pour ses agents partenaires qui nécessitent un accès aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée de partenaire pour gérer les ressources client. Le partenaire a besoin de plus de temps pour effectuer la mise en œuvre de l’authentification multifacteur. Ce problème est-il une raison valable pour demander une exception technique ?

**Réponse**  : Non. Le partenaire doit élaborer des plans pour mettre en œuvre l’authentification multifacteur pour ses utilisateurs afin d’éviter toute interruption de service.

> [!NOTE]
> Même si le partenaire n’a pas mis en œuvre l’authentification multifacteur pour ses agents partenaires, les agents partenaires peuvent toujours accéder aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée de partenaire, à condition de pouvoir effectuer l’inscription MFA et la vérification MFA lorsqu’ils y sont invités pendant la connexion au locataire client. La réalisation de l’inscription MFA ne permet pas automatiquement à l’utilisateur d’utiliser l’authentification multifacteur.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problème 2 : Le partenaire n’a pas mis en œuvre l’authentification multifacteur pour les comptes d’utilisateur qui n’utilisent pas les privilèges d’administration déléguée
Un partenaire a des utilisateurs dans ses locataires de partenaire qui ne nécessitent pas un accès aux portails Microsoft Online Services pour gérer les ressources client à l’aide de privilèges d’administration déléguée de partenaire. Le partenaire est en phase de mise en œuvre de l’authentification multifacteur pour ces utilisateurs et il a besoin de plus de temps. Ce problème est-il une raison valable pour demander une exception technique ?

**Réponse**  : Non. Comme ces comptes d’utilisateur n’utilisent pas de privilèges d’administration déléguée de partenaire pour gérer les ressources client, ils ne sont pas tenus de se connecter au locataire client. Ils ne sont pas affectés par le fait qu’Azure AD nécessite une vérification MFA lors de la connexion au locataire client.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problème 3 : Le partenaire n’a pas mis en œuvre l’authentification multifacteur pour les comptes de service utilisateur
Un partenaire a des comptes d’utilisateur dans ses locataires partenaires, qui sont utilisés par les appareils comme comptes de service. Il s’agit de comptes à faibles privilèges qui n’ont pas besoin d’accéder à l’Espace partenaires ni aux portails Microsoft Online Services pour gérer les ressources client à l’aide des privilèges d’administration déléguée de partenaire. Ce problème est-il une raison valable pour demander une exception technique ?

**Réponse**  : Non. Comme ces comptes d’utilisateur n’utilisent pas de privilèges d’administration déléguée de partenaire pour gérer les ressources client, ils ne sont pas tenus de se connecter au locataire client. Ils ne sont pas affectés par le fait qu’Azure AD nécessite une vérification MFA lors de la connexion au locataire client.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problème 4 : Le partenaire ne peut pas mettre en œuvre l’authentification multifacteur à l’aide de l’application Microsoft Authenticator
Un partenaire a mis en place une politique de « rangement de bureau », qui n’autorise pas les employés à apporter leurs appareils mobiles personnels sur leur lieu de travail. Sans accès à leurs appareils mobiles personnels, les employés ne peuvent pas installer l’application Microsoft Authenticator, qui est la seule vérification MFA prise en charge par les paramètres de sécurité par défaut Azure AD. Ce problème est-il une raison valable pour demander une exception technique ?

**Réponse**  : Non, ce n’est pas une raison valable pour demander une exception technique. Le partenaire doit prendre en compte les alternatives suivantes, afin que ses employés puissent toujours effectuer la vérification MFA lors de l’accès à l’Espace partenaires :
- Le partenaire peut également s’inscrire auprès d’Azure AD Premium ou de solutions d’authentification multifacteur tierces (compatibles avec Azure AD) susceptibles de fournir des méthodes de vérification supplémentaires.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problème 5 : Le partenaire ne peut pas mettre en œuvre l’authentification multifacteur en raison de l’utilisation de protocoles d’authentification hérités
Un partenaire a des agents partenaires qui utilisent encore des protocoles d’authentification hérités, qui ne sont pas compatibles avec l’authentification multifacteur. Par exemple, les utilisateurs utilisent encore Outlook 2010, qui est basé sur des protocoles d’authentification hérités. L’activation de l’authentification multifacteur pour ces agents partenaires perturbera l’utilisation des protocoles d’authentification hérités.

**Réponse**  : Non, ce n’est pas une raison valable pour demander une exception technique. Les partenaires sont vivement encouragés à abandonner l’utilisation des protocoles d’authentification hérités en raison des implications de sécurité potentielles, car ces protocoles ne peuvent pas être protégés par la vérification MFA et sont bien plus vulnérables à une compromission des informations d’identification. Si l’abandon de l’utilisation des protocoles d’authentification hérités n’est pas une option, les partenaires doivent envisager de s’inscrire à Azure AD Premium, qui prend en charge l’utilisation des mots de passe d’application. Les mots de passe d’application sont des mots de passe à usage unique générés par le système et sont généralement plus forts que les mots de passe générés par les humains. En utilisant des mots de passe d’application, les partenaires peuvent mettre en œuvre l’authentification multifacteur pour leurs utilisateurs, tout en revenant aux mots de passe d’application pour les protocoles d’authentification hérités uniquement.

Lisez le billet relatif à l’[authentification de base et Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) pour comprendre les plans les plus récents concernant la prise en charge de l’authentification héritée pour Outlook, et suivez le [blog de l’équipe Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) pour connaître les dernières actualités. 

> [!NOTE]
> Même si le partenaire n’a pas mis en œuvre l’authentification multifacteur pour ses agents partenaires, les agents partenaires peuvent toujours accéder aux portails Microsoft Online Services à l’aide des privilèges d’administration déléguée de partenaire, à condition de pouvoir effectuer l’inscription MFA et la vérification MFA lorsqu’ils y sont invités pendant la connexion au locataire client. La réalisation de l’inscription MFA ne permet pas automatiquement à l’utilisateur d’utiliser l’authentification multifacteur.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problème 6 : Le partenaire a implémenté une authentification multifacteur tierce qui n’est pas reconnue par Azure AD
Un partenaire a implémenté l’authentification multifacteur pour ses utilisateurs à l’aide d’une solution d’authentification multifacteur tierce. Toutefois, le partenaire ne parvient pas à configurer correctement la solution d’authentification multifacteur tierce pour qu’elle relaie à Azure AD que la vérification MFA a été effectuée pendant l’authentification de l’utilisateur. Cela est-il une raison valable pour demander une exception technique ?

**Réponse**  : Oui, ce problème peut être considéré comme une raison valable pour demander une exception technique. Avant de soumettre une demande d’exception technique, vérifiez auprès du fournisseur de la solution d’authentification multifacteur tierce que cette solution ne peut pas être configurée pour transmettre la revendication *authenticationmethodsreferences* (avec la valeur *multipleauthn* ) à Azure AD pour indiquer que la vérification MFA a été effectuée pendant l’authentification de l’utilisateur. Lors de l’envoi d’une demande d’exception technique, vous devez fournir les détails de la solution d’authentification multifacteur tierce utilisée et indiquer la méthode d’intégration (par exemple via la fédération d’identité ou l’utilisation du contrôle personnalisé Azure AD), et fournir les informations suivantes dans la demande d’exception technique en tant que documents de prise en charge :

- Les configurations MFA tierces

- Le résultat de l’exécution des [tests des exigences de sécurité du partenaire](/powershell/partnercenter/test-partner-security-requirements) par le compte prenant en charge l’authentification MFA tierce

- Le bon de commande de la solution MFA tierce que vous utilisez ou que vous envisagez d’utiliser

## <a name="how-to-submit-a-request-for-technical-exception"></a>Procédure d’envoi d’une demande d’exception technique

Les partenaires peuvent demander une exception technique pour supprimer la vérification MFA s’ils rencontrent des problèmes techniques avec Microsoft Online Services et s’il n’existe pas de solution réalisable ou de solution de contournement. Avant cela, passez en revue la [liste des problèmes courants](#list-of-common-issues) dans la section précédente.

Pour envoyer une demande d’exception technique :

1. Connectez-vous à l’Espace partenaires en tant qu’administrateur général ou agent d’administration.

2. Créez une demande de service partenaire en accédant à **Support** > **Demandes de support de partenaire** et en cliquant sur **Nouvelle demande**.

3. Tapez **MFA - Demande d’exception** dans la zone de recherche, ou sélectionnez **CSP** dans Catégorie, puis sélectionnez **Comptes, Intégration, Accès** dans Rubrique, puis sélectionnez **MFA - Demande d’exception** dans la sous-rubrique, puis sélectionnez **Étape suivante**.

4. Fournissez les détails nécessaires pour soumettre une demande de service pour une exception technique, puis cliquez sur **Soumettre**.

Microsoft peut prendre jusqu’à trois jours ouvrables pour fournir une réponse à une demande d’exception technique.

## <a name="next-steps"></a>Étapes suivantes

 - [Statut des exigences de sécurité des partenaires](partner-security-compliance.md)