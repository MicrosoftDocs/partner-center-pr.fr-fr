---
title: Préparer votre déplacement à partir de l’appartenance de partenaires pour les partenaires | Partenaires
ms.topic: article
ms.date: 06/13/2019
description: Éléments à considérer avant de passer votre entreprise de PMC pour partenaires
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0f1df50c5fa94707ac733a91b0d981b6821de8c0
ms.sourcegitcommit: 7b3847a788365a05628a4cf2938dfd61782d6e4e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/29/2019
ms.locfileid: "67468027"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Préparer votre déplacement à partir de partenaire Membership Center (PMC) pour les partenaires

Nous déplaçons gestion des appartenances à partir de partenaire Membership Center (PMC) vers l’espace partenaires – la destination unique pour gérer votre relation commerciale avec Microsoft. Nous voulons votre passage au centre de partenaires pour être aussi efficace et facile que possible. Nous avons identifié certains domaines où PMC diffère de l’espace partenaires, et nous pensons que vous souhaitez comprendre et à préparer avant du déplacer.

## <a name="account-and-identity-setup"></a>Programme d’installation de compte et d’identité

**Qu’est un compte de travail Azure Active Directory (Azure AD) ?**

Un compte professionnel Azure est une représentation virtuelle dédiée et isolée de votre entreprise dans le cloud public Azure. Il est créé pour vous lorsque vous vous abonnez à un service de cloud computing Microsoft tel qu’Azure, Microsoft Intune ou Office 365.

Votre compte professionnel héberge vos utilisateurs Azure AD et les informations les concernant - leur e-mail les mots de passe, les données de profil, autorisations et ainsi de suite. Le compte de travail contient également des groupes, applications et autres informations se rapportant à une société et sa sécurité. Pour plus d’informations, consultez...

Dans l’espace partenaires, vous allez utiliser votre adresse de messagerie professionnelle pour se connecter à votre compte pas votre adresse e-mail personnelle.
- Votre compte professionnel : john@contoso.com
- Votre compte personnel : John@outlook.com

