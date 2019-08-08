---
title: Forum aux questions sur la confirmation de l’acceptation du contrat Microsoft Cloud par le client | Espace partenaires
ms.topic: article
ms.date: 03/15/2019
Description: FAQ pour la confirmation de l’acceptation du client
author: LauraBrenner
ms.author: labrenne
keywords: client, clients, consentement, FAQ, MCA, Microsoft Cloud contrat
ms.localizationpriority: medium
ms.openlocfilehash: c6681b4b979352b58258837d85d8c88543d16ed0
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820466"
---
# <a name="microsoft-cloud-agreement-customer-acceptance-confirmation-frequently-asked-questions"></a>Forum aux questions sur la confirmation de l’acceptation du contrat Microsoft Cloud par le client

-   [Processus](##processfaq)

-   [Règlement](#policyfaq)

-   [Documentation](#technicalfaq)

-   [Ressources supplémentaires](#additionalresourcesfaq)


## <a href="" id="processfaq"></a>Traiter

**Quel est le nouveau processus permettant de confirmer l’acceptation par le client de l’accord de Microsoft Cloud?**

Microsoft s’engage à aider nos clients et nos partenaires à rester en conformité. En tant que partenaire du programme fournisseur de solutions Cloud (CSP) de Microsoft, vous êtes responsable de l’examen des conditions générales de Microsoft, y compris l’utilisation acceptable des produits et services Microsoft avec les clients. Pour mieux aider les partenaires à répondre aux exigences de conformité et pour garantir la transparence, nous mettons en place un nouveau processus nécessitant des partenaires CSP pour confirmer que leurs clients ont accepté les conditions du contrat de Microsoft Cloud. Depuis le 7 août 2018, nous avons introduit un nouveau champ dans l’interface utilisateur du tableau de bord de l’espace partenaires, ainsi qu’une API de l’espace partenaires pour les partenaires afin de fournir ces informations. Au départ, il sera facultatif de fournir cette confirmation, mais il sera nécessaire à partir du 7 novembre 2018. 

**Quand cette exigence est-elle appliquée?**

Les partenaires peuvent commencer à confirmer l'acceptation dès la mise à disposition de cette fonctionnalité, le 7 août 2018. À partir du 7 novembre 2018, les utilisateurs du tableau de bord de l’espace partenaires sont tenus de confirmer l’acceptation par le client du contrat de Microsoft Cloud sur toutes les nouvelles transactions. Le 22 mars, les utilisateurs de l’API de l’espace partenaires 2019 seront tenus d’en faire de même. L’échéance pour les utilisateurs d’API a été étendue pour leur permettre de prendre du temps supplémentaire pour l’implémentation technique.

**NOUVEAU | Microsoft valide-t-il l’exactitude des informations client fournies par le partenaire?**

Microsoft valide que l’adresse de messagerie du client est correctement formatée. Il incombe au partenaire de fournir des informations précises et de corriger toutes les informations jugées inexactes. 

**NOUVEAU | Comment un partenaire peut-il prouver que le client accepte le contrat de Microsoft Cloud, qu’il soit signé, documenté, numérisé ou sur papier?**

Il incombe au partenaire de s’assurer que le client a accepté les termes du contrat de Microsoft Cloud et de gérer ses propres processus et enregistrements. En utilisant le tableau de bord de l’espace partenaires ou le processus de l’API espace partenaires, le partenaire confirme que le client a accepté les termes du contrat de Microsoft Cloud.

**NOUVEAU | Comment Microsoft vérifiera-t-il que le processus de confirmation est terminé pour un client?**

À compter du 7 novembre 2018, lorsqu’un partenaire CSP initie une transaction à l’aide du tableau de bord de l’espace partenaires pour un client nouveau ou existant, les systèmes de Microsoft vérifient automatiquement si les informations de confirmation du client sont présentes dans l’espace partenaires. Commandes. Si tel n’est pas le cas, la transaction ne pourra pas aboutir. 

À compter du 22 mars 2019, lorsqu’un partenaire CSP initie une transaction pour un client nouveau ou existant à l’aide de l’API de l’espace partenaires, les systèmes de Microsoft vérifient automatiquement si les informations de confirmation du client sont présentes. Si tel n’est pas le cas, la transaction ne pourra pas aboutir. 

**NOUVEAU | La notification est-elle envoyée aux clients dont l’adresse e-mail est fournie dans le processus de confirmation?**

Il n’existe aucun processus de notification.

## <a href="" id="policyfaq"></a>Renvoi

**Pourquoi Microsoft requiert-il des partenaires pour confirmer que les clients ont accepté le contrat de Microsoft Cloud?** 

Le contrat Microsoft Cloud protège les partenaires, les clients et Microsoft en indiquant au client ses droits d’utilisation et les conditions générales concernant les commandes de produits et services Microsoft Cloud. 

L’exécution correcte du contrat de Microsoft Cloud protège nos partenaires, nos clients et Microsoft en assurant l’alignement mutuel sur de nombreux sujets importants, notamment la sécurité, la confidentialité et la protection des données. Le processus de confirmation garantit la transparence et l’alignement et permet à Microsoft de mieux aider les clients qui ont besoin de répondre rapidement aux demandes réglementaires.

**Quelles sont les informations client requises pour terminer le processus de confirmation?**
Les informations nécessaires concernant la personne qui a accepté le contrat sont les suivantes :
-   Date d’acceptation du contrat
-   Nom de famille et prénom
-   Adresse électronique
-   Numéro de téléphone (facultatif) 

**NOUVEAU | Que se passe-t-il si la date d’échéance n’est pas respectée?**

Les partenaires peuvent commencer à confirmer l'acceptation dès la mise à disposition de cette fonctionnalité, le 7 août 2018. À partir du 7 novembre 2018, les utilisateurs du tableau de bord de l’espace partenaires sont tenus de confirmer l’acceptation par le client du contrat de Microsoft Cloud sur toutes les nouvelles transactions. Le 22 mars, les utilisateurs de l’API de l’espace partenaires 2019 seront tenus d’en faire de même.

Au moment de la mise en application, les nouveaux achats pour un client existant ou les modifications apportées au nombre de sièges sur les abonnements existants ne seront autorisés qu’une fois l’acceptation du client confirmée. Pour un nouveau client, les transactions ne seront pas autorisées jusqu'à ce que l’acceptation soit confirmée. Le renouvellement automatique n’est pas concerné par cette exigence.

**À quelles régions cette exigence s’applique-t-elle?**

La confirmation de l’acceptation du client au contrat de Microsoft Cloud est requise pour toutes les régions dans le cloud public Microsoft. La confirmation de l’acceptation du client n’est pas compatible avec les clouds nationaux (notamment Microsoft Cloud for US Government et Microsoft Cloud Germany).

**Quels sont les partenaires chargés de confirmer l’acceptation du client pour le contrat de Microsoft Cloud?**

À compter du 7 novembre, 2018, les fournisseurs de services Cloud (CSP) indirects et les partenaires de facturation directe sont tous deux responsables de la confirmation de l’acceptation du client et peuvent utiliser l’API espace partenaires ou le tableau de bord espace partenaires pour le faire. Les fournisseurs indirects devront peut-être d’abord collecter les informations requises auprès de leurs revendeurs indirects, puis les mettre à la disposition de Microsoft via l’API de l’espace partenaires ou le tableau de bord espace partenaires. Contractuellement, il s’agit d’un fournisseur indirect disposant d’un contrat de liaison avec Microsoft pour s’assurer que les clients finaux des revendeurs de fournisseurs de solutions Cloud ont accepté le contrat de Microsoft Cloud. 

**Quels scénarios client requièrent la confirmation de l’acceptation du client du contrat de Microsoft Cloud?**

L’acceptation du contrat de Microsoft Cloud doit être confirmée lorsque les partenaires CSP veulent effectuer les transactions suivantes:
1.  Un nouveau client effectue de nouveaux achats
2.  Un client existant effectue de nouveaux achats
3.  Un client existant met à jour le nombre de sièges pour les abonnements existants

**Puis-je confirmer que les clients existants sont séparés de leurs nouveaux achats ou ajouts de sièges?**

Oui. L’acceptation du client peut être confirmée pour tous les clients couverts par le contrat de Microsoft Cloud.

**Quelles sont les conditions requises pour les clients qui ont plusieurs partenaires CSP?**

La confirmation d’acceptation est confirmée par le partenaire. Si un client effectue des transactions avec plusieurs partenaires fournisseurs de solutions Cloud, chaque partenaire doit confirmer l’acceptation.

**Je suis revendeur indirect indirect travaillant avec des fournisseurs de services de chiffrement indirects. Quelle est ma responsabilité?**

Contractuellement, il s’agit du fournisseur indirect qui a un contrat de liaison avec Microsoft pour s’assurer que le client final a accepté le contrat de Microsoft Cloud. Cependant, les fournisseurs indirects peuvent avoir des accords distincts avec des revendeurs indirects pour recueillir l’acceptation du client. Dans ce cas, les fournisseurs indirects devront peut-être d’abord recueillir les informations d'acceptation du client nécessaires auprès de leurs revendeurs indirects, puis les mettre à disposition de Microsoft via l'API de l'Espace partenaires ou le tableau de bord de l'Espace partenaires. Vous pouvez prendre en charge ce processus en fournissant rapidement les informations requises à vos fournisseurs indirects à leur demande.

**Je suis un fournisseur de services de chiffrement indirect. Ai-je besoin de coordonner avec mon revendeur de solutions de CHIFFREment indirect pour être préparé?**

Il est conseillé aux fournisseurs indirects qui doivent recueillir les informations d’acceptation du client requises auprès de leurs revendeurs indirects de communiquer immédiatement cette exigence à leurs revendeurs indirects afin de coordonner la distribution et la réception de ces informations.

**Comment puis-je expliquer à mes clients qu’ils doivent confirmer leur acceptation du contrat de Microsoft Cloud?**

L’exécution appropriée de l’accord de Microsoft Cloud protège Microsoft, ses partenaires et ses clients en assurant l’alignement mutuel sur de nombreuses rubriques importantes, notamment la sécurité, la confidentialité et la protection des données. Le processus de confirmation garantit la transparence et l’alignement et permet à Microsoft de mieux aider les clients qui ont besoin de répondre rapidement aux demandes réglementaires.

**NOUVEAU | Si un client travaille avec un fournisseur CSP indirect unique, mais que les transactions sont terminées avec plusieurs revendeurs indirects du CSP, chaque revendeur de solutions de CHIFFREment indirect doit-il fournir au fournisseur CSP indirect les informations de confirmation?**

Le fournisseur CSP indirect est chargé de fournir la confirmation de l’acceptation du client de Microsoft Cloud accord à Microsoft. Pour chaque compte client, une seule confirmation peut être enregistrée dans le tableau de bord de l’espace partenaires en même temps. 

Le fournisseur de services de chiffrement indirects est chargé de confirmer qu’une personne chargée de contacter le client est responsable de l’acceptation du contrat de Microsoft Cloud, quel que soit le nombre de revendeurs indirects du fournisseur de services de chiffrement.

**NOUVEAU | Qui doit être la personne autorisée à confirmer l’acceptation du contrat de Microsoft Cloud au sein de l’organisation cliente?**

Il incombe au partenaire d’obtenir l’acceptation par le client de l’accord de Microsoft Cloud auprès d’une personne au sein de l’organisation cliente. Il incombe au client de déterminer qui est autorisé à fournir une acceptation. 

**NOUVEAU | Quelle version du contrat de Microsoft Cloud les partenaires sont responsables de la confirmation de l’acceptation du client? Les partenaires doivent-ils indiquer la version du contrat de Microsoft Cloud qui a été acceptée par le client?**

Les partenaires sont responsables de l’utilisation du contrat de Microsoft Cloud le plus récent lorsqu’ils effectuent des transactions CSP avec un nouveau client. Les partenaires doivent confirmer l’acceptation du contrat de Microsoft Cloud le plus récent lors du renouvellement, de la modification ou de l’exécution de nouvelles transactions avec un client existant. 

Si le contrat de Microsoft Cloud est mis à jour avant le renouvellement, les partenaires n’ont pas besoin de demander au client d’obtenir immédiatement l’acceptation du client du contrat de Microsoft Cloud, mais il doit reconfirmer le consentement du contrat de Microsoft Cloud avant à renouveler. Toutefois, vous souhaiterez peut-être que le client accepte les nouveaux termes avant le renouvellement pour tirer parti des termes nouveaux et améliorés du contrat de Microsoft Cloud.

**NOUVEAU | Je suis revendeur indirect du CSP. Si j’enregistre l’acceptation du client du contrat de Microsoft Cloud dans les enregistrements de mon entreprise, dois-je également fournir ces informations via le tableau de bord de l’espace partenaires ou l’API de l’espace partenaires?**

Contractuellement, il s’agit du fournisseur indirect qui a un contrat de liaison avec Microsoft pour s’assurer que le client final a accepté le contrat de Microsoft Cloud. Cependant, les fournisseurs indirects peuvent avoir des accords distincts avec des revendeurs indirects pour recueillir l’acceptation du client. Dans ce cas, les fournisseurs indirects devront peut-être d’abord recueillir les informations d'acceptation du client nécessaires auprès de leurs revendeurs indirects, puis les mettre à disposition de Microsoft via l'API de l'Espace partenaires ou le tableau de bord de l'Espace partenaires.

**NOUVEAU | Que se passe-t-il si mon client n’accepte pas les termes du contrat de Microsoft Cloud?**

En tant que partenaire du programme CSP de Microsoft, vous êtes responsable de l’acceptation par le client du contrat de Microsoft Cloud avant de passer une commande. Il ne s’agit pas d’une nouvelle exigence. Pour une raison quelconque, si le client n’accepte plus le contrat de Microsoft Cloud, le partenaire doit annuler les abonnements associés à ce client.

**NOUVEAU | Un revendeur peut-il fournir son consentement pour le compte du client?**

Non.

**Une fois que je confirme qu’un client a fourni son acceptation, dois-je le reconfirmer pour le client à l’avenir?**

Une fois que vous avez confirmé que le client a accepté le contrat de Microsoft Cloud, ces informations sont conservées dans la section compte client de l’espace partenaires et il n’est pas nécessaire de reconfirmer l’acceptation pour la durée pendant laquelle le client est couvert par conditions du contrat. Vous devez uniquement confirmer l’acceptation avant de passer une nouvelle commande.

Si le contrat de Microsoft Cloud est mis à jour avant le renouvellement, les partenaires n’ont pas besoin de demander au client d’obtenir immédiatement l’acceptation du client du contrat de Microsoft Cloud, mais il doit reconfirmer le consentement du contrat de Microsoft Cloud avant à renouveler. Toutefois, vous souhaiterez peut-être que le client accepte les nouveaux termes avant le renouvellement pour tirer parti des termes nouveaux et améliorés du contrat de Microsoft Cloud.

**NOUVEAU | Je ne suis pas à l’aise pour donner des informations de contact direct à Microsoft mon client final. Comment Microsoft utilise-t-il ces informations?**

Lorsqu’un partenaire crée un locataire client, il doit fournir des informations de contact principales pour le client. Selon les termes des services en ligne, «Microsoft traitera les données personnelles uniquement sur les instructions documentées du client».

## <a href="" id="technicalfaq"></a>Documentation

**Comment les partenaires confirment-ils l’acceptation du client et le fournissent à Microsoft? Quels outils sont disponibles pour prendre en charge ce processus?**

Deux méthodes sont disponibles à partir du 7 août 2018 pour aider les partenaires: 
1.  Les partenaires peuvent utiliser l'API de l'Espace partenaires pour confirmer par programme l’acceptation du client. 
2.  Les partenaires peuvent utiliser le tableau de bord espace partenaires pour confirmer l’acceptation du client.

**NOUVEAU | Je suis un partenaire CSP qui utilise l’API espace partenaires. Quelles modifications d’API dois-je prendre en compte?** 

Dans ce cas, l’API change en compte pour:

-   [https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent) 

-   [https://docs.microsoft.com/partner-center/develop/get-agreement-metadata](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [https://docs.microsoft.com/partner-center/develop/confirm-customer-consent](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)

**Que se passe-t-il si je rencontre des difficultés lors de l’implémentation de l’API espace partenaires?**

L'acceptation peut être confirmée manuellement via le tableau de bord de l'Espace partenaires.

**NOUVEAU | En guise d’alternative à l’utilisation du tableau de bord de l’espace partenaires ou de l’API espace partenaires, puis-je télécharger en bloc un fichier avec les informations de confirmation du client?**

À ce stade, le tableau de bord de l’espace partenaires et l’API de l’espace partenaires constituent le seul moyen d’assurer la confirmation de l’acceptation par le client de l’accord de Microsoft Cloud.

**NOUVEAU | Je suis partenaire à l’aide d’une plateforme tierce, ou «middleware», qui exécute les fonctionnalités permettant de connecter les systèmes de mon entreprise à l’espace partenaires. Que dois-je faire?**

Les partenaires qui utilisent des plateformes qui intègrent l’API espace partenaires sont invités à parler directement avec les fournisseurs de leurs plans et chronologies pour l’intégration de la fonctionnalité de l’API espace partenaires qui automatise le processus de confirmation du client.

**NOUVEAU | Pouvez-vous fournir un exemple de workflow d’API pour l’importation du nom complet du client, de l’adresse de messagerie et de la date de Microsoft Cloud acceptation du contrat?**

Les partenaires sont invités à consulter la documentation de l’API de l’espace partenaires pour obtenir des informations et des exemples.

**NOUVEAU | Comment faire obtenir le contrat de Microsoft Cloud le plus récent à afficher au client et l’utiliser dans l’enregistrement de confirmation dans le cadre de mon processus API?**

L’API actuelle de l’espace partenaires est très basique et ne permet pas aux partenaires de récupérer par programmation une copie du contrat de Microsoft Cloud, ni de capturer les versions du contrat de Microsoft Cloud acceptées par un client dans le cadre de la confirmation. 

**NOUVEAU | L’utilisation de l’API espace partenaires pour ce processus nécessite un paramètre userID. Comment faire gérer cette exigence lorsque les commandes sont placées via des plateformes tierces qui ne s’intègrent pas à Azure AD?**

Dans ce cas, l’ID d’utilisateur identifie l’employé sous le locataire partenaire qui fournit la confirmation du consentement du client. Si l’employé n’a pas de compte d’utilisateur Azure AD correspondant sous le locataire du partenaire, vous êtes invité à désigner un compte d’utilisateur spécifique à cet effet et à créer un processus pour capturer séparément l’identité de l’employé qui fournit le confirmé. 

**NOUVEAU | Pourquoi Microsoft a-t-il besoin du partenaire pour confirmer le consentement du client au contrat de Microsoft Cloud au lieu de l’obtenir directement auprès du client?**

Le client achète auprès du partenaire CSP, et non directement auprès de Microsoft. Pour utiliser les services fournis par Microsoft, Microsoft fournit des termes documentés dans le contrat de Microsoft Cloud. L’accord de revendeurs Microsoft Cloud oblige les partenaires CSP à consulter et à accepter le contrat de Microsoft Cloud avant de passer une commande. 

**NOUVEAU | J’utilise l’interface utilisateur Web de l’API et du tableau de bord de l’espace partenaires pour confirmer l’acceptation du client de l’accord de Microsoft Cloud. Après le 7 novembre 2018, quelles sont les options permettant de confirmer l’acceptation du client?**

Les deux options sont disponibles et acceptables pour confirmer Microsoft Cloud acceptation du client du contrat. Les transactions qui utilisent le tableau de bord espace partenaires nécessitent une confirmation à partir du 7 novembre 2018. Les transactions à l’aide de l’API espace partenaires requièrent que la confirmation soit présente à partir du 22 mars 2019.

## <a href="" id="additionalresourcesfaq"></a>Ressources supplémentaires

Pour en savoir plus sur la façon de confirmer l’acceptation par un client du contrat de Microsoft Cloud, consultez [confirmer l’acceptation du client du contrat de Microsoft Cloud](https://docs.microsoft.com/partner-center/confirm-consent).

Pour rechercher des modèles de client d’accord de Microsoft Cloud spécifiques à une région dans toutes les langues prises en charge, consultez [Microsoft Cloud accords par région et langue](agreements.md).
