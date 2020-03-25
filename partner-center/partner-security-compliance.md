---
title: Statut des exigences de sécurité des partenaires | Espace partenaires
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez les nouveaux critères obligatoires de renforcement de la sécurité pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires du programme Fournisseur de solutions Cloud.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: high
ms.topic: conceptual
ms.openlocfilehash: 2fc0926f2277cea8eebd7157af44338aabfaa94c
ms.sourcegitcommit: e98684319d8f9bfc2cadad77fd7c51d7aa32c419
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80136320"
---
# <a name="partner-security-requirements-status"></a>Statut des exigences de sécurité des partenaires

**S’applique à**

- Tous les partenaires du programme Fournisseur de solutions Cloud
  - Facturation directe
  - Fournisseurs indirects
  - Revendeur indirect
- Tous les fournisseurs de panneau de contrôle
- Tous les conseillers

**Utilisateurs appropriés**
-    Tous les utilisateurs activés, y compris les utilisateurs invités

L’amélioration de la sécurité et de la protection de la confidentialité fait partie de nos premières priorités. Nous savons que la meilleure défense est la prévention et que nous ne sommes pas plus solides que notre maillon le plus faible. C’est pourquoi nous avons besoin que tous les membres de notre écosystème puissent agir et s’assurer qu’ils disposent des protections de sécurité appropriées. Pour aider à protéger les partenaires et les clients, nous proposons un ensemble d’exigences de sécurité obligatoires pour les conseillers, les fournisseurs de panneau de contrôle et les partenaires participant au programme Fournisseur de solutions Cloud.

Depuis le 1er août 2019, tous les partenaires doivent mettre en œuvre l’authentification multifacteur pour tous les utilisateurs, y compris les comptes de service, dans leur locataire de partenaire. Pour obtenir des informations plus détaillées sur les nouvelles stratégies de sécurité, consultez [Exigences de sécurité des partenaires](partner-security-requirements.md).

Nous voulons nous assurer que chaque utilisateur passe un test MFA pour chaque authentification unique. Cela est possible en procédant de l’une des façons suivantes :

