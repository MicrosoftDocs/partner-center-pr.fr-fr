---
title: Départ du Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consultez les informations utiles et les questions fréquentes avant de transférer votre activité de Partner Membership Center vers l’Espace partenaires.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 08b1b547fc6f494dfdb1199824221aecad9120bc
ms.sourcegitcommit: c71df4cc61dfd0d6ef4a93f9c92fb822201c7773
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2020
ms.locfileid: "87433887"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Préparer votre transfert du Partner Membership Center (PMC) vers l’Espace partenaires

**Rôles appropriés**
- Administrateur général
- Administrateur des utilisateurs
- Agent commercial
- Agent d’administration

Nous transférons actuellement la gestion des appartenances du Partner Membership Center (PMC) vers l’Espace partenaires (la seule destination pour gérer votre relation commerciale avec Microsoft). Nous souhaitons que votre transfert dans l’Espace partenaires soit aussi simple et efficace que possible. Sachant que l’Espace partenaires présente quelques différences par rapport à PMC, nous avons jugé utile de vous les présenter de façon à vous préparer au mieux avant le transfert.

## <a name="account-and-identity-setup"></a>Configuration d’un compte et d’une identité

**Qu’est-ce qu’un compte professionnel Azure Active Directory (Azure AD) ?**

Un compte professionnel Azure est une représentation virtuelle dédiée et isolée de votre entreprise dans le cloud public Azure. Il est créé pour vous quand vous vous abonnez à un service cloud Microsoft comme Azure, Microsoft Intune ou Office 365.

Votre compte professionnel héberge vos utilisateurs Azure AD et les informations les concernant : adresses e-mail, mots de passe, données de profil, autorisations, etc. Le compte professionnel contient aussi des groupes, des applications et toutes les informations relatives à une entreprise et à sa sécurité. 

