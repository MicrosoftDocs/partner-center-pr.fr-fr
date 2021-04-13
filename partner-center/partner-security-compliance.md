---
title: Rapport sur l’état des exigences de sécurité
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrir comment vérifier la conformité de vos exigences de sécurité avec le rapport sur l’état des exigences de sécurité et le rapport MFA de l’Espace partenaires
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086547"
---
# <a name="security-requirements-status-report"></a>Rapport sur l’état des exigences de sécurité

**Rôles appropriés**
- Administrateur CPV
- Administrateur général

Cet article explique le rapport sur l’état des exigences de sécurité dans l’Espace partenaires. Ce rapport fournit des métriques sur la conformité des utilisateurs de votre locataire partenaire aux [exigences de sécurité des partenaires](partner-security-requirements.md) en matière d’authentification multifacteur (MFA).

Pour accéder à ce rapport dans l’[Espace partenaires](https://partner.microsoft.com/dashboard), accédez à **Paramètres** > **Paramètres du compte** > **État des exigences de sécurité**. Le rapport est mis à jour quotidiennement et reflète les données de connexion des sept derniers jours.

>[!NOTE]
>Le rapport sur l’état des exigences de sécurité est pris en charge uniquement dans l’Espace partenaires. Il n’est pas disponible dans Microsoft Cloud for US Government ni Microsoft Cloud Allemagne. Nous recommandons vivement aux partenaires qui effectuent des transactions par le biais d’un cloud souverain (US Government et Allemagne) d’adopter immédiatement ces nouvelles exigences de sécurité. Toutefois, ces partenaires ne sont pas actuellement tenus de satisfaire aux nouvelles exigences de sécurité. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

## <a name="security-status-metrics"></a>Métriques d’état de la sécurité

Le rapport sur l’état des exigences de sécurité offre des insights sur l’implémentation de MFA des partenaires et fournit des métriques basées sur la configuration MFA et les activités dans l’Espace partenaires des locataires partenaires. Les sections suivantes expliquent ces métriques de façon plus détaillée.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Configuration de MFA sur un locataire partenaire

La métrique **Pourcentage de comptes utilisateurs activés avec MFA appliquée utilisant les options répertoriées ici** indique le pourcentage de comptes d’utilisateur activés sur votre locataire partenaire pour lesquels MFA est appliquée. Vous pouvez utiliser l’une de ces [options MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) pour vous mettre en conformité. Ces données sont capturées et signalées quotidiennement. Par exemple :

- Contoso est un partenaire CSP avec 110 comptes d’utilisateur dans le locataire, dont 10 sont désactivés. 
- Sur les 100 comptes d’utilisateur restants, 90 ont MFA appliqué en utilisant les [options MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) fournies. Par conséquent, la métrique affiche 90 %. 

### <a name="partner-center-requests-with-mfa"></a>Demandes adressées à l’Espace partenaires avec MFA

Chaque fois que vos employés se connectent à l’Espace partenaires pour travailler ou, par le biais d’API, recevoir ou envoyer des données via l’Espace partenaires, leur statut de sécurité est testé et suivi. Vos applications et les applications de tout fournisseur de panneau de contrôle sont également incluses dans le suivi du statut de sécurité. Ces données sont présentées dans les métriques sous **Pourcentage de demandes adressées à l’Espace partenaires avec MFA** et reflètent les sept derniers jours.

#### <a name="dashboard-mfa-verification"></a>Vérification de MFA dans le tableau de bord

La métrique **Via le portail de l’Espace partenaires** est liée aux activités figurant dans le tableau de bord de l’Espace partenaires. Elle mesure le pourcentage des opérations effectuées par les utilisateurs qui ont effectué la vérification MFA. Par exemple :

- Contoso est un partenaire fournisseur de solutions Cloud employant deux agents d’administration, Jane et John.
- Le premier jour, Jane s’est connectée au tableau de bord de l’Espace partenaires sans vérification MFA et a effectué trois opérations.
- Le deuxième jour, John s’est connecté au tableau de bord de l’Espace partenaires sans vérification MFA et a effectué cinq opérations.
- Le troisième jour, Jane s’est connectée au tableau de bord de l’Espace partenaires avec la vérification MFA et a effectué deux opérations.
- Aucune opération n’a été effectuée par ces agents les quatre jours restants.
- Parmi les dix opérations effectuées dans cette fenêtre de sept jours, deux ont été effectuées par un utilisateur avec la vérification MFA. Par conséquent, la métrique affiche 20 %.

Utilisez le fichier des demandes de portail sans MFA (**Portal requests without MFA**) pour déterminer l’utilisateur qui s’est connecté au tableau de bord de l’Espace partenaires sans avoir recours à la vérification MFA et l’heure de la dernière visite dans la fenêtre de rapports.

#### <a name="appuser-mfa-verification"></a>Vérification de MFA dans Application+Utilisateur

La métrique **Via l’API ou le SDK**  est liée à l’authentification Application+Utilisateur par le biais de demandes d’API de l’Espace partenaires. Elle mesure le pourcentage de demandes d’API effectuées en utilisant un jeton d’accès avec la revendication MFA. Par exemple :

- Fabrikam est un partenaire fournisseur de solutions Cloud et possède une application CSP qui utilise une combinaison de méthodes d’authentification Application+Utilisateur et d’authentification d’application uniquement.
- Le premier jour, cette application a effectué trois demandes d’API qui ont été appuyées par un jeton d’accès obtenu par le biais de la méthode d’authentification Application+Utilisateur sans vérification MFA.
- Le deuxième jour, l’application a effectué cinq demandes d’API, qui ont été appuyées par un jeton d’accès obtenu à l’aide de l’authentification d’application uniquement.
- Le troisième jour, l’application a effectué deux demandes d’API, qui ont été appuyées par un jeton d’accès obtenu par le biais de la méthode d’authentification Application+Utilisateur avec vérification MFA.
- Aucune opération n’a été effectuée par ces agents les quatre jours restants.
- Les cinq demandes d’API du deuxième jour, qui ont été appuyées par un jeton d’accès obtenu par le biais de l’authentification d’application uniquement, sont omises de la métrique, car elle n’utilise pas les informations d’identification de l’utilisateur. Parmi les cinq opérations restantes, deux ont été appuyées par un jeton d’accès obtenu avec la vérification MFA. Par conséquent, la métrique affiche 40 %.

Si vous souhaitez savoir quelles sont les activités Application+utilisateur qui empêchent la métrique d’afficher 100 %, utilisez les fichiers suivants :

- Le fichier de synthèse des demandes d’API (**API requests summary**) pour comprendre l’état d’authentification MFA global par application.
- Le fichier regroupant les demandes d’API (**All API requests**) pour comprendre les détails de chaque demande d’API effectuée par les utilisateurs de votre locataire ; le résultat est limité aux 10 000 demandes les plus récentes pour une meilleure expérience de téléchargement.

## <a name="actions-for-mfa-status-below-100"></a>Actions à effectuer si l’état de MFA est inférieure à 100 %

Certains partenaires qui ont implémenté MFA peuvent constater des métriques inférieures à 100 % dans le rapport. Pour comprendre pourquoi, voici quelques facteurs à prendre en compte.

> [!NOTE]
> Vous devez travailler avec une personne de votre organisation qui maîtrise la gestion des identités et l’implémentation de l’authentification multifacteur pour le locataire de votre partenaire.

### <a name="implemented-mfa-for-your-partner-tenant"></a>MFA implémentée pour votre locataire partenaire

Vous devez implémenter MFA pour votre locataire partenaire afin de vous mettre en conformité. Pour obtenir des détails sur l’implémentation de MFA, consultez [Exigences de sécurité concernant l’utilisation de l’Espace partenaires ou des API de l’Espace partenaires](partner-security-requirements.md).

>[!NOTE]
> Les métriques MFA sont calculées quotidiennement et prennent en compte les opérations effectuées au cours des sept derniers jours. Si vous avez récemment effectué l’implémentation de MFA seulement pour votre locataire partenaire, les métriques peuvent ne pas encore indiquer 100 %.

### <a name="verify-mfa-on-all-user-accounts"></a>Vérifier MFA sur tous les comptes d’utilisateur

Déterminez si votre implémentation de l’authentification multifacteur actuelle couvre tous les comptes d’utilisateur ou seulement certains. Certaines solutions MFA sont basées sur des stratégies et prennent en charge l’exclusion des utilisateurs, tandis que d’autres peuvent vous obliger à activer explicitement MFA pour chaque utilisateur. Vérifiez que vous n’avez exclu aucun utilisateur de votre implémentation MFA actuelle. Tout compte d’utilisateur qui est exclu et qui se connecte à l’Espace partenaires pour effectuer une activité quelconque liée à un fournisseur de solutions Cloud, fournisseur de panneau de contrôle ou conseiller Advisor peut donner lieu à des métriques n’atteignant pas 100 %.

### <a name="review-your-mfa-conditions"></a>Passer en revue les conditions de MFA

Déterminez si votre implémentation actuelle applique uniquement MFA dans des conditions spécifiques. Certaines solutions MFA offrent une flexibilité permettant d’appliquer l’authentification multifacteur uniquement lorsque certaines conditions sont remplies. Par exemple, l’accès de l’utilisateur s’effectue à partir d’un appareil inconnu ou d’un emplacement inconnu. Un utilisateur configuré pour l’authentification multifacteur mais qui n’est pas tenu d’effectuer la vérification MFA lorsqu’il accède à l’Espace partenaires peut donner lieu à des métriques ne correspondant pas à 100 %.

>[!NOTE]
>Pour les partenaires qui ont implémenté l’authentification MFA à l’aide des paramètres de sécurité par défaut d’Azure AD, il est important de noter que, pour les comptes d’utilisateur non-administrateur, l’authentification multifacteur est appliquée en fonction du risque. Les utilisateurs font l’objet d’une authentification MFA uniquement durant les tentatives de connexion à risques (par exemple, l’utilisateur se connecte depuis un autre emplacement). De plus, les utilisateurs ont jusqu’à 14 jours pour s’inscrire auprès de l’authentification MFA. Les utilisateurs qui ne sont pas inscrits auprès de l’authentification MFA ne font pas l’objet d’une vérification MFA durant cette période de 14 jours. Ainsi, les métriques ne sont probablement pas de 100 % pour les partenaires ayant implémenté l’authentification MFA à l’aide des paramètres de sécurité par défaut d’Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Passer en revue les configurations MFA tierces

Si vous utilisez une solution MFA tierce, identifiez la façon dont vous l’intégrez à Azure AD. En général, il existe deux méthodes, la fédération et les contrôles personnalisés :

* **Fédération des identités** - Quand Azure AD reçoit une demande d’authentification, Azure AD redirige l’utilisateur vers le fournisseur d’identité fédérée pour son authentification. Une fois l’authentification réussie, le fournisseur d’identité fédérée redirige l’utilisateur vers Azure AD avec un jeton SAML. Pour qu’Azure AD reconnaisse que l’utilisateur a effectué la vérification MFA lors de son authentification auprès du fournisseur d’identité fédérée, le jeton SAML doit inclure la revendication *authenticationmethodsreferences* (avec la valeur *multipleauthn* ). Vérifiez si le fournisseur d’identité fédérée prend en charge l’émission d’une telle revendication. Si c’est le cas, vérifiez si le fournisseur d’identité fédérée a été configuré pour cela. Si la revendication est manquante, Azure AD (et donc l’Espace partenaires) ne saura pas que l’utilisateur a effectué la vérification MFA et ce défaut de revendication peut donner lieu à une métrique ne correspondant pas à 100 %.

* **Contrôle personnalisé** - Le contrôle personnalisé Azure AD ne peut pas être utilisé pour déterminer si un utilisateur a effectué la vérification MFA via une solution MFA tierce. Par conséquent, tout utilisateur qui a effectué la vérification MFA via un contrôle personnalisé apparaîtra toujours à Azure AD (et, à son tour, à l’Espace partenaires) comme n’ayant pas effectué la vérification MFA. Dans la mesure du possible, il est recommandé d’adopter la fédération des identités par opposition au contrôle personnalisé lors de l’intégration avec Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifier les utilisateurs qui se sont connectés à l’Espace partenaires sans MFA

Il peut s’avérer utile d’identifier les utilisateurs qui se connectent à l’Espace partenaires sans vérification MFA et de les vérifier par rapport à votre implémentation MFA actuelle. Vous pouvez utiliser le [rapport de connexion Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) pour déterminer si un utilisateur a effectué ou non la vérification MFA. Le rapport de connexion Azure AD est disponible uniquement pour les partenaires qui se sont abonnés à Azure AD Premium ou à une référence O365 qui inclut Azure AD Premium (par exemple, EMS).

## <a name="next-steps"></a>Étapes suivantes

- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Exigences de sécurité de l’Espace partenaires](partner-security-requirements.md)
- [Questions fréquentes (FAQ) sur les exigences de sécurité de l’Espace partenaires](partner-security-requirements-faq.md)
