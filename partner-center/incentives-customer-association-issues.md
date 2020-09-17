---
title: Problèmes liés aux associations de client pour les incentives
description: Découvrez comment résoudre les problèmes qui se posent quand vous travaillez avec des associations de clients CPOR.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: ab2c26cf097d6212375382cadd9ac5f4f80b5c2a
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/17/2020
ms.locfileid: "90714473"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problèmes liés aux associations de clients d’enregistrement (CPOR) revendiqués

**S’applique à :**

- Espace partenaires

**Rôles appropriés :**

- Administrateur de la facturation
- Administrateur général
- Administrateur de primes incitatives

Le contenu ci-dessous vous aidera à résoudre les problèmes que vous pouvez rencontrer lorsque vous travaillez avec des associations de clients.

## <a name="domain-tenant-mismatch"></a>Incompatibilité de domaine-locataire

Dans le processus de revendication d’association CPOR (partenaire de l’enregistrement) revendiqué, vous serez invité à fournir l’ID et le sous-domaine du locataire client. Si vous recevez une erreur indiquant qu’elles ne correspondent pas, contactez votre client pour vous assurer que vous disposez des détails appropriés.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Erreurs d’abonnement dans le workflow de revendication d’association CPOR

Dans le circuit de revendications d’association CPOR, vous pouvez être invité à fournir un abonnement pour un produit que vous essayez de réclamer via Business Applications (Dynamics 365). Nous vous demandons l’abonnement, car nous vérifions dynamiquement que le produit et l’abonnement appartiennent au locataire demandé. Nous vérifions également que l’abonnement est dans un état actif/de grâce.

Si vous recevez l’erreur, il peut y avoir plusieurs raisons à cela :

- Le produit sélectionné n’existe pas sur le locataire du client
- L’abonnement fourni n’est pas pour Dynamics
- L’abonnement fourni est destiné aux fournisseurs de solutions cloud (CSP)
- Le client n’a pas encore activé/approvisionné les produits de cet abonnement
- Cet abonnement a déjà été demandé
- L’identificateur fourni n’est pas un ID d’abonnement

Si vous avez une question sur la précision de votre abonnement, contactez votre client pour vous assurer que l’abonnement est correct et que vous utilisez l’ID de locataire correct.

Si cet itinéraire n’a pas résolu votre problème, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Quand les abonnements seront disponibles pour la revendication

Lorsque vous demandez un abonnement, une erreur s’affiche si l’abonnement n’a pas encore été approvisionné. Il y a plusieurs étapes que le client doit effectuer pour que l’abonnement soit disponible pour la plateforme CPOR pour le récupérer et le rendre disponible en réclamation. Si vous recevez une erreur lorsque vous tentez de revendiquer un abonnement, contactez votre client pour vous assurer qu’il a été configuré et que l’abonnement que vous demandez est correct. Si vous avez déjà suivi cet itinéraire, contactez le [support technique](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Quelle activité dois-je choisir ?

La plateforme de revendication CPOR autorise les revendications d’association CPOR liées aux zones de solution Business Applications et Microsoft 365. Les activités qui s’appliquent à chaque zone de solution sont répertoriées ci-dessous. Sélectionnez l’activité appropriée en fonction des descriptions pour éviter d’avoir à récupérer à l’avenir. La revendication d’une activité incorrecte peut entraîner un manque d’éligibilité et des gains d’incentives.


| Domaine fonctionnel | Activité | S’applique à |
| ------ | ----------- | ----------- |
| Applications métier      | Support prévente   | Sélectionnez cette option si vous avez influencé l’achat d’un produit éligible et souhaitez demander des incentives avant la vente. Cette option s’applique uniquement si le client a acheté ces produits via un contrat de licence en volume ou Web-direct. |
|    |  Utilisation  | Sélectionnez si vous Encouragez l’adoption et l’utilisation d’une charge de travail éligible et souhaitez demander des incentives sur l’utilisation. Cette option s’applique uniquement si le client a acheté ces produits via un contrat de licence en volume ou Web-direct. |
|    | Association du chiffre d’affaires   | Sélectionnez si vous avez influencé la sélection d’un produit éligible en tant qu’influenceur commercial. Cette option est réservée à l’Association du chiffre d’affaires, et non aux paiements incitatives. Cette option s’applique uniquement si le client a acheté ces produits via un contrat de licence en volume ou Web-direct.   |
| Microsoft 365   | Utilisation   | Sélectionnez si vous Encouragez l’adoption et l’utilisation d’une charge de travail éligible et souhaitez demander des incentives sur l’utilisation. |

## <a name="which-mpn-do-i-choose"></a>Quels MPN-je choisir ?

Dans le workflow de revendication d’association CPOR, vous serez invité à choisir un MPN d’entreprise qui doit être associé au travail que vous demandez au client final. Votre entreprise peut avoir plusieurs MPNs, dont certaines peuvent être inscrites dans des programmes d’incentives, et d’autres associées à un type de partenaire tel que FRP FastTrack. Le workflow de la revendication d’association CPOR identifie les MPNs qui sont inscrits dans un programme d’incentives, mais ne vous indique pas s’il s’agit d’un type de partenaire MPN spécifique. Il est important de sélectionner le MPN approprié pour éviter d’avoir à récupérer à l’avenir. La revendication d’un MPN incorrect peut entraîner un manque d’éligibilité et des gains d’incentives.

Si vous ne savez pas quels MPN utiliser, contactez votre administrateur général.

Si le MPN que vous souhaitez utiliser n’est pas inscrit, vous pouvez le gérer sous l' [onglet de vue d’ensemble des incentives](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (connexion requise).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Choix d’un produit et entrée d’un abonnement

Lorsqu’un produit Dynamics est revendiqué et approuvé, le partenaire peut consulter l’ID d’abonnement dans la revendication d’association CPOR elle-même. Lorsque cet abonnement est demandé, il est actif ou dans un état de grâce, mais il peut y avoir une heure à laquelle l’abonnement se termine, et les nouveaux abonnements doivent être revendiqués dans une revendication d’association CPOR distincte.

## <a name="competing-claims"></a>Revendications en concurrence

Si vous créez une revendication d’association CPOR pour un client et leurs produits qui sont déjà associés à un autre partenaire, votre revendication passera en arbitrage :

1. Une fois que vous avez créé une association de clients, Microsoft vérifie les détails de l’association et la preuve d’exécution fournie pour garantir sa précision.

2. Si vous et un autre partenaire revendiquez les mêmes client et produit/charge de travail, Microsoft examinera la documentation relative à la preuve de l’exécution de chaque partenaire pour déterminer le partenaire à approuver.

3. Des informations supplémentaires peuvent être demandées par les deux partenaires, ce qui peut entraîner des retards dans le traitement de votre demande d’association.

4. Votre revendication d’association CPOR sera toujours examinée dans un délai de cinq jours ouvrables, bien que son état puisse rester en _cours d’examen_ sur une période plus longue. Ce scénario peut se produire lorsque Microsoft collabore avec le partenaire actuellement propriétaire du produit/de la charge de travail. Si c’est le cas, vous recevrez une notification dans la section des commentaires de votre revendication. 

>[!IMPORTANT]
>Si nous avons besoin d’informations supplémentaires pour vérifier votre CPOR d’Association (PoE), nous vous contacterons via la section commentaires de la revendication d’association CPOR.

## <a name="next-steps"></a>Étapes suivantes

- [Bien commencer avec les incentives](incentives-get-started-intro.md)