- En implémentant Azure AD Premium pour vérifier l’application de l’authentification multifacteur pour chaque utilisateur
- Implémentation des [paramètres de sécurité par défaut d’Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- En implémentant une solution tierce pour vérifier l’application de l’authentification multifacteur pour chaque utilisateur

## <a name="partner-security-requirements-status"></a>Statut des exigences de sécurité des partenaires

Ce rapport peut vous aider à vérifier le statut des exigences de sécurité en vous permettant de voir d’éventuels manquements. Le suivi est régulièrement mis à jour.

>[!NOTE]
>Le rapport sur le statut des exigences de sécurité des partenaires est pris en charge uniquement dans l’Espace partenaires. Il n’est pas disponible dans Microsoft Cloud for US Government ni Microsoft Cloud Allemagne. Nous recommandons vivement que tous les partenaires qui effectuent des transactions par le biais d’un cloud souverain (21Vianet, US Government et Allemagne) adoptent immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux nouvelles exigences de sécurité à compter du 1er août 2019. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

## <a name="multi-factor-authentication-mfa-report"></a>Rapport d’authentification multifacteur (« MFA »)

Le rapport MFA de l’Espace partenaires offre des insights sur l’implémentation de MFA chez les partenaires en proposant deux métriques basées sur la configuration MFA et les activités dans l’Espace partenaires du locataire CSP : 

### <a name="mfa-configuration-on-a-csp-tenant"></a>Configuration MFA sur un locataire CSP

Cette métrique est liée à la configuration MFA sur un locataire CSP qui a effectué des captures et des rapports tous les jours. Elle mesure le pourcentage de comptes d’utilisateur activés avec MFA appliqué en utilisant l’une de ces [options MFA](https://aka.ms/partner-mfa-get-started). Par exemple :

- Contoso est un partenaire CSP avec 110 comptes d’utilisateur dans le locataire, dont 10 sont désactivés. 
- Sur les 100 comptes d’utilisateur restants, 90 ont MFA appliqué en utilisant les [options MFA](https://aka.ms/partner-mfa-get-started) fournies. Par conséquent, la métrique affiche 90 %. 

### <a name="partner-center-activities-with-mfa"></a>Activités dans l’Espace partenaires avec MFA

Chaque fois que vos employés se connectent à l’Espace partenaires pour travailler ou, par le biais d’API, recevoir ou envoyer des données via l’Espace partenaires, leur statut de sécurité est testé et suivi. Vos applications et les applications de tout fournisseur de panneau de contrôle sont également incluses dans le suivi du statut de sécurité. Le statut affiché correspond aux sept derniers jours.

#### <a name="mfa-verification-completed-by-users"></a>Vérification MFA effectuée par les utilisateurs

Cette métrique est liée aux activités figurant dans le tableau de bord de l’Espace partenaires. Elle mesure le pourcentage des opérations effectuées par les utilisateurs qui ont effectué la vérification MFA. Par exemple :

- Contoso est un partenaire fournisseur de solutions Cloud employant deux agents d’administration, Jane et John.
- Le premier jour, Jane s’est connectée au tableau de bord de l’Espace partenaires sans vérification MFA et a effectué 3 opérations.
- Le deuxième jour, John s’est connecté au tableau de bord de l’Espace partenaires sans vérification MFA et a effectué 5 opérations.
- Le troisième jour, Jane s’est connectée au tableau de bord de l’Espace partenaires avec la vérification MFA et a effectué 2 opérations.
- Aucune opération n’a été effectuée par ces agents les 4 jours restants.
- Parmi les 10 opérations effectuées dans cette fenêtre de 7 jours, 2 ont été effectuées par un utilisateur avec la vérification MFA. Par conséquent, la métrique affiche 20 %.

#### <a name="appuser-authentication"></a>Authentification Application+Utilisateur

Cette métrique est liée à l’utilisation des demandes d’API de l’Espace partenaires effectuées à l’aide de l’authentification Application+Utilisateur. Elle mesure le pourcentage de demandes d’API effectuées en utilisant un jeton d’accès avec la revendication MFA. Par exemple :

- Fabrikam est un partenaire fournisseur de solutions Cloud et possède une application CSP qui utilise une combinaison de méthodes d’authentification Application+Utilisateur et d’authentification d’application uniquement.
- Le premier jour, cette application a effectué trois demandes d’API qui ont été appuyées par un jeton d’accès obtenu par le biais de la méthode d’authentification Application+Utilisateur sans vérification MFA.
- Le deuxième jour, l’application a effectué cinq demandes d’API qui ont été appuyées par un jeton d’accès obtenu à l’aide de l’authentification d’application uniquement.
- Le troisième jour, l’application a effectué deux demandes d’API qui ont été appuyées par un jeton d’accès obtenu par le biais de la méthode d’authentification Application+Utilisateur avec vérification MFA.
- Aucune opération n’a été effectuée par ces agents les quatre jours restants.
- Les cinq demandes d’API du deuxième jour qui ont été appuyées par un jeton d’accès obtenu par le biais de l’authentification d’application uniquement sont omises de la métrique, car elle n’utilise pas les informations d’identification de l’utilisateur. Parmi les cinq opérations restantes, deux ont été appuyées par un jeton d’accès obtenu avec la vérification MFA. Par conséquent, la métrique affiche 40 %.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Que dois-je faire si les métriques du rapport MFA ne correspondent pas à 100 %

Il est possible que les métriques du rapport d’authentification multifacteur de l’Espace partenaires ne correspondent pas à 100 % pour les partenaires qui ont implémenté l’authentification multifacteur. Pour comprendre pourquoi, voici quelques facteurs à prendre en compte.

> [!NOTE]
> Vous devez travailler avec une personne de votre organisation qui maîtrise la gestion des identités et l’implémentation de l’authentification multifacteur pour le locataire de votre partenaire.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Avez-vous implémenté l’authentification multifacteur pour le locataire de votre partenaire ?

Si vous ne l’avez pas fait, vous devez commencer par implémenter l’authentification multifacteur pour le locataire de votre partenaire. Pour plus d’informations sur la manière d’implémenter l’authentification multifacteur, consultez l’article [Exigences de sécurité des partenaires](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Avez-vous implémenté l’authentification multifacteur récemment seulement ?

Les métriques sont calculées quotidiennement et prennent en compte les opérations effectuées au cours des 7 derniers jours. Si vous avez effectué l’implémentation de l’authentification multifacteur récemment seulement pour le locataire de votre partenaire, les métriques peuvent ne pas représenter 100 %.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Certains comptes d’utilisateur ont-ils été exclus de l’implémentation de l’authentification multifacteur ?

Déterminez si votre implémentation de l’authentification multifacteur actuelle couvre tous les comptes d’utilisateur ou seulement certains. Certaines solutions MFA sont basées sur des stratégies et prennent en charge l’exclusion des utilisateurs, tandis que d’autres peuvent vous obliger à activer explicitement MFA pour chaque utilisateur. Vérifiez que vous n’avez exclu aucun utilisateur de votre implémentation MFA actuelle. Tout compte d’utilisateur qui est exclu et qui se connecte à l’Espace partenaires pour effectuer une activité quelconque liée à un fournisseur de solutions Cloud peut donner lieu à des métriques n’atteignant pas 100 %.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>L’authentification multifacteur est-elle nécessaire uniquement lorsque certaines conditions sont remplies ?

Déterminez si votre implémentation actuelle applique uniquement MFA dans des conditions spécifiques. Certaines solutions MFA offrent une flexibilité permettant d’appliquer l’authentification multifacteur uniquement lorsque certaines conditions sont remplies. Par exemple, l’accès de l’utilisateur s’effectue à partir d’un appareil inconnu ou d’un emplacement inconnu. Un utilisateur configuré pour l’authentification multifacteur mais qui n’est pas tenu d’effectuer la vérification MFA lorsqu’il accède à l’Espace partenaires peut donner lieu à des métriques ne correspondant pas à 100 %.

>[!NOTE]
>Pour les partenaires qui ont implémenté l’authentification MFA à l’aide des paramètres de sécurité par défaut d’Azure AD, il est important de noter que, pour les comptes d’utilisateur non-administrateur, l’authentification multifacteur est appliquée en fonction du risque. Les utilisateurs font l’objet d’une authentification MFA uniquement durant les tentatives de connexion à risques (par exemple, l’utilisateur se connecte depuis un autre emplacement). De plus, les utilisateurs ont jusqu’à 14 jours pour s’inscrire auprès de l’authentification MFA. Les utilisateurs qui ne sont pas inscrits auprès de l’authentification MFA ne font pas l’objet d’une vérification MFA durant cette période de 14 jours. Ainsi, les métriques ne sont probablement pas de 100 % pour les partenaires ayant implémenté l’authentification MFA à l’aide des paramètres de sécurité par défaut d’Azure AD.

### <a name="are-you-using-3rd-party-mfa-solution"></a>Utilisez-vous une solution MFA tierce ?

Si vous utilisez une solution MFA tierce, identifiez la façon dont vous l’intégrez à Azure AD. En général, il existe deux méthodes, la fédération et les contrôles personnalisés :

* **Fédération des identités** - Quand Azure AD reçoit une demande d’authentification, Azure AD redirige l’utilisateur vers le fournisseur d’identité fédérée pour son authentification. Une fois l’authentification réussie, le fournisseur d’identité fédérée redirige l’utilisateur vers Azure AD avec un jeton SAML. Pour qu’Azure AD reconnaisse que l’utilisateur a effectué la vérification MFA lors de son authentification auprès du fournisseur d’identité fédérée, le jeton SAML doit inclure la revendication *authenticationmethodsreferences* (avec la valeur *multipleauthn* ). Vérifiez si le fournisseur d’identité fédérée prend en charge l’émission d’une telle revendication. Si c’est le cas, vérifiez si le fournisseur d’identité fédérée a été configuré pour cela. Si la revendication est manquante, Azure AD (et par conséquent l’Espace partenaires) ne saura pas que l’utilisateur a effectué la vérification MFA et cela peut donner lieu à une métrique ne correspondant pas à 100 %.

* **Contrôle personnalisé** - Le contrôle personnalisé Azure AD ne peut pas être utilisé pour déterminer si un utilisateur a effectué la vérification MFA via une solution MFA tierce. Par conséquent, tout utilisateur qui a effectué la vérification MFA via un contrôle personnalisé apparaîtra toujours à Azure AD (et, à son tour, à l’Espace partenaires) comme n’ayant pas effectué la vérification MFA. Dans la mesure du possible, il est recommandé d’adopter la fédération des identités par opposition au contrôle personnalisé lors de l’intégration avec Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identifier les utilisateurs qui se sont connectés à l’Espace partenaires sans MFA

Il peut s’avérer utile d’identifier les utilisateurs qui se connectent à l’Espace partenaires sans vérification MFA et de les vérifier par rapport à votre implémentation MFA actuelle. Vous pouvez utiliser le [rapport de connexion Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) pour déterminer si un utilisateur a effectué ou non la vérification MFA. Le rapport de connexion Azure AD est actuellement disponible uniquement pour les partenaires qui se sont abonnés à Azure AD Premium ou à une référence O365 incluant Azure AD Premium (par exemple, EMS).

**Pour plus d’informations**

- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Exigences de sécurité de l’Espace partenaires](partner-security-requirements.md)
- [Questions fréquentes (FAQ) sur les exigences de sécurité de l’Espace partenaires](partner-security-requirements-faq.md)
