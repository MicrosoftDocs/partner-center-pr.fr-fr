---
title: Préparez-vous à passer du centre d’appartenance au partenaire à l’espace partenaires | Espace partenaires
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Points à prendre en compte avant de déplacer votre activité de PMC vers l’espace partenaires
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8ad7b761c69cfa1f320eb9427806f5b1803e84e6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652190"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Préparez-vous à passer du centre d’appartenance partenaire (PMC) à l’espace partenaires

Nous allons déplacer la gestion des appartenances du Partner Membership Center (PMC) vers l’espace partenaires. il s’agit de la seule destination pour gérer votre relation commerciale avec Microsoft. Nous souhaitons que votre migration vers le centre partenaires soit aussi efficace et facile que possible. Nous avons identifié certains domaines dans lesquels l’espace partenaires diffère du PMC, et nous pensons que vous souhaiterez les comprendre et les préparer avant d’effectuer le déplacement.

## <a name="account-and-identity-setup"></a>Configuration du compte et de l’identité

**Qu’est-ce qu’un compte professionnel Azure Active Directory (Azure AD) ?**

Un compte professionnel Azure est une représentation virtuelle dédiée et isolée de votre entreprise dans le cloud public Azure. Il est créé pour vous lorsque vous vous abonnez à un service de cloud computing Microsoft tel qu’Azure, Microsoft Intune ou Office 365.

Votre compte professionnel héberge vos utilisateurs Azure AD et les informations les concernant (par e-mail, mots de passe, données de profil, autorisations, etc.). Le compte professionnel contient également des groupes, des applications et d’autres informations concernant une société et sa sécurité. Pour plus d’informations, consultez...

Dans l’espace partenaires, vous allez utiliser votre adresse de messagerie professionnelle pour vous connecter à votre compte et non à votre adresse e-mail personnelle.
- Votre compte professionnel : john@contoso.com
- Votre compte personnel : John@outlook.com