Votre adresse de messagerie professionnelle fait partie de votre client Azure active directory. Pour qu’un compte Centre de partenaires, vous devez disposer d’un locataire AAD. Pour plus d’informations sur Azure Active Directory, consultez [créer votre annuaire dans Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Lorsque vous déplacer vers partenaires de PMC, quel compte vous devez vous être connecté au Partner Center avec if ont un locataire AAD avec Microsoft (pour Office 365 par exemple) et que vous avez également un locataire pour votre entreprise CSP ?**

Vous pouvez accéder à des partenaires avec le compte CSP ou votre compte de messagerie professionnel MPN. Si vous choisissez de vous connecter à l’aide de votre adresse de messagerie professionnelle CSP, le volet de navigation gauche sur votre tableau de bord affiche les informations de programme MPN et CSP. Si vous vous connectez avec votre adresse de messagerie professionnelle de locataire MPN Azure AD, vous verrez uniquement vos informations de programme MPN. Rôles d’utilisateur diffèrent entre MPN et CSP si vous utilisez le même compte pour les entreprises MPN et CSP, veillez à affecter des rôles d’utilisateur en conséquence. Pour plus d’informations sur les rôles d’utilisateur, consultez [attribuer des rôles d’utilisateur et autorisations](permissions-overview.md).

**Quelle est la différence entre le rôle d’administrateur général AAD et le rôle d’administrateur général PMC MPN ?**

Il s’agit de deux rôles complètement différentes avec des autorisations différentes. L’administrateur général du locataire AAD dans partenaires administre le locataire : ajoute ou supprime les utilisateurs, fournit et gère les mots de passe, les rôles et les autorisations et a accès aux programmes de tous les leur société de partenaires. 

Le rôle d’administrateur général de MPN dans PMC pourrait les opérations suivantes :

- Afficher et modifier toutes les données associées à l’entreprise et tous les emplacements de la société

-  Ajouter des administrateurs au niveau global ou local.  En outre, les administrateurs généraux peuvent affecter toute personne à n’importe quel emplacement les accès administrateur Global qui leur accorde l’accès global, quel que soit l’endroit où ils sont associés.
-  Effectuer un partenaire quelconque accessible sur la fonction de l’interface utilisateur, y compris : 

-  Ajouter/supprimer des utilisateurs

 - Attribuer/supprimer des rôles 

 - Emplacements d’Ajout/Suppression/mise à jour 

 - Achat compétence/mappages 

-  Afficher les avantages

Lorsque l’administrateur général MPN se déplace au centre de partenaires le rôle est appelé Administrateur partenaire MPN possède des autorisations différentes et des tâches que l’administrateur général de partenaires. Pour plus d’informations sur les rôles et autorisations dans l’espace partenaires, consultez [attribuer des rôles d’utilisateurs et les autorisations](permissions-overview.md)

**Rôles d’utilisateur, y compris les rôles d’utilisateur invité dans l’espace partenaires**

Partenaires a différents types de rôles en fonction des types de travail à effectuer. Il existe des rôles, tels qu’Administrateur général qui sont des rôles Azure AD. Certains des rôles sont spécifiques à des programmes tels que le programme de fournisseur de services Cloud ou les primes, et il existe des rôles qui sont spécifiques à MPN. Pour découvrir tous les rôles de partenaires, lire [attribuer des rôles d’utilisateurs et les autorisations](permissions-overview.md).



**Que se passe-t-il pour les rôles de mes utilisateurs lorsqu’ils passent de PMC pour partenaires ?**

À l’exception de l’administrateur général de MPN ou un contact de programme principal qui effectue la migration, tous les utilisateurs dans PMC perdrez leurs rôles d’administrateur. La personne qui termine la migration devez attribuer des rôles dans l’espace partenaires. Les rôles de partenaires diffèrent de ceux dans PMC. Lecture [attribuer des rôles d’utilisateurs et les autorisations](permissions-overview) et [déplacement PMC vers partenaires](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) pour plusieurs rôles d’utilisateur sur Centre partenaires.


**Quelle est la différence entre mon profil d’entreprise et mon profil d’entreprise ?**

Profil de votre société est les informations sur votre entreprise qui inclut l’adresse, emplacements, contact principal, les informations fiscales et bancaires.

Votre profil d’entreprise est la façon dont vous vous présentez aux clients et est une page marketing qui affiche votre logo, plus d’informations sur le focus de votre entreprise, de votre expertise, etc.

**Ce qui ne tient compte moyenne de consolidation pour mon compte ?**

Si vous utilisez le même locataire Azure AD pour migrer plusieurs comptes MPN au Partner Center, le système sera automatiquement qui reconnaît et vous demander de consolider vos comptes. Cela est vrai même si vous avez plusieurs domaines associés au même locataire Azure AD. 

Vous pouvez toujours décider de migrer vers les partenaires à l’aide de locataires AAD séparés, mais Veuillez noter que cette évaluation isolée de vos compétences et supplémentaire entraîne des coûts d’achat. 

**Si j’ai plusieurs locataires AAD et un seul compte MPN, est-il possible de les lier dans partenaires ?**

Oui, dans l’espace partenaires, vous pouvez lier plusieurs locataires Azure AD à un seul compte espace partenaires.
En savoir plus ici. 

**Existe-t-il des restrictions à l’ajout de plusieurs locataires Azure AD à un seul compte espace partenaires ?**

Si le client Azure AD est déjà associé à un compte espace partenaires existant, il ne peut pas être associée aux nouveaux comptes de partenaires à l’aide de la fonctionnalité d’une architecture mutualisée. Une autre façon de penser qu’il est, un locataire Azure AD peut uniquement être associé à un compte espace partenaires, mais un compte espace partenaires peut avoir plusieurs locataires qui lui sont associées.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migration de l’appartenance au Microsoft Partner Network (MPN) 

**Qui peut effectuer le déplacement à partir de PMC pour partenaires ?**

Votre administrateur général de MPN de société ou le contact principal de programme (ces deux rôles sont souvent détenus par la même personne) peut lancer et effectuer le déplacement.

**La personne à la fin de la migration deviendra le contact principal sur le profil d’entreprise juridique dans partenaires ?**

Pas nécessairement, toutefois, le contact principal doit être une personne qui a l’autorisation pour signer des contrats.

**Microsoft pour migrer mon adhésion à MPN pour moi ?**

Non. Microsoft ne peut pas vous aider à déplacer votre compte de l’appartenance à des partenaires. Vous devrez déplacer votre compte en vous connectant PMC avec votre compte professionnel (informations d’identification de connexion) commencer le processus de migration. Une fois que vous avez terminé les étapes pour déplacer votre compte, vous pouvez commencer à gérer votre abonnement et attribuer des rôles d’utilisateur et des autorisations à votre équipe afin de pouvoir accéder aux avantages et aider à gérer l’appartenance. Microsoft migre automatiquement les compétences actuelles, des avantages, des informations d’emplacement, bank/taxes relatives primes et des associations MCP y compris l’accès de l’Université de partenaire.

Microsoft migre automatiquement les compétences actuelles, des avantages, des informations d’emplacement, bank/taxes relatives primes et des associations MCP y compris l’accès de l’Université de partenaire.

**Comment va changer la stratégie de renouvellement ?**

 Dans le centre de partenaires, la fenêtre de renouvellement est à partir de votre date d’anniversaire via les 30 jours suivants.

**Nos compétences reste inchangés après que nous passons à des partenaires ?**

Oui, compentencies ne seront pas affectés par le passage à des partenaires. Si vous remarquez des écarts, contactez [prise en charge](https://partner.microsoft.com/support).


 **Mes avantages (y compris les avantages du cloud, support technique, avantages des logiciels, Visual Studio) changera une fois que nous passons ?**

 Vos avantages éligibles ne changera pas. Si vous remarquez des écarts, contactez [prise en charge](https://partner.microsoft.com/support).

 **Seront honorées nos comptes Microsoft qui ont des allocations des avantages de Visual Studio ?**


 Oui. Les avantages de Visual Studio allouées aux comptes de service administrés seront honorées et conservées. Elles sont également conservées après le renouvellement de partenaires. Toutefois, si vous supprimez une allocation MSA une fois migrés dans Partner Center, il ne peut pas être rajoutée à Partner Center.

Dans Partner Center, un partenaire peut ajouter des comptes professionnels et les comptes d’utilisateur invité qui sont MSA provenant du même locataire où le partenaire est administrateur MPN dans le locataire Azure AD. Si le partenaire est un administrateur global dans plusieurs locataires Azure AD et que tous les clients de ces soient associés au même compte de partenaires, le partenaire est autorisé pour ajouter des utilisateurs sur tous les locataires ces dans les avantages de Visual Studio et les allocations basée sur l’utilisation de Azure.

Bien que les utilisateurs invités peuvent recevoir basée sur l’utilisation des abonnements de Visual Studio par l’administrateur MPN ou l’administrateur global, les utilisateurs invités connexion impossible à l’espace partenaires à l’aide de leur compte de service administré. Les utilisateurs invités peuvent, toutefois, la connexion à Azure et Visual Studio pour valider et utiliser leurs avantages attribués.


 **Comment dois-je gérer notre associations MCP et notre accès Partner University ?**

 Il n’y a aucune modification aux associations MCP qui déplacent de PMC. Toutefois, les nouveaux employés nouveau après avoir déplacé les partenaires devrez être associées aux partenaires. Toutes les autorisations de votre université de partenaire pour les utilisateurs existants resteront mais les nouveaux employés doivent atteindre [le centre de formation](https://partner.microsoft.com/training) pour plus d’informations sur la façon d’accéder à l’Université de partenaire.

 **Les références client sont utilisés dans l’espace partenaires ?**

 Non, vous n’avez pas besoin des références de client pour répondre aux exigences de compétence dans partenaires.

 **Associations de partenaire de référence se déplacera vers partenaires ?**

 Oui, il n’existe aucune modification Partner of Record. Apprenez-en davantage sur [liant votre ID partenaire à vos clients](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Y a-t-il un impact sur les primes en raison du déplacement pour partenaires ?**

Non, il n’est aucun impact sur les primes si vous avez déplacé votre compte sans consolidant des emplacements. Si votre entreprise comporte plusieurs comptes dans PMC et, lorsque vous déplacez vers le centre de partenaires que vous décidez de consolider dans un compte global, il n’y aura aucune perte de primes, mais offre incitative paiement peut prendre un certain. Si vous ne déplacez pas tous vos comptes PMC qui ont été impliquées dans des programmes de primes, vous pouvez arrêter l’obtention de primes qui sont liées à ces comptes.


**Quelles sont les rôles d’utilisateur offre incitative dans partenaires ?** 

Rôles offre incitatives dans partenaires sont basés sur l’emplacement et incluent des primes destinées aux utilisateurs admin et incitations. Pour plus d’informations sur ce que peuvent faire ces rôles, consultez [attribuer des rôles d’utilisateurs et les autorisations](permissions-overview.md).

**Les utilisateurs des incitations affectables au niveau global et l’emplacement ?**

 Oui. Vous pouvez affecter un administrateur de primes pour être l’administrateur de primes pour tous les emplacements ou chaque emplacement peut avoir son propre administrateur de primes.

 **Primes peuvent être payés au niveau global ou emplacement ?**

 Primes sont payés uniquement au niveau du magasin.

**Concernant les références, les profils d’entreprise combien pouvons-nous créer ?**

Votre entreprise pouvez créer plusieurs profils d’entreprise en tant que vos besoins pour représentent entièrement les intérêts de votre entreprise. Dans chaque profil d’entreprise, vous pouvez répertorier jusqu'à cinq sites, un emplacement par pays. Chacun des profils d’entreprise peut recevoir des références pour chacun de ses emplacements.

**Comment sont les redirections affectés, quelles modifications puis-je attendre ? Par exemple, si j’ai une entreprise globale dans un marché et les emplacements dans les autres marchés, comment les références recevront ?**

Les références sont affectés selon les paramètres de recherche définie par l’utilisateur. Ce que vous ayez un emplacement ou plusieurs, si les clients spécifie un emplacement souhaité et que vous avez un il répond à d’autres paramètres, puis la référence accédaient à cet emplacement.








