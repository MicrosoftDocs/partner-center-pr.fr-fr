---
title: Exigences de sécurité du partenaire | Espace partenaires
ms.topic: article
ms.date: 10/11/2019
description: Découvrez les exigences de sécurité pour les conseillers et les partenaires participant au programme Fournisseur de solutions Microsoft Cloud.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, fournisseur de solutions Cloud, programme Fournisseur de solutions Cloud, CSP, fournisseur de panneau de contrôle, CPV, authentification multifacteur, MFA, modèle d’application sécurisé, sécurité
ms.localizationpriority: high
ms.openlocfilehash: 4c7f4e61cc249fb51f58e4a94892a2d937cae4e1
ms.sourcegitcommit: 1fe366f787d97c96510cfd409304e7d48af7c286
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/30/2019
ms.locfileid: "73141979"
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

## <a name="overview"></a>Vue d’ensemble

Depuis le 1er août 2019, tous les partenaires doivent mettre en œuvre l’authentification multifacteur pour tous les comptes d’utilisateur dans leur locataire partenaire. Les conditions associées aux exigences de sécurité du partenaire ont été ajoutées au [guide du programme Fournisseur de solutions Cloud](https://go.microsoft.com/fwlink/p/?LinkId=617100). En ce qui concerne les conseillers, les mêmes exigences contractuelles sont en place.

> [!NOTE]
> Nous recommandons fortement que tous les partenaires qui effectuent des transactions via un cloud souverain (21Vianet, US Government et Germany) agissent et adoptent immédiatement ces exigences de sécurité. Toutefois, ces partenaires ne sont pas tenus de satisfaire aux exigences de sécurité à compter du 1er août 2019. Microsoft fournira des informations supplémentaires sur la mise en œuvre de ces exigences de sécurité pour les clouds souverains à l’avenir.

Les partenaires qui n’implémentent pas les exigences de sécurité obligatoires ne seront pas en mesure d’effectuer des transactions dans le cadre du programme Fournisseur de solutions Cloud ou de gérer les locataires clients en tirant parti des droits d’administrateur délégué, une fois ces exigences appliquées.

## <a name="actions-that-you-need-to-take"></a>Actions que vous devez effectuer

Pour vous conformer aux exigences de sécurité des partenaires, vous devez appliquer l’authentification multifacteur pour chaque compte d’utilisateur de votre locataire partenaire. Pour cela, vous pouvez procéder de l’une des façons suivantes :

- Implémenter la fonctionnalité des stratégies de protection de base de référence [Exiger l’authentification multifacteur pour les administrateurs](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) et [Protection de l’utilisateur final](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) d’Azure Active Directory sans coût supplémentaire
- Acheter Azure Active Directory Premium pour chaque compte d’utilisateur. Pour plus d’informations, consultez [Planification d’un déploiement Azure Multi-Factor Authentication basé sur le cloud](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).
- Utiliser une solution de tiers pour appliquer l’authentification multifacteur pour chaque compte d’utilisateur de votre locataire partenaire. Pour plus d’informations, consultez [Mode d’application des exigences de sécurité](#how-the-requirements-will-be-enforced) afin de garantir que la solution fournira les informations attendues.

### <a name="consideration"></a>Facteur

Comme ces exigences s’appliquent à tous les comptes d’utilisateur de votre locataire partenaire, plusieurs éléments doivent être pris en compte pour garantir un déploiement sans problèmes. Ces considérations incluent l’identification des comptes d’utilisateur dans Azure Active Directory qui ne peuvent pas effectuer l’authentification multifacteur, et l’identification des applications et des appareils utilisés par votre organisation qui ne prennent pas en charge l’authentification moderne.

Avant d’effectuer une action, il est recommandé d’identifier les éléments suivants :

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Avez-vous une application ou un appareil qui ne prend pas en charge l’utilisation de l’authentification moderne ?

Quand vous appliquez l’authentification multifacteur héritée, les protocoles comme IMAP, POP3 et SMTP sont bloqués, car ils ne prennent pas en charge l’authentification multifacteur. Pour passer outre cette limitation, vous pouvez utiliser une fonctionnalité appelée [Mots de passe d’application](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) pour vous assurer que l’application ou l’appareil peut toujours s’authentifier. Vous devez consulter les considérations relatives à l’utilisation des mots de passe d’application documentées [ici](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) pour déterminer si vous pouvez utiliser ces derniers dans votre environnement.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Avez-vous des utilisateurs qui recourent à Office 365 dans le cadre de licences associées à votre locataire partenaire ?

Avant d’implémenter une solution, il est recommandé de déterminer la version de Microsoft Office qui est utilisée par les utilisateurs de votre locataire partenaire. Consultez [Planifier l’authentification multifacteur pour les déploiements d’Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) avant d’entreprendre une action. Il y a un risque que vos utilisateurs rencontrent des problèmes de connectivité avec des applications comme Outlook. Avant d’appliquer l’authentification multifacteur, il est important de vérifier qu’Outlook 2013 SP1 ou ultérieur est utilisé et que l’authentification moderne est activée pour votre organisation. Pour plus d’informations, consultez [Activer l’authentification moderne dans Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Pour activer l’authentification moderne pour tous les appareils exécutant Windows et sur lesquels Microsoft Office 2013 est installé, vous devez créer deux clés de registre. Consultez [Activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Existe-t-il une stratégie qui empêche les utilisateurs de recourir à leurs appareils mobiles quand ils travaillent ?

Il est important d’identifier toute stratégie d’entreprise qui empêche les employés d’utiliser des appareils mobiles quand ils travaillent, car elle influe sur la solution d’authentification multifacteur que vous implémentez. Il existe des solutions, comme celles fournies via l’implémentation des [stratégies de protection de base de référence](/azure/active-directory/conditional-access/concept-baseline-protection), qui autorisent seulement l’utilisation d’une application d’authentification pour la vérification. Si votre organisation a une stratégie qui empêche l’utilisation d’appareils mobiles, vous devez envisager l’une des options suivantes :

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

Pour mieux comprendre ce qui ou qui fait l’objet d’une authentification sans demande d’authentification multifacteur, il est recommandé de passer en revue l’activité de connexion. Avec Azure Active Directory Premium, vous pouvez tirer parti du rapport de connexions. Pour plus d’informations, consultez les [rapports d’activité de connexion dans le portail Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins). Si vous n’avez pas Azure Active Directory Premium ou si vous recherchez un moyen de l’obtenir via PowerShell, vous devrez tirer parti de l’applet de commande [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) à partir du module [PowerShell de l’Espace partenaires](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Comment les spécifications seront appliquées

Les exigences de sécurité des partenaires seront appliquées par Azure Active Directory et ensuite par l’Espace partenaires, en vérifiant la présence de la revendication MFA pour déterminer si la vérification de l’authentification multifacteur a eu lieu. Si vous utilisez Azure Multi-Factor Authentication ou les stratégies de protection de base de référence, aucune action supplémentaire n’est nécessaire.

Lors de l’utilisation d’une solution d’authentification multifacteur de tiers, il est possible que la revendication MFA ne soit pas émise. Si cette revendication est manquante, Azure Active Directory ne sera pas en mesure de déterminer si la demande d’authentification a imposé l’authentification multifacteur. Pour plus d’informations sur la façon de vérifier si votre solution émet la revendication attendue, consultez [Test des exigences de sécurité du partenaire](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements).

> [!IMPORTANT]
> Si votre solution de tiers n’émet pas la revendication attendue, vous devez collaborer avec le fournisseur qui a développé la solution pour déterminer les actions à entreprendre.

## <a name="resources-and-support"></a>Ressources et support

Voici des ressources qui vous permettent de trouver du support et des exemples de code :

- [Communauté du groupe d’aide sur la sécurité de l’Espace partenaires](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : cette communauté en ligne vous permet de découvrir les événements à venir et de poser des questions.
- [Exemples .NET pour l’Espace partenaires](https://github.com/microsoft/partner-center-dotnet-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de .NET, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Exemples Java pour l’Espace partenaires](https://github.com/microsoft/partner-center-java-samples) : ce dépôt GitHub contient des exemples, développés à l’aide de Java, qui illustrent la façon dont vous pouvez implémenter le framework Modèle d’application sécurisé.
- [Module PowerShell pour l’Espace partenaires - Authentification multifacteur](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) : cet article fournit des détails sur la façon d’implémenter le framework Modèle d’application sécurisé avec PowerShell.