Votre adresse e-mail professionnelle fait partie intégrante de votre locataire Azure Active Directory. Pour avoir un compte dans l’Espace partenaires, vous devez disposer d’un locataire AAD. Pour plus d’informations sur Azure Active Directory, consultez [Créer votre annuaire dans Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

Dans l’Espace partenaires, vous vous connecterez à l’aide de votre adresse e-mail professionnelle et non de votre adresse personnelle.
- Votre compte professionnel : john@contoso.com
- Votre compte personnel : John@outlook.com

**Avec quel compte devez-vous vous connecter à l’Espace partenaires si vous disposez d’un locataire AAD auprès de Microsoft (pour Office 365 par exemple), mais que vous possédez aussi un locataire pour votre activité de fournisseur de solutions Cloud ?**

Vous pouvez vous connecter à l’Espace partenaires soit avec le compte CSP soit avec votre compte de messagerie professionnel MPN. Si vous choisissez de vous connecter à l’aide de votre adresse e-mail professionnelle CSP, le volet de navigation gauche de votre tableau de bord affiche les informations des programmes MPN et CSP. Si vous vous connectez avec l’adresse e-mail professionnelle de votre locataire MPN Azure AD, vous ne verrez que les informations du programme MPN. 

**Si vous ne souhaitez pas utiliser votre client Office 365 Azure AD pour l’Espace partenaires, vous pouvez créer un nouveau locataire avant de migrer à partir de PMC.**

Vous pouvez avoir de nombreuses raisons de ne pas vouloir utiliser un locataire Azure AD existant pour configurer votre compte Espace partenaires. Avant de débuter votre migration vers l’Espace partenaires, accédez au [portail Azure](https://ms.portal.azure.com/#home) pour créer un locataire Azure AD. Suivez les recommandations livrées dans [Créer un locataire dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Utilisez le nouveau locataire AAD pour configurer votre compte Espace partenaires. Vous devez être administrateur général pour créer le locataire. 


**Rôles d’utilisateurs incluant les rôles d’utilisateurs invités dans l’Espace partenaires**

L’Espace partenaires comporte différents types de rôles qui varient en fonction du type de travail à effectuer. Certains rôles, comme celui d’administrateur général, sont des rôles Azure AD. Il existe d’autres qui sont propres aux programmes, par exemple les programmes Fournisseur de services cloud (CSP) et Incentives, et d’autres qui sont propres à MPN. Pour connaître les différents rôles de l’Espace partenaires, consultez [Affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md).

**Que deviennent les rôles d’utilisateurs lors du transfert de PMC vers l’Espace partenaires ?**

À l’exception de l’administrateur général MPN ou du contact principal du programme qui se charge de la migration, tous les utilisateurs de PMC perdent leur rôle d’administrateur. La personne qui effectue la migration doit attribuer des rôles dans l’Espace partenaires. Les rôles de l’Espace partenaires sont différents de ceux de PMC. Pour plus d’informations sur les rôles d’utilisateurs dans l’Espace partenaires, consultez [Affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md et [Passage de PMC à l’Espace partenaires](move-pmc-pc-map.md#user-roles).


**Quelle est la différence entre le profil de la société et le profil commercial ?**

Le profil de la société présente les informations sur la société, notamment son adresse, ses sites, son contact principal et les détails sur sa banque et les taxes.

Le profil commercial est la façon dont vous vous présentez aux clients ainsi qu’une page marketing qui affiche votre logo, les détails de votre objectif commercial, votre savoir-faire, etc.

**Que signifie la consolidation de comptes pour votre compte ?**

Si vous utilisez le même locataire Azure AD pour migrer plusieurs comptes MPN dans l’Espace partenaires, le système le détecte automatiquement et vous demande de consolider vos comptes. Cela est vrai même si plusieurs domaines sont associés au même locataire Azure AD. 

Vous pouvez toujours décider de migrer vers l’Espace partenaires en utilisant des locataires AAD distincts, mais vos compétences sont alors évaluées de manière isolée et les coûts d’achat sont supérieurs. Pour plus d’informations sur la consolidation des comptes, consultez [Consolider vos comptes d’entreprise](consolidate-accounts.md)

**Si j’ai plusieurs locataires AAD et un seul compte MPN, est-il possible de les lier dans l’Espace partenaires ?**

Oui, dans l’Espace partenaires, vous pouvez lier plusieurs locataires Azure AD pour en faire un seul et unique compte Espace partenaires.
Pour plus d’informations sur la consolidation des comptes, consultez [Consolider vos comptes d’entreprise](consolidate-accounts.md)

**L’ajout de plusieurs locataires Azure AD à un même compte Espace partenaires est-il soumis à des restrictions ?**

Si le locataire Azure AD est déjà associé à un compte Espace partenaires existant, il ne peut pas être associé à un nouveau compte Espace partenaires à l’aide de la fonctionnalité de multilocation. Autrement dit, un locataire Azure AD ne peut être associé qu’à un seul compte Espace partenaires, mais un compte Espace partenaires peut avoir plusieurs locataires associés.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migration des adhésions à Microsoft Partner Network (MPN) 

**Qui peut effectuer le transfert de PMC vers l’Espace partenaires ?**

L’administrateur général MPN ou le contact principal du programme (ces deux rôles sont souvent détenus par la même personne) de votre entreprise sont les seuls à pouvoir initier et effectuer le transfert.

**La personne qui effectue la migration devient-elle le contact principal dans le profil juridique de l’entreprise dans l’Espace partenaires ?**

Pas nécessairement, mais le contact principal doit être une personne autorisée à signer les contrats.

**Microsoft peut-il migrer mon adhésion à MPN à ma place ?**

Non. Microsoft ne peut pas vous aider à transférer votre compte d’adhésion vers l’Espace partenaires. Vous devez transférer votre compte en vous connectant à PMC avec votre compte professionnel (informations de connexion) pour lancer le processus de migration. Après avoir effectué les étapes de transfert de votre compte, vous pouvez commencer à gérer votre adhésion et attribuer des rôles et des autorisations aux utilisateurs de votre équipe pour leur permettre d’accéder aux avantages et de gérer l’adhésion. 

Microsoft migre automatiquement les informations actives sur les compétences, les avantages, les sites, la banque/taxes pour les incentives ainsi que les associations MCP, y compris l’accès à Partner University.

**En quoi la stratégie de renouvellement change-t-elle ?**

 Dans l’Espace partenaires, la fenêtre de renouvellement se situe entre la date d’anniversaire et les 30 jours suivants.

**Les compétences sont-elles inchangées après un transfert vers l’Espace partenaires ?**

Oui, les compétences ne sont pas affectées par le transfert vers l’Espace partenaires. Si vous notez des différences, contactez le [Support](https://partner.microsoft.com/support).


 **Est-ce que les avantages (avantages cloud, support technique, avantages logiciels, Visual Studio, etc.) changent après le transfert ?**

 Les avantages auxquels vous aviez droit ne changent pas. Si vous notez des différences, contactez le [Support](https://partner.microsoft.com/support).

 **Les avantages Visual Studio alloués aux comptes Microsoft seront-ils honorés ?**


 Oui. Les avantages Visual Studio alloués aux comptes MSA vont être honorés et conservés. Ils sont également conservés après l’opération de renouvellement dans l’Espace partenaires. Cependant, si vous supprimez une allocation de compte MSA une fois la migration effectuée dans l’Espace partenaires, vous ne pourrez plus la réintégrer dans l’Espace partenaires.

Dans l’Espace partenaires, un partenaire peut ajouter des comptes professionnels et des comptes d’utilisateurs invités représentant des comptes MSA du locataire où le partenaire est l’administrateur MPN sur le locataire Azure AD. Si le partenaire est administrateur général de plusieurs locataires Azure AD, et si tous ces locataires sont associés au même compte de l’Espace partenaires, le partenaire est autorisé à ajouter des utilisateurs à l’ensemble des locataires dans le cadre des allocations d’avantages Visual Studio et des allocations basées sur l’utilisation d’Azure.

Bien que l’administrateur MPN ou l’administrateur général puisse affecter des abonnements basés sur l’utilisation de Visual Studio aux utilisateurs invités, ces derniers ne peuvent pas se connecter à l’Espace partenaires à l’aide de leur compte MSA. Toutefois, les utilisateurs invités peuvent se connecter à Azure et à Visual Studio pour valider et utiliser les avantages qui leur ont été affectés.

 **Comment gérer les associations MCP et l’accès Partner University ?**

 Les associations MCP qui sont transférées à partir de PMC ne subissent aucun changement. Cependant, les nouveaux employés ajoutés après le transfert dans l’Espace partenaires doivent être associés dans ce dernier. Si toutes les autorisations Partner University de vos utilisateurs existants sont conservées, les nouveaux employés doivent se rendre dans [le centre de formation](https://partner.microsoft.com/training) pour savoir comment obtenir un accès à Partner University.

 **Comment faire pour consulter les informations de MCP une fois le transfert dans l’Espace partenaires effectué ?**

Sélectionnez **Compétences** dans le volet de navigation gauche du tableau de bord. Dans la page **Compétences**, vous pouvez télécharger le rapport sur les qualifications. Ce rapport dresse la liste de vos utilisateurs qui ont acquis des qualifications en rapport avec les compétences de l’Espace partenaires. Si vos utilisateurs ont acquis des qualifications qui n’ont aucun rapport avec les compétences visées, ils ne sont pas listés dans le rapport.


 **Les références client sont-elles utilisées dans l’Espace partenaires ?**

 Non, vous n’avez pas besoin de références client pour satisfaire les exigences de compétences dans l’Espace partenaires.

 **Les associations Partenaire de référence sont-elles transférées dans l’Espace partenaires ?**

 Oui, rien ne change pour le Partenaire de référence. Découvrez plus en détail comment [lier votre ID partenaire à vos clients](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Le transfert dans l’Espace partenaires a-t-il un impact sur les incentives ?**

Non, si vous avez transféré votre compte sans regrouper les sites, il n’y a aucun impact sur les incentives. Si votre entreprise possède plusieurs comptes dans PMC et que vous décidez de les consolider dans un même compte global pendant la transfert dans l’Espace partenaires, aucun incentive n’est perdu, mais le versement des revenus liés aux incentives risque d’être retardé. 

Si vous ne transférez pas tous vos comptes PMC qui ont été impliqués dans les programmes d’incentives, il se peut que vous cessiez de gagner les incentives liés à ces comptes.


**Quels sont les rôles Incentive dans l’Espace partenaires ?** 

Les rôles Incentive dans l’Espace partenaires sont basés sur le site et incluent l’administrateur d’incentives et l’utilisateur d’incentives. Pour plus d’informations sur ces rôles, consultez [Affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md).

**Les administrateurs d’incentives peuvent-ils être affectés au niveau global et au niveau du site ?**

 Oui. Vous pouvez attribuer à un administrateur d’incentives le rôle d’administrateur d’incentives pour l’ensemble des sites ou pour chaque site qui a son propre administrateur d’incentives.

 **Les incentives peuvent-ils être payés au niveau global ou au niveau du site ?**

 Les incentives sont payés uniquement au niveau du site.

**Dans le cas des références, combien de profils commerciaux est-il possible de créer ?**

Votre entreprise peut créer autant de profils commerciaux dont elle a besoin pour représenter tous ses intérêts. Dans chaque profil professionnel, vous pouvez lister jusqu’à cinq sites, un par pays. Chaque profil commercial peut recevoir des références pour chacun de ses sites.

**Comment les références seront-elles affectées et à quels changements s’attendre ? Par exemple, dans le cas d’une entreprise mondiale présente sur un marché et disposant de sites sur d’autres marchés, comment les références seront-elles affectées ?**

Les références sont affectées en fonction des paramètres de recherche définis par le client. Quel que soit le nombre de sites que vous avez (un ou une multitude), si les clients indiquent préférer un site et que vous avez une activité qui répond aux autres paramètres, la référence est affectée à ce site.

**Je migre vers l’Espace partenaires depuis la Russie. Je reçois un message d’erreur relatif à Web Direct. Comment faire poursuivre la migration ?**

Si vous recevez un message d’erreur parce que vous participez au programme Web direct, vous devez effectuer les opérations suivantes :

1. Connectez-vous à portal.Azure.com et créez un locataire Azure AD. Pour plus d’informations, consultez [Créer un locataire Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-access-create-new-tenant).
1. Une fois que vous avez créé le locataire Azure AD, utilisez-le pour migrer du Partner Membership Center vers l’Espace partenaires ou pour vous inscrire en tant que nouveau membre dans l’Espace partenaires.