Votre adresse de messagerie professionnelle fait partie de votre locataire Azure Active Directory. Pour disposer d’un compte dans l’espace partenaires, vous devez disposer d’un locataire AAD. Pour plus d’informations sur Azure Active Directory, consultez [création de votre répertoire dans Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Lorsque vous accédez au centre des partenaires à partir de PMC, quel compte devez-vous vous connecter à l’espace partenaires avec si vous disposez d’un locataire AAD avec Microsoft (pour Office 365, par exemple) et que vous avez également un locataire pour votre activité CSP ?**

Vous pouvez vous connecter à l’espace partenaires à l’aide du compte CSP ou de votre compte de messagerie de travail MPN. Si vous choisissez de vous connecter à l’aide de votre adresse de messagerie de fournisseur de services de chiffrement, le volet de navigation gauche de votre tableau de bord affiche les informations des programmes MPN et CSP. Si vous vous connectez avec votre adresse de messagerie MPN Azure AD client, vous ne verrez que les informations de votre programme MPN. Les rôles d’utilisateur diffèrent entre MPN et CSP. ainsi, si vous utilisez le même compte pour les entreprises MPN et CSP, veillez à affecter des rôles d’utilisateur en conséquence. Pour plus d’informations sur les rôles d’utilisateur, consultez [affecter des rôles d’utilisateur et des autorisations](permissions-overview.md).

**Si vous ne souhaitez pas utiliser votre client Office 365 Azure AD pour l’espace partenaires, vous pouvez créer un locataire avant d’effectuer la migration à partir de PMC.**

Il peut y avoir de nombreuses raisons pour lesquelles vous ne souhaitez pas utiliser un locataire Azure AD existant pour configurer votre compte espace partenaires. Avant de commencer la migration vers l’espace partenaires, accédez à la [portail Azure](https://ms.portal.azure.com/#home) pour créer un locataire Azure ad. Suivez les instructions de la [création d’un locataire dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Une fois que vous avez créé le nouveau locataire, utilisez ce locataire AAD pour configurer votre compte espace partenaires lorsque vous passez de PMC à l’espace partenaires. Vous devez être administrateur général pour créer le locataire. Utilisez ce nouveau répertoire pour effectuer la migration vers l’espace partenaires.


**Quelle est la différence entre le rôle d’administrateur global AAD et le rôle d’administrateur global PMC MPN ?**

Il s’agit de deux rôles complètement différents avec des autorisations différentes. L’administrateur global de locataire AAD dans l’espace partenaires administre le locataire : ajoute ou supprime des utilisateurs, fournit et gère les mots de passe, les rôles et les autorisations, et a accès à tous les programmes de leur entreprise dans l’espace partenaires. 

Le rôle d’administrateur général MPN dans PMC peut effectuer les opérations suivantes :

- Afficher et modifier toutes les données associées à la société et à tous les emplacements de l’entreprise

-  Ajoutez des administrateurs au niveau global ou local.  En outre, les administrateurs généraux peuvent attribuer à n’importe quel utilisateur à n’importe quel emplacement un accès administrateur général qui leur accorde un accès global, quel que soit l’emplacement auquel ils sont associés.
-  Exécuter toute fonction d’interface utilisateur partenaire, y compris : 

-  Ajouter/supprimer des utilisateurs

 - Affecter/supprimer des rôles 

 - Ajouter/supprimer/mettre à jour des emplacements 

 - Acheter des compétences/cartes 

-  Afficher les avantages

Lorsque l’administrateur général MPN se déplace vers l’espace partenaires, le rôle est appelé administrateur du partenaire MPN qui a des autorisations et des tâches différentes de celles de l’administrateur général de l’espace partenaires. Pour plus d’informations sur les rôles et les autorisations dans l’espace partenaires, consultez [affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md).

**Rôles d’utilisateur, y compris les rôles d’utilisateur invité dans l’espace partenaires**

L’espace partenaires offre différents types de rôles en fonction des types de travail à effectuer. Certains rôles, tels que l’administrateur général, sont des rôles Azure AD. Certains des rôles sont spécifiques aux programmes tels que le programme ou les incentives du fournisseur de services Cloud, et certains rôles sont spécifiques à MPN. Pour savoir ce que sont tous les rôles de l’espace partenaires, consultez [affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md).



**Qu’advient-il des rôles des utilisateurs lorsqu’ils passent de PMC à l’espace partenaires ?**

À l’exception de l’administrateur général MPN ou du contact de programme principal qui effectue la migration, tous les utilisateurs de PMC perdront leurs rôles d’administrateur. La personne qui effectue la migration doit attribuer des rôles dans l’espace partenaires. Les rôles de l’espace partenaires diffèrent de ceux de PMC. Lisez [affecter des rôles et des autorisations d’utilisateurs] (autorisations-overview.md et [passage de PMC à l’espace partenaires](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) pour plus d’informations sur les rôles d’utilisateur dans l’espace partenaires.


**Quelle est la différence entre mon profil d’entreprise et mon profil d’entreprise ?**

Votre profil d’entreprise contient les informations relatives à votre société qui incluent l’adresse, les emplacements, le contact principal, les informations bancaires et fiscales.

Votre profil d’entreprise vous permet de vous présenter à vos clients et constitue une page marketing qui affiche votre logo, les détails de votre entreprise, votre expertise, etc.

**Quelle est la moyenne de la consolidation des comptes pour mon compte ?**

Si vous utilisez le même Azure AD locataire pour migrer plusieurs comptes MPN dans l’espace partenaires, le système reconnaît automatiquement et vous demande de consolider vos comptes. Cela est vrai même si vous avez plusieurs domaines associés au même Azure AD locataire. 

Vous pouvez toujours décider de migrer vers l’espace partenaires à l’aide de locataires AAD distincts, mais notez que cela entraîne une évaluation isolée de vos compétences et des coûts d’achat supplémentaires. 

**Si j’ai plusieurs locataires AAD et un seul compte MPN, est-il possible de les lier dans l’espace partenaires ?**

Oui, dans l’espace partenaires, vous pouvez lier plusieurs locataires Azure AD à un seul compte Center de partenaire.
Pour en savoir plus, cliquez ici. 

**Existe-t-il des restrictions relatives à l’ajout de plusieurs locataires Azure AD à un seul compte de l’espace partenaires ?**

Si le client Azure AD est déjà associé à un compte espace partenaires existant, il ne peut pas être associé à de nouveaux comptes de l’espace partenaires à l’aide de la fonctionnalité d’architecture mutualisée. Une autre façon de penser qu’il s’agit d’un locataire Azure AD ne peut être associé qu’à un seul compte d’espace partenaires, mais un compte espace partenaires peut être associé à plusieurs locataires.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migration de l’appartenance Microsoft Partner Network (MPN) 

**Qui peut effectuer le passage de PMC à l’espace partenaires ?**

L’administrateur général MPN de votre entreprise ou le contact principal du programme (ces deux rôles sont souvent détenus par la même personne) peuvent initier et effectuer le déplacement.

**La personne qui termine la migration deviendra-t-elle le contact principal dans le profil juridique de l’entreprise dans l’espace partenaires ?**

Toutefois, ce n’est pas nécessairement le contact principal qui doit être une personne disposant de l’autorisation de signature des accords.

**Microsoft peut-il migrer mon abonnement MPN pour moi ?**

Non. Microsoft ne peut pas vous aider à déplacer votre compte d’appartenance vers l’espace partenaires. Vous devrez déplacer votre compte en vous connectant à PMC avec votre compte professionnel (informations d’identification de connexion) pour commencer le processus de migration. Une fois que vous avez terminé les étapes pour déplacer votre compte, vous pouvez commencer à gérer votre appartenance et affecter des rôles d’utilisateur et des autorisations à votre équipe afin qu’ils puissent accéder aux avantages et aider à gérer l’appartenance. Microsoft migrera automatiquement les compétences, les avantages, les informations d’emplacement, les informations bancaires/fiscales en cours pour les incentives et les associations MCP, y compris l’accès à l’Université partenaire.

Microsoft migrera automatiquement les compétences, les avantages, les informations d’emplacement, les informations bancaires/fiscales en cours pour les incentives et les associations MCP, y compris l’accès à l’Université partenaire.

**Quelles sont les modifications apportées à la stratégie de renouvellement ?**

 Dans l’espace partenaires, la fenêtre de renouvellement est comprise entre votre date anniversaire et les 30 jours suivants.

**Nos compétences restent-elles inchangées après le passage à l’espace partenaires ?**

Oui, compentencies ne sera pas affecté par le déplacement vers l’espace partenaires. Si vous remarquez des différences, contactez le [support technique](https://partner.microsoft.com/support).


 **Mes avantages (y compris les avantages Cloud, le support technique, les avantages logiciels, Visual Studio) évoluent après le déplacement ?**

 Vos avantages éligibles ne seront pas modifiés. Si vous remarquez des différences, contactez le [support technique](https://partner.microsoft.com/support).

 **Nos comptes Microsoft avec les avantages de Visual Studio sont-ils honorés ?**


 Oui. Les avantages Visual Studio alloués aux comptes MSA vont être honorés et conservés. Ils sont également conservés après l’opération de renouvellement dans l’Espace partenaires. Toutefois, si vous supprimez une allocation de MSA une fois migrée dans l’espace partenaires, elle ne peut pas être rajoutée dans l’espace partenaires.

Dans l’Espace partenaires, un partenaire peut ajouter des comptes professionnels et des comptes d’utilisateur invité représentant des comptes MSA du locataire où le partenaire est l’administrateur MPN sur le locataire Azure AD. Si le partenaire est administrateur général de plusieurs locataires Azure AD, et si tous ces locataires sont associés au même compte de l’Espace partenaires, le partenaire est autorisé à ajouter des utilisateurs à l’ensemble des locataires dans le cadre des allocations d’avantages Visual Studio et des allocations basées sur l’utilisation d’Azure.

Bien que l’administrateur MPN ou l’administrateur général puisse affecter des abonnements basés sur l’utilisation de Visual Studio aux utilisateurs invités, ces derniers ne peuvent pas se connecter à l’Espace partenaires à l’aide de leur compte MSA. Toutefois, les utilisateurs invités peuvent se connecter à Azure et à Visual Studio pour valider et utiliser les avantages qui leur ont été affectés.


 **Comment gérer nos associations MCP et notre accès à l’Université des partenaires ?**

 Aucune modification n’a été apportée aux associations MCP qui se déplacent de PMC. Toutefois, les nouveaux nouveaux employés après avoir été déplacés vers l’espace partenaires devront être associés dans l’espace partenaires. Toutes les autorisations de votre Université partenaire pour les utilisateurs existants seront conservées, mais tous les nouveaux employés devront accéder au [Centre de formation](https://partner.microsoft.com/training) pour obtenir des informations sur l’accès à l’Université partenaire.

 **Comment faire afficher les informations du MCP une fois que je passe à l’espace partenaires ?**

Dans le tableau de bord, sélectionnez **compétences** dans le panneau de navigation de gauche. À partir de la page **compétences** , vous pouvez télécharger le rapport compétences. Le rapport compétences répertorie les utilisateurs qui ont acquis des compétences en rapport avec les compétences et les programmes de l’espace partenaires. Si vos utilisateurs ont acquis des compétences, mais que ces compétences ne sont pas pertinentes pour les compétences que vous travaillez, elles ne sont pas répertoriées dans le rapport.


 **Les références client sont-elles utilisées dans l’espace partenaires ?**

 Non, vous n’avez pas besoin de références client pour répondre aux exigences de compétence dans l’espace partenaires.

 **Les associations d’enregistrements seront-elles déplacées vers l’espace partenaires ?**

 Oui, aucune modification n’est apportée au partenaire d’enregistrement. En savoir plus sur [la liaison de votre ID de partenaire à vos clients](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Y a-t-il un impact sur les incentives en raison de la migration vers l’espace partenaires ?**

Non, il n’y a aucun impact sur les incentives si vous avez déplacé votre compte sans consolider les emplacements. Si votre entreprise possède plusieurs comptes dans PMC et que, lorsque vous passez à l’espace partenaires, vous décidez de consolider un compte global, il n’y aura aucune perte aux incentives, mais il peut y avoir un retard dans le paiement de l’incentive. Si vous ne déplacez pas tous les comptes PMC qui ont été impliqués dans des programmes d’incentives, vous pouvez cesser d’accumuler des incentives liés à ces comptes.


**Quels sont les rôles d’utilisateur d’incentives dans l’espace partenaires ?** 

Les rôles d’incentives de l’espace partenaires sont basés sur l’emplacement et incluent un utilisateur administrateur et incentives incitants. Pour plus d’informations sur ce que ces rôles peuvent faire, consultez [affecter des rôles et des autorisations aux utilisateurs](permissions-overview.md).

**Les utilisateurs peuvent-ils être affectés au niveau global et au niveau de l’emplacement ?**

 Oui. Vous pouvez affecter un administrateur d’incentives à l’administrateur des Incentives pour tous les emplacements, ou chaque emplacement peut avoir son propre administrateur d’incentives.

 **Les incentives peuvent-ils être payés au niveau global ou de l’emplacement ?**

 Les incentives sont payés uniquement au niveau de l’emplacement.

**En ce qui concerne les références, combien de profils d’entreprise pouvez-vous créer ?**

Votre entreprise peut créer autant de profils d’entreprise que nécessaire pour représenter pleinement les intérêts de votre entreprise. Dans chaque profil d’entreprise, vous pouvez répertorier jusqu’à cinq emplacements, un emplacement par pays. Chacun des profils d’entreprise peut recevoir des références pour chacun de ses emplacements.

**Comment les références seront-elles affectées, quelles modifications puis-je attendre ? Par exemple, si j’ai une société internationale sur un marché et des lieux sur d’autres marchés, comment les références seront-elles affectées ?**

Les références sont attribuées en fonction des paramètres de recherche définis par le client. Ainsi, que vous ayez un ou plusieurs emplacements, si les clients spécifient un emplacement souhaité et que vous avez une entreprise qui répond aux autres paramètres, la référence est alors ajoutée à cet emplacement.








