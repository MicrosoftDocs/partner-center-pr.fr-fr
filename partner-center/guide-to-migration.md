---
title: Migrer de PMC vers l’Espace partenaires
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Découvrez comment migrer votre société depuis Partner Membership Center (PMC) vers l’Espace partenaires.
author: LauraBrenner
ms.author: labrenne
keywords: PMC, migration, migration vers l’Espace partenaires
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b81580e9b4e24d710151fb61d88e22c873c6c88d
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795830"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guide de migration de PMC vers l’Espace partenaires

**Rôles appropriés**

- Administrateur général

Le site web des partenaires Microsoft à l’adresse partner.microsoft.com propose une expérience numérique unifiée pour les partenaires. Ce site web vous permet d’explorer vos opportunités et de participer à des expériences guidées pour aider votre entreprise à créer et à vendre des applications et services avec Microsoft. À l’aide du lien Tableau de bord disponible sur le site web des partenaires, les membres du Microsoft Partner Network peuvent se connecter à l’Espace partenaires pour gérer leur relation avec Microsoft, participer à des programmes et s’inscrire à des offres.

Le Partner Membership Center (PMC) est sur le point d’être mis hors service. Votre entreprise a été invitée à transférer la gestion des membres du Microsoft Partner Network vers l’Espace partenaires. Ce guide a pour but de préparer votre transition du PMC à l’Espace partenaires.

>[!Note]
>Même si votre entreprise a plusieurs comptes ou emplacements, vous devez commencer par transférer un compte (votre premier compte) vers l’Espace partenaires.

## <a name="get-started"></a>Prendre en main

Le transfert commence dans PMC. Votre administrateur général reçoit une invitation pour commencer le transfert.

### <a name="prepare-in-pmc"></a>Se préparer dans PMC

- Vérifier les détails de votre entreprise
- Vérifier le contact principal du programme
- Vérifier les emplacements de l’entreprise
- Mettre à jour vos utilisateurs approuvés

### <a name="when-youre-ready"></a>Quand vous êtes prêt

Sélectionnez **Démarrer** dans votre invitation. Vous êtes alors dirigé vers la page de connexion à l’Espace partenaires.

![Prendre en main](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>Commencer par votre adresse e-mail professionnelle

Si votre entreprise ne dispose pas d’une adresse e-mail professionnelle et d’un locataire AAD, nous pouvons vous aider à les configurer au cours du processus de connexion à l’Espace partenaires. Quand vous essayez de vous connecter avec un compte e-mail qui n’est pas une adresse e-mail professionnelle, par exemple un compte personnel, vous êtes invité à fournir des informations sur votre entreprise afin que nous puissions configurer un locataire AAD et une adresse e-mail professionnelle. Ces détails sur votre entreprise étant utilisés pour finaliser votre compte dans l’Espace partenaires, vérifiez qu’ils ne contiennent pas d’erreurs.

>[!Note]
>Si vous êtes partenaire en Chine et que vous êtes inscrit à la fois au Microsoft Partner Network (MPN) et au programme Fournisseur de solutions Cloud (CSP), vous avez un locataire distinct pour chaque compte. Votre compte associé au programme Fournisseur de solutions Cloud est géré sur le cloud national, tandis que votre compte Microsoft Partner Network est géré sur le cloud global. Les deux comptes ne peuvent pas être liés.

![Donner des renseignements sur votre entreprise](images/migration/newtellusabout.png)

Après avoir vérifié ou mis à jour les informations, sélectionnez **Accepter et continuer**.
Les conditions générales figurant dans cette page sont **exactement les mêmes** que celles contenues dans l’accord que votre entreprise a déjà signé dans PMC.  
Cette étape lance la création de votre locataire Azure AD et vous fournit votre compte professionnel.

Le fait de sélectionner **Accepter et continuer** a également les conséquences suivantes :

- Migre votre compte et TOUS ses emplacements vers l’Espace partenaires

- Migre les compétences ou Microsoft Action Packs que vous avez achetés dans PMC

- Migre l’ensemble des programmes, offres et ressources marketing (Microsoft Action Packs, Silver, Gold) que vous aviez dans PMC

## <a name="invite-employees-to-join-you"></a>Inviter des employés à vous joindre

Une fois votre locataire Azure AD créé, vous pouvez inviter vos employés à se connecter à l’Espace partenaires.

![Inviter des employés](images/migration/invite.png)

Si vous vous êtes connecté avec un locataire AAD existant, vos employés sont transférés avec vous. Dans ce cas, attribuez à vos employés des rôles qui contrôlent ce qu’ils peuvent faire dans l’Espace partenaires. Remarque : Les rôles dans l’Espace partenaires sont différents des rôles dans PMC. Pour plus d’informations, consultez [Passage de PMC à l’Espace partenaires](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Vérifier votre domaine et devenir administrateur général  

Si votre locataire AAD vient d’être créé, le rôle d’administrateur général n’est attribué à personne. Pour devenir administrateur général, vous devez vérifier la propriété de votre domaine. Vous devrez peut-être contacter l’administrateur de domaine pour obtenir de l’aide. Même si vous pouvez utiliser les offres que vous avez déjà achetées, vous ne pourrez pas en acheter de nouvelles tant que vous n’aurez pas obtenu un administrateur général.

![Prendre le contrôle](images/migration/takecontrol.png)

Quand vous sélectionnez Démarrer, l’écran suivant s’affiche :

![Vérifier la propriété du domaine](images/migration/verifytxt.png)

Votre bureau d’enregistrement de domaines est déjà indiqué. Seul le propriétaire du domaine peut mettre à jour le fichier DNS. Par conséquent, en copiant et en ajoutant le fichier texte à votre enregistrement DNS, nous pouvons vérifier que vous êtes bien le propriétaire. La mise à jour nécessite quelques minutes. Vous devez ensuite vous déconnecter de l’Espace partenaires, puis vous reconnecter. Le rôle d’administrateur général vous est alors attribué.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Se familiariser avec le tableau de bord et l’Espace partenaires

Explorez votre tableau de bord. Ici, vous pouvez gérer votre adhésion, ajouter un profil d’entreprise pour les références, vous inscrire au programme Fournisseur de solutions Cloud et consulter les notifications et les offres pertinentes pour votre entreprise en sélectionnant **Tableau de bord** à tout moment. Vous pouvez également gérer les incentives, faire des achats dans la Place de marché, vous inscrire à des services de mise sur le marché et bien plus encore.  

![Visite guidée](images/migration/fre.png)

## <a name="next-steps"></a>Étapes suivantes

- [Créer des comptes d’utilisateur](create-user-accounts-and-set-permissions.md)

- [Attribuer des rôles et des autorisations aux utilisateurs](permissions-overview.md)

- [Gérer les programmes dont vous êtes membre](renew-mpn-offers.md)

- [Créer le profil commercial de votre société](create-a-marketing-profile.md)

- [Entrer en contact avec les clients via des références](responding-to-referrals.md)

- [Guide de migration de plusieurs entreprises de PMC vers l’Espace partenaires](move-multiple-companies.md)
